# AutonomousShipment – Trial Roll-Out (Part 1)

Welcome to the **AutonomousShipment** trial-roll-out repository!  
This README summarises the requirements and tasks for the analytic manager’s report that will guide our one-month pilot of autonomous delivery robots in and around **Leeds, UK**.

---

## 📦 Background

AutonomousShipment is a Leeds-based start-up using **autonomous robot drones** to perform last-leg logistics, delivering goods directly to customers’ doorsteps.  
The project is backed by UK venture-capital investors and government support. By automating deliveries we aim to:

* Provide **faster delivery** for consumers  
* Achieve **cost optimisation** and operational efficiency for the company  

For the pilot we will partner with local **grocery, clothing, sport-equipment, and tech stores**.

---

## 🛑 Key Management Decisions

1. **Prototype Selection** – choose **one** of four in-house robot prototypes for the trial.  
2. **Robot Allocation** – decide how many robots each store type receives while meeting budget and resource constraints.

---

## 📂 Data Files

| File | Purpose |
|------|---------|
| `Robot_Info.csv` | Quantitative specs for each robot prototype |
| `Management_Priority.xlsx` | Weights/importance of each decision criterion (derived July 2023) |

---

## 🏗 Prototype Robots

| ID | Codename |
|----|----------|
| A032 | Archer |
| B23  | Bowler |
| CJKL | Corner |
| DSXX | Deviant |

### Evaluation Criteria

| Criterion | Unit | Preference |
|-----------|------|------------|
| **Carrying Capacity** | Litres | Larger is better |
| **Battery Size** | Hours | Larger is better |
| **Average Speed** | km / h | Higher is better |
| **Cost per Unit** | GBP | Lower is better |
| **Reliability** | Hours between breakdowns | Higher is better |

> **Note:** Software/autonomous-navigation performance is out of scope; focus solely on **hardware**.

---

## 🎯 Task 1 – Prototype Recommendation (Max 1 500 words; 50 % of marks)

* Use the criteria above and the management weightings to **maximise overall utility**.  
* Provide a clear, data-driven recommendation of **which single prototype** should be used in the trial.  
* Present findings with appropriate **tables, figures, and narrative** for senior management.

---

## 🛒 Store Types & Trial Parameters

| Store Type | ⬆️ Orders / Robot / Day | ⚙️ Operating Cost / Robot / Month | 👷 Technician Hours / Robot / Week |
|------------|-----------------------|----------------------------------|------------------------------------|
| Grocery            | 9 | £1 600 | 10 |
| Clothing           | 6 | £1 000 | 7 |
| Sport Equipment    | 4 | £600   | 5 |

---

## 💰 Budget & Resource Constraints

1. **Total budget:** **£250 000** (acquisition **+** operating costs).  
2. **Each store must receive ≥ 5 robots.**  
3. **Technician capacity:** **≤ 250 staff-hours/week**.  
4. **Goal:** maximise the **total daily orders fulfilled** within the constraints.

---

## 🎯 Task 2 – Allocation Optimisation

* Using the prototype selected in **Task 1**, decide **how many robots** to allocate to **grocery, clothing, and sport-equipment stores**.  
* Ensure **all constraints** are satisfied and **daily order throughput** is maximised.  
* Summarise your optimisation logic, assumptions, and results with clear visuals and commentary.

---

## ✅ Deliverable – Management Report

Produce a concise (≤ 1 500 words) report that:

* Presents the **prototype selection** (Task 1) and **allocation plan** (Task 2).  
* Includes **tables/figures** to support decisions.  
* Is formatted for executive consumption (clarity, succinctness, actionable insights).

---

### Suggested Report Structure

1. **Executive Summary** – one-page overview of key recommendations.  
2. **Prototype Evaluation** – methodology, results, and chosen robot.  
3. **Allocation Model** – optimisation approach, constraints, final distribution.  
4. **Projected Outcomes** – expected daily orders, budget utilisation, technician workload.  
5. **Risks & Mitigations** – any limitations or contingencies.  
6. **Appendices** – detailed calculations or supplementary charts.

---

## 🛠 How to Use This Repo

1. Clone the repository.  
2. Place `Robot_Info.csv` and `Management_Priority.xlsx` in `/data`.  
3. Use the notebook or scripts in `/analysis` to perform your evaluation and optimisation.  
4. Export figures to `/figures` and compile the final report in `/report`.

---

## 🤝 Contributing

Please open issues or pull requests for clarifications, improvements, or additional analysis tools.

---

### Licence

© 2025 AutonomousShipment Ltd. All rights reserved.

