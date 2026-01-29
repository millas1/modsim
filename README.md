#  SIR Model - Vaccination

A system dynamics modeling project analyzing COVID-19 pandemic responses using an extended SIR (Susceptible-Infectious-Recovered) model with vaccination strategies.

##  Project Overview

This project models disease transmission dynamics with a focus on hospital and ICU capacity constraints. The classical SIR model is extended to include disease severity compartments (Home, Severe, Critical) and vaccination strategies.

---

##  Project Structure

### Task 1: Model Design
*Causal loop diagram and stock-and-flow diagram implementation*
- `influenza_baseline_model_task1.alp` — Initial SIR model in AnyLogic

### Task 2: Sensitivity Analysis & Lockdown Events
*Parameter variation and intervention modeling*
- `task2/` — Lockdown event definitions and parameter sensitivity analysis
- `task2/lockdownEventDescription.txt` — Lockdown event specifications

### Task 3: Historical Data Calibration
*COVID-19 UK first wave parameter fitting*
- `task3/task3.ipynb` — Parameter calibration notebook
- `task3/influenza_task3.alp` — Calibrated model
- `task3/anylogic_parameters.csv` — Fitted parameters
- `task3/lockdown_events.csv` — Historical lockdown timeline

### Task 4: Vaccination Implementation
*Adding vaccination flows to the model*
- `task4/influenza_task4.alp` — Extended model with vaccination

### Task 5: Vaccination Dose Requirements
*Determining vaccination targets for ICU capacity control*
- `task5/influenza_task5.alp` — Scenario analysis model

---

##  Key Model Parameters

| Parameter | Description |
|-----------|-------------|
| **α** | Infection probability per contact |
| **c** | Daily contacts per person |
| **p_h, p_s, p_c** | Severity probabilities (home, hospital, ICU) |
| **β_h, β_s, β_c** | Recovery rates by severity level |

---

## Tools Used

- **AnyLogic** — System dynamics simulation
- **Python/Jupyter** — Data analysis and calibration
