# Automotive OBD-II Diagnostic Scanner

LabVIEW-based vehicle diagnostic tool capable of requesting live OBD-II PIDs, filtering CAN traffic, reading DTC fault codes, and clearing vehicle errors.

---

## Overview

This project consists of an automotive diagnostic interface developed in LabVIEW and tested on real production vehicles.

The system establishes an OBD-II diagnostic session, clears previous CAN traffic, and provides an interactive HMI dashboard for requesting live vehicle parameters.

Validated on:

* Nissan Sentra 2020
* Lincoln MKZ Hybrid 2018
* Honda HRV 2017
* Suzuki Swift 2022
* Ford Fiesta 2019

---

## Core Features

✅ Start diagnostic session via OBD-II
✅ Real-time PID requests
✅ Fuel level monitoring
✅ Vehicle speed reading
✅ Battery / voltage values
✅ CAN message filtering
✅ Read Diagnostic Trouble Codes (DTCs)
✅ Clear DTC fault codes
✅ Graphical HMI interface in LabVIEW

---

## How It Works

Each UI switch sends a specific OBD-II request to the vehicle ECU.

Examples:

* Fuel percentage
* Linear speed
* Voltage
* Additional live sensor parameters

The system simultaneously filters CAN traffic to identify and display only relevant messages associated with each request.

---

## Technologies

* LabVIEW
* OBD-II Protocol
* CAN Bus
* Automotive Diagnostics
* HMI Development
* Real Vehicle Testing

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

## Applications

* Vehicle diagnostics
* ECU communication analysis
* CAN reverse engineering
* Automotive validation
* Engineering tools development

---

## 👨‍💻 Author

Gael Alejandro Morales Rodríguez
