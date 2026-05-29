# ✈️ Flight Price Prediction using AWS SageMaker

## 📌 Project Overview

This project predicts airline ticket prices using Machine Learning and AWS SageMaker.

The complete pipeline includes:

* Data preprocessing and feature engineering
* Feature selection
* Hyperparameter tuning using AWS SageMaker
* XGBoost model training
* Streamlit web application for real-time predictions

The goal of this project is to provide accurate flight fare predictions based on airline, source, destination, travel date, duration, stops, and additional flight information.

---

## 🚀 Tech Stack

### Machine Learning

* Python
* Scikit-Learn
* XGBoost
* Feature Engine

### Cloud Services

* AWS SageMaker
* Amazon S3

### Deployment

* Streamlit

---

## 📂 Project Structure

```text
flight_sagemaker_project/
│
├── app.py
├── requirements.txt
├── preprocessor.joblib
├── README.md
│
├── model/
│   └── xgboost-model-v2.json
│
├── data/
│   ├── train.csv
│   ├── val.csv
│   └── test.csv
│
└── notebooks/
```

---

## ⚙️ Machine Learning Pipeline

### Data Preprocessing

The preprocessing pipeline includes:

* Missing value treatment
* Rare category encoding
* One-Hot Encoding
* Mean Encoding
* Feature Scaling
* Outlier Treatment using Winsorization
* Datetime Feature Extraction
* Custom Feature Engineering

---

### Feature Selection

Feature selection was performed using:

* Random Forest Regressor
* SelectBySingleFeaturePerformance

This helped retain only the most informative features for model training.

---

## 🤖 Model Training

The model was trained using:

* AWS SageMaker
* XGBoost Regressor

Hyperparameter tuning was performed using Bayesian Optimization.

### Tuned Parameters

* Learning Rate (eta)
* Alpha
* Maximum Depth

---

## 🌐 Web Application

The Streamlit application allows users to:

* Select Airline
* Choose Source and Destination
* Enter Journey Date
* Enter Departure and Arrival Time
* Specify Flight Duration
* Enter Number of Stops
* Predict Flight Ticket Price Instantly

---

## ▶️ Running the Project

### Clone Repository

```bash
git clone <your-repository-url>
cd flight_sagemaker_project
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Streamlit App

```bash
streamlit run app.py
```

---

## 📊 Sample Prediction Workflow

1. User enters flight details
2. Preprocessor transforms the input
3. XGBoost model generates prediction
4. Streamlit displays estimated ticket price

---

## 🔮 Future Improvements

* Containerization using Docker
* CI/CD Pipeline
* AWS Endpoint Deployment
* Real-Time Flight Data Integration
* Model Monitoring and Retraining

---

## 👩‍💻 Author

**Kashish**

Machine Learning | Data Engineering | Generative AI Enthusiast


