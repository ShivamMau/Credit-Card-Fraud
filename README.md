# Credit-Card-Fraud

This project aims to develop a machine learning pipeline for detecting fraudulent credit card transactions. The dataset consists of labeled transactions, with a highly imbalanced class distribution (fraudulent vs. legitimate transactions). The solution involves preprocessing the data, applying feature engineering techniques, and training a logistic regression model. The trained model is then deployed via a Flask web application, allowing real-time predictions for new transactions. This end-to-end pipeline is packaged for easy deployment, including all necessary files for training, evaluation, and prediction

# Project Components
Data Preprocessing: Data cleaning, feature engineering, and balancing techniques like SMOTE to handle the class imbalance.
Model Training: Logistic Regression model trained on balanced data.
Model Evaluation: Performance evaluation using metrics such as ROC-AUC, Precision, Recall, and F1-score.
Model Deployment: A Flask web application to serve the trained model for fraud detection predictions.
Model Serialization: The trained model and scaler are saved for later use in predictions.

# Installation
1. Clone the repository or download the project files:
   [(https://github.com/ShivamMau/Credit-Card-Fraud-Project)
   cd fraud_detection_project](https://github.com/ShivamMau/Credit-Card-Fraud-Project)
   

# Running the Project
1. Running the Flask API
To serve the trained fraud detection model via a Flask web application, run:python app.py
2. Making Predictions
Send a POST request to the /predict endpoint with transaction data as a JSON object: curl -X POST -H "Content-Type: application/json" -d '{"features": [31282.0, 0.963593, -0.437060, ...]}' http://127.0.0.1:5000/predict
3. Model Training
To retrain the model on new data, run the train_model.py script:python train_model.py


# Benefits for the Company
Real-time Fraud Detection: By integrating this solution into the company’s transaction systems, fraudulent transactions can be flagged in real-time, preventing financial loss.
Scalability: The solution is scalable for processing large volumes of transactions, making it suitable for a wide range of financial platforms.
Cost Efficiency: Automating the fraud detection process reduces the need for manual review, saving time and resources.
Accuracy: Using machine learning techniques like logistic regression, along with handling imbalanced data, ensures high detection accuracy and minimizes false positives, maintaining customer trust.
