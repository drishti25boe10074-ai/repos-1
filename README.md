# repos🌟 Overview
This project is a real-time system designed to automatically ingest patient vital signs (Heart Rate, Temperature, SpO2), process them against configurable critical thresholds, and immediately notify assigned caregivers of life-threatening events. The system significantly reduces intervention time compared to manual monitoring.

## ✨ Features
* **Real-Time Data Ingestion:** Collects vital data stream via an MQTT/API endpoint.
* **Critical Alerting:** Automatic generation of 'Warning' or 'Critical' alerts based on configurable rules.
* **Caregiver Notification:** Integration with notification APIs (e.g., Twilio, SendGrid) for SMS/Email alerts.
* **Historical Data Visualization:** Web dashboard displaying current status and 24-hour historical trends.

## 🛠️ Technologies/Tools Used
* **Backend:** Python (Flask/FastAPI)
* **Messaging:** Apache Kafka / RabbitMQ (for message queuing)
* **Database:** InfluxDB (Time-Series Database)
* **Version Control:** Git

## 🏃 Steps to Install & Run the Project
1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/yourusername/vitals-monitor.git](https://github.com/yourusername/vitals-monitor.git)
    cd vitals-monitor
    ```
2.  **Setup Environment:** Ensure Docker/Docker-Compose is installed to run Kafka and InfluxDB.
3.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
4.  **Start Services:**
    ```bash
    docker-compose up -d
    python main.py
    ```
    The web dashboard will be accessible at `http://localhost:5000`.

## 🧪 Instructions for Testing
To test the alerting mechanism:
1.  Run the included `test_data_simulator.py` script.
2.  Modify the script to send a Heart Rate value of `130` (Critical threshold is 120).
3.  Verify that an alert message is logged in the console and appears on the web dashboard within 500ms.-1
