# 🌿 AgriPulse
### *Automated Climate-Controlled Storage for Post-Harvest Crop Preservation*


![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=arduino&logoColor=white)

Onions are one of India's most consumed crops and one of the most wasted. AgriPulse is a hardware-software ecosystem built to fix that. A physical Arduino-based climate control unit monitors the storage environment in real time, while an Android app gives farmers live visibility into what's happening inside their storage: temperature, humidity, gas levels, before spoilage even begins.

---

## 🚨 The Problem

Post-harvest losses in perishable crops like onions, garlic, and bulbs account for 30 to 40% of a farmer's total yield. The culprit isn't bad farming, it's bad storage. Fluctuating temperature and humidity, combined with gas buildup from rotting produce, create a chain reaction that farmers can't see until it's too late. Static storage with zero monitoring means by the time something smells wrong, the damage is already done.

---

## 💡 Our Solution

We built an automated climate-controlled storage system where the environment actively adjusts itself based on sensor readings. The hardware monitors conditions continuously and triggers exhaust fans when thresholds are crossed. The Android app connects via HC-05 Bluetooth (Firebase used for full feature demonstration) so farmers can monitor all 6 storage shelves remotely, get instant alerts, and track how conditions are changing over time, all from their phone.

---

## 🔧 Hardware Architecture

| Component | Role |
|---|---|
| Arduino Uno | Brain of the system, reads sensors and triggers actuators |
| DHT-11 | Monitors temperature and humidity in real time |
| MQ-135 | Detects harmful gas levels from rotting produce |
| HC-05 | Bluetooth module, streams data to Android app |
| 16x2 I2C LCD | Local real-time display of climate data |
| Exhaust Fans | Auto-triggered to expel heat and regulate environment |

---

## 📱 App Features

- **Splash & Secure Login** via Firebase Authentication
- **6-Shelf Live Dashboard** with color-coded shelf status (🟢 Safe / 🟡 Warning / 🔴 Critical)
- **Live Stats** with real-time temperature, humidity and gas readings
- **Rate of Change Graphs** showing how conditions shift over time (MPAndroidChart)
- **Smart Alerts** when gas, temperature or humidity cross safe thresholds
- **Multilingual Support** in English, Hindi (हिन्दी) and Marathi (मराठी)

---

## 🛠️ Tech Stack

- **Platform:** Android Studio (Java, Min SDK 23)
- **Database:** Firebase Realtime Database
- **Auth:** Firebase Authentication
- **Bluetooth:** HC-05 (hardware data source)
- **Charts:** MPAndroidChart
- **UI:** Material Design Components

## 📸 App Screenshots

| | | | |
|:----:|:----:|:----:|:----:|
| <img src="WhatsApp%20Image%202026-06-06%20at%208.54.57%20AM.jpeg" width="200"/> | <img src="WhatsApp%20Image%202026-06-06%20at%208.54.57%20AM%20(1).jpeg" width="200"/> | <img src="WhatsApp%20Image%202026-06-06%20at%208.54.58%20AM.jpeg" width="200"/> | <img src="WhatsApp%20Image%202026-06-06%20at%208.54.58%20AM%20(1).jpeg" width="200"/> |
| Login Screen | Navigation Drawer | Home Screen | Language Select |
| <img src="WhatsApp%20Image%202026-06-06%20at%208.54.58%20AM%20(2).jpeg" width="200"/> | <img src="WhatsApp%20Image%202026-06-06%20at%208.54.59%20AM.jpeg" width="200"/> | <img src="WhatsApp%20Image%202026-06-06%20at%208.54.59%20AM%20(1).jpeg" width="200"/> | <img src="WhatsApp%20Image%202026-06-06%20at%208.55.00%20AM.jpeg" width="200"/> |
| Shelf Monitoring | Shelf Alert | Stats Over Time | Push Notification |



---

## 🎯 Goal

To reduce spoilage in perishable crops by giving farmers real-time visibility and automated climate control, increasing shelf life, cutting losses, and protecting farmer income.

---

*Built by AgriPulse because farmers deserve better tools.*
