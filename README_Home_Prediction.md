# Project Title: Housing Price Prediction Using Machine Learning
<samp>Notebook to project can be found here:</samp> <br>
https://github.com/WilliamHallPortfolio/01-Home_Price_Prediction/blob/main/Housing%20Price%20Prediction%20Final.ipynb <br>
<samp>Link to Google Colab environment provided to test code yourself.</samp>
<br>
### Objective:
This project aims to predict house prices based on features and amenities that are included within the property. This project involves data cleaning, feature selection, exploratory data analysis (EDA), and the implementation of a predictive model to accurately estimate house prices.
<p align="center">
<img src="https://media.istockphoto.com/id/1276901709/photo/beautiful-new-home-near-chicago.jpg?s=612x612&w=0&k=20&c=fA28eXUWXVGA-L8u3OBXLanr8U95xz1XA18kMjexK-A=" width="300" height="300" border="10"/>
</p>

### Dataset:
Source: The dataset consists of two CSV files: train.csv and test.csv. These files contain detailed information about houses, including various features such as LotFrontage, YearBuilt, GarageArea, and SalePrice (target variable).
Key Attributes:
SalePrice (Target): The price of the home (target variable).
Features include attributes like square footage (GrLivArea), number of bathrooms (FullBath), garage area (GarageArea), year built (YearBuilt), and more.
Methodology:
### 1. Data Preprocessing:
Handling Missing Values:
Missing data in numerical columns (e.g., LotFrontage, GarageYrBlt) were imputed using the median value.
For categorical columns, missing values were filled with the mode (most frequent value). Columns with a large proportion of missing data (over one-third missing) were dropped.
Log Transformation: The target variable SalePrice exhibited a right-skewed distribution, so a log transformation was applied to stabilize variance and reduce the impact of outliers.
### 2. Feature Selection:
SelectKBest: A feature selection technique was employed to identify the most relevant features for predicting housing prices. Features were selected based on their F-scores and p-values, which indicated their statistical significance in relation to the target variable.
Feature Engineering: After selecting the best features, the test set was preprocessed to match the training set in terms of selected features and data types.
### 3. Exploratory Data Analysis (EDA):
Correlation Heatmap: A heatmap was generated to examine the relationships between the selected features. Strongly correlated features helped in identifying potential predictors of housing prices.
Scatter Plots: Scatterplots were created for the top features to visualize their relationship with SalePrice, helping to better understand how each feature influences the target variable.
### 4. Modeling (Future Step):
Although not implemented in this notebook, the cleaned and transformed dataset is ready for model building using algorithms such as Linear Regression, Random Forest, or XGBoost to predict housing prices based on the selected features.
#### Results:
Data Cleaning: Missing values were handled effectively, with numerical and categorical imputation applied as needed.
Feature Selection: Statistically significant features were identified using SelectKBest, reducing dimensionality and improving model performance potential.
EDA: Visualizations such as heatmaps and scatterplots provided insights into the relationships between features and the target variable, preparing the data for predictive modeling.
Conclusion:
This project successfully cleaned the dataset, selected key features, and performed an exploratory analysis to understand the relationships between various house attributes and sale prices. The data is now prepared for modeling, which can be the next step to finalize a predictive model for housing price estimation.
