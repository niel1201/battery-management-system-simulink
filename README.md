# Battery Management System (BMS) in Simulink

## Overview

This project presents the design and implementation of a Battery Management System (BMS) using MATLAB Simulink. It includes modeling of battery dynamics, SOC estimation, thermal behavior, protection logic, cell balancing, and Kalman-based SOC estimation.

---

## Features

* First-order battery model (OCV + RC network)
* SOC estimation using Coulomb counting
* Thermal modeling (Rth–Cth)
* Protection system (overvoltage, undervoltage, temperature)
* Multi-cell battery system
* Passive cell balancing
* Kalman filter-based SOC estimation

---

## Project Structure

### 1. Single Cell BMS

* Battery equivalent circuit model
* SOC estimation (Coulomb counting)
* Thermal model
* Protection logic

---

### 2. Two-Cell BMS with Balancing

* Multi-cell system
* Voltage-based passive balancing
* Control tuning for stability

---

### 3. Kalman Filter SOC Estimation

* Voltage-based SOC correction
* Comparison with Coulomb counting
* Improved estimation accuracy

---

## Key Equations

SOC estimation:
[
SOC = SOC_0 - \frac{1}{Q} \int I dt
]

Thermal model:
[
\frac{dT}{dt} = \frac{I^2 R}{C_{th}} - \frac{T - T_{amb}}{R_{th} C_{th}}
]

Kalman update:
[
SOC = SOC_{pred} + K (V_{actual} - V_{est})
]

---

## Tools Used

* MATLAB Simulink

---

## Learning Outcomes

* Battery modeling and simulation
* State estimation techniques
* Control system design
* Multi-cell balancing strategies

---

## Future Work

* Extended Kalman Filter (EKF)
* Real-time implementation (Arduino / PIC)
* State of Health (SOH) estimation

---

## Author

Nirmith Puneet
