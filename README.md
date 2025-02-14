# Automatic RFID-Based Toll Management System

## Description  
This project automates toll collection using RFID tags for vehicle identification and GSM for balance updates via SMS. The system features real-time fee deduction based on vehicle type (Bike/Bus/Car/Truck), LCD status display, servo-controlled gate mechanisms, and EEPROM-based balance storage. Administrators can adjust account balances directly via hardware buttons.

## Key Features
- **RFID Authentication**: Validates registered vehicle tags (5 pre-configured users).
- **Dynamic Toll Fees**: Charges ₹5 (Bike), ₹10 (Bus), ₹15 (Car), and ₹20 (Truck).
- **SMS Notifications**: Sends payment success/low-balance alerts via GSM module.
- **Gate Control**: Opens/closes toll gates using a servo motor after payment verification.
- **Balance Management**: Updates stored balances in EEPROM and allows manual adjustment via UI.

## Hardware Components
- Arduino Uno 
- RFID Reader (SoftwareSerial)  
- GSM Module (SIM800L)  
- 16x2 LCD  
- SG90 Servo Motor  
- Tactile Switches (for balance setup)  

## Pin Mapping
| Component       | Arduino Pin |
|-----------------|-------------|
| LCD RS          | A1          |
| LCD EN          | A0          |
| LCD D4-D7       | A5, A4, A3, A2 |
| Servo           | 9           |
| RFID RX/TX      | 8
