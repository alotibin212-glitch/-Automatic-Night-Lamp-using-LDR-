# 💡 Automatic Night Lamp using LDR

An energy-efficient, automated lighting system designed to control illumination based on real-time ambient light conditions. The system utilizes an Arduino Uno as the central controller to monitor light levels via a Light Dependent Resistor (LDR) and trigger a light source accordingly.

---

## 🔗 Project Resources
Access the full project repository and documentation files via the link below:
[📁 Project Google Drive Folder](https://drive.google.com/drive/folders/1GnBpwa7SiXpvqVREdGcvxS_bQd_9XebG)

---

## 📊 System Architecture
The system operates through a simple, robust logic flow:
* Light Sensing: The LDR acts as a voltage divider, where resistance changes based on ambient light intensity.
* Processing Core: The Arduino Uno reads the analog value from the LDR and compares it against a pre-defined threshold.
* Switching Mechanism: Once darkness is detected, the microcontroller triggers a relay module to activate the light bulb.
<img width="1117" height="761" alt="لقطة شاشة 2026-07-18 145526" src="https://github.com/user-attachments/assets/a58e6a3e-485e-48e5-9c92-2ab41c7ba425" />

---

## 🔌 Circuit Specifications
The prototype is constructed using the following core components:
* Arduino Uno: The brain of the operation.
* LDR (Light Dependent Resistor): To detect ambient light levels.
* 10kΩ Resistor: Used in the voltage divider circuit with the LDR.
* Relay Module: To safely control the high-voltage light bulb via the low-voltage Arduino signals.
<img width="906" height="738" alt="لقطة شاشة 2026-07-18 145618" src="https://github.com/user-attachments/assets/87ca69e5-2c6c-4a24-9fee-eb0c86dfad1e" />


---

## 💻 Firmware Logic
The firmware utilizes simple analogRead() functions to monitor the sensor:
* Calibration: The threshold value can be adjusted in the code to suit different lighting environments.
* Automation: The loop() function continuously evaluates the light levels, ensuring the light turns on immediately at dusk and off at dawn.

---

## 👤 Developer
* Eng. Noura Abbad Al-Qathami - [https://github.com/alotibin212-glitch](https://github.com/alotibin212-glitch)
