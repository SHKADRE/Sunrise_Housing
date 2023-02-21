# Sunrise Housing Company Advanced Regression Model
> Outline a brief description of your project.


## Table of Contents
* [General Info](#general-information)
* [Conclusions](#conclusions)


<!-- You can include any other section that is pertinent to your problem -->

## General Information
### Background: 
Sunrise Housing Company is an US nased housing company and have an ambisius plans to do do new business in Australlian market. For this they need to purchase the low cost housing properties and sell them at higher prices at correct time. The old Australlian data is available in CSV format. From this data, a regularization based Regression model is required to make a business decision for the prediction of correct housing properties values and for the decesion making for the probable investments.

## Business Goals: 

Using advanced regression techniques, it is required to build a model of housing prices vs various independent variables. Following are the expectations from this regression model:
- The dependency of housing prices on the different independent variables
- The effect of selecting the right indepenedent variables on the housing prices
- The newly developed regression model should be able to predict the variations of these variables on housing prices
- 
#### Following main steps were performed for this analysis
- Data Exploration , including missing values and outliers.
    - Univariate Analysis
    -  Segmented Univariate Analysis
    - Bivariate Analysis
    - Heat Maps
- Data cleansing
     - Elaborate Missing value treatment
     - Outlier Treatment
- Feature Engineering
     - Deriving new useful features
     - Other feature engineering activities
     - Dummy variables
     - Feature transformation using BocCox1p
     - Feature scaling with StandardScaler
- Preaparing data Reression Model
     - Train-Test split
     - Treating multicolinearity
     - Why VIF is not used
- Regression Moel with Regularizaiton
     - Building Ridge model and finding out ptimum alpha and getting top features
     - Building Lasso model and finding out ptimum alpha and getting top features

- Analyst's Final Recommendations
### The data set features are defined as follows: 
-	Id
-	MSSubClass
-	MSZoning
-	LotFrontage
-	LotArea
-	Street
-	Alley
-	LotShape
-	LandContour
-	Utilities
-	LotConfig
-	LandSlope
-	Neighborhood
-	Condition1
-	Condition2
-	BldgType
-	HouseStyle
-	OverallQual
-	OverallCond
-	YearBuilt
-	YearRemodAdd
-	RoofStyle
-	RoofMatl
-	Exterior1st
-	Exterior2nd
-	MasVnrType
-	MasVnrArea
-	ExterQual
-	ExterCond
-	Foundation
-	BsmtQual
-	BsmtCond
-	BsmtExposure
-	BsmtFinType1
-	BsmtFinSF1
-	BsmtFinType2
-	BsmtFinSF2
-	BsmtUnfSF
-	TotalBsmtSF
-	Heating
-	HeatingQC
-	CentralAir
-	Electrical
-	1stFlrSF
-	2ndFlrSF
-	LowQualFinSF
-	GrLivArea
-	BsmtFullBath
-	BsmtHalfBath
-	FullBath
-	HalfBath
-	BedroomAbvGr
-	KitchenAbvGr
-	KitchenQual
-	TotRmsAbvGrd
-	Functional
-	Fireplaces
-	FireplaceQu
-	GarageType
-	GarageYrBlt
-	GarageFinish
-	GarageCars
-	GarageArea
-	GarageQual
-	GarageCond
-	PavedDrive
-	WoodDeckSF
-	OpenPorchSF
-	EnclosedPorch
-	3SsnPorch
-	ScreenPorch
-	PoolArea
-	PoolQC
-	Fence
-	MiscFeature
-	MiscVal
-	MoSold
-	YrSold
-	SaleType
-	SaleCondition
-	SalePrice

## Conclusions
#### Regurization Techniques for Regression- Ridge and Lasso
- For Ridge Regression various values of Alpha parameters were changes and using Grid Search optimization algorithm, the final value of Alha is 100
- For Lasso Regression various values of Alpha parameters were changes and using Grid Search optimization algorithm, the final value of Alha is 0.01

#### Model Performance Metrics
- For both Ridge and Lasso Regression Models, the R2 score for train and test data is close and near 0.9. It is as per industry norms and predictions made by these models for sales price will be accurate and ultimately help business

#### Top five features of Ridge Regression Model are as follows (Parameters, Coefficient)
- ('constant', 33.578)
- ('tot_sq_ft', 0.301)
- ('GrLivArea', 0.291)
- ('OverallQual', 0.233)
- ('RoofMatl_ClyTile', -0.223)
- ('LotArea', 0.205)

#### Top five features of Lasso Regression Model are as follows (Parameters, Coefficient)
-  ('constant', 33.578)
-  ('tot_sq_ft', 0.473)
-  ('GrLivArea', 0.439)
-  ('OverallQual', 0.297)
-  ('RoofMatl_ClyTile', -0.267)
-  ('YearsBuiltAge', -0.229)




