# Kaggle-House-Prices-Advanced-Regression-Techniques


### Data Structure and Description
'data.frame':	1460 obs. of  81 variables:  

| |Name |Description |Class |Levels |Data |
|--- |--- |--- |--- |---|---|
|01 |ID  |  |  |  |  |
|02 |MSSubClass |The building class|int  |  |60 20 60 70 60 50 20 60 50 190 ...  | 
|03 |MSZoning |The general zoning classification |Factor |5 |"C (all)","FV",..: 4 4 4 4 4 4 4 4 5 4 ...  |
|04 |LotFrontage |Linear feet of street connected to property |int  | |65 80 68 60 84 85 75 NA 51 50 |
|05 |LotArea |Lot size in square feet |int  | |8450 9600 11250 9550 14260 14115 10084 10382 6120 7420 ... |
|06 |Street |Type of road access |Factor |2 |"Grvl","Pave": 2 2 2 2 2 2 2 2 2 2 ...  |
|07 |Alley |Type of alley access |Factor |2 |"Grvl","Pave": NA NA NA NA NA NA NA NA NA NA ...   |
|08 |LotShape |General shape of property |Factor |4 |"IR1","IR2","IR3",..: 4 4 1 1 1 1 4 1 4 4 ... |
|09 |LandContour |Flatness of the property |Factor |4 |"Bnk","HLS","Low",..: 4 4 4 4 4 4 4 4 4 4 ...  |
|10 |Utilities |Type of utilities available |Factor |2 |"AllPub","NoSeWa": 1 1 1 1 1 1 1 1 1 1 ...  |
|11 |LotConfig |Lot configuration |Factor |5 |"Corner","CulDSac",..: 5 3 5 1 3 5 5 1 5 1 ...  |
|12 |LandSlope |Slope of property |Factor |3 |"Gtl","Mod","Sev": 1 1 1 1 1 1 1 1 1 1 ...  |
|13 |Neighborhood |Physical locations within Ames city limits |Factor |25 |"Blmngtn","Blueste",..: 6 25 6 7 14 12 21 17 18 4 ...  |
|14 |Condition1 |Proximity to main road or railroad |Factor |9 |"Artery","Feedr",..: 3 2 3 3 3 3 3 5 1 1 ...  |
|15 |Condition2 |Proximity to main road or railroad (if a second is present) |Factor |8 |"Artery","Feedr",..: 3 3 3 3 3 3 3 3 3 1 ...  |
|16 |BldgType |Type of dwelling |Factor |5 |"1Fam","2fmCon",..: 1 1 1 1 1 1 1 1 1 2 ...   |
|17 |HouseStyle |Style of dwelling |Factor|8 |"1.5Fin","1.5Unf",..: 6 3 6 6 6 1 3 6 1 2 ...  |
|18 |OverallQual |Overall material and finish quality |int |  |7 6 7 7 8 5 8 7 7 5 ...  |
|19 |OverallCond |Overall condition rating |int | |5 8 5 5 5 5 5 6 5 6 ...  |
|20 |YearBuilt |Original construction date |int | |2003 1976 2001 1915 2000 1993 2004 1973 1931 1939 ...  |
|21 |YearRemodAdd |Remodel date |int | |2003 1976 2002 1970 2000 1995 2005 1973 1950 1950 ...  |
|22 |RoofStyle |Type of roof |Factor |6 |"Flat","Gable",..: 2 2 2 2 2 2 2 2 2 2 ...  |
|23 |RoofMatl |Roof material |Factor |8 |"ClyTile","CompShg",..: 2 2 2 2 2 2 2 2 2 2 ...  |
|24 |Exterior1st |Exterior covering on house |Factor |15 |"AsbShng","AsphShn",..: 13 9 13 14 13 13 13 7 4 9 ...  |
|25 |Exterior2nd |Exterior covering on house (if more than one material) |Factor |16 |"AsbShng","AsphShn",..: 14 9 14 16 14 14 14 7 16 9 ...  |
|26 |MasVnrType |Masonry veneer type |Factor |4 |"BrkCmn","BrkFace",..: 2 3 2 3 2 3 4 4 3 3 ...  |
|27 |MasVnrArea |Masonry veneer area in square feet |int | |196 0 162 0 350 0 186 240 0 0 ...  |
|28 |ExterQual |Exterior material quality |Factor |4 |"Ex","Fa","Gd",..: 3 4 3 4 3 4 3 4 4 4 ...   |
|29 |ExterCond |Present condition of the material on the exterior |Factor |5 |"Ex","Fa","Gd",..: 5 5 5 5 5 5 5 5 5 5 ...  |
|30 |Foundation |Type of foundation |Factor |6 |"BrkTil","CBlock",..: 3 2 3 1 3 6 3 2 1 1 ... |
|31 |BsmtQual |Height of the basement |Factor|4 |"Ex","Fa","Gd",..: 3 3 3 4 3 3 1 3 4 4 ...  |
|32 |BsmtCond |General condition of the basement |Factor |4 |"Fa","Gd","Po",..: 4 4 4 2 4 4 4 4 4 4 ...  |
|33 |BsmtExposure |Walkout or garden level basement walls |Factor|4 |"Av","Gd","Mn",..: 4 2 3 4 1 4 1 3 4 4 ...  |
|34 |BsmtFinType1 |Quality of basement finished area |Factor |6 |"ALQ","BLQ","GLQ",..: 3 1 3 1 3 3 3 1 6 3 ...  |
|35 |BsmtFinSF1 |Type 1 finished square feet |int | |706 978 486 216 655 732 1369 859 0 851 ...  |
|36 |BsmtFinType2 |Quality of second finished area (if present) |Factor |6 |"ALQ","BLQ","GLQ",..: 6 6 6 6 6 6 6 2 6 6 ...  |
|37 |BsmtFinSF2 |Type 2 finished square feet |int | |0 0 0 0 0 0 0 32 0 0 ...  |
|38 |BsmtUnfSF |Unfinished square feet of basement area |int | |150 284 434 540 490 64 317 216 952 140 ...  |
|39 |TotalBsmtSF |Total square feet of basement area |int | |856 1262 920 756 1145 796 1686 1107 952 991 ...  |
|40 |Heating |Type of heating |Factor |6 |"Floor","GasA",..: 2 2 2 2 2 2 2 2 2 2 ...  |
|41 |HeatingQC |Heating quality and condition |Factor|5 |"Ex","Fa","Gd",..: 1 1 1 3 1 1 1 1 3 1 ...  |
|42 |CentralAir |Central air conditioning |Factor |2 |"N","Y": 2 2 2 2 2 2 2 2 2 2 ...  |
|43 |Electrical |Electrical system |Factor|5 |"FuseA","FuseF",..: 5 5 5 5 5 5 5 5 2 5 ...  |
|44 |1stFlrSF |First Floor square feet |int | |856 1262 920 961 1145 796 1694 1107 1022 1077 ...  |
|45 |2ndFlrSF |Second floor square feet |int | |854 0 866 756 1053 566 0 983 752 0 ...  |
|46 |LowQualFinSF |Low quality finished square feet (all floors) |int | |0 0 0 0 0 0 0 0 0 0 ...  |
|47 |GrLivArea |Above grade (ground) living area square feet |int | |1710 1262 1786 1717 2198 1362 1694 2090 1774 1077 ...  |
|48 |BsmtFullBath |Basement full bathrooms |int | |1 0 1 1 1 1 1 1 0 1 ...  |
|49 |BsmtHalfBath |Basement half bathrooms |int | |0 1 0 0 0 0 0 0 0 0 ...  |
|50 |FullBath |Full bathrooms above grade |int | |2 2 2 1 2 1 2 2 2 1 ...  |
|51 |HalfBath |Half baths above grade |int | |1 0 1 0 1 1 0 1 0 0 ...  |
|52 |Bedroom |Number of bedrooms above basement level |int | |3 3 3 3 4 1 3 3 2 2 ...  |
|53 |Kitchen |Number of kitchens |int | |1 1 1 1 1 1 1 1 2 2 ...  |
|54 |KitchenQual |Kitchen quality |Factor |4 |"Ex","Fa","Gd",..: 3 4 3 3 3 4 3 4 4 4 ...  |
|55 |TotRmsAbvGrd |Total rooms above grade (does not include bathrooms) |int | |8 6 6 7 9 5 7 7 8 5 ...  |
|56 |Functional |Home functionality rating |Factor |7 |"Maj1","Maj2",..: 7 7 7 7 7 7 7 7 3 7 ...  |
|57 |Fireplaces |Number of fireplaces |int | |0 1 1 1 1 0 1 2 2 2 ...  |
|58 |FireplaceQu |Fireplace quality |Factor |5 |"Ex","Fa","Gd",..: NA 5 5 3 5 NA 3 5 5 5 ...  |
|59 |GarageType |Garage location |Factor |6 |"2Types","Attchd",..: 2 2 2 6 2 2 2 2 6 2 ...  |
|60 |GarageYrBlt |Year garage was built |int | |2003 1976 2001 1998 2000 1993 2004 1973 1931 1939 ...  |
|61 |GarageFinish |Interior finish of the garage |Factor |3 |"Fin","RFn","Unf": 2 2 2 3 2 3 2 2 3 2 ...  |
|62 |GarageCars |Size of garage in car capacity |int | |2 2 2 3 3 2 2 2 2 1 ...  |
|63 |GarageArea |Size of garage in square feet |int | |548 460 608 642 836 480 636 484 468 205 ... |
|64 |GarageQual |Garage quality |Factor |5 |"Ex","Fa","Gd",..: 5 5 5 5 5 5 5 5 2 3 ...  |
|65 |GarageCond |Garage condition |Factor |5 |"Ex","Fa","Gd",..: 5 5 5 5 5 5 5 5 5 5 ...  |
|66 |PavedDrive |Paved driveway |Factor |3 |"N","P","Y": 3 3 3 3 3 3 3 3 3 3 ...  |
|67 |WoodDeckSF |Wood deck area in square feet |int | |0 298 0 0 192 40 255 235 90 0 ...  |
|68 |OpenPorchSF |Open porch area in square feet |int | |61 0 42 35 84 30 57 204 0 4 ...  |
|69 |EnclosedPorch |Enclosed porch area in square feet |int | |0 0 0 272 0 0 0 228 205 0 ...  |
|70 |3SsnPorch |Three season porch area in square feet |int | |0 0 0 0 0 320 0 0 0 0 ...  |
|71 |ScreenPorch |Screen porch area in square feet |int | |0 0 0 0 0 0 0 0 0 0 ...  |
|72 |PoolArea |Pool area in square feet |int | |0 0 0 0 0 0 0 0 0 0 ...  |
|73 |PoolQC |Pool quality |Factor |3 |"Ex","Fa","Gd": NA NA NA NA NA NA NA NA NA NA ...  |
|74 |Fence |Fence quality |Factor|4 |"GdPrv","GdWo",..: NA NA NA NA NA 3 NA NA NA NA ...  |
|75 |MiscFeature |Miscellaneous feature not covered in other categories |Factor |4 |"Gar2","Othr",..: NA NA NA NA NA 3 NA 3 NA NA ...  |
|76 |MiscVal |$Value of miscellaneous feature |int | |0 0 0 0 0 700 0 350 0 0 ...  |
|77 |MoSold |Month Sold |int | |2 5 9 2 12 10 8 11 4 1 ...  |
|78 |YrSold |Year Sold |int | |2008 2007 2008 2006 2008 2009 2007 2009 2008 2008 ...  |
|79 |SaleType |Type of sale |Factor |9 |"COD","Con","ConLD",..: 9 9 9 9 9 9 9 9 9 9 ...  |
|80 |SaleCondition |Condition of sale |Factor |6 |"Abnorml","AdjLand",..: 5 5 5 1 5 5 5 5 1 5 ...  |
|81 |SalePrice |The property's sale price in dollars |int | |208500 181500 223500 140000 250000 143000 307000 200000 129900 118000 ... | 

Correlations with Sale Price for all continuous variables
Factor variables use logistic regression?
Continuous Variables - MSSubClass, LotFrontage, LotArea
Factors Variables - MSZoning, Street, Alley, LotShape, LandContour,


