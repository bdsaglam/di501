
## Dataset

The categorical variables of which categories has an order are assumed as ordinal variables.
The rest of the categorical variables are assumed as nominal variables. For each variable,
the data type is as following:

\begin{table}[]
\begin{tabular}{lllllllll}
Variable      & DataType  & Variable     & DataType  & Variable     & DataType  & Variable     & DataType  &  \\
1stFlrSF      & numerical & 2ndFlrSF     & numerical & 3SsnPorch    & numerical & Alley        & nominal   &  \\
BedroomAbvGr  & numerical & BldgType     & nominal   & BsmtCond     & ordinal   & BsmtExposure & ordinal   &  \\
BsmtFinSF1    & numerical & BsmtFinSF2   & numerical & BsmtFinType1 & nominal   & BsmtFinType2 & nominal   &  \\
BsmtFullBath  & numerical & BsmtHalfBath & numerical & BsmtQual     & ordinal   & BsmtUnfSF    & numerical &  \\
CentralAir    & nominal   & Condition1   & nominal   & Condition2   & nominal   & Electrical   & nominal   &  \\
EnclosedPorch & numerical & ExterCond    & ordinal   & ExterQual    & ordinal   & Exterior1st  & nominal   &  \\
Exterior2nd   & nominal   & Fence        & nominal   & FireplaceQu  & ordinal   & Fireplaces   & numerical &  \\
Foundation    & nominal   & FullBath     & numerical & Functional   & nominal   & GarageArea   & numerical &  \\
GarageCars    & numerical & GarageCond   & ordinal   & GarageFinish & nominal   & GarageQual   & ordinal   &  \\
GarageType    & nominal   & GarageYrBlt  & ordinal   & GrLivArea    & numerical & HalfBath     & numerical &  \\
Heating       & nominal   & HeatingQC    & ordinal   & HouseStyle   & nominal   & KitchenAbvGr & numerical &  \\
KitchenQual   & ordinal   & LandContour  & nominal   & LandSlope    & ordinal   & LotArea      & numerical &  \\
LotConfig     & nominal   & LotFrontage  & numerical & LotShape     & nominal   & LowQualFinSF & numerical &  \\
MSSubClass    & nominal   & MSZoning     & nominal   & MasVnrArea   & numerical & MasVnrType   & nominal   &  \\
MiscFeature   & nominal   & MiscVal      & numerical & MoSold       & ordinal   & Neighborhood & nominal   &  \\
OpenPorchSF   & numerical & OverallCond  & ordinal   & OverallQual  & ordinal   & PavedDrive   & nominal   &  \\
PoolArea      & numerical & PoolQC       & ordinal   & RoofMatl     & nominal   & RoofStyle    & nominal   &  \\
SaleCondition & nominal   & SalePrice    & numerical & SaleType     & nominal   & ScreenPorch  & numerical &  \\
TotRmsAbvGrd  & numerical & TotalBsmtSF  & numerical & Utilities    & nominal   & WoodDeckSF   & numerical &  \\
YearBuilt     & ordinal   & YearRemodAdd & ordinal   & YrSold       & ordinal   &              &           & 
\end{tabular}
\end{table}

## Data quality

There are varying number of missing values in each variable in the dataset. The variables
with missing values are:
PoolQC          1453
MiscFeature     1406
Alley           1369
Fence           1179
FireplaceQu      690
LotFrontage      259
GarageType        81
GarageYrBlt       81
GarageFinish      81
GarageQual        81
GarageCond        81
BsmtExposure      38
BsmtFinType2      38
BsmtFinType1      37
BsmtCond          37
BsmtQual          37
MasVnrArea         8
MasVnrType         8
Electrical         1

For the majority of the categorical variables, there is a category defined representing
missing value (`NA` or `None`) in the data description.
The missing values in those categorical variables are filled with the corresponding missing 
value determined. 
For the rest of the categorical variables, the most frequent value is used to impute missing values for those variables.
For numerical variables, the mean imputation is used.


`Street` variable's values are always 