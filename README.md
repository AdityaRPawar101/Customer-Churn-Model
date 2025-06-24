# 🚀 Customer Churn Prediction Web App

**A Flask-powered web application that predicts customer churn using a trained machine learning model.**

---

## 🧠 Overview

Predicting whether a customer is likely to churn is vital for retention strategies and revenue growth. This project:

- Allows users to input customer data via a web form  
- Loads a pre-trained pickle model and matching feature schema (from `columns.json`)  
- Outputs a probability score and churn/no-churn label  

Ideal for internal analysts or customer success teams aiming to proactively intervene and retain at-risk customers.

---

## ⚙️ Features

- **Interactive Form** – Input key customer metrics including `tenure`, `gender`, `coupon used`, and more.  
- **Real-time Prediction** – Returns churn probability and label instantly.  
- **Extensible Architecture** – Plug in updated models or feature columns easily.  
- **Lightweight & Containerizable** – Perfect fit for Docker/Kubernetes deployment.

---

<pre lang="markdown"> ## 📦 Project Structure ``` Customer-Churn-Model/ ├── app.py # Main Flask app ├── templates/ # HTML templates for web interface │ ├── index.html # Input form page │ └── result.html # Result display page ├── models/ │ ├── churn_prediction_model.pkl # Pre-trained ML model │ └── columns.json # Feature columns used by model ├── static/ # (Optional) Static files like CSS/JS └── README.md # Project documentation ``` </pre>


---

## 📝 Usage Instructions

### Requirements

- Python 3.7+  
- Install dependencies:
  ```bash
  pip install flask numpy scikit-learn

### Run Locally
Ensure models/ contains both .pkl and .json files.
Start the server:
--export FLASK_ENV=development
--python app.py
Visit http://localhost:5000
Fill the form -> submit -> view churn prediction.
