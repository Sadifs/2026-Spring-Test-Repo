# Titanic Survival Predictor 

## Course Information
**Course:** BSAN 6070 – Machine Learning & Analytics  
**Instructor:** Dr. Arin Brahma  
**Institution:** Loyola Marymount University  

---

## Overview
This project is a machine learning-powered web application that predicts whether a passenger would have survived the Titanic disaster based on key personal and travel attributes.

The application is built using Streamlit and a pre-trained classification model, enabling users to interactively input passenger details and receive real-time predictions.

---

## Problem Statement
Using historical Titanic passenger data, the objective is to develop a predictive model that determines survival outcomes based on features such as:
- Passenger class  
- Gender  
- Age  
- Family relationships aboard  
- Fare paid  

---

## Features
- Interactive web interface built with Streamlit  
- Real-time survival predictions  
- User-friendly input controls  
- Lightweight and easy to run locally  

---

## Application Inputs
Users provide the following details:
- Gender  
- Age  
- Ticket Class (Pclass)  
- Number of Siblings/Spouses Aboard (SibSp)  
- Number of Parents/Children Aboard (Parch)  
- Fare  

---

## Model Details
- Model Type: Classification (scikit-learn)  
- Serialized Model: titanic_predictor.sav  

### Input Features
- Pclass  
- Sex (Female = 1, Male = 0)  
- Age  
- SibSp  
- Parch  
- Fare  

### Output
- 1 → Survived  
- 0 → Did Not Survive  

---

## Project Structure
2026-Titanic-Predictor/  
├── app.py                  # Streamlit application  
├── titanic_predictor.sav   # Trained ML model  
├── Titanic_Data.csv        # Dataset  
├── requirements.txt        # Dependencies  
└── README.md               # Documentation  

---

## Installation & Setup

1. Clone the repository
git clone https://github.com/your-username/2026-Titanic-Predictor.git  
cd 2026-Titanic-Predictor  

2. Install dependencies
pip install -r requirements.txt  

3. Run the application
streamlit run app.py  

---

## Dependencies
- streamlit==1.50.0  
- scikit-learn==1.6.1  

---

## Key Implementation Details
- Model is loaded using Python’s pickle library  
- User inputs are transformed into a feature vector  
- Gender encoding:
  - Female → 1  
  - Male → 0  
- Prediction is generated using model.predict([features])  

---

## Future Improvements
- Add model evaluation metrics (Accuracy, F1-score)  
- Include feature importance visualization  
- Deploy the app (Streamlit Cloud / AWS)  
- Enhance feature engineering (e.g., family size, titles)  
- Add prediction probabilities  

---

## Author
Sadaf Sarbazi  
MS Business Analytics – Loyola Marymount University  

---

## Notes
This project demonstrates:
- End-to-end machine learning workflow  
- Model deployment using Streamlit  
- Application of classification models to real-world data  
