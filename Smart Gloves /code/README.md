# Overview

The Smart Gloves are a key component of the Smart Assistance System designed to support individuals with hearing or speech impairments. The gloves detect hand gestures and convert them into text or speech using embedded sensors and a microcontroller. This project focuses on building, programming, and testing the glove hardware as the second phase following the development of the smart glasses.

# Objectives

Detect specific gestures using flex sensors and motion sensors (e.g., MPU6050).

Convert gestures into recognizable text or speech through software integration.

Transmit gesture data wirelessly to the main system (e.g., via Bluetooth or Wi-Fi).

Provide real-time feedback to users via audio or display.

# Features

Embedded flex sensors for finger movement detection.

MPU6050 for orientation and motion detection.

Microcontroller (ESP32 or Arduino Nano) for processing sensor input.

Wireless communication (Bluetooth/Wi-Fi) with the central unit or mobile app.

Integration with a text-to-speech module or app for gesture translation.

# Hardware Components
Component	Description
Flex Sensors	Detect bending of fingers
MPU6050	Measures motion and tilt
ESP32 / Arduino Nano	Microcontroller for processing
Bluetooth / Wi-Fi Module	Wireless communication
Power Source	Rechargeable battery or USB
Jumper Wires, Breadboard	Circuit connection and testing

# Software & Tools

Arduino IDE – for programming the microcontroller

C / C++ – main programming language

Serial Monitor / Bluetooth App – for testing gesture data

Text-to-Speech API – converts recognized gestures to speech

# Working Principle

Input: User performs a hand gesture.

Detection: Flex and motion sensors measure finger bending and orientation.

Processing: The microcontroller interprets sensor data.

Transmission: Processed gesture data is sent via Bluetooth/Wi-Fi.

Output: The receiver displays or speaks the corresponding text.

# Testing

Each gesture was tested for consistency and accuracy using the serial monitor.

Data transmission was verified between gloves and receiver module.

Real-time response was optimized through code calibration.


# Future Improvements

Add machine learning for more gesture recognition.

Integrate haptic feedback for communication confirmation.

Combine with smart glasses for full bidirectional communication.
