# Fraudulent Detection in Online Payments

 Fraudulent Detection in Online Payments
 Project Overview

This project implements a machine learning–based fraud detection system to classify online financial transactions as fraudulent or legitimate.
It extends an existing open-source repository and enhances it with:

Machine Learning Pipeline

Flask REST API

Frontend Dashboard (Upload + Results Visualization)

CI/CD and Automated Testing

Version Control & Software Engineering Practices

 Project Team
Name	Role	GitHub Username
Group Leader	Repository Admin	@vardolnaveen2307-create
Member 2	Machine Learning Engineer	
Member 3	Backend Developer	
Member 4	UI/Testing + CI/CD	
 Tech Stack
Component	Technology
Language	Python
ML Frameworks	Scikit-learn, XGBoost
Backend	Flask (REST API)
Frontend	HTML, CSS, Bootstrap, Jinja2
Tools	Git, Google Colab, Jupyter
Testing	PyTest
CI/CD	GitHub Actions
 Project Structure
Fraudulent-Detection-In-Online-Payments/
│
├── src/                 # ML model scripts
├── api/                 # Flask backend
├── web/                 # Frontend UI (HTML + CSS + JS)
│   ├── templates/       # Jinja pages
│   ├── static/          # CSS / JS / Images
│
├── notebooks/           # Research and Colab files
├── models/              # Saved machine learning model
├── data/                # Dataset (ignored in Git)
├── tests/               # Unit tests
│
├── requirements.txt
├── README.md
└── .github/workflows/   # CI/CD pipeline config

▶ Running the Project
pip install -r requirements.txt
python api/app.py

 Future Improvements

Model retraining automation

Docker deployment

Integration with live transaction systems

 2️ requirements.txt Starter

Create/update your requirements.txt with:

pandas
numpy
scikit-learn
xgboost
flask
joblib
matplotlib
seaborn
plotly
pytest
flask-cors


Later you'll update this after your final implementation.

 3️ Dataset + Preprocessing Notebook Template

Create a file in notebooks/ named:

 01_dataset_preprocessing.ipynb

Contents:

import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load dataset
df = pd.read_csv('/content/onlinefraud.csv')  # update path when needed

# Basic info
print(df.head())
print(df.info())
print(df.describe())

# Check missing values
print(df.isnull().sum())

# Visualize class imbalance
sns.countplot(x='isFraud', data=df)
plt.title("Fraud vs Non-Fraud Distribution")


Later, we will:
✔ encode categories
✔ scale features
✔ split and train model
✔ save .pkl

 4️ GitHub Kanban (Project Board)

Go to your repo → Projects → New → Choose:

 Board (Kanban)

Add Lists:

Backlog

To Do

In Progress

In Review

Completed

Add these starting tasks:

Task
Setup repo and branching
Dataset preprocessing (ML)
Model training & evaluation
Flask API implementation
UI dashboards
Unit testing (pytest)
CI/CD setup
Final documentation
 5️ Next Tasks for Your Group
Order	Task
1	Folder structure created and committed
2	Create feature branches (ML / API / UI / Testing / CI)
3	Start ML notebook (preprocessing + modeling)
4	Build ML pipeline in src/
5	Build /predict Flask endpoint
6	Add upload UI + prediction result display
7	Add PyTest and GitHub Actions
8	Final refactoring + testing + documentation
