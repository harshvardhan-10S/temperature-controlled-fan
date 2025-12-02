# 🌡️ Temperature Controlled Fan System
A smart automation system that automatically controls a fan based on real-time temperature readings using the LM35 temperature sensor and a microcontroller (Arduino/NodeMCU).

---

## 📌 Overview
The **Temperature Controlled Fan** is designed to turn a fan ON/OFF (or adjust its speed) automatically depending on the surrounding temperature. The system uses the LM35 temperature sensor to monitor heat levels and triggers the fan when the temperature crosses a predefined threshold.

Depending on the version, the fan is controlled either using:
- **PWM (Arduino Version)** for speed control  
- **Relay Switching (NodeMCU Version)** for ON/OFF automation  

This project improves energy efficiency and eliminates the need for manual fan control in varying temperature conditions.

---

## 🎯 Objectives
- Automatically control a fan based on room temperature  
- Reduce energy consumption  
- Provide a hands-free temperature-based cooling solution  
- Demonstrate sensor-based automation using embedded systems  

---

## 🧠 Working Principle

### ✔ 1. Temperature Sensing (LM35)
- LM35 outputs **10 mV per °C**.
- The microcontroller reads analog voltage using ADC.
- Temperature is calculated using:


---

### ✔ 2. Threshold-Based Control
The system compares the measured temperature with preset levels:

| Temperature | Fan Action |
|------------|------------|
| Below 25°C | Fan OFF |
| 25°C–35°C  | Fan ON (Medium/Normal) |
| Above 35°C | Fan ON (High Speed) |

---

### ✔ 3. Fan Control Mechanism

#### **Arduino-Based Version**
- PWM signal controls fan speed  
- TIP30 transistor drives the fan  
- 1N4007 diode protects against back EMF  

#### **NodeMCU-Based Version**
- Relay module switches fan ON/OFF  
- NodeMCU reads temperature and controls relay  

---

## 🖥️ Circuit Diagram
Below is the system connection map (Arduino version + NodeMCU version shown):

![Circuit Diagram](Temperature%20Controlled%20Fan%20Circuit%20Diagram.png)

---

## 🧰 Components Used
### **Hardware**
- LM35 Temperature Sensor  
- Arduino UNO / NodeMCU ESP8266  
- TIP30 Transistor (for fan driving)  
- Relay Module (for ON/OFF control)  
- 1kΩ Resistor  
- 1N4007 Diode (flyback protection)  
- DC Fan (5V/12V)  
- External 5V Power Supply  
- Jumper Wires, Breadboard  

### **Software**
- Arduino IDE  
- Embedded C/C++ Programming  

---

## 📝 Methodology

1. Read temperature from LM35  
2. Convert analog reading to Celsius  
3. Compare with threshold values  
4. Generate PWM (Arduino) or activate relay (NodeMCU)  
5. Turn fan ON/OFF accordingly  

---

## 📊 Results
- Fan turns ON automatically when temperature crosses the threshold  
- Stable and accurate LM35 temperature readings  
- Relay switches without flickering  
- Reduced power consumption when not required  
- Demonstrates successful sensor-based automation  

---

## 🚀 Applications
- Smart room cooling  
- Server room temperature control  
- Greenhouse temperature automation  
- Industrial heat management  
- Laboratory cooling systems  

---

## 🌟 Future Scope
- Add IoT dashboard for real-time monitoring  
- Mobile control using MQTT/Blynk  
- OLED/LCD temperature display  
- Multi-speed AC fan control  
- Auto logging of temperature data  

---

## 📄 Project Documentation
All documentation files for this project are included in the repository:
- Detailed Project Report  
- Project Presentation (PPT)  
- Circuit Diagram  
- Source Code
  
---

## 👨‍💻 Developer
**Harshvardhan Shinde**  
Electronics & Telecommunication Engineering (ENTC)  
VIT Pune  
