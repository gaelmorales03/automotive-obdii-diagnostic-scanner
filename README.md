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

## Implementation details 

The system was implemented in LabVIEW using a modular block-diagram architecture.

- CAN frames are processed as byte arrays (payload[0-7])
- Case structures are used to interpret PIDs and diagnostic responses, as well as filtering data the user wants.
- Data flows through multiple processing stages before visualization (the data is decoded and filtered before arriving to the UI).

---

## System architecture

The system is structured in modular layers:

1. **CAN INTERFACE**
   - Handles the communication with the vehicle ECU.
   - Sends and receives CAN frames
     
2. **OBD-II REQUEST HANDLER**
   - Divides the tasks between PID request queries and DTC reading process.

3. **FRAME PARSERS**
   - Extracts the payload data from the CAN messages.
   - Identifies the responses filtering the data based on CAN IDs

4. **PID/DTC Processing**
   - Decodes the raw data into readable values to be displayed on the UI.
   - Interprets diagnostic trouble codes showing the error code and identifying which module is at fault.
  
5. **User Interface**
   - Displays real-time vehicle parameters
   - Shows system status and diagnostic results
   - Allows the user to select certain PIDs and erase DTCs.

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
