# IoST: Automated Stumping Detection System for Error-Free Decision Making

## 📌 Project Overview
Cricket umpiring decisions, especially stumpings, are often prone to delays and human error.  
This project proposes an **IoT-based smart umpiring system** using:
- ⏱️ **Time-of-Flight (ToF) sensors** to measure batter’s distance from the crease
- ⚡ **Accelerometer** to detect stump disturbances
- 💡 **LED indicators** to provide real-time visual feedback
- ☁️ **ESP8266 & ThingSpeak** for cloud-based data logging and visualization

## 🎯 Objectives
- Automate stumping decisions in cricket
- Provide instant "Out" or "Not Out" feedback
- Reduce umpiring delays and errors
- Enable cloud integration for analysis and record-keeping

## 🛠️ Components Used
- Arduino UNO
- VL53L0X Time-of-Flight (ToF) Sensor
- MPU6050 Accelerometer
- ESP8266 Wi-Fi Module
- Red LEDs
- Breadboard, jumper wires, soldering kit

## ⚙️ System Workflow
1. ToF sensor measures the distance of the batter’s foot from the crease.
2. Accelerometer detects stump disturbance.
3. Arduino processes data:
   - If `distance > 30 cm` and `acceleration > 5g` → **OUT**
   - Else → **NOT OUT**
4. LEDs incorporated in stums blinks(10sec) for OUT and remains constant(remains red LED without blinking) for NOT OUT.
5. Data uploaded to ThingSpeak cloud.

## 📊 Results
- Achieved 95% decision accuracy
- Average response time: <1000 ms
- Cloud integration ensures real-time monitoring

## 🚀 Future Scope
- Extend to no-ball detection and run-out analysis
- Integrate AI for predictive analytics
- Develop a mobile app for live umpiring assistance

## 📄 Publications
- IEEE Paper: *IoST: Automated Stumping Detection System for Error-Free Decision Making* (Accepted, 2025).
