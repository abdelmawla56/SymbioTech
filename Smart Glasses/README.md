# Overview

The Smart Glasses are the first core device in the SymbioTech Assistive Ecosystem, designed to empower visually impaired individuals by enhancing independence, navigation, and situational awareness.
Using AI, ESP32-CAM, and ultrasonic sensors, the glasses can read printed text aloud, recognize faces and objects, and assist users with navigation through real-time audio feedback.

# Objectives

Provide real-time audio feedback for object and text recognition.

Enhance navigation and obstacle detection for blind users.

Serve as the foundation for future ecosystem integration with the Smart Gloves and Mobile App.
# Features

Text-to-Speech: Reads printed text aloud using OCR and speech synthesis.
Object & Face Recognition: Identifies items and people via the ESP32-CAM.
Obstacle Detection: Uses ultrasonic sensors to detect nearby obstacles.
Wireless Connectivity: Communicates with the central mobile application via Wi-Fi/Bluetooth.

# System Architecture
Camera (ESP32-CAM)
      ↓
Image Processing (AI model)
      ↓
Text/Object Recognition
      ↓
Audio Feedback via Speaker
      ↓
User Interaction & Navigation Guidance

# Components Used
Component	Function
ESP32-CAM	Captures video and images for processing.
Ultrasonic Sensor (HC-SR04)	Detects obstacles and measures distance.
Speaker / Buzzer	Provides voice feedback and alerts.
Power Source (Battery Module)	Powers the system for portability.
Mobile App (Wi-Fi Link)	Receives and sends processed data.
 Setup Instructions
 Hardware Setup

Connect HC-SR04 ultrasonic sensor to ESP32-CAM (VCC → 5V, GND → GND, Trig → GPIO12, Echo → GPIO13).

Attach mini speaker to the ESP32-CAM for audio output.

Power via USB or Li-ion battery.

 Software Setup

Install Arduino IDE and ESP32 board drivers.

Add ESP32-CAM by selecting “AI Thinker ESP32-CAM” under Tools → Board Manager.

Upload the esp32_camera_setup.ino file.

Configure your Wi-Fi SSID and password in the sketch.

Open the CameraWebServer serial monitor to view live stream.

# Testing
Test Case ID	Test Description	Expected Output	Status
TC01	Detect object within camera frame	Object name spoken aloud	 Passed
TC02	Recognize text from image	Text read via TTS	 Passed
TC03	Detect obstacle using ultrasonic sensor	Distance alert sound	 In Progress
TC04	Connect to mobile app	Data transmitted successfully	 Passed
# Future Enhancements

GPS integration for outdoor navigation.

Emotion detection and context-aware audio tone.

Cloud connectivity for AI model updates.
