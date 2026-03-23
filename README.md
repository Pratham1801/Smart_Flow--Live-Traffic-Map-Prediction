# 🚦 SmartFlow – Traffic Prediction and Monitoring System

## Introduction

SmartFlow is a machine learning based traffic prediction system designed to analyze traffic patterns and estimate congestion levels at different road junctions. The aim of this project is to provide a simple platform that can visualize traffic conditions and help in understanding how traffic changes over time.

The system uses a Random Forest machine learning model trained on a traffic dataset to classify traffic levels as **Low, Medium, or High**. A web dashboard is also developed to display predictions, analytics, and traffic information in an interactive way.

---

## Key Features

* Traffic prediction using a machine learning model
* Interactive dashboard for traffic monitoring
* Data visualization using charts and graphs
* Map interface showing different junctions
* Admin panel to view logs and system statistics
* REST API endpoints for predictions and analytics

---

## Technologies Used

### Frontend

* Next.js
* React.js
* Tailwind CSS
* Chart.js / Recharts

### Backend

* Python
* FastAPI

### Machine Learning

* Scikit-learn
* Pandas
* NumPy

### Model

* Random Forest Classifier

---

## Machine Learning Model

The prediction model is trained using a traffic dataset.

**Input Features**

* Hour
* Day
* Month
* Junction
* Weekend indicator

**Output**

* Traffic Level (Low / Medium / High)

The dataset was divided into **training and testing data** to evaluate the performance of the model.

---

## Project Structure

```
smartflow-project/

├── SmartFlow_Dashboard.html
├── README.md

├── backend
│   ├── app.py
│   ├── train_model.py
│   ├── requirements.txt
│   ├── model
│   │   ├── traffic_model.pkl
│   │   └── stats.json
│   └── dataset
│       └── traffic.csv

└── frontend
    ├── pages
    │   ├── index.tsx
    │   ├── map.tsx
    │   ├── dashboard.tsx
    │   └── admin.tsx
    ├── components
    ├── styles
    └── package.json
```

---

## How to Run the Project

### 1. Run Backend

```
cd backend
pip install -r requirements.txt
python train_model.py
uvicorn app:app --reload
```

Backend server will run at
http://localhost:8000

---

### 2. Run Frontend

```
cd frontend
npm install
npm run dev
```

Frontend will run at
http://localhost:3000

---

## Dataset

This project uses a traffic dataset obtained from Kaggle which contains information about vehicle counts at different road junctions.

Dataset fields include:

* DateTime
* Junction
* Vehicles
* ID

---

## Future Improvements

* Integration with live traffic APIs
* Deployment on cloud platforms
* Mobile-friendly dashboard
* Improved prediction models
* Real-time traffic monitoring

---

## Author

Vaibhav Vilas Datkhil
B.Tech – Information Technology
AISSMS Institute of Information Technology, Pune
Prathmesh Rajesh Bawane
M.Sc-Compter application
Modern college , pune
