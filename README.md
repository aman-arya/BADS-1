# AutonomousShipment Autonomous Delivery Trial

## Overview  
This repository contains all instructions and data needed to conduct a one-month trial roll-out of AutonomousShipment’s last-leg delivery robots around Leeds. Management will use this trial to:

1. **Select** the optimal prototype robot for the trial (Task 1).  
2. **Allocate** a fleet of robots across different store types under budget, staffing, and coverage constraints (Task 2).

---

## Table of Contents

- [Background](#background)  
- [Data Files](#data-files)  
- [Task 1: Prototype Selection](#task-1-prototype-selection)  
  - [Decision Criteria](#decision-criteria)  
  - [What to Deliver](#what-to-deliver)  
- [Task 2: Fleet Allocation](#task-2-fleet-allocation)  
  - [Store Types & Delivery Rates](#store-types--delivery-rates)  
  - [Costs & Staffing](#costs--staffing)  
  - [Constraints & Objectives](#constraints--objectives)  
  - [What to Deliver](#what-to-deliver-1)  
- [Report Requirements](#report-requirements)  
- [Submission](#submission)

---

## Background  
AutonomousShipment is a Leeds-based start-up backed by VC investors and the UK government. We operate autonomous robot drones for last-mile deliveries, aiming for faster service and lower costs. To prepare for full scale-up, we will trial one prototype robot type—deployed across grocery, clothing and sport-equipment stores—in the Leeds area.

---

## Data Files  
Place the following in this repo’s root before you begin:

- **`Robot_Info.csv`**  
  Contains numeric data for each prototype’s:  
  - Carrying capacity (litres)  
  - Battery life (hours)  
  - Average speed (km/h)  
  - Unit cost (GBP)  
  - Reliability (hours between breakdowns)

- **`Management_Priority.xlsx`**  
  Management’s weighting of each decision criterion (derived July 2023).

---

## Task 1: Prototype Selection  

### Decision Criteria  
Select one robot out of:  
- **Robot A032 – Archer**  
- **Robot B23 – Bowler**  
- **Robot CJKL – Corner**  
- **Robot DSXX – Deviant**  

Evaluate each by:  
1. **Carrying Capacity** (higher = better)  
2. **Battery Size** (hours; higher = better)  
3. **Average Speed** (km/h; higher = better)  
4. **Cost per Unit** (GBP; lower = better)  
5. **Reliability** (hours between breakdowns; higher = better)  

Weight each criterion by the values in `Management_Priority.xlsx` to **maximize overall utility**.

### What to Deliver  
- A clear **recommendation**: which prototype to trial.  
- A **utility-scoring table** showing each robot’s normalized score × weight.  
- A brief **justification** (approx. 300 – 400 words) referencing both quantitative scores and any qualitative considerations.

---

## Task 2: Fleet Allocation  

### Store Types & Delivery Rates  
| Store Type             | Orders/robot/day |
|------------------------|------------------|
| Grocery Store          | 9                |
| Clothing Store        | 6                |
| Sport Equipment Store | 4                |

### Costs & Staffing  
- **Acquisition Cost**: unit cost of selected prototype (from Task 1).  
- **Operating Cost (month)**:  
  - Grocery: £1,600/robot  
  - Clothing: £1,000/robot  
  - Sport Equipment: £600/robot  
- **Technician Support** (hours/robot/week):  
  - Grocery: 10 h  
  - Clothing: 7 h  
  - Sport Equipment: 5 h  

### Constraints & Objectives  
1. **Minimum fleet**: at least **5 robots** per store type.  
2. **Budget cap**: total acquisition + operating costs ≤ **£250,000**.  
3. **Staffing cap**: total technician hours ≤ **250 h/week**.  
4. **Goal**: maximize **total orders per day** across all stores.

### What to Deliver  
- An **allocation table**: number of robots per store.  
- **Cost calculation** showing acquisition + operating vs. budget.  
- **Staffing calculation** vs. available hours.  
- **Total daily orders** achieved.  
- A concise **recommendation** explaining your allocation logic (approx. 300 – 400 words).

---

## Report Requirements  
- **Format**: single report (Word or PDF).  
- **Length**: ≤ 1,500 words total for both tasks.  
- **Include**:  
  - Tables and figures as needed.  
  - Clear headings corresponding to each deliverable.  
  - Appendix with raw calculation tables (if desired).

---

## Submission  
1. Push your completed report (`AutonomousShipment_Trial_Report.docx` or `.pdf`) to this repo.  
2. Include any supporting spreadsheets or export tables as CSVs under a `/data` directory.  
3. Create a Pull Request against the **`main`** branch by the deadline.

Good luck! If you have any questions, please open an Issue in this repository.
