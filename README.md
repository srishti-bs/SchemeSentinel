# SchemeSentinel
Smart Fraud Detection System for Government Welfare Schemes
# 🛡️ SchemeSentinel  
### Smart Fraud Detection Dashboard for Government Welfare Schemes

SchemeSentinel is a full-stack fraud detection system designed to identify suspicious activities in Indian government welfare schemes using rule-based risk scoring and pattern detection.

This project was developed as part of a hackathon to demonstrate how technology can improve transparency and prevent misuse of public funds.



# 🚨 Problem Statement

Government welfare schemes often face fraudulent activities such as:

- Duplicate beneficiaries
- Shared bank accounts
- Fake addresses
- Cross-scheme misuse
- Fraud rings using shared identities

These fraudulent activities result in:

- Financial loss
- Resource misallocation
- Reduced trust in public systems

SchemeSentinel addresses these issues by detecting suspicious applications and identifying coordinated fraud patterns.

---

# 🎯 Key Features

## 📊 Dashboard Overview
Displays real-time fraud statistics:

- Total Applications Processed
- Suspicious Applications
- Applications Under Review
- Estimated Money Saved
- Active Fraud Rings

Includes:

- Fraud Heatmap (India Map)
- Risk Score Visualization
- Live Threat Feed

---

## 🔎 Application Investigation

Search any application using:

Application ID

Displays:

- Risk Score
- Applicant Details
- Scheme Information
- Evidence List

Example Evidence:

- Location mismatch
- Shared bank account
- Duplicate phone number
- Same device usage

Allows actions:

- Approve
- Mark Suspicious
- Block

---

## 🕸️ Fraud Ring Detection

Automatically detects fraud rings based on:

- Shared Bank Accounts
- Shared Device IDs
- Shared Phone Numbers

If:

3 or more applications share common data

The system flags:
Fraud Ring Detected


Displays:

- Ring Size
- Connected Applications
- Risk Level

---

## ⚠️ Cross-Scheme Alerts

Detects fraud across multiple schemes:

Supported Schemes:

- PM-KISAN
- MGNREGA
- PMAY
- PDS

Example:
Fraud detected in PM-KISAN linked to PDS
via shared bank account.

---

# 🧠 Risk Scoring Logic

Each application is assigned a **risk score (0–100)** based on predefined rules.

## Rules Used:

| Condition | Risk Added |
|----------|------------|
| IP Location ≠ Declared Address | +30 |
| Shared Bank Account | +25 |
| Same Device Used Multiple Times | +20 |
| Duplicate Phone Number | +15 |

---

## Risk Classification

| Score Range | Risk Level |
|-------------|-------------|
| 0–30 | Low Risk |
| 31–60 | Medium Risk |
| 61–100 | High Risk |

---

# 🏗️ Tech Stack

## Frontend

- React.js
- Tailwind CSS
- Chart.js
- Leaflet.js

---

## Backend

- Python
- Flask
- Pandas
- NumPy

---

## Data Storage

- CSV-based dataset
- Simulated government scheme records

---

# 📂 Project Structure
SchemaSentinel/
│
├── backend/
│ ├── app.py
│ ├── requirements.txt
│ ├── dataset/
│ │ └── applications.csv
│ ├── utils/
│ ├── risk_scoring.py
│ ├── fraud_detection.py
│
├── frontend/
│ ├── src/
│ ├── package.json
│
└── README.md


---

# ▶️ How to Run Locally

## Step 1 — Install Python Requirements

---

cd backend
py -3.11 -m pip install -r requirements.txt


---

## Step 2 — Run Backend
py -3.11 app.py


Runs on:
http://127.0.0.1:5000


---

## Step 3 — Run Frontend
cd frontend
npm install
npm run dev


Open:
http://localhost:3000


---

# 📊 Sample Dataset

The system uses:
applications.csv

Contains:

- Application ID
- Name
- Scheme
- City
- State
- Bank Account
- Phone Number
- Device ID
- IP Location
- Declared Address
- Status

---

# 🎥 Demo Workflow

1. Open Dashboard
2. View Fraud Heatmap
3. Search Application ID
4. Analyze Risk Evidence
5. Detect Fraud Rings
6. Review Cross-Scheme Alerts

---

# 🌍 Real-World Impact

SchemeSentinel can help:

- Prevent welfare fraud
- Improve transparency
- Detect coordinated misuse
- Save public funds
- Strengthen governance systems

---

# 🚀 Future Enhancements

- Machine Learning-based prediction
- Aadhaar validation integration
- Real-time API data ingestion
- Role-based access system
- Cloud deployment support

---

# 👩‍💻 Developed For Hackathon

Project Name:
SchemeSentinel
Smart Fraud Detection Dashboard.


Built to demonstrate scalable fraud detection for government welfare systems.

---

# 📜 License

This project is created for educational and hackathon demonstration purposes.







