# 🔬 Zener Diode Tester using Op-Amp (Simulation Project)

This project involves designing and simulating a **Zener Diode Tester using Op-Amp**. The circuit uses the LM741 operational amplifier configured as a comparator to detect the breakdown voltage of a Zener diode and indicate the result via an LED. The simulation is done in **Proteus Design Suite**.

## 📌 Project Overview

- **Type:** Analog Simulation Project  
- **Platform:** Proteus Design Suite  
- **Tools Used:** LM741 Op-Amp, 1N4733A Zener Diode (5.1V), Resistors, Potentiometer, LED  
- **Goal:** To visually identify when a Zener diode reaches its breakdown voltage using comparator logic.

## ⚙️ Circuit Description

The LM741 Op-Amp is used in comparator mode:

- **Non-Inverting Input (+):** Receives 5.1V from a reverse-biased Zener diode  
- **Inverting Input (−):** Gets a variable voltage from a 1kΩ potentiometer  
- **Output:**
  - **HIGH (LED ON)** when V− < 5.1V
  - **LOW (LED OFF)** when V− > 5.1V

This simulates real-world testing of a Zener diode in lab environments.

## 🔧 Components Used

| Component       | Value / Model | Quantity | Role                                 |
|----------------|----------------|----------|--------------------------------------|
| Zener Diode     | 1N4733A (5.1V) | 1        | Provides reference voltage           |
| Op-Amp          | LM741          | 1        | Comparator configuration             |
| Resistors       | 1kΩ, 330Ω      | 3 total  | Current limiting and voltage divider|
| Potentiometer   | 1kΩ            | 1        | Adjusts inverting input voltage      |
| LED             | Red            | 1        | Indicates comparator output          |
| Power Supply    | 12V DC         | 1        | Powers the circuit                   |

## 🧪 Simulation Process

1. Built and connected components in Proteus.  
2. Placed the Zener diode in reverse bias for 5.1V reference.  
3. Connected potentiometer to the inverting terminal of the Op-Amp.  
4. Ran simulation and gradually varied the potentiometer.  
5. Observed LED behavior to determine threshold crossing.  
6. Confirmed sharp transition using oscilloscope tool.

## 📊 Observation Table

| Time (ms) | V− (Inverting) | V+ (Zener Ref) | Output Voltage | LED Status |
|-----------|----------------|----------------|----------------|------------|
| 0.0–0.5   | < 5.1V         | ≈ 5.1V         | HIGH (~12V)    | ON         |
| ~0.6      | ≈ 5.1V         | ≈ 5.1V         | Transition     | Switching  |
| >0.6      | > 5.1V         | ≈ 5.1V         | LOW (~0V)      | OFF        |

## 🧠 Learnings

- Basics of Op-Amp comparator configuration  
- Behavior of Zener diodes in reverse bias  
- Circuit simulation and debugging using Proteus  
- Visual voltage threshold detection

## 📁 File Structure

zener-diode-tester/ ├── README.md ├── Report/ │ └── Zener_Diode_Tester_Report.pdf ├── CircuitDiagram/ │ └── zener_tester_diagram.png ├── SimulationFiles/ │ └── zener_tester.pdsprj


## 🚀 Future Improvements

- Display Zener voltage using 7-segment or digital LCD  
- Add microcontroller for automated diode detection  
- Use precision Op-Amps for critical analog testing  
- Support for multiple diode types and voltages

## 📎 Resources

- 📄 [Project Report (PDF)](https://github.com/Vansh0917/zener-diode-tester/blob/0940c9c582d043307591ce8ff3f7ea467f41897c/zener-diode-tester/Report/Project%20_%20Zener%20Diode%20Tester%20using%20Op-Amp%20(1).pdf)
- 🔗 [Google Drive Circuit Diagram](https://drive.google.com/file/d/17hUvKsxiCaZJrs70Yhgb6Tc4fQ2AnfWu/view?usp=sharing)

## 👤 Author

**Vansh Vaghela**  
Electronics & Communication Engineering  (4TH SEM)
Government Engineering College, Gandhinagar  

