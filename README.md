Trying Different Methods to Deal with Missing Data

One of the main challenges we encountered during our analysis was the presence of missing values in the dataset. In order to address this issue, we explored various techniques for imputing missing data, particularly focusing on methods suitable for univariate analysis
We employed various imputation methods on the EuStockMarkets dataset available in R and selected the best method based on the Root Mean Square Error (RMSE). Here is a summary of the methods we used:

Mean Imputation: We replaced missing values with the mean of the variable.
Median Imputation: We replaced missing values with the median of the variable.
Forward Imputation: We used the next observed value to fill in missing values.
K-Nearest Neighbors (KNN) Imputation: We imputed missing values by considering the values of the nearest neighbors based on a similarity measure.
Linear Regression Imputation: We used a linear regression model to estimate missing values based on the relationship with other variables.
Moving Average Imputation: We replaced missing values with the average of neighboring values.
MICE (Multivariate Imputation by Chained Equations): We employed the MICE library, which uses a "brute force" method by creating multiple imputed datasets.
Decision Tree Imputation: We used a decision tree algorithm to predict missing values based on other variables.
Random Forest Imputation: We employed the random forest algorithm to impute missing values by considering the relationships between variables.
Interpolation: We used different interpolation techniques, including linear, cubic spline, and ruled, to estimate missing values based on the trend and shape of the data.
After applying these methods, we evaluated their performance using RMSE. The method with the lowest RMSE was considered the best for our purpose.

It's worth noting that the choice of imputation method should be carefully considered based on the specific characteristics of the dataset and research objectives
