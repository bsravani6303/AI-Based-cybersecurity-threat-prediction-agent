# AI-Based Cybersecurity Threat Prediction Agent

##  Overview

This is an advanced, AI-powered cybersecurity threat prediction and monitoring system. It processes real-time data from network sources, analyzes anomalies, predicts potential threats, and provides actionable insights through dashboards, live monitoring tools, and automated reports.

This project includes:

* Live threat monitoring
* VPN/WiFi threat detection
* Dataset management
* Flask-based web dashboard
* Trained ML models for prediction

---

## Tech Stack

### **Backend**

* Python
* Flask
* Flask-SocketIO

### **Frontend**

* HTML
* CSS
* Vanilla JavaScript

### **Visualization**

* Chart.js (threat charts & analytics)
* Leaflet (live threat map)
* Three.js (3D interactive threat globe)

### **Data & Storage**

* SQLite (default local DB)
* Optional integrations:

  * MySQL
  * PostgreSQL
  * MongoDB
  * Redis
  * DynamoDB
  * Cassandra
  * SQL Server

### **Reporting**

* reportlab (PDF report generation)

---

## 📁 Folder Structure

```
MY_FIRST/
├── __pycache__/
│   └── app.cpython-311.py
├── data/
│   ├── ids_datasets/
│   │   └── url_labeled.csv
│   ├── vpn_datasets/
│   ├── wifi_datasets/
│   ├── threat_events.db
│   └── threat_snapshots.json
├── reports/
├── src/
├── static/
├── templates/
├── trained_models/
├── app.py
├── app_flask.py
├── DATASETS_REFERENCE.md
├── FINAL_SUMMARY.md
├── LIVE_MONITORING.md
├── LIVE_THREAT_MODEL_README.md
├── LIVE_THREAT_SETUP_SUMMARY.md
├── NEW_DATASET_GUIDE.md
├── QUICK_START.md
├── requirements.txt
├── stream_listener.py
└── VPN_WIFI_MODELS_GUIDE.md
```

---

## 🔐 Key Modules

### **1. Data Processing & Storage**

* Handles IDS, VPN, and WiFi datasets
* Stores processed threat events in `threat_events.db`
* Maintains JSON snapshots for fast loading

### **2. AI Prediction Models**

* Pretrained models stored in `trained_models/`
* Predicts threat categories, severity levels, and anomaly scores

### **3. Web Application**

* `app.py` & `app_flask.py` power the intuitive UI
* Flask dashboards for real-time threat monitoring

### **4. Live Stream Listener**

* `stream_listener.py` listens to network or API streams
* Feeds data to the threat prediction engine

---

##  Getting Started

### **Prerequisites**

* Python **3.8+** (3.10 recommended)
* `pip` (Python package manager)
* Optional but recommended:

  * Python virtual environment (`venv`)

---

### **1. Clone / Open the Project**

Place the project folder  somewhere on your machine and open it in your IDE or terminal.

---

### **2. Create & Activate a Virtual Environment (optional)**

```
python -m venv .venv

# Windows
.venv\Scripts\activate

# macOS / Linux
source .venv/bin/activate
```

---

### **3. Install Dependencies**

Run from project root (where `requirements.txt` exists):

```
pip install -r requirements.txt
```

If additional database drivers are required (e.g., `psycopg2-binary`, `pymongo`, `pyodbc`), install them separately using pip.

---

### **4. Run the Flask App**

```
python app_flask.py
```

Expected output:

```
* Serving Flask app 'app_flask'
* Debug mode: on
```

---

### **5. Open the Dashboard**

Open your browser and go to:

```
http://localhost:5000
```

Use **Ctrl + F5** to hard-refresh and ensure all static assets load correctly.

---

## 📊 Documentation Files

This repository includes detailed guides:

* **QUICK_START.md** – Easy setup guide
* **LIVE_MONITORING.md** – How live monitoring works
* **NEW_DATASET_GUIDE.md** – Add new datasets
* **DATASETS_REFERENCE.md** – Dataset details
* **VPN_WIFI_MODELS_GUIDE.md** – VPN & WiFi model architecture
* **FINAL_SUMMARY.md** – Full project summary

---

## Features

* Real-time threat prediction
* VPN/WiFi anomaly detection
* URL risk classification
* AI-based severity scoring
* Live dashboards and monitoring tools
* Automatic dataset ingestion

---

## Future Enhancements

* Cloud deployment (AWS/GCP/Azure)
* SIEM integration
* Mobile-based threat alerts
* Automated dataset labeling pipeline
* Automatic model retraining system

---
