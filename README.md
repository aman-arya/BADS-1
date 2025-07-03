# AutonomousShipment — Trial Roll-Out (Part 1)

Welcome to the *AutonomousShipment* project!  
This repository contains everything needed to reproduce the analysis and recommendations for the first stage of our autonomous-delivery pilot in Leeds.

---

## 📜 Overview

We have two key managerial decisions to make:

1. **Prototype Selection** – choose **one** of four autonomous-robot prototypes for the trial.  
2. **Resource Allocation** – decide how many of the chosen robots to assign to each partner store so that we maximise daily deliveries **within budget and staffing limits**.

The outcome of this work will guide our one-month pilot across grocery, clothing and sports-equipment retailers in the Leeds area.

---

## 1  Background

AutonomousShipment is a Leeds-based start-up backed by UK venture-capital funds and government support.  
Our goal is to use small ground-based delivery robots to speed up last-leg logistics, cutting costs for retailers and delighting consumers with faster, greener deliveries.

For this pilot we have built four hardware prototypes:

| Prototype | Nickname |
|-----------|----------|
| `A032` | **Archer** |
| `B23`  | **Bowler** |
| `CJKL` | **Corner** |
| `DSXX` | **Deviant** |

Only one of these will be taken into the live trial.

---

## 2  Decision #1 – Prototype Selection

### 2.1  Decision criteria

| Criterion | What it means | Preferred direction |
|-----------|---------------|---------------------|
| **Carrying capacity** (litres) | Cargo volume | *Higher* |
| **Battery size** (hours) | Un-recharged run-time | *Higher* |
| **Average speed** (km h⁻¹) | Typical cruising speed | *Higher* |
| **Cost per unit** (£) | Capital expense | *Lower* |
| **Reliability** (hours MTBF) | Mean time between failures | *Higher* |

> ⚠️ *The autonomous-navigation software is **not** part of this evaluation – focus strictly on the hardware specs.*

### 2.2  Data sources

| File | Description |
|------|-------------|
| **`data/Robot_Info.csv`** | Raw specs for each prototype |
| **`data/Management_Priority.xlsx`** | Relative weights/importance (agreed July 2023) |

---

## 3  Decision #2 – Robot Allocation

Once a prototype is chosen, we must allocate robots to three partner stores:

| Store type | Code | Orders / robot / day | Operating cost / robot / month (£) | Technician hours / robot / week |
|------------|------|----------------------|------------------------------------|---------------------------------|
| Grocery | `G` | **9** | **1 600** | **10** |
| Clothing | `C` | **6** | **1 000** | **7** |
| Sports equipment | `S` | **4** | **600** | **5** |

### 3.1  Trial constraints

* Minimum **5 robots per store**  
* **Budget** ≤ **£250 000** (purchase **+** one-month operating costs)  
* **Technician capacity** ≤ **250 staff-hours / week**  
* Objective: **maximise total daily orders delivered**

---

## 4  Repository Layout

