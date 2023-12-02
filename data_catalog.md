# Data Catalog

## Folder: data

## Folder: ch01

### park.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

## Workspace: region.gdb

### fireStations

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### landCover

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- Shape_Length: Double
- Shape_Area: Double

### trail

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### tree

Type: RasterDataset

Format: FGDBR

Fields:

- Value: Integer
- Count: Double

### workzones

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Zone: String
- Shape_Length: Double
- Shape_Area: Double

## Folder: ch02

### fires.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FireId: Integer
- Organizati: String
- RegionStat: String
- RegionSt_1: String
- ReportingU: String
- Reportin_1: String
- CalendarYe: Integer
- FiscalYear: Integer
- FireNumber: Integer
- FireCode: String
- FireName: String
- FireType_P: Integer
- FireType: Integer
- Protection: Integer
- Completion: String
- IndexTime: Date
- IndexTimeS: String
- SizeClass: String
- LastModifi: Date
- CauseCateg: String
- Reimbursab: String
- BurningInd: String
- Nrvc: String
- Area: String
- AreaName: String
- Owner: Integer
- OriginAccu: String
- LocationMe: String
- Coordinate: String
- Datum: String
- LatitudeDD: Double
- LongitudeD: Double
- LatitudeDM: String
- Longitud_1: String
- LatitudeEn: String
- LongitudeE: String
- LatitudeNA: Double
- LongitudeN: Double
- UtmZone: Integer
- UtmEasting: Double
- UtmNorthin: Double
- StartTime: Date
- DetectionT: String
- StartAcres: Double
- InitialAtt: Date
- InitialA_1: Double
- ControlTim: Date
- ControlAcr: Double
- OutDate: Date
- Topography: Integer
- Aspect: Integer
- Slope: Integer
- Elevation: Integer
- Station: Integer
- FbpsFuelMo: String
- MsgcModel: String
- MsgcSlope: Integer
- MsgcGrass: String
- MsgcClimat: Integer
- SpecialAre: String
- WildlandUr: String
- Structures: String
- Authorized: String
- Authoriz_1: String
- Authoriz_2: Date
- EnteredByN: String
- EnteredByT: String
- EnteredDat: Date
- ProvidedBy: String
- Provided_1: String
- ProvidedDa: String
- CostAccoun: String

### park.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

## Folder: ch05

### park.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

## Folder: ch06

### data1.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- value: Integer
- POINT_X: Double
- POINT_Y: Double
- result: Integer
- measure: Integer

### park.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

### points.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- ORIG_FID: Integer

### special_regions.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer

### workzones.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- Zone: String

## Workspace: rastSmall.gdb

### out2

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- Value: Integer
- Count: Double

### out3

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- Value: Integer
- Count: Double

### out1

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- Value: Integer
- Count: Double

### dataRast

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- VALUE: Integer
- COUNT: Integer

## Folder: ch07

### park.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

### special_regions.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer

### trails.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FNODE_: Integer
- TNODE_: Integer
- LPOLY_: Integer
- RPOLY_: Integer
- LENGTH: Double
- NPS_NTRAIL: Integer
- NPS_NTRA_1: Integer
- OBJECTID: Integer
- PARK_NAME: String
- ALPHA_CODE: String
- DESIGNATIO: String
- ID: Integer
- FROMNODE: Integer
- TONODE: Integer
- LEFTPOLYGO: Integer
- RIGHTPOLYG: Integer
- SHAPE_LEN: Double

## Folder: My data

### landmarks.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- REFNUM: String
- STATE: String
- UTMZONE: String
- UTMEAST: Double
- UTMNRTH: Double
- RESNAME: String
- ADDRESS: String
- CITY: String
- VICINITY: String
- COUNTY: String
- LISTED_DAT: String
- MULTNAME: String
- CORRECT_ST: String
- OID_: Integer
- REFNUM_1: String
- OTHDOCCD: String
- OID_1: Integer
- OTHDOCCD_1: String
- OTHDOC: String
- Correct_Co: String
- NEAR_FID: Integer
- NEAR_DIST: Double

### trails.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FNODE_: Integer
- TNODE_: Integer
- LPOLY_: Integer
- RPOLY_: Integer
- LENGTH: Double
- NPS_NTRAIL: Integer
- NPS_NTRA_1: Integer
- OBJECTID: Integer
- PARK_NAME: String
- ALPHA_CODE: String
- DESIGNATIO: String
- ID: Integer
- FROMNODE: Integer
- TONODE: Integer
- LEFTPOLYGO: Integer
- RIGHTPOLYG: Integer
- SHAPE_LEN: Double

## Folder: ch09

### park.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

### trails.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FNODE_: Integer
- TNODE_: Integer
- LPOLY_: Integer
- RPOLY_: Integer
- LENGTH: Double
- NPS_NTRAIL: Integer
- NPS_NTRA_1: Integer
- OBJECTID: Integer
- PARK_NAME: String
- ALPHA_CODE: String
- DESIGNATIO: String
- ID: Integer
- FROMNODE: Integer
- TONODE: Integer
- LEFTPOLYGO: Integer
- RIGHTPOLYG: Integer
- SHAPE_LEN: Double

## Workspace: tester.gdb

### c1

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### c2

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### data1

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### data2

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### data3

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### fireStations

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### Line0

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### Line1

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### Line2

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### park

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- Shape_Length: Double
- Shape_Area: Double

### ptdata4

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### sample

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### scatter

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### schools

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### trail

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### aspect

Type: RasterDataset

Format: FGDBR

Fields:

- Value: Integer
- Count: Double

### regions2

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Input_FID: Integer
- Shape_Length: Double
- Shape_Area: Double
- rating: Integer

### workzones

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Zone: String
- Shape_Length: Double
- Shape_Area: Double

### regions1

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double
- Shape_Area: Double
- rating: Integer

### shp

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- FID_workzones: Integer
- Id: Integer
- Zone: String
- FID_schools: Integer

### smallWoods2

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- Shape_Length: Double
- Shape_Area: Double

### reg1

Type: FeatureClass

Geometry Type: Polygon

Alias Name: reg1

Fields:

- OBJECTID: OID
- Shape: Geometry
- Shape_Length: Double
- Shape_Area: Double

### c1_buffer

Type: FeatureClass

Geometry Type: Polygon

Alias Name: c1_buffer

Fields:

- OBJECTID: OID
- Shape: Geometry
- BUFF_DIST: Double
- ORIG_FID: Integer
- Shape_Length: Double
- Shape_Area: Double

## Folder: ch10

### data1.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- value: Integer
- POINT_X: Double
- POINT_Y: Double
- result: Integer
- measure: Integer

### data2.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- value: Integer
- POINT_X: Double
- POINT_Y: Double
- value2: Integer
- value3: Integer

### data3.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- value: Integer
- POINT_X: Double
- POINT_Y: Double

### data4.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- value: Integer
- POINT_X: Double
- POINT_Y: Double

### landmarks.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- REFNUM: String
- STATE: String
- UTMZONE: String
- UTMEAST: Double
- UTMNRTH: Double
- RESNAME: String
- ADDRESS: String
- CITY: String
- VICINITY: String
- COUNTY: String
- LISTED_DAT: String
- MULTNAME: String
- CORRECT_ST: String
- OID_: Integer
- REFNUM_1: String
- OTHDOCCD: String
- OID_1: Integer
- OTHDOCCD_1: String
- OTHDOC: String
- Correct_Co: String

### park.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

### parkLines.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- LEFT_FID: Integer
- RIGHT_FID: Integer

## Folder: archive

### data1.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- value: Integer
- POINT_X: Double
- POINT_Y: Double
- result: Integer
- measure: Integer

### data2.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- value: Integer
- POINT_X: Double
- POINT_Y: Double
- value2: Integer
- value3: Integer

### linesOUT.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- LEFT_FID: Integer
- RIGHT_FID: Integer

### outData.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- value: Integer
- POINT_X: Double
- POINT_Y: Double
- result: Integer
- measure: Integer

### park.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

### parkLines.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- LEFT_FID: Integer
- RIGHT_FID: Integer

### parkOutput.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

## Workspace: county.gdb

### fireStations

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer

### schools

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- CID: Integer

## Folder: pics

## Folder: italy

## Folder: venice

## Folder: jerusalem

## Folder: info

## Folder: ch11

### data1.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- value: Integer
- POINT_X: Double
- POINT_Y: Double
- result: Integer
- measure: Integer

### park.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

### USA.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FID_: Integer
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double

## Folder: pics

## Folder: italy

## Folder: venice

## Folder: jerusalem

## Workspace: rastTester.gdb

### elev

Type: RasterDataset

Format: FGDBR

### landcov

Type: RasterDataset

Format: FGDBR

### soilsid

Type: RasterDataset

Format: FGDBR

### getty_cover

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- VALUE: Integer
- COUNT: Integer

### landc197

Type: RasterDataset

Format: FGDBR

### landuse

Type: RasterDataset

Format: FGDBR

Fields:

- Value: Integer
- Count: Double

### aspect

Type: RasterDataset

Format: FGDBR

Fields:

- Value: Integer
- Count: Double

### soils_kf

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- VALUE: Integer
- COUNT: Integer

### plus_ras

Type: RasterDataset

Format: FGDBR

### CoverMinus

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- VALUE: Integer
- COUNT: Integer
- Location: String

### elev_srt

Type: RasterDataset

Format: FGDBR

Fields:

- Value: Integer
- Count: Double

### elev_sh

Type: RasterDataset

Format: FGDBR

### elev_ned

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- VALUE: Integer
- COUNT: Integer

### Int_rand1

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- Value: Integer
- Count: Double

### Int_rand2

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- Value: Integer
- Count: Double

### landc196

Type: RasterDataset

Format: FGDBR

### TimesCOVER

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- Value: Integer
- Count: Double
- blades: Integer

## Workspace: tester.gdb

### c1

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### c2

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### data1

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### data2

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### data3

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### fireStations

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### Line0

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### Line1

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### Line2

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### park

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- Shape_Length: Double
- Shape_Area: Double

### ptdata4

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### sample

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### scatter

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### schools

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### trail

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### aspect

Type: RasterDataset

Format: FGDBR

Fields:

- Value: Integer
- Count: Double

### regions2

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Input_FID: Integer
- Shape_Length: Double
- Shape_Area: Double
- rating: Integer

### workzones

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Zone: String
- Shape_Length: Double
- Shape_Area: Double

### regions1

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double
- Shape_Area: Double
- rating: Integer

### shp

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- FID_workzones: Integer
- Id: Integer
- Zone: String
- FID_schools: Integer

### smallWoods2

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- Shape_Length: Double
- Shape_Area: Double

### reg1

Type: FeatureClass

Geometry Type: Polygon

Alias Name: reg1

Fields:

- OBJECTID: OID
- Shape: Geometry
- Shape_Length: Double
- Shape_Area: Double

### c1_buffer

Type: FeatureClass

Geometry Type: Polygon

Alias Name: c1_buffer

Fields:

- OBJECTID: OID
- Shape: Geometry
- BUFF_DIST: Double
- ORIG_FID: Integer
- Shape_Length: Double
- Shape_Area: Double

## Folder: trains

### regions1.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- Input_FID: Integer
- Shape_Leng: Double
- rating: Integer

### regions2.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- Input_FID: Integer
- Shape_Leng: Double
- rating: Integer

### s1.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer

### s2.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer

## Folder: ch12

### data1.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- value: Integer
- POINT_X: Double
- POINT_Y: Double
- result: Integer
- measure: Integer

### data2.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- value: Integer
- POINT_X: Double
- POINT_Y: Double
- value2: Integer
- value3: Integer

### data3.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- value: Integer
- POINT_X: Double
- POINT_Y: Double

### data4.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- value: Integer
- POINT_X: Double
- POINT_Y: Double

### park.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

## Folder: comp

## Folder: pics

## Folder: italy

## Folder: venice

## Folder: jerusalem

## Folder: wTest

### data1.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- value: Integer
- POINT_X: Double
- POINT_Y: Double
- result: Integer
- measure: Integer

## Folder: trains

### regions1.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- Input_FID: Integer
- Shape_Leng: Double
- rating: Integer

### s2.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer

## Workspace: tSmall.gdb

### c1

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### trail

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### aspect

Type: RasterDataset

Format: FGDBR

Fields:

- Value: Integer
- Count: Double

### regions1

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double
- Shape_Area: Double
- rating: Integer

## Folder: info

## Folder: ch13

## Workspace: smallTest.gdb

### cover

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- Shape_Length: Double
- Shape_Area: Double

### fires

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- FireId: Double
- CalendarYe: Double
- FireNumber: Double
- FireName: String
- FireType_P: Double
- SizeClass: String
- StartTime: Date
- Authoriz_1: String

### park

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- LEFT_FID: Integer
- RIGHT_FID: Integer
- Shape_Length: Double

## Workspace: tester.gdb

### c1

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- veld: Integer

### c2

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### data1

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### data2

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### data3

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### fireStations

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### Line0

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### Line1

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### Line2

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### park

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- Shape_Length: Double
- Shape_Area: Double

### ptdata4

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### sample

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### scatter

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### schools

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### trail

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### aspect

Type: RasterDataset

Format: FGDBR

Fields:

- Value: Integer
- Count: Double

### regions2

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Input_FID: Integer
- Shape_Length: Double
- Shape_Area: Double
- rating: Integer

### workzones

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Zone: String
- Shape_Length: Double
- Shape_Area: Double

### regions1

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double
- Shape_Area: Double
- rating: Integer

### shp

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- FID_workzones: Integer
- Id: Integer
- Zone: String
- FID_schools: Integer

### smallWoods2

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- Shape_Length: Double
- Shape_Area: Double

### reg1

Type: FeatureClass

Geometry Type: Polygon

Alias Name: reg1

Fields:

- OBJECTID: OID
- Shape: Geometry
- Shape_Length: Double
- Shape_Area: Double

### c1_buffer

Type: FeatureClass

Geometry Type: Polygon

Alias Name: c1_buffer

Fields:

- OBJECTID: OID
- Shape: Geometry
- BUFF_DIST: Double
- ORIG_FID: Integer
- Shape_Length: Double
- Shape_Area: Double

## Folder: trains

### regions1.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- Input_FID: Integer
- Shape_Leng: Double
- rating: Integer

### regions2.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- Input_FID: Integer
- Shape_Leng: Double
- rating: Integer

### s1.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer

### s2.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer

## Folder: ch14

### buffer.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- BUFF_DIST: Double

### cover.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

### dummyFile.shp

Type: ShapeFile

### fires.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FireId: Integer
- CalendarYe: Integer
- FireNumber: Integer
- FireName: String
- FireType_P: Integer
- SizeClass: String
- StartTime: Date
- Authoriz_1: String

### no_damage.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

### parkLines.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- LEFT_FID: Integer
- RIGHT_FID: Integer

## Folder: predict

### coverPolygons.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

### firePoints.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FireId: Integer
- CalendarYe: Integer
- FireNumber: Integer
- FireName: String
- FireType_P: Integer
- SizeClass: String
- StartTime: Date
- Authoriz_1: String

### parkLines.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- LEFT_FID: Integer
- RIGHT_FID: Integer

## Workspace: rastTester.gdb

### elev

Type: RasterDataset

Format: FGDBR

### landcov

Type: RasterDataset

Format: FGDBR

### soilsid

Type: RasterDataset

Format: FGDBR

### getty_cover

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- VALUE: Integer
- COUNT: Integer

### landc197

Type: RasterDataset

Format: FGDBR

### landuse

Type: RasterDataset

Format: FGDBR

Fields:

- Value: Integer
- Count: Double

### aspect

Type: RasterDataset

Format: FGDBR

Fields:

- Value: Integer
- Count: Double

### soils_kf

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- VALUE: Integer
- COUNT: Integer

### plus_ras

Type: RasterDataset

Format: FGDBR

### CoverMinus

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- VALUE: Integer
- COUNT: Integer
- Location: String

### elev_srt

Type: RasterDataset

Format: FGDBR

Fields:

- Value: Integer
- Count: Double

### elev_sh

Type: RasterDataset

Format: FGDBR

### elev_ned

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- VALUE: Integer
- COUNT: Integer

### Int_rand1

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- Value: Integer
- Count: Double

### Int_rand2

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- Value: Integer
- Count: Double

### landc196

Type: RasterDataset

Format: FGDBR

### TimesCOVER

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- Value: Integer
- Count: Double
- blades: Integer

## Folder: ch15

### park.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

### scratchparkBox.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- ORIG_FID: Integer

### scratchscratchparkBoxBox.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- ORIG_FID: Integer
- ORIG_FID_1: Integer

### scratchscratchscratchparkBoxBoxBox.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- ORIG_FID: Integer
- ORIG_FID_1: Integer
- ORIG_FID_2: Integer

## Folder: scratch

### buffer.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- BUFF_DIST: Double

### bufferBuff.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- BUFF_DIST: Double
- ORIG_FID: Integer

### bufferOut.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- BUFF_DIST: Double
- ORIG_FID: Integer

### cover.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

### coverBuff.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- BUFF_DIST: Double
- ORIG_FID: Integer

### coverOut.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- BUFF_DIST: Double
- ORIG_FID: Integer

### fires.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FireId: Integer
- CalendarYe: Integer
- FireNumber: Integer
- FireName: String
- FireType_P: Integer
- SizeClass: String
- StartTime: Date
- Authoriz_1: String

### firesBuff.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FireId: Integer
- CalendarYe: Integer
- FireNumber: Integer
- FireName: String
- FireType_P: Integer
- SizeClass: String
- StartTime: Date
- Authoriz_1: String
- BUFF_DIST: Double
- ORIG_FID: Integer

### firesOut.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FireId: Integer
- CalendarYe: Integer
- FireNumber: Integer
- FireName: String
- FireType_P: Integer
- SizeClass: String
- StartTime: Date
- Authoriz_1: String
- BUFF_DIST: Double
- ORIG_FID: Integer

### no_damage.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

### no_damageBuff.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- BUFF_DIST: Double
- ORIG_FID: Integer

### no_damageOut.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- BUFF_DIST: Double
- ORIG_FID: Integer

### parkLines.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- LEFT_FID: Integer
- RIGHT_FID: Integer

### parkLinesBuff.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- LEFT_FID: Integer
- RIGHT_FID: Integer
- BUFF_DIST: Double
- ORIG_FID: Integer

### parkLinesOut.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- LEFT_FID: Integer
- RIGHT_FID: Integer
- BUFF_DIST: Double
- ORIG_FID: Integer

## Workspace: tester.gdb

### c1

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### c2

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### data1

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### data2

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### data3

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### fireStations

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### Line0

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### Line1

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### Line2

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### park

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- Shape_Length: Double
- Shape_Area: Double

### ptdata4

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### sample

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### scatter

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### schools

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### trail

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### aspect

Type: RasterDataset

Format: FGDBR

Fields:

- Value: Integer
- Count: Double

### regions2

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Input_FID: Integer
- Shape_Length: Double
- Shape_Area: Double
- rating: Integer

### workzones

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Zone: String
- Shape_Length: Double
- Shape_Area: Double

### regions1

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double
- Shape_Area: Double
- rating: Integer

### shp

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- FID_workzones: Integer
- Id: Integer
- Zone: String
- FID_schools: Integer

### smallWoods2

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- Shape_Length: Double
- Shape_Area: Double

## Folder: ch16

### park.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

## Folder: pics

## Folder: italy

## Folder: venice

## Folder: jerusalem

## Workspace: rastTester.gdb

### elev

Type: RasterDataset

Format: FGDBR

### landcov

Type: RasterDataset

Format: FGDBR

### soilsid

Type: RasterDataset

Format: FGDBR

### getty_cover

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- VALUE: Integer
- COUNT: Integer

### landc197

Type: RasterDataset

Format: FGDBR

### landuse

Type: RasterDataset

Format: FGDBR

Fields:

- Value: Integer
- Count: Double

### aspect

Type: RasterDataset

Format: FGDBR

Fields:

- Value: Integer
- Count: Double

### soils_kf

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- VALUE: Integer
- COUNT: Integer

### plus_ras

Type: RasterDataset

Format: FGDBR

### CoverMinus

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- VALUE: Integer
- COUNT: Integer
- Location: String

### elev_srt

Type: RasterDataset

Format: FGDBR

Fields:

- Value: Integer
- Count: Double

### elev_sh

Type: RasterDataset

Format: FGDBR

### elev_ned

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- VALUE: Integer
- COUNT: Integer

### Int_rand1

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- Value: Integer
- Count: Double

### Int_rand2

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- Value: Integer
- Count: Double

### landc196

Type: RasterDataset

Format: FGDBR

### TimesCOVER

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- Value: Integer
- Count: Double
- blades: Integer

## Folder: ch17

### agg.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer

### aggCopy.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer

### fires.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FireId: Integer
- CalendarYe: Integer
- FireNumber: Integer
- FireName: String
- FireType_P: Integer
- SizeClass: String
- StartTime: Date
- Authoriz_1: String

### firesCopy.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FireId: Integer
- CalendarYe: Integer
- FireNumber: Integer
- FireName: String
- FireType_P: Integer
- SizeClass: String
- StartTime: Date
- Authoriz_1: String

### firesCopy2.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FireId: Integer
- CalendarYe: Integer
- FireNumber: Integer
- FireName: String
- FireType_P: Integer
- SizeClass: String
- StartTime: Date
- Authoriz_1: String

### firesCopy3.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FireId: Integer
- CalendarYe: Integer
- FireNumber: Integer
- FireName: String
- FireType_P: Integer
- SizeClass: String
- StartTime: Date
- Authoriz_1: String

### park.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

### parkCopy2.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

### parkCopy3.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

### parkLines.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- LEFT_FID: Integer
- RIGHT_FID: Integer

### parkLinesCopy.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- LEFT_FID: Integer
- RIGHT_FID: Integer

### special_regions.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer

## Workspace: tester.gdb

### c1

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### c2

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### data1

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### data2

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### data3

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### fireStations

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### Line0

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### Line1

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### Line2

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### park

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- Shape_Length: Double
- Shape_Area: Double

### ptdata4

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### sample

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### scatter

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- value: Integer

### schools

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry

### trail

Type: FeatureClass

Geometry Type: Polyline

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double

### aspect

Type: RasterDataset

Format: FGDBR

Fields:

- Value: Integer
- Count: Double

### regions2

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Input_FID: Integer
- Shape_Length: Double
- Shape_Area: Double
- rating: Integer

### workzones

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Zone: String
- Shape_Length: Double
- Shape_Area: Double

### regions1

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- Id: Integer
- Shape_Length: Double
- Shape_Area: Double
- rating: Integer

### shp

Type: FeatureClass

Geometry Type: Point

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- FID_workzones: Integer
- Id: Integer
- Zone: String
- FID_schools: Integer

### smallWoods2

Type: FeatureClass

Geometry Type: Polygon

Alias Name: 

Fields:

- OBJECTID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- Shape_Length: Double
- Shape_Area: Double

## Folder: ch18

### narniaHike.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Classifica: String
- Tra_Width: String

### parkAreas.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- F_AREA: Double

## Folder: smallDir

### a.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- Name: String
- Culture: String
- AltName: String
- Area: Single

## Workspace: a.kml

### Polygons

Type: FeatureClass

Geometry Type: Polygon

Alias Name: Polygons

Fields:

- OID: OID
- Shape: Geometry
- Name: String
- FolderPath: String
- SymbolID: Integer
- AltMode: SmallInteger
- Base: Double
- Clamped: SmallInteger
- Extruded: SmallInteger
- Snippet: String
- PopupInfo: String

## Folder: ch19

## Folder: smallDir

### a.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- Name: String
- Culture: String
- AltName: String
- Area: Single

## Workspace: a.kml

### Polygons

Type: FeatureClass

Geometry Type: Polygon

Alias Name: Polygons

Fields:

- OID: OID
- Shape: Geometry
- Name: String
- FolderPath: String
- SymbolID: Integer
- AltMode: SmallInteger
- Base: Double
- Clamped: SmallInteger
- Extruded: SmallInteger
- Snippet: String
- PopupInfo: String

## Folder: ch20

### park.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

## Folder: htmlExamplePages

## Workspace: park.kmz

### Polygons

Type: FeatureClass

Geometry Type: Polygon

Alias Name: Polygons

Fields:

- OID: OID
- Shape: Geometry
- Name: String
- FolderPath: String
- SymbolID: Integer
- AltMode: SmallInteger
- Base: Double
- Clamped: SmallInteger
- Extruded: SmallInteger
- Snippet: String
- PopupInfo: String

## Folder: pics

## Workspace: rastTester.gdb

### elev

Type: RasterDataset

Format: FGDBR

### landcov

Type: RasterDataset

Format: FGDBR

### soilsid

Type: RasterDataset

Format: FGDBR

### getty_cover

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- VALUE: Integer
- COUNT: Integer

### landc197

Type: RasterDataset

Format: FGDBR

### landuse

Type: RasterDataset

Format: FGDBR

Fields:

- Value: Integer
- Count: Double

### aspect

Type: RasterDataset

Format: FGDBR

Fields:

- Value: Integer
- Count: Double

### soils_kf

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- VALUE: Integer
- COUNT: Integer

### plus_ras

Type: RasterDataset

Format: FGDBR

### CoverMinus

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- VALUE: Integer
- COUNT: Integer
- Location: String

### elev_srt

Type: RasterDataset

Format: FGDBR

Fields:

- Value: Integer
- Count: Double

### elev_sh

Type: RasterDataset

Format: FGDBR

### elev_ned

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- VALUE: Integer
- COUNT: Integer

### Int_rand1

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- Value: Integer
- Count: Double

### Int_rand2

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- Value: Integer
- Count: Double

### landc196

Type: RasterDataset

Format: FGDBR

### TimesCOVER

Type: RasterDataset

Format: FGDBR

Fields:

- OBJECTID: OID
- Value: Integer
- Count: Double
- blades: Integer

## Workspace: restaurants.kml

### Points

Type: FeatureClass

Geometry Type: Point

Alias Name: Points

Fields:

- OID: OID
- Shape: Geometry
- Name: String
- FolderPath: String
- SymbolID: Integer
- AltMode: SmallInteger
- Base: Double
- Snippet: String
- PopupInfo: String
- HasLabel: SmallInteger
- LabelID: Integer

## Workspace: Sample_7_Day_GPS_Data.kml

### Polylines

Type: FeatureClass

Geometry Type: Polyline

Alias Name: Polylines

Fields:

- OID: OID
- Shape: Geometry
- Name: String
- FolderPath: String
- SymbolID: Integer
- AltMode: SmallInteger
- Base: Double
- Clamped: SmallInteger
- Extruded: SmallInteger
- Snippet: String
- PopupInfo: String

### Points

Type: FeatureClass

Geometry Type: Point

Alias Name: Points

Fields:

- OID: OID
- Shape: Geometry
- Name: String
- FolderPath: String
- SymbolID: Integer
- AltMode: SmallInteger
- Base: Double
- Snippet: String
- PopupInfo: String
- HasLabel: SmallInteger
- LabelID: Integer

## Folder: ch21

## Folder: ch22

### park.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

## Folder: outputDir

## Folder: smallDir

### a.shp

Type: ShapeFile

## Workspace: a.kml

### Polygons

Type: FeatureClass

Geometry Type: Polygon

Alias Name: Polygons

Fields:

- OID: OID
- Shape: Geometry
- Name: String
- FolderPath: String
- SymbolID: Integer
- AltMode: SmallInteger
- Base: Double
- Clamped: SmallInteger
- Extruded: SmallInteger
- Snippet: String
- PopupInfo: String

## Folder: ch24

## Folder: mapProjects_forPython3

## Folder: maps

## Folder: otherData

### centers.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double
- ORIG_FID: Integer

### COVER4.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- COVER: String
- RECNO: Double

### workzones.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- Id: Integer
- Zone: String

## Folder: sandbox

## Folder: symbolTraining

### gradColorsNE.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FID_: Integer
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double
- Category: Integer

### gradSymbols.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FID_: Integer
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double
- Category: Integer

## Folder: USstates

### CT.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double

### eastNorthCentral.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FID_: Integer
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double

### eastSouthCentral.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FID_: Integer
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double

### MA.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FID_: Integer
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double

### midAtlantic.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FID_: Integer
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double

### mountain.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FID_: Integer
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double

### NC.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double

### NEstates.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FID_: Integer
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double
- Category: Integer

### newEngland.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FID_: Integer
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double

### pacific.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FID_: Integer
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double

### RI.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double

### southAtlantic.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FID_: Integer
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double

### USA_States_Generalized.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FID_: Integer
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double

### VA.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double

### VT.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double

### westNorthCentral.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FID_: Integer
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double

### westSouthCentral.shp

Type: ShapeFile

Fields:

- FID: OID
- Shape: Geometry
- FID_: Integer
- STATE_NAME: String
- SUB_REGION: String
- STATE_ABBR: String
- POP2010: Integer
- POP10_SQMI: Double
- POP2012: Integer
- POP12_SQMI: Double
- WHITE: Integer
- BLACK: Integer
- AMERI_ES: Integer
- ASIAN: Integer
- HAWN_PI: Integer
- HISPANIC: Integer
- OTHER: Integer
- MULT_RACE: Integer
- MALES: Integer
- FEMALES: Integer
- AGE_UNDER5: Integer
- AGE_5_9: Integer
- AGE_10_14: Integer
- AGE_15_19: Integer
- AGE_20_24: Integer
- AGE_25_34: Integer
- AGE_35_44: Integer
- AGE_45_54: Integer
- AGE_55_64: Integer
- AGE_65_74: Integer
- AGE_75_84: Integer
- AGE_85_UP: Integer
- MED_AGE: Double
- MED_AGE_M: Double
- MED_AGE_F: Double
- HOUSEHOLDS: Integer
- AVE_HH_SZ: Double
- HSEHLD_1_M: Integer
- HSEHLD_1_F: Integer
- MARHH_CHD: Integer
- MARHH_NO_C: Integer
- MHH_CHILD: Integer
- FHH_CHILD: Integer
- FAMILIES: Integer
- AVE_FAM_SZ: Double
- HSE_UNITS: Integer
- VACANT: Integer
- OWNER_OCC: Integer
- RENTER_OCC: Integer
- NO_FARMS07: Double
- AVG_SIZE07: Double
- CROP_ACR07: Double
- AVG_SALE07: Double
- SQMI: Double

