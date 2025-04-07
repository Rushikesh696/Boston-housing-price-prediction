# Boston-housing-price-prediction

### **Overview**

- The Boston Housing Dataset is a well-known dataset often used for practicing machine learning and statistical analysis. It contains information about housing prices in Boston and the features (predictors) that might influence these prices.

### Data Cleaning

- Removing outliers is essential to ensure the data is more generalized, reducing the impact of extreme values that may distort the model. This step also helps in eliminating skewness, leading to a more balanced and representative dataset that improves the model's performance and predictive accuracy.

### EDA

- Performing univariate and bivariate analysis is crucial to understand the distribution and relationships within the data. In univariate analysis, we examine each feature individually to analyze its distribution and detect any potential outliers. We can use histograms and box plots to visualize the spread and central tendency of numerical features.In bivariate analysis, we investigate the relationships between pairs of features, focusing particularly on how each feature correlates with the target variable (housing prices).
- Scatter plots are ideal for visualizing the relationship between continuous variables, while bar charts can be used for categorical features to see how they impact the target.This analysis helps in identifying the strength and nature of each feature's relationship with the target variable, providing insights into which features most influence housing prices.

### Model preparation

- To prepare the data for machine learning, we begin by selecting the relevant features needed to predict housing prices. First, we inspect the unique values of each categorical feature and convert them into numerical representations using label encoding. This ensures that categorical variables are appropriately formatted for the algorithm. Once the features are selected and encoded, the data is ready to be fed into machine learning models for training and prediction.

### Training and testing

- First, we split the dataset into independent variables (features) and the dependent variable (target). After separating the target variable, we proceed to scale the independent variables using StandardScaler to standardize the data, ensuring all features are on the same scale, which improves the performance of the model.
Next, we split the data into training and testing sets using train_test_split, ensuring the model can be evaluated on unseen data. After splitting, we apply the Linear Regression algorithm to the training data, then use the trained model to make predictions on both the training and testing datasets.

### Model building

- Develop a Linear Regression model to predict housing prices by applying both simple regression (using one feature) and multiple regression (using multiple features). Additionally, implement polynomial regression to capture non-linear relationships in the data. This process helps build a robust predictive model and evaluate which regression method performs best in predicting housing prices.

### Conclusion

- The model is now ready to predict house prices based on the most correlated features, LSTAT (percentage of lower-status population) and RM (average number of rooms per dwelling). These two features significantly impact housing prices, with higher room counts generally correlating with higher prices and a higher percentage of lower-status population typically leading to lower prices. By focusing on these key features, the model is able to provide accurate predictions. Additionally, further feature engineering and model tuning could improve the accuracy of the predictions even more.
