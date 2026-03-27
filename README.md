# Calendar-Based-Night-Lighting
A smart embedded lighting controller that combines calendar-based scheduling, real-time clock synchronization, and environmental light sensing to deliver autonomous, energy-efficient lighting without reliance on cloud or IoT infrastructure.




# 🌙 Smart Calendar-Based Night Lighting System

## 📌 Overview

This project presents a smart embedded lighting system that automatically controls indoor and outdoor lighting based on calendar scheduling and real-time environmental conditions.

The system is designed using an AVR microcontroller and operates independently without requiring internet connectivity, making it reliable, low-cost, and energy-efficient.

---

## 🧠 Key Idea

Traditional lighting systems rely on fixed timers, which do not adapt to seasonal changes or real-world conditions.

This project improves upon that by combining:

* 📅 Calendar-based scheduling (predictive logic)
* ⏰ Real-Time Clock (RTC) synchronization
* 🌗 Ambient light sensing (reactive logic)

This hybrid approach ensures lighting operates only when needed, reducing energy consumption and improving automation accuracy.

---

## 🎯 Features

* Automatic night lighting based on time and date
* Calendar-aware scheduling (weekdays, weekends, events)
* Real-time light detection using LDR sensor
* Autonomous operation (no cloud or IoT dependency)
* Energy-efficient control logic
* Reliable operation with power-loss recovery

---

## ⚙️ Technologies Used

* **Microcontroller:** AVR (ATmega series)
* **Programming Language:** Embedded C
* **Development Environment:** Microchip Studio
* **RTC Module:** DS1307 (I2C communication)
* **Sensors:** LDR (Light Dependent Resistor)
* **Storage:** EEPROM (for persistent calendar data)
* **Communication Protocol:** I2C

---

## 🏗️ System Architecture

The system consists of the following components:

* **AVR Microcontroller** → Main controller (decision-making unit)
* **RTC (DS1307)** → Provides accurate date and time
* **LDR Sensor** → Detects ambient light levels
* **Relay/Driver Circuit** → Controls lighting output
* **EEPROM** → Stores schedules and configuration

The microcontroller continuously reads time and light data, then decides whether to turn the lighting system ON or OFF.

---

## 🔄 How It Works

1. The RTC module provides the current date and time
2. The system checks if the current time matches scheduled calendar events
3. The LDR sensor measures ambient light intensity
4. The controller applies decision logic:

   * If it is the correct time **AND** it is dark → lights turn ON
   * Otherwise → lights remain OFF
5. The system repeats this process continuously

---

## 💡 Key Concepts Implemented

* Calendar-driven automation
* Embedded system design
* I2C communication (RTC interface)
* ADC-based sensor reading
* EEPROM data persistence
* Interrupt-driven and efficient control logic

---

## 📊 Results

* Successfully controlled lighting based on calendar schedules
* Maintained accurate time using RTC with battery backup
* Demonstrated reliable operation under different conditions
* Showed potential for significant energy savings

---

## ⚠️ Limitations

* No occupancy detection (e.g., PIR sensor)
* Manual update of calendar data
* Fixed scheduling without dynamic location-based adjustments

---

## 🚀 Future Improvements

* Wireless synchronization (Wi-Fi / BLE)
* Mobile application for remote control
* Integration with occupancy sensors (PIR)
* Real-time astronomical calculations (sunrise/sunset)
* Ultra-low power optimization using sleep modes

---

## 🔐 Safety & Reliability

* Flyback diode used for relay protection
* Electrical isolation for safe operation with AC loads
* EEPROM ensures data persistence after power loss
* Robust I2C communication with error handling

---

## 👤 Author

** JIM (LCNx7D1) **

---

## 📄 License

This project is for educational and academic purposes.
