## Customer Churn Prediction
This project is a Customer Churn Prediction web application built using Streamlit, TensorFlow, and Scikit-learn. The model predicts the probability of a customer churning based on user-provided input.

## Features
Predicts the likelihood of a customer churning based on input data.
Utilizes a pre-trained TensorFlow model to make predictions.
Encodes categorical variables (Gender, Geography) and scales input data using pre-loaded encoders and a scaler.
Displays the churn probability and indicates whether the customer is likely to churn.
## Installation
To run this application locally, follow these steps:

1. Clone the repository
```bash
git clone https://github.com/DIXIT0043/Churn_Classification_ANN
```
## Install the required libraries
2. Use pip to install the dependencies:
```bash
pip install streamlit tensorflow scikit-learn pandas numpy
```
## Prepare the model and encoders
Make sure you have the following files in your project directory:

model.h5: The pre-trained Keras model for churn prediction. label_encoder_gender.pkl: Pre-fitted label encoder for the Gender column. onehot_encoder_geo.pkl: Pre-fitted one-hot encoder for the Geography column. scaler.pkl: Pre-fitted scaler for input data normalization.

## Run the application
Run the Streamlit app by using the following command:
````bash
streamlit run app.py
````
## Usage
Provide input for: Geography: Select the customer's country. Gender: Choose the gender of the customer. Age: Specify the age of the customer (18 to 92 years). Balance: Enter the customer's account balance. Credit Score: Input the customer's credit score. Estimated Salary: Provide the customer's estimated salary. Tenure: Specify the tenure (years as a customer). Number of Products: Select the number of products held by the customer. Has Credit Card: Indicate whether the customer has a credit card (0 or 1). Is Active Member: Specify whether the customer is an active member (0 or 1). Click Submit to see the churn probability.

The application will display the churn probability and whether the customer is likely to churn. File Descriptions

app.py: The main Streamlit application file. model.h5: Pre-trained TensorFlow model used for prediction. label_encoder_gender.pkl, onehot_encoder_geo.pkl, scaler.pkl: Pre-trained encoders and scaler used to process input data.

## Example
A sample prediction for a customer:

Geography: France Gender: Male Age: 35 Credit Score: 750 Balance: 20000 Estimated Salary: 50000 Tenure: 5 years Number of Products: 2 Has Credit Card: Yes Is Active Member: Yes