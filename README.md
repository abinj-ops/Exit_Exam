# 🛍️ Shopping Behaviour Prediction Using Machine Learning

## 📌 Project Overview

This project focuses on predicting customers' preferred shopping modes using Machine Learning techniques. It analyses customer shopping behaviour, purchasing habits, spending patterns and other personal preferences to predict whether a customer prefers **Online, Offline, or Equal / both** shopping.

The project also includes a web application developed using **Flask**, allowing users to enter shopping behaviour details and receive predictions through a simple, user-friendly interface.

## 🎯 Project Objectives

- Analyse customer shopping behaviour using a dataset.
- Perform data cleaning and preprocessing.
- Build and train multiple Machine Learning classification models.
- Evaluate and compare model performance using different evaluation metrics.
- Identify important features influencing shopping preferences.
- Develop a Flask web application for real-time shopping mode prediction.

## 📂 Dataset Description

**Dataset:** `G1.csv`

The dataset contains 500 customer responses with information about:

- Age and gender
- Occupation status
- Country and monthly income range
- Online shopping frequency
- Preferred shopping platform
- Primary shopping device
- Spending category
- Price comparison and discount preferences
- Social media advertisement influence
- Payment methods
- Online shopping satisfaction
- Customer purchasing behaviour

**Target Variable:** `Best_Shopping_Mode`

The target variable contains three shopping categories:

1. Online
2. Offline
3. Equal / both

Rows with missing target values are excluded during model training.

## 🧰 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Flask
- HTML
- CSS
- Joblib
- Jupyter Notebook / Google Colab

## 🤖 Machine Learning Models

The following classification algorithms are used in this project:

1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier
4. K-Nearest Neighbours (KNN)
5. Support Vector Machine (SVM)

### Model Evaluation

The models are evaluated and compared using:

- Accuracy
- Precision
- Recall
- F1-score
- Macro F1-score
- Balanced Accuracy
- Confusion Matrix
- Cross-validation

The best model is selected based on the cross-validation results in the notebook and saved for use in the Flask application.

## 🌐 Flask Web Application

The project includes a web application with two main pages.

### 1. Home Page

- Provides an overview of the project.
- Explains the purpose of shopping behaviour prediction.
- Introduces the Machine Learning approach.
- Provides a button to access the prediction page.

### 2. Prediction Page

- Allows users to enter customer shopping behaviour details.
- Collects information through input fields and dropdown menus.
- Sends the entered details to the trained Machine Learning pipeline.
- Displays the predicted shopping preference.

### Prediction Categories

- Online Shopping
- Offline Shopping
- Equal / Both Shopping

## 📁 Project Structure

```text
Shopping-Behaviour-Prediction/
│
├── G1.csv
│
├── exit_exam (5).ipynb
│
├── app.py
│
├── shopping_mode_model.joblib
│
├── templates/
│   ├── index.html
│   └── predict.html
│
└── README.md
```

## ⚙️ Installation and Setup

### Step 1: Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### Step 2: Navigate to the Project Folder

```bash
cd Shopping-Behaviour-Prediction
```

### Step 3: Install Required Libraries

```bash
pip install pandas numpy scikit-learn matplotlib seaborn flask joblib
```

### Step 4: Train and Save the Model

1. Open the Jupyter Notebook.
2. Load the `G1.csv` dataset.
3. Execute the data preprocessing and model training cells.
4. Execute the model-saving cell to generate:

```text
shopping_mode_model.joblib
```

Make sure the saved model file is in the project root directory.

### Step 5: Run the Flask Application

```bash
python app.py
```

### Step 6: Open the Application

Open your browser and visit:

```text
http://127.0.0.1:5000/
```

The home page will be displayed. Click **Start Prediction** to enter customer shopping behaviour details and generate a prediction.

## 📊 Expected Output

The application predicts one of the following shopping preferences:

| Prediction | Description |
|---|---|
| Online | Customer is predicted to prefer online shopping. |
| Offline | Customer is predicted to prefer physical store shopping. |
| Equal / both | Customer is predicted to prefer both shopping modes. |

## 🔍 Project Workflow

1. Dataset collection
2. Data understanding and exploration
3. Data cleaning and preprocessing
4. Exploratory Data Analysis (EDA)
5. Feature selection and preparation
6. Model training
7. Model evaluation and comparison
8. Best model selection
9. Model saving
10. Flask application development
11. Shopping mode prediction

## ⚠️ Limitations

- The dataset contains a limited number of labelled customer responses.
- Missing values may affect prediction quality.
- Customer shopping preferences can change over time.
- Model predictions are estimates and should not be treated as guaranteed customer preferences.
- Prediction performance depends on the quality and representativeness of the training dataset.

## 🚀 Future Enhancements

- Add more customer responses to improve prediction quality.
- Improve model performance through hyperparameter tuning.
- Add visual analytics and shopping behaviour dashboards.
- Include prediction probability scores.
- Develop a customer prediction history feature.
- Deploy the application online for public access.

## 👨‍💻 Conclusion

This project demonstrates how Machine Learning can be applied to understand customer shopping behaviour and predict shopping preferences.

By combining data analysis, classification algorithms and Flask web development, the project provides an interactive application that allows users to explore shopping behaviour predictions.

---

**Project Title:** Shopping Behaviour Prediction Using Machine Learning

**Application Framework:** Flask

**Programming Language:** Python

**Dataset:** G1.csv
