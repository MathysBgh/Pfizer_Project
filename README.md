# Pfizer Sales Territory Optimization

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![Optimization](https://img.shields.io/badge/Optimization-MILP-orange)](https://en.wikipedia.org/wiki/Integer_programming)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 📌 Project Overview
This project aims to optimize the commercial territory alignment for Pfizer's sales force. Using **Mixed-Integer Linear Programming (MILP)**, the objective is to redesign sales sectors to maximize operational efficiency while maintaining workload equity and organizational stability.

The project follows a multi-step optimization approach to balance three competing objectives:
1. **Distance Minimization:** Reducing travel time for sales representatives.
2. **Workload Balancing:** Ensuring a fair distribution of commercial potential across the team.
3. **Change Management (Relocation):** Minimizing the disruption caused by reassigning sectors to different representatives.

## 📂 Project Structure
The analysis is divided into three progressive Jupyter Notebooks:

### 🔹 Step 1: Basic Distance Optimization
- Implementation of the core MILP model.
- Focus on assigning 100 sectors to 10 representatives.
- Primary goal: Minimize the total geographical distance between representatives' base locations and assigned sectors.

### 🔹 Step 2: Workload Balancing
- Integration of a "Workload Index" for each sector based on commercial potential. 
- Constraint implementation to ensure the total workload per representative stays within a specific range of the mean.
- Introduction of the trade-off between geographical proximity and workload fairness.

### 🔹 Step 3: Multi-Objective Optimization & Pareto Frontier
- Advanced model incorporating **Relocation Costs** (minimizing sector handovers).
- Generation of a **Pareto Frontier** to visualize the trade-offs between distance, workload equity, and stability.
- Sensitivity analysis to assist decision-making in real-world commercial restructuring.

## 📊 Data Description
The repository includes several Excel datasets used for the optimization:
- `distances.xlsx`: Matrix containing travel distances between locations.
- `data-100x10.xlsx`: Sector details and current representative assignments.
- `indexValues.xlsx`: Workload and potential metrics for each sector.
