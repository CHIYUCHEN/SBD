# Milestone 5: Final Report
## Peter Chen
## Topic: Urban Development and Land Use Patterns in Philadelphia

**Project Overview:**

This project centers on the examination of land use data sourced from Philadelphia, focusing on a dataset of 560,104 records retrieved from the [OpenDataPhilly platform](https://opendataphilly.org/datasets/land-use/). The primary aim is to extract meaningful insights by normalizing the data based on the dependent variable's definition. The analysis concentrates on understanding the distribution and attributes of various land use categories, with a specific emphasis on commercial, civic/institutional, and vacant properties.

The project underscores the importance of conducting a thorough analysis of diverse land use aspects across different census tracts to contribute to well-informed decision-making in urban development and planning. The initial focus is on commercial land use, aiming to comprehend its distribution patterns. This analysis aids decision-makers in pinpointing areas suitable for development, redevelopment, or interventions. It also sheds light on census tracts with a lower count of commercial land use, providing crucial insights for urban planners, policymakers, and researchers interested in areas with less prevalent commercial development.

The second aspect involves scrutinizing civic/institutional land use, particularly in library areas. The objective is to gain insights into the distribution of such land use across various census tracts, offering essential information for assessing community access to cultural resources and assisting in formulating policies related to public services.

The third focus revolves around generating a detailed dataset highlighting census tracts containing vacant land. This dataset goes a step further by providing information on the types of vacant buildings within those tracts. The intention is to provide a nuanced understanding of the distribution and characteristics of vacant land within a specified geographic area. This information is considered valuable for urban planning, development, and policy-making, empowering stakeholders to make more informed decisions regarding the utilization of vacant land and the development potential of specific areas.

**Questions:**

1. What is/are the census tract(s) with the lowest count of commercial land use, and what is the respective count of commercial land use in each of these tracts?

   Visualization in QGIS:

<img src="https://github.com/CHIYUCHEN/SBD/raw/main/Commercial%20Land%20Use%20Count%20by%20Census%20Tract.jpg" alt="Commercial Land Use Count" width="500">

2. What is the census tract with the largest total area (in square meters) designated as Civic/Institutional land use, specifically for category library area?

   Visualization in QGIS:

<img src="https://github.com/CHIYUCHEN/SBD/raw/main/Largest%20Library%20Land%20Use%20Area%20by%20Census%20Tract.jpg" alt="Largest Library Land Use Area" width="500">

3. Which census tracts contain vacant land use with vacant buildings recorded within these tracts?

   Visualization in QGIS:

<img src="https://github.com/CHIYUCHEN/SBD/raw/main/Vacant%20Land%20by%20Census%20Tract.jpg" alt="Vacant Land by Census Tract" width="500">

**Data source:**
1. [Land Use Dataset - OpenDataPhilly](https://opendataphilly.org/datasets/land-use/)
2. [Census Tracts Dataset - OpenDataPhilly](https://opendataphilly.org/datasets/census-tracts/)

**Metadata:** 
1. [Land Use Dataset Metadata](https://metadata.phila.gov/#home/datasetdetails/5543864420583086178c4e74/representationdetails/55438a7f9b989a05172d0cf3/)
2. [Census Tracts Metadata](https://metadata.phila.gov/#home/datasetdetails/5543867720583086178c4f47/representationdetails/55438aca9b989a05172d0d7a/)

## Normalization Process and ERD

Normalization is about organizing data to reduce redundancy and dependency. The script below achieves this by splitting information into separate tables and using foreign keys to establish relationships between them, ensuring data consistency and eliminating repetitive information.

### Original Data Table

The initial data is stored in the table named `landuse`. It contains information about land use categorized by several codes and their respective descriptions.

### Normalization

#### Cleanup Table Creation

The script starts by creating a cleanup table `landuse_cleanup` by selecting specific columns from the original `landuse` table based on certain conditions and ordering.

#### Distinct Description Tables

Separate tables are created to store distinct codes (`cdig1`, `cdig2`, `cdig3`) along with their descriptions (`cdig1desc`, `cdig2desc`, `cdig3desc`). These tables help in maintaining a clean reference to the codes and their corresponding descriptions.

#### Intermediate Tables

Tables `landuse1`, `landuse2`, and `landuse3` are created to handle the relationships between the codes and their descriptions. These tables have foreign key constraints referencing the respective description tables.

#### Parcel Table

A table named `parcel` is created to store parcel information, including geometry (`geom`) related to land use. This table references the `landuse3` table via a foreign key constraint.

#### Lookup Table

Tables named `cdig1desc`, `cdig2desc`, `cdig3desc`, and `vacbldg` are created to store codes for various states of their descriptions.

#### Data Insertion

- The script populates the various description tables (`cdig1desc`, `cdig2desc`, `cdig3desc`, `vacbldg`) with their respective codes and descriptions.
- Inserts data into intermediate tables (`landuse1`, `landuse2`, `landuse3`) that link the codes with their descriptions.
- Inserts data into the `parcel` table, which contains information about parcels of land, referencing the `landuse3` table.

#### Normalization ETL Code

```sql
SET search_path TO term_project, public;
-- Create a cleanup table to store the original table landuse
DROP TABLE IF EXISTS landuse_cleanup CASCADE;
CREATE TABLE landuse_cleanup AS
SELECT id, geom, objectid, year, vacbldg, C_DIG1, C_DIG1DESC, C_DIG2, C_DIG2DESC, C_DIG3, C_DIG3DESC
FROM landuse
WHERE CAST(C_DIG2DESC AS VARCHAR(3)) LIKE CONCAT(C_DIG1DESC, '%')
AND CAST(C_DIG3DESC AS VARCHAR(3)) LIKE CONCAT(C_DIG2DESC, '%')
ORDER BY C_DIG1DESC, C_DIG2DESC, C_DIG3DESC;
DROP TABLE IF EXISTS cdig1desc CASCADE;
CREATE TABLE cdig1desc (
cdig1 Integer PRIMARY KEY,
Description VARCHAR(50)
);
INSERT INTO cdig1desc (cdig1, Description)
VALUES 
(1, 'Residential'),
(2, 'Commercial'),
(3, 'Industrial'),
(4, 'Civic/Institution'),
(5, 'Transportation'),
(6, 'Culture/Recreation'),
(7, 'Park/Open Space'),
(8, 'Water'),
(9, 'Vacant or Other');
DROP TABLE IF EXISTS landuse1 CASCADE;
CREATE TABLE landuse1 (
cdig1 Integer,
cdig1desc VARCHAR,
PRIMARY KEY (cdig1)
);
INSERT INTO landuse1 (cdig1, cdig1desc)
SELECT DISTINCT c_dig1::int, c_dig1desc::VARCHAR
FROM landuse_cleanup l
ORDER BY c_dig1;
-- Combine the tables using a JOIN operation
SELECT l1.cdig1, l1.cdig1desc, c1.Description AS cdig1desc_description
FROM landuse1 l1
JOIN cdig1desc c1 ON l1.cdig1 = c1.cdig1;
DROP TABLE IF EXISTS cdig2desc CASCADE;
CREATE TABLE cdig2desc (
cdig2 Integer PRIMARY KEY,
Description VARCHAR(50)
);
INSERT INTO cdig2desc (cdig2, Description)
VALUES 
(11, 'Residential Low'),
(12, 'Residential Medium'),
(13, 'Residential High'),
(21, 'Commercial Consumer'),
(22, 'Commercial Business/Professional'),
(23, 'Commercial Mixed Residential'),
(31, 'Industrial'),
(41, 'Civic/Institution'),
(51, 'Transportation'),
(61, 'Culture/Amusement'),
(62, 'Active Recreation'),
(71, 'Park/Open Space'),
(72, 'Cemetery'),
(81, 'Water'),
(91, 'Vacant'),
(92, 'Other/Unknown');
DROP TABLE IF EXISTS landuse2 CASCADE;
CREATE TABLE "landuse2" (
"cdig1" Integer,
"cdig2" Integer,
"cdig1desc" VARCHAR,
"cdig2desc" VARCHAR,
PRIMARY KEY ("cdig2"),
CONSTRAINT "FK_landuse2.cdig1"
FOREIGN KEY ("cdig1")
REFERENCES "landuse1"("cdig1")
);
INSERT INTO landuse2 (cdig1, cdig1desc, cdig2, cdig2desc)
SELECT DISTINCT ON (c_dig2)
l1.cdig1, l1.cdig1desc,
l.c_dig2::int, l.c_dig2desc::VARCHAR
FROM landuse_cleanup l
JOIN landuse1 l1 ON l1.cdig1 = l.c_dig1
ORDER BY l.c_dig2;
-- Combine the tables using a JOIN operation
SELECT l2.cdig1, l2.cdig2, l2.cdig1desc, l2.cdig2desc, c2.Description AS cdig2desc_description
FROM landuse2 l2
JOIN cdig2desc c2 ON l2.cdig2 = c2.cdig2;
DROP TABLE IF EXISTS cdig3desc CASCADE;
CREATE TABLE cdig3desc (
cdig3 INT PRIMARY KEY,
Description VARCHAR(100)
);
INSERT INTO cdig3desc (cdig3, Description)
VALUES 
(111, 'Residential Detached'),
(112, 'Residential SemiDetached'),
(113, 'Residential Condo 1 to 1.5 stry'),
(119, 'Other RLD'),
(121, 'Residential Rowhouse'),
(122, 'Residential Detached Converted to Apts LT 3stry LT 5 units'),
(123, 'Residential SemiDetached Converted to Apts LT 3stry LT 5 units'),
(124, 'Residential Rowhouse Converted to Apts LT 3st LT 5 units'),
(125, 'Apt House or Condo LT 5 units incl Duplex or Quad LT 3stry'),
(129, 'Other RMD'),
(131, 'Apt House GT or equal to 5 units'),
(132, 'Residential Detached or SemiDetached Converted to Apts GT 3stry LT 5 units'),
(133, 'Residential Rowhouse Converted to Apts or Apts or Condos GT 3stry LT 5 units'),
(135, 'Hotel Motel'),
(136, 'Residential Care Facility'),
(137, 'Dormitory'),
(138, 'Correctional Facility'),
(139, 'Other RHD'),
(211, 'Commercial Store'),
(212, 'Commercial Food Service and Drinking'),
(213, 'Commercial Auto'),
(219, 'Other CC'),
(221, 'Commercial Office'),
(222, 'Commercial Service'),
(229, 'Other CBP'),
(231, 'Commercial Store or Office with Apts'),
(232, 'Rowhouse Store or Office with Apts'),
(233, 'Detached or SemiDetached with Store or Office'),
(239, 'Other CMR'),
(311, 'Manufacturing food beverages textiles apparel'),
(312, 'Manufacturing wood paper printing petroleum chemicals plastics rubber'),
(313, 'Manufacturing metal machinery computer electronics transp equip furniture'),
(314, 'Utilities'),
(315, 'Construction'),
(316, 'Wholesale Trade'),
(317, 'Warehousing and Distribution'),
(318, 'Other production distribution repair maintenance'),
(319, 'Other Industrial'),
(411, 'Heath Care'),
(412, 'Day Care'),
(413, 'Education'),
(414, 'Library'),
(415, 'Courts'),
(416, 'Public Safety'),
(417, 'Worship'),
(418, 'Fraternal Organizations and Social Clubs'),
(419, 'Other Civic'),
(511, 'Transportation Street and Sidewalk ROW'),
(512, 'Transportation Rail ROW Yards Stations'),
(513, 'Transportation Truck Bus Taxi'),
(514, 'Transportation Parking'),
(515, 'Transportation Parking Commercial Mix'),
(516, 'Transportation Marine'),
(517, 'Transportation Aviation'),
(518, 'Transportation Pipeline'),
(519, 'Other Trans'),
(611, 'Performing Arts'),
(612, 'Cultural and Natural History'),
(613, 'Amusement'),
(619, 'Other Cultural Amusement'),
(621, 'Active Recreation'),
(711, 'Park Open Space'),
(721, 'Cemetery'),
(719, 'Other POS'),
(811, 'Water'),
(819, 'Other Water'),
(911, 'Vacant Parcels'),
(921, 'Other Unknown');
DROP TABLE IF EXISTS landuse3 CASCADE;
CREATE TABLE "landuse3" (
"cdig2" Integer,
"cdig3" Integer,
"cdig2desc" VARCHAR,
"cdig3desc" VARCHAR,
PRIMARY KEY ("cdig3"),
CONSTRAINT "FK_landuse3.cdig2"
FOREIGN KEY ("cdig2")
REFERENCES "landuse2"("cdig2")
);
INSERT INTO landuse3 (cdig2, cdig2desc, cdig3, cdig3desc)
SELECT DISTINCT ON (l.c_dig3)
l.c_dig2::int, l.c_dig2desc::VARCHAR,
COALESCE(l.c_dig3::int, -1), COALESCE(l.c_dig3desc::VARCHAR, '')
FROM landuse_cleanup l
JOIN landuse2 l2 ON l2.cdig2 = l.c_dig2
ORDER BY l.c_dig3;
-- Combine the tables using a JOIN operation
SELECT l3.cdig2, l3.cdig3, l3.cdig2desc, l3.cdig3desc, c3.Description AS cdig3desc_description
FROM landuse3 l3
LEFT JOIN cdig3desc c3 ON l3.cdig3 = c3.cdig3;
DROP TABLE IF EXISTS vacbldg CASCADE;
CREATE TABLE vacbldg (
vacbldg CHAR(1) PRIMARY KEY,
Description VARCHAR(50)
);
INSERT INTO vacbldg (vacbldg, Description)
VALUES 
('1', 'Fully vacant building'),
('2', 'Partially vacant building'),
('V', 'Fully vacant building'),
('P', 'Partially vacant building'),
(' ', 'No data collected');
DROP TABLE IF EXISTS parcel CASCADE;
CREATE TABLE "parcel" (
"gid" Integer,
"cdig3" Integer,
"objectid" Integer,
"year" Integer,
"vacbldg" VARCHAR,
"geom" geometry(MultiPolygon, 2272), -- Corrected syntax for the geom column
PRIMARY KEY ("gid"),
CONSTRAINT "fk_parcel_cdig3" -- Corrected constraint name
FOREIGN KEY ("cdig3")
REFERENCES "landuse3"("cdig3")
);
INSERT INTO "parcel" ("gid", "cdig3", "objectid", "year", "vacbldg", "geom")
SELECT l.id, l.c_dig3, l.objectid, l.year, l.vacbldg, ST_SetSRID(l.geom, 2272) -- Assuming NULL for the geom column
FROM "landuse_cleanup" l
JOIN "landuse3" l3 ON l.c_dig3 = l3.cdig3;
SELECT p.gid, p.cdig3, p.objectid, p.year, p.vacbldg, p.geom, vl.Description AS vacbldg_description
FROM parcel p
LEFT JOIN vacbldg vl ON p.vacbldg = vl.vacbldg;
```
### ERD
<img src="https://github.com/CHIYUCHEN/SBD/raw/main/ERD.jpg" alt="ERD">

## Optimization and Analysis

### 1.Data Normalization and Table Creation
•	The landuse_cleanup table is created by filtering data from the landuse table based on certain conditions using c_dig1desc, c_dig2desc and c_dig3desc.

•	This table possibly contains refined, normalized, or cleaned-up data compared to the original landuse table. It might have fewer records due to filtering out specific entries.

#### Code

```sql
set search_path to term_project, public;
--original data count: 560,104
--normalization result: 551,236
DROP TABLE IF EXISTS landuse_cleanup CASCADE;
CREATE TABLE landuse_cleanup AS
SELECT id, geom, c_dig1desc, c_dig2desc, c_dig3desc, vacbldg
FROM landuse
WHERE CAST(c_dig2desc AS VARCHAR(3)) LIKE CONCAT(c_dig1desc, '%')
AND CAST(c_dig3desc AS VARCHAR(3)) LIKE CONCAT(c_dig2desc, '%')
ORDER BY c_dig1desc, c_dig2desc, c_dig3desc;
--recheck normalization result: 8,868
SELECT id, geom, c_dig1desc, c_dig2desc, c_dig3desc, vacbldg
FROM landuse
WHERE NOT (CAST(c_dig2desc AS VARCHAR(3)) LIKE CONCAT(c_dig1desc, '%')
AND CAST(c_dig3desc AS VARCHAR(3)) LIKE CONCAT(c_dig2desc, '%'))
ORDER BY c_dig1desc, c_dig2desc, c_dig3desc;
```

### 2.Index Creation
•	Indexes are created on columns (c_dig1desc, c_dig2desc, c_dig3desc, vacbldg) used in filtering, joining, and grouping operations.

•	Purpose: Indexes enhance query performance by allowing the database engine to quickly locate relevant rows based on these indexed columns. They act as pointers to speed up data retrieval.

**Reasoning for Each Index:**

• CREATE INDEX ON landuse_cleanup (c_dig1desc). <br />
&nbsp;&nbsp;o Reasoning: This index optimizes filtering operations based on the c_dig1desc column. <br />
&nbsp;&nbsp;o Likely Usage: If queries frequently filter or join based on the first-level description of land use (c_dig1desc), this index will significantly speed up those operations. <br />

• CREATE INDEX ON landuse_cleanup (c_dig2desc). <br />
&nbsp;&nbsp;o Reasoning: This index optimizes filtering operations based on the c_dig2desc column. <br />
&nbsp;&nbsp;o Likely Usage: If queries often involve filtering or joining data using the second-level description of land use (c_dig2desc), this index will enhance query performance in such scenarios. <br />

• CREATE INDEX ON landuse_cleanup (c_dig3desc). <br />
&nbsp;&nbsp;o Reasoning: This index optimizes filtering operations based on the c_dig3desc column. <br />
&nbsp;&nbsp;o Likely Usage: When queries predominantly filter or join data using the third-level description of land use (c_dig3desc), this index will accelerate these operations. <br />

• CREATE INDEX ON landuse_cleanup (vacbldg). <br />
&nbsp;&nbsp;o Reasoning: This index optimizes filtering operations based on the vacbldg column. <br />
&nbsp;&nbsp;o Likely Usage: If queries frequently involve filtering data based on whether a building is vacant or not (vacbldg), this index will improve query performance by efficiently accessing relevant records. <br />

**Overall Impact:**

These indexes cater to specific columns used in filtering, joining, and possibly grouping operations in the provided queries. By indexing these columns, the code aims to speed up data retrieval and improve query performance where these columns are utilized for filtering or joining conditions.

The choice to index these columns is that these columns play a crucial role in the filtering or joining conditions within the spatial data context, as evidenced by the queries and the subsequent optimizations.

#### Code

```sql
--Index Creation:
--Columns c_dig1desc, c_dig2desc, c_dig3desc, and vacbldg are commonly used in filters and joins. Consider creating indexes on these columns
SELECT indexname FROM pg_indexes WHERE tablename = 'landuse_cleanup';
CREATE INDEX ON landuse_cleanup (c_dig1desc);
CREATE INDEX ON landuse_cleanup (c_dig2desc);
CREATE INDEX ON landuse_cleanup (c_dig3desc);
CREATE INDEX ON landuse_cleanup (vacbldg);
```
### 3.Query Optimizations and Timings

**Reasoning for Each Index:**

1. Q1: Census Tracts with Lowest Count of Commercial Land Use
&nbsp;&nbsp;•	Queries involve finding the lowest count of commercial land use per census tract. <br />
&nbsp;&nbsp;•	Timings are recorded using EXPLAIN ANALYZE to assess the query performance. <br />
&nbsp;&nbsp;•	Index landuse_cleanup_c_dig1desc_idx is dropped to analyze the impact of indexing on the query. <br />
&nbsp;&nbsp;•	The query filters by lu.c_dig1desc = '2', potentially querying commercial land use. <br />

#### Code

```sql
--With index: 343.392ms
EXPLAIN ANALYZE
SELECT cth.namelsad10, COUNT(lu.*) AS commercial_landuse_count
FROM censustract cth
LEFT JOIN landuse_cleanup lu
ON ST_Intersects(cth.geom, lu.geom)
WHERE lu.c_dig1desc = '2'
GROUP BY cth.namelsad10
ORDER BY commercial_landuse_count asc
LIMIT 5;

--Without index: 388.411ms
DROP INDEX landuse_cleanup_c_dig1desc_idx;
EXPLAIN ANALYZE
SELECT cth.namelsad10, COUNT(lu.*) AS commercial_landuse_count
FROM censustract cth
LEFT JOIN landuse_cleanup lu
ON ST_Intersects(cth.geom, lu.geom)
WHERE lu.c_dig1desc = '2'
GROUP BY cth.namelsad10
ORDER BY commercial_landuse_count asc
LIMIT 5;

```

2. Q2: Census Tract with Largest Library Area for Civic/Institutional Land Use
&nbsp;&nbsp;•	Queries aim to find the census tract with the largest total area designated as a library.. <br />
&nbsp;&nbsp;•	Timings are noted using EXPLAIN ANALYZE before and after dropping index landuse_cleanup_c_dig3desc_idx. <br />
&nbsp;&nbsp;•	This query filters by lu.c_dig3desc = '414', presumably representing library areas. <br />

#### Code

```sql
--With index: 586.362ms
EXPLAIN ANALYZE
SELECT cth.namelsad10, 
SUM(ST_Area(ST_Intersection(ST_Transform(cth.geom, 2272), ST_Transform(lu.geom, 2272)))) AS total_library_area_m²
FROM censustract cth
LEFT JOIN landuse_cleanup lu
ON ST_Intersects(ST_Transform(cth.geom, 2272), ST_Transform(lu.geom, 2272))
WHERE lu.c_dig3desc = '414'
GROUP BY cth.namelsad10
ORDER BY total_library_area_m² desc
LIMIT 1;

--Without index: 606.061ms
DROP INDEX landuse_cleanup_c_dig3desc_idx;
EXPLAIN ANALYZE
SELECT cth.namelsad10, 
SUM(ST_Area(ST_Intersection(ST_Transform(cth.geom, 2272), ST_Transform(lu.geom, 2272)))) AS total_library_area_m²
FROM censustract cth
LEFT JOIN landuse_cleanup lu
ON ST_Intersects(ST_Transform(cth.geom, 2272), ST_Transform(lu.geom, 2272))
WHERE lu.c_dig3desc = '414'
GROUP BY cth.namelsad10
ORDER BY total_library_area_m² desc
LIMIT 1;
```

3. Q3: Census Tracts Containing Vacant Land Use with Recorded Vacant Buildings
&nbsp;&nbsp;•	Queries aim to find census tracts containing vacant land use with vacant buildings. <br />
&nbsp;&nbsp;•	Timings are recorded using EXPLAIN ANALYZE. <br />
&nbsp;&nbsp;•	Indexes landuse_cleanup_c_dig3desc_idx and landuse_cleanup_vacbldg_idx are dropped to analyze their impact on the query execution time. <br />

#### Code

```sql
--With index: 214.473ms
EXPLAIN ANALYZE
SELECT cth.namelsad10, lu.*
FROM censustract cth
JOIN landuse_cleanup lu ON ST_Intersects(ST_Transform(cth.geom, 2272), ST_Transform(lu.geom, 2272))
WHERE 
lu.c_dig3desc = '911' -- Vacant land
AND (lu.vacbldg = '1' OR lu.vacbldg = 'V');

--Without index: 235.570ms
DROP INDEX landuse_cleanup_c_dig3desc_idx;
DROP INDEX landuse_cleanup_vacbldg_idx;
EXPLAIN ANALYZE
SELECT cth.namelsad10, lu.*
FROM censustract cth
JOIN landuse_cleanup lu ON ST_Intersects(ST_Transform(cth.geom, 2272), ST_Transform(lu.geom, 2272))
WHERE 
lu.c_dig3desc = '911' -- Vacant land
AND (lu.vacbldg = '1' OR lu.vacbldg = 'V');
```

### 4.	Impact of Indexing:
&nbsp;&nbsp;•	By creating and dropping specific indexes before and after executing queries, the code measures the performance difference, indicating how indexing affects query execution times. <br />
&nbsp;&nbsp;•	The EXPLAIN ANALYZE command helps evaluate query execution plans and timings, facilitating a comparative analysis of query performance with and without specific indexes. <br />
&nbsp;&nbsp;•	The code demonstrates a systematic approach to evaluating the impact of indexing on query performance, particularly in the context of spatial data analysis involving census tracts and land use information.. <br />
