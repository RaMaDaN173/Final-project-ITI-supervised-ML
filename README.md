## Heart Attack Prediction Project

### Overview
This project aims to develop a web application that predicts the risk of a heart attack based on various health parameters. It uses machine learning models to analyze the provided data and make predictions. The application is built using Flask for the backend, and it integrates a pre-trained machine learning pipeline.

### Dataset
The dataset used in this project is a heart disease dataset containing several health-related attributes:
- Age
- Sex
- Chest Pain Type (cp)
- Resting Blood Pressure (trtbps)
- Cholesterol (chol)
- Fasting Blood Sugar (fbs)
- Resting Electrocardiographic Results (restecg)
- Maximum Heart Rate Achieved (thalachh)
- Exercise Induced Angina (exng)
- ST Depression Induced by Exercise (oldpeak)
- Slope of the Peak Exercise ST Segment (slp)
- Number of Major Vessels (caa)
- Thalassemia (thall)
- Output (target variable indicating heart attack risk)

### Project Structure
The project is divided into several steps:

1. **Loading and Exploring Data:**
   - Loading the dataset
   - Displaying the data information and statistics
   - Visualizing distributions using pair plots

2. **Data Preprocessing:**
   - Defining features and target variables
   - Scaling numeric features using `StandardScaler`

3. **Model Pipelines:**
   - Building pipelines for various machine learning models including SVM (linear and polynomial), Logistic Regression, KNN, Decision Tree, Linear Regression, and Random Forest
   - Each pipeline integrates preprocessing and classification/regression steps

4. **Training and Evaluation:**
   - Splitting the data into training, validation, and test sets
   - Training and evaluating each model
   - Displaying confusion matrices and classification reports
   - Selecting the model with the highest accuracy

5. **Saving the Model:**
   - Saving the best-performing model pipeline using `joblib`
   - In this project, the model that achieved the highest accuracy was **[model name]** with an accuracy of **[accuracy percentage]**.

6. **Web Application:**
   - Creating a Flask web application to serve the model
   - Designing a user-friendly HTML form for inputting health parameters
   - Making predictions and displaying results on the web page

### Files
- `heart.csv`: The dataset file.
- `model_pipeline.py`: Contains the code for data loading, preprocessing, model training, evaluation, and saving.
- `app.py`: The Flask application file.
- `templates/index.html`: HTML template for the web application.
- `static/styles.css`: CSS file for styling the web application.
- `static/script.js`: JavaScript file for handling form submission and displaying predictions.

### Usage
1. **Data Preparation and Model Training:**
   - Run the `model_pipeline.py` script to load the data, preprocess it, train various models, evaluate them, and save the best model pipeline.
   
2. **Web Application:**
   - Run the `app.py` script to start the Flask web server.
   - Open a web browser and navigate to `http://127.0.0.1:5000/`.
   - Enter the health parameters in the form and submit to get the heart attack risk prediction.

### Requirements
- Python 3.x
- Pandas
- Seaborn
- Matplotlib
- Scikit-learn
- Flask
- Joblib

### Contributors
- Mohamed Ramadan
- Gohar Hany
- Ahmed Ashraf
- Omar Ayman

### License
This project is licensed under the MIT License.

### Conclusion
This project demonstrates how to build a machine learning pipeline, evaluate different models, and deploy a predictive model as a web application. It provides a practical approach to solving health prediction problems using machine learning techniques. The best-performing model in this project was **KNN**, which achieved an accuracy of **90%**.
