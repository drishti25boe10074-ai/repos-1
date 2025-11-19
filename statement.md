Problem Statement

The current reliance on manual, periodic collection of patient vital signs (e.g., heart rate, temperature, SpO2) creates a critical window of time during which a life-threatening change in a patient's condition can go unnoticed. This results in delayed medical intervention, which significantly increases the risk of complications, severe health decline, or preventable mortality, particularly in high-acuity or remote care settings.

Scope of the Project

The project is a proof-of-concept system focusing on real-time data ingestion, processing, and alerting.

The scope includes:

Monitored Vitals: Heart Rate (HR), Body Temperature (Temp), and Oxygen Saturation (SpO2).

Alert Mechanism: Threshold-based logic for classifying patient status (Normal, Warning, Critical) and triggering notifications.

Visualization: A simple, real-time web dashboard for current status monitoring and basic historical data review (last 24 hours).

Exclusions: The project will not integrate with existing Hospital Electronic Health Records (EHRs), nor will it include complex machine learning for predictive analysis; it is strictly focused on rule-based alerting and data pipeline reliability.

Target Users

Nurses and Caregivers: The primary end-users who rely on the system for immediate, actionable alerts to prioritize patient needs.

On-Call Doctors: Users who require high-level status visibility and historical data access for diagnosis and treatment planning.

System Administrators: Users responsible for configuring system parameters, such as alert thresholds and caregiver contact details.

High-Level Features

Data Ingestion: Reliable, high-frequency intake of vital sign data streams.

Automated Alert Processing: Instantaneous comparison of new data against clinical thresholds.

Prioritized Notification: Delivery of urgent alerts via designated channels (e.g., SMS, email API) to assigned staff.

Real-Time Dashboard: Centralized display of patient status, active alerts, and vital sign trends
