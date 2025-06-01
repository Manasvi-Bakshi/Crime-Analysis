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

1. **Decision Tree Regressor**
2. **Random Forest Regressor** 
3. **K-Nearest Neighbors Regressor (KNN)** 
4. **Support Vector Machine Regressor (SVM)** 

### Evaluation 

| Model         | MAE  | MSE    | RMSE  | R² Score | Explained Variance |
|---------------|------|--------|-------|----------|---------------------|
| Decision Tree | 6.46 | 383.91 | 19.59 | 0.94     | 0.94                |
| Random Forest | 6.66 | 309.28 | 17.59 | 0.96     | 0.96                |
| KNN           | 6.53 | 659.79 | 25.69 | 0.90     | 0.91                |
| SVM           | 3.59 | 98.52  | 9.93  | 0.99     | 0.99                |


### Performance Visualization

We compared the models' performance visually by plotting the following:

- **MAE, MSE, RMSE**: These metrics were plotted together to compare how the models performed in terms of error.
- **R², Explained Variance**: These metrics were plotted separately to assess the models' predictive accuracy and variance explanation.

### Installation

Ensure all datasets from the **dataset** folder are added to your runtime environment, and verify that the file paths in the code match the location of these datasets. Once the paths are correctly configured, you can run all the cells seamlessly.


