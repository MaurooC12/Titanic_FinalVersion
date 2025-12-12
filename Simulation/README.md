# Simulation Engine & Source Code

---

## Overview
This folder contains the **computational core** of the project. Here, the abstract architecture designed in previous workshops is translated into executable Python code.
It hosts the raw system inputs (datasets), the environment dependencies, and the main simulation script that executes both the **Data-Driven** (ML) and **Event-Based** (Automata) scenarios.

---

## File Structure & Contents

| File / Folder | Role | Description |
| :--- | :--- | :--- |
| **`titanic/`** | **Raw System Inputs** | Contains the original Kaggle datasets representing the initial chaotic state of the system:<br>• `train.csv` (labeled data)<br>• `test.csv` (unlabeled data)<br>• `gender_submission.csv` (format reference) |
| **`Workshop4_Sim.ipynb`** | **The Execution Core** | The main Jupyter Notebook. It implements:<br>1. **Reliability Layer:** Imputation & Cleaning.<br>2. **Sensitivity Analysis:** Random Forest Model.<br>3. **Emergence Visualization:** Cellular Automata logic. |
| **`requirements.txt`** | **Environment Specs** | List of all Python dependencies (`pandas`, `numpy`, `scikit-learn`, `matplotlib`) required to replicate the simulation environment exactly. |

---

## How to Run the Simulation

To reproduce the results and visualizations presented in the technical report, follow these steps:

1.  **Environment Setup:**
    Ensure you are inside this folder and install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

2.  **Launch the System:**
    Open the notebook using Jupyter:
    ```bash
    jupyter notebook Workshop4_Sim.ipynb
    ```

3.  **Execute:**
    Run all cells sequentially. The notebook will:
    * Ingest data from the `titanic/` folder.
    * Apply the **Reliability Layer** (cleaning).
    * Train the models and generate the **Sensitivity Plots**.
    * Run the Automata and render the **Emergent Behavior Grid**.
