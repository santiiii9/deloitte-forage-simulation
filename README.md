# Deloitte Data Analytics Job Simulation — Forage

**Platform:** Forage  
**Company:** Deloitte Australia  
**Track:** Data Analytics  
**Completed:** June 2026  
**Author:** Santi Aulia Dewi | [github.com/santiiii9](https://github.com/santiiii9)

---

## Overview

This repository contains my completed work for the Deloitte Data Analytics
Job Simulation on Forage. The simulation involved two real-world tasks
based on a fictional client, Daikibo Industrials — a global manufacturing
company collecting telemetry data across 4 factories worldwide.

---

## Tasks

### Task 1 — Data Analysis (Tableau)

**Objective:** Build an interactive dashboard to answer two business questions:
1. Which factory location had the most machine downtime?
2. Which machines broke most often at that location?

**Approach:**
- Imported Daikibo's JSON telemetry dataset into Tableau
- Created a calculated field `Unhealthy` to quantify downtime in minutes
  (each unhealthy status = 10 minutes, since machines send messages every 10 mins)
- Built two bar charts: Downtime Per Factory and Downtime Per Machine
- Combined into an interactive dashboard with factory-level filter

**Key Finding:**
Daikibo Factory Seiko (Osaka, Japan) had the highest total downtime.
The LaserWelder and HeavyDutyDrill were the most frequently broken machines
at that location.

**Tools:** Tableau Public

---

### Task 2 — Forensic Technology (Excel)

**Objective:** Complete a gender pay equality analysis by classifying
equality scores for each job role across all Daikibo factory locations.

**Approach:**
- Added an `Equality Class` column to the provided Excel dataset
- Applied classification logic using nested IF formula:

```excel
=IF(AND(C2>=-10,C2<=10),"Fair",
   IF(OR(C2<-20,C2>20),"Highly Discriminative","Unfair"))
```

**Classification Rules:**

| Score Range | Class |
|-------------|-------|
| -10 to +10 | Fair |
| -20 to -11 or +11 to +20 | Unfair |
| Below -20 or above +20 | Highly Discriminative |

**Key Finding:**
The majority of job roles across all 4 factories showed Unfair or
Highly Discriminative equality scores, with senior roles (C-Level, VP)
showing the most extreme gender pay gaps.

**Tools:** Microsoft Excel

---

## Repository Structure

```
deloitte-forage-simulation/
├── README.md
├── task1-tableau/
│   └── deloitte_dashboard.png        ← dashboard screenshot
└── task2-excel/
    └── Task_5_Equality_Table_Completed.xlsx
```

---

## Skills Demonstrated

- Data visualisation with Tableau
- Calculated field creation and dashboard design
- Excel formula logic (nested IF, AND, OR)
- Business problem-solving with real-world datasets
- Data storytelling — translating raw telemetry into actionable insights

---

## Certificate

Completed and certified via [Forage](https://www.theforage.com) — 
Deloitte Australia Data Analytics Job Simulation (2026)

---

*Part of my Data Analytics portfolio. See more at [github.com/santiiii9](https://github.com/santiiii9)*
