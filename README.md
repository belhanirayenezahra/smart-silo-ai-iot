# Smart Silo – AI & IoT Grain Storage System

A complete intelligent grain storage system designed to monitor, analyze, and predict wheat quality using **IoT**, **AI**, **FastAPI**, **InfluxDB**, **MQTT**, and a **React Dashboard**.

This project is part of a real-world smart agriculture solution that includes:
- ESP32 + sensors (Temperature, Humidity, CO₂, Sound)
- AI detection of insects using sound frequency analysis
- AI prediction of wheat quality
- Real-time storage monitoring via MQTT
- FastAPI backend with PDF report generation
- Grafana data visualization
- Digital Twin visualization

---

## 🚀 Features

1. IoT Sensor System (ESP32)**
- Temperature & humidity monitoring  
- CO₂ gas measurement  
- Sound analysis for insect detection  
- Real-time data transmission via MQTT  

2. Artificial Intelligence**
- Wheat quality prediction (Good / Medium / Bad)  
- Insect presence detection based on sound frequencies  
- Data pre-processing using SMOTE  
- TensorFlow neural network model  

3. FastAPI Backend**
- Receives sensor data  
- Runs AI models  
- Generates weekly PDF reports  
- Sends alerts (temperature rise, humidity problems, insects detected)  
- Connects to InfluxDB for time-series data  

4. Grafana Dashboard**
- Real-time industrial visualization  
- Statistics & weekly analysis  

5. React Web Dashboard**
- Silo list + detailed view  
- Real-time indicators  
- AI predictions  
- Alerts panel  


---

## 🧱 Project Structure

