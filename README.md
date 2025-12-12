# Titanic
**[Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic)**

---

## The Systemic Perspective
While the [Titanic Kaggle Competition](https://www.kaggle.com/competitions/titanic) is often treated as a standard Machine Learning challenge, this project approaches it as a **Complex Engineering Challenge**.
We moved beyond simple data analysis to model the Titanic as a **Closed Sociotechnical System** governed by strict internal rules (Social Stratification, Physical Access, and Family Grouping).

### 1. The Problem: Structural Instability
Our initial diagnosis revealed that the system is inherently unstable due to:
* **Structural Chaos (Entropy):** The dataset inherits the confusion of the disaster, with 19% missing Age data and 77% missing Cabin data acting as systemic noise.
* **High Sensitivity:** The system exhibits a "Butterfly Effect". Small variations in input conditions ($Age \pm 1$, $Sex$) drastically invert the survival outcome.

### 2. The Focus: Engineering Stability
Instead of ad-hoc data cleaning, our goal was to **engineer order out of chaos**.
We focused on designing an **ISO-25010 Compliant Architecture** capable of:
* **Absorbing Chaos:** Using a dedicated *Reliability Layer* to stabilize inputs.
* **Ensuring Reproducibility:** Decoupling logic through a *Maintainability Layer*.
* **Validating Dynamics:** Proving system rules through computational simulation.

---

## The Solution: Closed-Loop Architecture
To solve the instability, we implemented a modular system that acts as a robust pipeline:

| Layer | Function | Engineering Goal |
| :--- | :--- | :--- |
| **Reliability Layer** | Imputation & Noise Filtering | **Fault Tolerance:** Prevents system failure due to missing data. |
| **Maintainability Layer** | Feature Engineering | **Modularity:** Isolates business logic (e.g., *FamilySize*) from ingestion. |
| **Simulation Layer** | Dual-Engine Execution | **Validation:** Tests the system under statistical and physical rules. |

---

## Repository Structure

This repository is organized to separate the engineering documentation from the executable core:

### [Final_documentation/](./Final_documentation)
Contains the formal artifacts of the engineering process:
* `Paper.pdf`: IEEE scientific summary of the research.
* `Technical_report.pdf`: Complete compendium of Workshops 1-4.
* `Poster.pdf`: Visual abstract of the architecture and results.
* `Slides.pdf`: Defense presentation deck.

### [Simulation/](./Simulation)
Contains the executable engine and source code:
* `Workshop4_Sim.ipynb`: The main notebook implementing the architecture.
* `titanic/`: Raw input datasets.
* `requirements.txt`: Environment dependencies.

---

## Authors
* **Julián Carvajal Garnica**
* **Andrés Mauricio Cepeda Villanueva**
* **Jhonatan David Moreno Barragán**
* **Andrés Camilo Ramos Rojas**
