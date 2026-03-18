🚦 SmartFlow – Traffic Prediction and Monitoring System
📌 Introduction

SmartFlow is a machine learning based system developed to analyze and predict traffic congestion at different road junctions. The goal of this project is to help visualize traffic patterns and provide predictions that can support smarter traffic management in urban areas.

The system uses a Random Forest classification model trained on a traffic dataset to predict the traffic level (Low, Medium, or High) based on time and location related features.

A web dashboard is also developed to display traffic predictions, analytics, and live traffic information in a simple and interactive interface.

⚙️ Key Features

Machine learning based traffic prediction

Interactive dashboard for traffic monitoring

Visualization of traffic data using charts

Map interface showing different junctions

Admin panel for viewing system logs and statistics

API endpoints for accessing prediction and analytics data

🧰 Technologies Used
Frontend

Next.js

React.js

Tailwind CSS

Chart.js / Recharts

Backend

FastAPI

Python

Machine Learning

Scikit-learn

Pandas

NumPy

Model

Random Forest Classifier

🧠 Machine Learning Approach

The prediction model is trained using traffic data collected from a Kaggle dataset.

Input Features

Hour

Day

Month

Junction

Weekend indicator

Output

Traffic Level (Low / Medium / High)

The dataset was divided into training and testing sets to evaluate model performance.

📁 Project Structure
smartflow-project/

SmartFlow_Dashboard.html
README.md

backend/
 ├── app.py
 ├── train_model.py
 ├── requirements.txt
 ├── model/
 │    ├── traffic_model.pkl
 │    └── stats.json
 └── dataset/
      └── traffic.csv

frontend/
 ├── pages/
 │    ├── index.tsx
 │    ├── map.tsx
 │    ├── dashboard.tsx
 │    └── admin.tsx
 ├── components/
 ├── styles/
 └── package.json
🚀 Running the Project
1️⃣ Start Backend
cd backend
pip install -r requirements.txt
python train_model.py
uvicorn app:app --reload

Backend server runs at:

http://localhost:8000
2️⃣ Start Frontend
cd frontend
npm install
npm run dev

Frontend will run at:

http://localhost:3000
📊 Dataset

This project uses a traffic dataset obtained from Kaggle containing information about vehicle counts at different road junctions over time.

Dataset columns include:

DateTime

Junction

Vehicles

ID

🔮 Future Improvements

Integration with live traffic APIs

Deployment on cloud platforms

Real-time data streaming

Mobile-friendly dashboard

Improved prediction models using deep learning
