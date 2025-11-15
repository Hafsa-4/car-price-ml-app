---
# 🚗 Car Price Prediction App

## 📌 Project Overview
This repository contains my **Final Year Project**: an end-to-end **Machine Learning pipeline** for predicting car prices based on user-input features.  
It demonstrates the full lifecycle of a data science project — from **data cleaning and exploratory data analysis (EDA)** to **model training and deployment** using **Streamlit**.

Users can interact with a web app to input car details and receive an estimated price powered by a trained **Random Forest Regressor**.

---

## 🛠️ Tech Stack
- **Python 3**
- **Pandas, NumPy** – data preprocessing
- **Scikit-learn** – model training (Random Forest, Linear Regression), Label Encoding
- **Matplotlib, Seaborn** – data visualization and EDA
- **Joblib** – model saving/loading
- **Streamlit** – web app deployment
- **Jupyter Notebook** – analysis and experimentation

---

## 📂 Repository Contents
```
final-project/
├── app.py                             # Streamlit app for prediction
├── car_price_model.pkl                # Trained Random Forest model
├── car_price_prediction.csv           # Cleaned dataset
├── car-price-prediction-with-randomforest.ipynb  # EDA & model training notebook
├── python script.py                   # Additional script (optional)
├── README.md                          # Project documentation
```

---

## 🔍 Data Preprocessing
- Removed duplicates and irrelevant columns (`ID`)
- Converted `Levy`, `Engine volume`, and `Mileage` to numeric types
- Engineered new feature: **Age of Car** from production year
- Encoded categorical variables using **LabelEncoder**
- Removed outliers using **IQR filtering**

---

## 📊 Exploratory Data Analysis (EDA)
- Histograms for numerical features
- Count plots for top categories
- Boxplots showing price variation across categories
- Correlation heatmap to identify feature relationships

**Key Insights:**
- Most cars have 4 cylinders
- Toyota and Hyundai are the most frequent manufacturers
- Petrol engines and automatic gearboxes dominate
- Price is influenced by age, engine volume, and wheel type

---

## 🤖 Model Training
- Target variable: `Price`
- Features: All relevant numeric and encoded categorical columns
- Models used:
  - **Random Forest Regressor** (final model)
  - Linear Regression (baseline)
- Evaluation metrics:
  - **R² Score**
  - **Mean Squared Error (MSE)**

---

## 🌐 Streamlit App
The app allows users to:
- Select car attributes via dropdowns and sliders
- Input numeric values like mileage, engine volume, and levy
- Click a button to predict the car price using the trained model

**To run the app:**
```bash
streamlit run app.py
```

---

## 📈 Results
- Random Forest achieved high accuracy and generalization
- Real-time predictions via Streamlit interface
- Demonstrates full ML workflow: **data → model → deployment**

---

## 🎯 Learning Outcomes
- Built a complete ML pipeline from scratch
- Applied EDA to extract insights and guide feature selection
- Trained and evaluated models using industry-standard metrics
- Deployed a user-friendly app with Streamlit
- Strengthened skills in **Python, ML, and deployment workflows**
```
