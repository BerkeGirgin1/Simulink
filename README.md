# Start-Stop Engine Control System (ECU) Simulation

## 📌 Project Description
This project simulates a vehicle's **Engine Control Unit (ECU)** using **MATLAB/Simulink** and **Stateflow**. It models the logic for a Start-Stop system, ensuring safety conditions are met before cranking and managing the alternator voltage during operation.

The system is validated with **100% Model Coverage (MCDC)** using automated Excel-based test scenarios.

## 🚀 Key Features
* **Safety Interlock Logic:** Ensures the engine only starts if the Gear is in **Park (P)** or **Neutral (N)** and the **Brake** is pressed.
* **Stateflow Logic:** Manages states: `OFF` -> `CRANKING` -> `RUNNING`.
* **System Protection:** Includes a **3-second Timer** to abort cranking if the engine fails to start.
* **Realistic Simulation:** Simulates battery voltage drop during cranking (10V) and alternator charging ramp (up to 12.5V).
* **Stall Protection:** Automatically cuts off the engine if RPM drops below 500.

## 🛠️ Tools Used
* Simulink
* Stateflow
* Simulink Coverage

## 📂 File Structure
* `Start_Stop_ECU.slx`: Main Simulink model.
* `Test_Cases.xlsx`: Test scenarios for coverage analysis.
* `Coverage_Report.html`: Proof of 100% decision coverage.

## 📊 Logic & Coverage
The model achieves **100% Decision and Execution Coverage**.
* **Input:** Excel-driven sequential testing.
* **Scenarios:** Includes Pass/Fail tests for Gear errors, Brake checks, and Timer timeouts.

## 👨‍💻 Author
Berke Girgin
Electronics and Communication Engineering Student
