# Foundations of Machine Learning Frameworks
Workshop on Data Streaming and Visualization Workshop
Use case: Robot Predictive Maintenance

In this hands-on session, you and your team will build an **Predictive Maintenance Dashboard** application, the visibility tool of an Anomaly Detection and response management workflow in a manufacturing facility.

![Image Description](./images/KawasakiMajorCurrentIncrease.png)

Purpose: Robot Predicative Maintenance tool that collects electrical load data for each joint and other relevant data, then applies Machine Learning to set standard operating patterns and identify anomalies.

The target is to **predict equipment failure** by using a condition monitoring system based on the collection of a robot’s power measurements and the detection of errors and inaccuracies based on electricity and torque data analysis. 

![Image Description](./images/KawasakiTrendAndAlert.png)



# Foundations of Machine Learning Frameworks  
**Workshop on Data Streaming and Visualization**  
**Use case:** Robot Predictive Maintenance  

In this hands-on session, you and your team will build a **Predictive Maintenance Dashboard** application — the visibility tool of an anomaly detection and response management workflow in a manufacturing facility.

![Robot Current Increase](./images/KawasakiMajorCurrentIncrease.png)

**Purpose:** Robot Predictive Maintenance tool that collects electrical load data for each joint and other relevant data, then applies Machine Learning to set standard operating patterns and identify anomalies.

The target is to **predict equipment failure** by using a condition monitoring system based on the collection of a robot’s power measurements and the detection of errors and inaccuracies based on electricity and torque data analysis. 

![Trend and Alerts](./images/KawasakiTrendAndAlert.png)

---

## Project Overview
This project simulates **real-time data streaming** from a manufacturing robot and provides a visual dashboard for monitoring key parameters. The workflow demonstrates:

- Data extraction from CSV
- Streaming simulation
- Database integration (Neon PostgreSQL)
- Threshold-based alert detection
- Dashboard visualization using Python

---

## Features
- **Streaming Simulator:** Simulates real-time feed of robot sensor data.  
- **Database Integration:** Loads data into a PostgreSQL database using SQLAlchemy.  
- **Alert Detection:** Detects maintenance alerts when thresholds are exceeded:  
  - `Axis #1` > 85  
  - `Axis #2` > 1.0  
- **Dashboard Visualization:** Plots `Axis #1` and `Axis #2` values over time with threshold lines.  
- **Data Inspection:** Quickly preview dataset using pandas.

---

## Prerequisites
- Python 3.x installed  
- Jupyter Notebook or VS Code with Python & Jupyter extensions  
- PostgreSQL database access (Neon in this example)

Required Python libraries:  
- pandas  
- sqlalchemy  
- psycopg2-binary  
- matplotlib

---

## Project Structure
Project(DataStreamVisualization_Workshop)/
│
├── data/
│ └── RMBR4-2_export_test.csv # Robot stream dataset
├── documents/
│── images/
│── venv/
├── DataStreamVisualization_Workshop.ipynb # Main Jupyter Notebook
│── README.md # Project description
├── robot_data.csv

## Instructions

(1) **Install Required Libraries**  
    ```bash
    pip install pandas sqlalchemy psycopg2-binary matplotlib

(2)Connect to Database
   Update the DATABASE_URL in the notebook to connect to your PostgreSQL database.

(3)Load and Inspect Data
   Load the CSV file and inspect the first few rows using pandas.

(4)Run the Streaming Simulator
   Simulate a real-time feed of the robot sensor data using the StreamingSimulator class.

(5)Detect Alerts and Visualize Data
   Monitor thresholds and display the dashboard with plots of Axis #1 (temperature/load) and Axis #2 (vibration).


Output:
Alerts detected: List of timestamps where thresholds were exceeded.
Dashboard plots: Visual representation of sensor values over time with threshold lines.

Author:
Param Avinashkumar Rasaniya
Viraj Dipakkumar Mistry
Sumanth Reddy Konannagari