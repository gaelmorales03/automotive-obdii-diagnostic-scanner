# Automotive OBD-II Diagnostic Scanner

This project implements a vehicle diagnostic scanner capable of sending OBD-II requests and intepreting ECU responses over CAN communication.

The system supports real-time PID and Diagnostic Trouble Code (DTC) management, simulating the behaviour of industry-level automotive diagnostics.

---

## Features

- Send OBD-II requests (Mode 01, Mode 03, Mode 04)
- Read en decode vehice PIDs (RPM, Fuel level, Battery Voltage, Linear speed, etc.)
- Retrieve and clear Diagnostic Trouble Codes (DTCs)
- Real-time CAN processing.
- Modular architecture for communication and data parsing.

---

## System architecture

The system is structured in modular layers:

1. **CAN INTERFACE**
   - Handles the communication with the vehicle ECU.
   - Sends and receives CAN frames
     
2. **OBD-II REQUEST HANDLER**

---

## Tested Vehicles

| Vehicle            | Model Year |
| ------------------ | ---------- |
| Nissan Sentra      | 2020       |
| Lincoln MKZ Hybrid | 2018       |
| Honda HRV          | 2017       |
| Suzuki Swift       | 2022       |
| Ford Fiesta        | 2019       |

---

##  Author

Gael Alejandro Morales Rodríguez
