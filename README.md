## Diabetes Predictor API


This is a Flask-based web application that provides a simple API for predicting diabetes based on input features. The application uses a pre-trained machine learning model to make predictions.

# Project Structure

- app.py: This file contains the main Flask application code, including routes for the homepage and the API endpoint for diabetes prediction.
- Model: This directory should contain the pre-trained machine learning model (modelForPrediction.pkl) and the standard scalar (standardScalar.pkl) used for data preprocessing.
- templates: This directory contains the HTML templates used for rendering the web pages.

    - index.html: The HTML template for the homepage, which welcomes users to the website.
    - single_prediction.html: The HTML template for displaying the prediction result.

## How to Run the Application

1. Clone this repository to your local machine.

    git clone https://github.com/Mohammad-Aadil/diabetes-prediction-api.git
    cd diabetes-prediction-api

1. Install the required Python packages:

    pip install flask numpy pandas scikit-learn

1. Download the pre-trained model and standard scalar files and place them in the Model directory.
2. Run the application:

    python app.py

1. The application should now be running locally at http://localhost:5000/.

## Usage

Homepage

Visit http://localhost:5000/ to access the homepage, where users are welcomed to the website.

Diabetes Prediction API
To use the prediction API, submit a POST request to http://localhost:5000/predictdata with the following parameters:

- Pregnancies: Number of pregnancies.
- Glucose: Glucose level.
- BloodPressure: Blood pressure.
- SkinThickness: Skin thickness.
- Insulin: Insulin level.
- BMI: Body Mass Index (BMI).
- DiabetesPedigreeFunction: Diabetes pedigree function.
- Age: Age of the person.

The API will return a prediction indicating whether the person is "Diabetic" or "Non-Diabetic."

## Contributing
Contributions are welcome! If you find any issues or want to add new features, feel free to open an issue or submit a pull request.



## Acknowledgments
- This project is based on a machine learning model trained on the Diabetes dataset.
- Thanks to the Flask community for the web framework.
- This project employs logistic regression, a powerful machine learning algorithm used for binary classification tasks, to predict diabetes.
- Logistic regression is widely used in the medical and healthcare domains for predicting and diagnosing various medical conditions, including diabetes.
- The logistic regression model used in this project was trained on a carefully curated dataset containing relevant features to make accurate predictions.
- The model's performance and accuracy were validated through rigorous testing and evaluation to ensure reliable results.
- Special thanks to the scikit-learn library for providing efficient and easy-to-use tools for implementing logistic regression in Python.
- The use of logistic regression showcases the power and simplicity of linear models in solving classification problems, making it an excellent choice for this application.