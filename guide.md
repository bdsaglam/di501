
## Workflow

- Read dataset description
- Identify continuous and categorical variables
- Check number of unique values for each variable. This can give an idea about data 
- Check dataset statistical properties
cleanliness. If there is a deviation from dataset description, it means there are some data
points recorded/written wrong.
- Check missing values
    - Use `missingno` library to visualize missing values correlation
- Cleanup data
    - Clean typos
    - Remove non-sense data points 
    - Map categories
    - Transform variables with pandas `apply` function
- Visualize variables' histogram
- Visualize correlations between variables
- Split dataset into train and validation sets
    - 80:20 is a common ratio
- Determine imputation method for each variable and build pipelines
using train set.
- When building a pipeline, `ColumnTransformer` with indices of variables/columns
are very practical.


## Data quality
