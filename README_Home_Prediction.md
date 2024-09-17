# Project Title: Housing Price Prediction Using Machine Learning
<samp>Notebook to project can be found here:</samp> <br>
https://github.com/WilliamHallPortfolio/01-Home_Price_Prediction/blob/main/Housing%20Price%20Prediction%20Final.ipynb <br>
<samp>Link to Google Colab environment provided to test code yourself.</samp>
<br>
### Objective:
This project aims to predict house prices based on features and amenities that are included within the property. This project involves data cleaning, feature selection, exploratory data analysis (EDA), and the implementation of a predictive model to accurately estimate house prices.
<p align="left">
<img src="https://images.unsplash.com/photo-1415604934674-561df9abf539?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2772&q=80](https://www.google.com/imgres?q=suburban%20house%20in%20a%20developement&imgurl=https%3A%2F%2Fmedia.gettyimages.com%2Fid%2F875403094%2Fphoto%2Faerial-shot-of-suburban-development.jpg%3Fs%3D612x612%26w%3Dgi%26k%3D20%26c%3DJV2w1k-qbY_-ndw8tbmGQ3xmqJQRGQKyfxkyI6jNF_4%3D&imgrefurl=https%3A%2F%2Fwww.gettyimages.com%2Fphotos%2Fsuburban-housing-development&docid=uqbmAVdRJXgvjM&tbnid=LdOdNaQ5TMVZGM&vet=12ahUKEwjV7fbV2MqIAxWlEFkFHeprGLMQM3oECG0QAA..i&w=612&h=459&hcb=2&ved=2ahUKEwjV7fbV2MqIAxWlEFkFHeprGLMQM3oECG0QAA)](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.centreforcities.org%2Fblog%2Fnew-homes-suburbs-housing-crisis%2F&psig=AOvVaw1n3A-lduo2ZT970HoZbP9z&ust=1726687057377000&source=images&cd=vfe&opi=89978449&ved=0CBQQjRxqFwoTCNj1rIPZyogDFQAAAAAdAAAAABAE)](https://media.istockphoto.com/id/1276901709/photo/beautiful-new-home-near-chicago.jpg?s=612x612&w=0&k=20&c=fA28eXUWXVGA-L8u3OBXLanr8U95xz1XA18kMjexK-A=)" width="100" height="100" border="10"/>
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
