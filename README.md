# Price-prediction
Predicting  Price of Ames housing data using Principal component analysis and Regression
Steps wise
  1. EDA expolatory data analysis 
        Total number of attributes equals 81, of which 36 is quantitative, 43 categorical + Id and SalePrice.

        Quantitative: 1stFlrSF, 2ndFlrSF, 3SsnPorch, BedroomAbvGr, BsmtFinSF1, BsmtFinSF2, BsmtFullBath, BsmtHalfBath,
        BsmtUnfSF, EnclosedPorch, Fireplaces, FullBath, GarageArea, GarageCars, GarageYrBlt, GrLivArea, HalfBath, KitchenAbvGr,
        LotArea, LotFrontage, LowQualFinSF, MSSubClass, MasVnrArea, MiscVal, MoSold, OpenPorchSF, OverallCond,
        OverallQual, PoolArea, ScreenPorch, TotRmsAbvGrd, TotalBsmtSF, WoodDeckSF, YearBuilt, YearRemodAdd, YrSold

        Qualitative: Alley, BldgType, BsmtCond, BsmtExposure, BsmtFinType1, BsmtFinType2, BsmtQual, CentralAir, Condition1,
        Condition2, Electrical, ExterCond, ExterQual, Exterior1st, Exterior2nd, Fence, FireplaceQu, Foundation, Functional,
        GarageCond, GarageFinish, GarageQual, GarageType, Heating, HeatingQC, HouseStyle, KitchenQual, LandContour,
        LandSlope, LotConfig, LotShape, MSZoning, MasVnrType, MiscFeature, Neighborhood, PavedDrive, PoolQC, RoofMatl,
        RoofStyle, SaleCondition, SaleType, Street, Utilities,
        
        we can intially see that our SalesPrice in left skewed which Indicates that the majority of prices
        are below the average price.
   
   2. Missing Values
         We should drop features like;
            PoolQC 
            MiscFeature 
            Alley 
            Fence 
            Fireplace Qu.
            Having missing values more than 1000 variables and the major cause of outliers. 
        Secondly Replacing missing value with mode of Qualitative data 
            Mszoning
            Electrical
            SaleType
            Exterior1st
            Exterior2nd
            KitchenQual
            filling zero for numerical data
         Lastly Filling missing values with subgrouping lotfrontage and neighborhood and filing median against it of each class.
    3. Normality and standerdizing
         Some features of data shows high skewness In this case,the square-root transformation may help to make the variances more
         constant throughout the study area and often makes the data appear normally distributed as well.
    4. Principal component analysis (PCA):is a statistical procedure that uses an orthogonal transformation to convert a set of       
         observations of possibly correlated variables into a set of values of linearly uncorrelated variables called principal 
         components.
    5.Using Advanced regression techniques to predict and analysing the rsquare value and mean square residual error.
          

