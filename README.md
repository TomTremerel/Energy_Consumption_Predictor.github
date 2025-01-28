# Energy_Consumption_Predictor.github

## Report ##

This dataset describe the energy consumption of a population on one year. 
The link of the dataset : https://www.kaggle.com/datasets/ajinilpatel/energy-consumption-prediction

### 1. Data Exploration and Visualization

Checks for missing values and duplicates, revealed that the dataset was clean in this regard.
Scatter plots were used to visualize the relationships between variables and histograms and KDE plots were employed to understand the distribution of Energy Consumption and Temperature.


Line plots illustrated the monthly trends of Temperature and Energy Consumption, highlighting potential seasonality.

 A correlation matrix and heatmap were generated to identify the strength and direction of relationships between numerical features. Strong correlations were observed between Energy Consumption, Temperature, HVAC Usage, and Lighting Usage.


 ### 2. Data Preprocessing and Feature Engineering

 Categorical features (DayOfWeek, Holiday, HVACUsage, LightingUsage) were encoded using Label Encoding to convert them into numerical representations for model training.
 The dataset was split into training and testing sets using train_test_split to evaluate the performance of the trained models.
 Numerical features were scaled to ensure that they have a similar range and prevent features with larger values from dominating the model.


 ### 3. Model Training and Evaluation

I trained a model to predict the energy consumption even if it was not asked in this exercise.  
Two regression models were trained to predict Energy Consumption: Random Forest Regressor and Linear Regression.
The models were evaluated using metrics such as Root Mean Squared Error and R-squared score. Random Forest Regressor exhibited better performance with a lower RMSE and a higher R^2 score compared to Linear Regression.

### 4. SQL part

The dataset was transformed into a relational database using SQLAlchemy. This allowed for performing SQL queries on the data, providing additional flexibility in data exploration and analysis. I encountered some difficulties for this part. 
