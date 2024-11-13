
#Weather Classification and Prediction

This project implements a weather classification and prediction system using various machine learning models, such as K-Nearest Neighbors (KNN), Support Vector Classifier (SVC), and Gaussian Naive Bayes. The dataset used for this project includes weather-related features such as temperature, humidity, wind speed, precipitation, atmospheric pressure, UV index, visibility, cloud cover, season, and location.


Project Overview

The main objective of this project is to classify the type of weather based on the given features and to provide an interactive prediction function using a trained machine learning model. The prediction is based on user input, where the model forecasts the weather type (e.g., overcast, partly cloudy, clear, etc.) using the provided atmospheric conditions.


Key Features

Data Preprocessing: The data is cleaned by handling missing and duplicate values, and categorical columns are encoded using Label Encoding and OneHotEncoding.

Feature Scaling: All numeric features are scaled using Min-Max Scaler to improve model performance.

Model Training: Multiple machine learning models (KNN, SVC, Gaussian Naive Bayes) are trained and evaluated using the classification report to compare their performance.

Interactive Prediction Function: A user-friendly function weatherprediction() allows users to input weather parameters and receive a predicted weather type.


Project Workflow

Data Loading: The weather dataset is loaded into a DataFrame using Pandas.

Data Cleaning: Handling missing and duplicate values and analyzing feature distributions.

Data Encoding: Label Encoding for the target variable and OneHotEncoding for categorical features (cloud cover, season, and location).

Feature Scaling: Applying Min-Max Scaler to scale the numeric features.

Model Training and Evaluation: Training KNN, SVC, and Gaussian Naive Bayes models and evaluating their performance on the test data.

Weather Prediction: An interactive function takes user input and predicts the weather type.

Requirements

Python 3.7+
Libraries: pandas, numpy, scikit-learn

How to Use

Clone the Repository:
bash
Copy code
git clone https://github.com/your-username/weather-classification-prediction.git
Install Dependencies:
bash
Copy code
pip install -r requirements.txt

Run the Script:

You can execute the Python script to train models and make predictions.
Use the weatherprediction() function for interactive weather type prediction.

Example Prediction

Run the script and input the following details when prompted:
mathematica

Copy code

Enter temperature: 30
Enter humidity: 77
Enter wind speed: 5.5
Enter precipitation: 28
Enter atmospheric pressure: 1012.69
Enter UV index: 3
Enter visibility: 9
Enter cloud cover (overcast, partly cloudy, clear, cloudy): overcast
Enter season (Winter, Spring, Autumn, Summer): Autumn
Enter location (inland, mountain, coastal): coastal

The script will output the predicted weather type.

Future Enhancements

Integrate additional models to improve prediction accuracy.
Implement more advanced feature engineering techniques.
Develop a web interface using Flask or Streamlit for easier user interaction.
