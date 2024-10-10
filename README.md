# CipherGate: Arduino-Powered Electromagnetic Door Lock System

## Project Overview

CipherGate is an Arduino-powered electromagnetic door locking system designed to provide secure and user-friendly access control. This system combines an RFID reader, keypad, and LCD display for convenient and secure entry. The project utilizes the Arduino Uno R4 WiFi board to manage authentication via RFID tags and a numeric keypad, displaying feedback through a 16x2 LCD screen.

---

## Table of Contents
1. [Introduction](#introduction)
2. [Components](#components)
3. [Circuit Diagram](#circuit-diagram)
4. [How It Works](#how-it-works)
5. [User Guide](#user-guide)
6. [License](#license)

---

## Introduction

Welcome to CipherGate! This project utilizes various components to create a secure, accessible, and efficient electromagnetic door lock system. CipherGate is designed to allow users to unlock doors using RFID tags or numeric passwords, ensuring a versatile and scalable solution for home or office security.

---

## Components

CipherGate consists of the following hardware components:

- **Arduino Uno R4 WiFi**: The microcontroller responsible for processing input and controlling the electromagnetic lock.
- **Single Channel 5V Relay**: Manages the high-power electromagnetic door lock.
- **JIS 842-901G Electromagnetic Lock**: The locking mechanism used to secure the door.
- **4x3 Keypad**: Allows users to input passwords for unlocking the door or adding new RFID tags.
- **MFRC522 RFID Reader**: Enables RFID tag authentication for door access.
- **16x2 LCD Display**: Provides visual feedback to the user, such as successful unlocks or password input errors.
- **I2C Controller for the 16x2 Display**: Manages communication between the Arduino and the LCD screen.
- **PNP Transistor BC557CBK**: Controls the relay switching.
- **Diode 1N4148**: Protects the circuit from voltage spikes.

---

## Circuit Diagram

The system integrates the Arduino with the RFID reader, keypad, and LCD display to control the electromagnetic lock. The circuit diagram illustrates how all components are connected to ensure proper functionality and reliable operation.

---

## How It Works

CipherGate operates in the following steps:
1. **Power Up**: The system starts up, and the LCD displays a welcome message.
2. **Adding a New RFID Tag**:
   - Enter `*001` followed by the current PIN on the keypad.
   - Approach a new RFID tag to the reader to register it.
   - You can add up to 5 RFID tags.
3. **Changing the PIN**:
   - Enter `*000` followed by the current password.
   - Set the new password using the keypad.
4. **Unlocking the Door**:
   - Enter the correct password or scan a registered RFID tag to unlock the door.
   - The electromagnetic lock disengages, and the door can be opened.

---

## User Guide

Follow these simple steps to use CipherGate:

1. **Step 1**: Connect the system to the power supply.
2. **Step 2**: Wait for the LCD screen to display the welcome message.
3. **Step 3**: To add a new RFID tag, enter `*001` followed by the current PIN on the keypad.
4. **Step 4**: Approach the RFID tag to the reader to register it. You can add up to 5 RFID tags.
5. **Step 5**: To change the password, enter `*000` followed by the current password and then set a new one.
6. **Step 6**: To unlock the door, either enter the correct password or scan a registered RFID tag.
7. **Step 7**: Congratulations! The door is now unlocked.

---

## License

This project is open-source and available under the [MIT License](LICENSE).
