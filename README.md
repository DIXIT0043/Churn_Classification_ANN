Churn Prediction Model with ANN
This project demonstrates a Churn Prediction system using an Artificial Neural Network (ANN). The model predicts whether a customer is likely to churn based on a set of features, and the application is deployed using Streamlit to provide an interactive and user-friendly web interface.

Table of Contents
Project Overview
Features
Installation
Usage
Model Architecture
Streamlit App
Dependencies
Contributing
License
Project Overview
Customer churn is a critical issue for businesses, and predicting churn helps in retaining customers. This project builds a churn prediction model using an ANN that is capable of predicting whether a customer will churn based on the available data. The model is integrated into a Streamlit application that allows users to interact with the model and view predictions.

Features
Artificial Neural Network for predicting churn.
Streamlit Web Application for easy model interaction.
Upload customer data as CSV and get real-time predictions.
Visualize input features and model predictions through the app.
Installation
To set up and run the project locally, follow the steps below:

Clone the Repository
bash
Copy code
git clone https://github.com/DIXIT0043/Churn_Prediction_Project.git
cd churn-prediction-ann
Set Up the Environment
Ensure you have Python 3.8+ installed.
Install the required dependencies by running:
bash
Copy code
pip install -r requirements.txt
Install Streamlit
bash
Copy code
pip install streamlit
Install TensorFlow (for ANN)
bash
Copy code
pip install tensorflow
Model Training (Optional)
If you want to retrain the ANN model:

Ensure you have your dataset in data/ folder.
Run the following to train and save the model:
bash
Copy code
python train_model.py
Usage
Running the Streamlit App
To launch the Streamlit app for churn prediction, run:

bash
Copy code
streamlit run app.py
This will open the app in your web browser, where you can:

Upload customer data in CSV format.
Get predictions for whether customers will churn.
View a summary of the model's prediction probabilities.
App Interface
Upload Section: Upload your dataset in CSV format.
Prediction: View churn prediction results for each customer.
Visualization: See input data features visualized for better understanding.
Model Architecture
The ANN model was built using TensorFlow/Keras and consists of:

Input Layer: Takes in customer features like tenure, monthly charges, etc.
Hidden Layers: Two hidden layers with 64 neurons each, using ReLU activation.
Output Layer: A single output neuron using Sigmoid activation for binary classification (churn or no churn).
The model is trained on historical customer data with the goal of predicting the likelihood of churn.

Model Parameters
Optimizer: Adam
Loss: Binary Crossentropy
Metrics: Accuracy
Streamlit App
The web interface is built using Streamlit, providing a simple and interactive platform for users to upload their data and get predictions.

Key functionalities of the Streamlit app:

CSV Upload: Uploaded a CSV file containing customer data.
Predictions: The model processes the data and outputs whether each customer is likely to churn or not.
Visualization: Graphs are displayed for a better understanding of feature distributions.
Dependencies
Python 3.8+
TensorFlow 2.0+
Pandas
NumPy
Scikit-learn
Streamlit
Matplotlib/Seaborn (for visualizations)
You can find all dependencies listed in the requirements.txt file.

Contributing
Feel free to open issues or submit pull requests if you have ideas for improvements or bug fixes.
