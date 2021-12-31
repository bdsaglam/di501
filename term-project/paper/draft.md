
## Data quality


There are varying number of missing values in each variable in the dataset. The variables
with most number of missing values are:
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