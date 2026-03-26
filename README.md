# 🚀 Premium-Predictor – Insurance Premium Prediction System

An end-to-end Machine Learning project that predicts **insurance premium categories** based on user data.
Built using **Python, FastAPI, and Streamlit**, this system provides real-time predictions through an interactive web interface.

---

## 📌 Project Overview

Insurance companies determine premium prices based on multiple factors such as age, income, lifestyle, and health.

This project uses **Machine Learning** to automate and optimize this process by predicting the **premium category** of a user.

---

## ⚙️ Tech Stack

* **Backend:** FastAPI
* **Frontend:** Streamlit
* **Machine Learning:** Scikit-learn (Random Forest)
* **Data Processing:** Pandas, NumPy
* **Model Serialization:** Pickle / Joblib

---

## 🧠 Features

* 🔍 Real-time premium prediction
* ⚡ Fast API-based backend
* 🎯 Feature engineering (BMI, Lifestyle Risk, City Tier)
* 📊 Confidence score output
* 🖥️ Interactive Streamlit UI
* 🔄 End-to-end pipeline (data → model → API → UI)

---

## 📊 Feature Engineering

The model uses custom engineered features:

* **BMI** = Weight / Height²
* **Age Group** = Young / Adult / Middle-aged / Senior
* **Lifestyle Risk** = Based on smoking & BMI
* **City Tier** = Tier 1 / Tier 2 / Tier 3 classification

---

## 🏗️ Project Structure

```
PREMIUM-PREDICTOR/
│── backend/
│   ├── app.py
│   ├── model.pkl
│
│── frontend/
│   ├── frontend.py
│
│── model/
│   ├── insurance_model.py
│
│── data/
│   ├── insurance.csv
│
│── requirements.txt
│── README.md
```

---

## 🚀 How to Run the Project

### 🔹 Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/InsureAI.git
cd InsureAI
```

---

### 🔹 Step 2: Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 🔹 Step 3: Run FastAPI Backend

```bash
uvicorn main:app --reload
```

👉 API will run at:
`http://127.0.0.1:8000`

---

### 🔹 Step 4: Run Streamlit Frontend

```bash
streamlit run app.py
```

👉 App will open at:
`http://localhost:8501`

---

## 📡 API Endpoint

### 🔹 POST `/predict`

#### Request Example:

```json
{
  "age": 30,
  "weight": 70,
  "height": 1.75,
  "income_lpa": 10,
  "smoker": false,
  "city": "Mumbai",
  "occupation": "private_job"
}
```

#### Response Example:

```json
{
  "predicted_category": "medium",
  "confidence": 87.5
}
```

---

## 📈 Model Details

* Algorithm: **Random Forest Classifier**
* Preprocessing:

  * OneHotEncoding for categorical variables
  * Feature scaling (if applied)
* Pipeline: **ColumnTransformer + Model**

---

## 💼 Use Cases

* Insurance companies for premium estimation
* Health risk assessment systems
* Financial planning tools
* AI-based underwriting systems

---

## 🔥 Future Improvements

* Add regression model for exact premium prediction
* Deploy using AWS / Render
* Add SHAP for model explainability
* User authentication system
* Dashboard analytics

---

## 👨‍💻 Author

**Shubham Nanasaheb Dalvi** <br>
*Machine Learning & GenAI Enthusiast

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub!

---

