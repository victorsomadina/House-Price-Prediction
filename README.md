# House Price Prediction - A machine learning project 
This is a hackathon project develop a predictive model that accurately estimates house prices based on a comprehensive set of relevant variables
More details about the hackathon is shown [here](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)

# Data Cleaning
Null values which appeared to be the one of the significant issues with the dataset was dealt by filling with appropriate values such as mean. 

# Exploratory Data Analysis
![download (3)](https://github.com/victorsomadina/House-price-prediction-using-random-forest/assets/103338741/d358979d-fbb4-4235-8d51-d82bcd8dd197)
The image shows the distribution of important variables. I found that variables like GrLivArea and 1stFlrsf are not normally distributed which can have a significant effect to the model. These variables was normalized using log transformation to better fit the model and improve validation score. 
# Feature importance
This was determined using mutual info regression model. This model accepts just numerical variables so converting categorical variable to numerical variable was an important step. This was done using the Factorize function. The base model was built on the result of this model showing the most important variables that is variables with significant relationship to the dependent variable (Sale Price).
![download (4)](https://github.com/victorsomadina/House-price-prediction-using-random-forest/assets/103338741/e02bbb74-c66a-48fb-baa0-935b4317a928)
# Model Training
XGBoost regressor model was used to build the prediction model which gave a validation score of 0.13. Note: **Feature Engineering** was carried out to improve model performance.
Find the link to the Python code attached 




