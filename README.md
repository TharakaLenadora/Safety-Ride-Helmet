# 🪖 Smart Helmet System

An IoT-based Smart Helmet developed using the **ESP32** to improve rider safety. The system detects crashes using an **MPU6050 accelerometer**, monitors rider drowsiness with an **IR eye-blink sensor**, tracks location using a **GPS module**, and sends emergency SMS alerts through a **SIM800L GSM module**. Voice warnings are provided using a **DFPlayer Mini**, while Bluetooth Low Energy (BLE) allows users to configure the emergency contact number and custom alert message from an Android application.

## ✨ Features

* 🚨 Crash detection using free-fall and impact detection
* 📍 GPS location tracking with Google Maps link
* 📱 Automatic emergency SMS notification
* 😴 Drowsiness detection with audio wake-up alert
* ⚠️ Overspeed warning based on GPS speed
* 🔊 Voice announcements using DFPlayer Mini
* 📶 BLE configuration for emergency contact and message
* 💾 Stores user settings permanently in ESP32 flash memory

## 🛠 Hardware

* ESP32
* MPU6050 Accelerometer
* SIM800L GSM Module
* Neo-6M GPS Module
* DFPlayer Mini
* IR Eye Blink Sensor
* Speaker
* MicroSD Card

## 📚 Required Libraries

* Adafruit MPU6050
* Adafruit Unified Sensor
* TinyGPS++
* DFRobotDFPlayerMini
* Preferences (ESP32)
* BLEDevice
* Wire

## ⚙️ System Workflow

1. The ESP32 continuously monitors acceleration, eye status, and GPS speed.
2. If a crash is confirmed, the GPS location is obtained and an emergency SMS with a Google Maps link is sent automatically.
3. If the rider's eyes remain closed for a predefined time, a wake-up audio alert is played.
4. When the vehicle exceeds the configured speed limit, an overspeed warning is issued.
5. Users can update the emergency contact number and custom SMS message through a BLE-enabled Android application.

## Images 
![image alt](https://github.com/TharakaLenadora/Safety-Ride-Helmet/blob/baa679bd3b04b845174b539d02964e7a2a752b50/WhatsApp%20Image%202026-07-24%20at%2002.26.32%20(2).jpeg)

![image alt](https://github.com/TharakaLenadora/Safety-Ride-Helmet/blob/baa679bd3b04b845174b539d02964e7a2a752b50/WhatsApp%20Image%202026-07-24%20at%2002.26.32%20(1).jpeg)

![image alt](https://github.com/TharakaLenadora/Safety-Ride-Helmet/blob/baa679bd3b04b845174b539d02964e7a2a752b50/WhatsApp%20Image%202026-07-24%20at%2002.26.32%20(3).jpeg)
