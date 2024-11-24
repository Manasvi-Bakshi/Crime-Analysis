# Crime Data Prediction and Analysis

This project uses machine learning models, including Decision Tree, Random Forest, K-Nearest Neighbors, and Support Vector Machine, to predict crime trends in Himachal Pradesh, focusing on crimes against Scheduled Castes (SC), Scheduled Tribes (ST), children, and women. By analyzing historical crime data, the goal is to uncover patterns and gain insights that can inform crime prevention strategies and policy decisions across the state.

## Dataset Used
The data was sourced from the [CKAN portal](https://ckan.himdataportal.com/dataset/crime-statistics), providing insights into crime trends and distributions across multiple years. Each dataset spans multiple years and includes crime records by district. We analyzed the following datasets:
- Crimes Against Scheduled Castes (SC)
- Crimes Against Scheduled Tribes (ST)
- District Wise Crimes Against Children
- District Wise Crimes Against Women

### Key Data Visualizations

- **Line Graphs**: Show crime trends over time, aggregated by year and district.
- **Histograms**: Visualize the distribution of crimes by year.
- **Heatmaps**: Display correlations between different crime types across the dataset.
- **Pie Charts**: Illustrate the distribution of crime types within each category.
- **Box Plots**: Identify outliers in the data using the Interquartile Range (IQR) method.

### Data Preprocessing

- **Data Integration**: All four datasets were merged into a single dataset for a unified analysis.
- **Feature Reduction**: Similar crime categories were grouped together for a more streamlined analysis (e.g., "Assault" and "Harassment").
- **Handling Missing Data**: Missing values were replaced with zero to ensure consistency.
- **Outlier Detection**: Outliers were identified using the IQR method and visualized with box plots.

## Models Used

This project uses the following machine learning models for regression:

1. **Decision Tree Regressor** - A decision tree-based algorithm that splits data into branches to make predictions.
2. **Random Forest Regressor** - An ensemble method based on multiple decision trees to reduce overfitting and improve accuracy.
3. **K-Nearest Neighbors Regressor (KNN)** - A simple algorithm that predicts the target variable based on the k-nearest training data points.
4. **Support Vector Machine Regressor (SVM)** - A linear regression model that finds the optimal hyperplane to minimize error.

### Evaluation Metrics

We evaluate the performance of the models using the following metrics:

- **Mean Absolute Error (MAE)**: The average of absolute differences between predicted and actual values.
- **Mean Squared Error (MSE)**: The average of squared differences between predicted and actual values.
- **Root Mean Squared Error (RMSE)**: The square root of MSE, interpretable in the same units as the target variable.
- **R² Score**: The proportion of variance explained by the model. A perfect score is 1.0.
- **Explained Variance Score**: Measures how well the model explains the variance in the target variable.

### Performance Visualization

We compared the models' performance visually by plotting the following:

- **MAE, MSE, RMSE**: These metrics were plotted together to compare how the models performed in terms of error.
- **R², Explained Variance**: These metrics were plotted separately to assess the models' predictive accuracy and variance explanation.




