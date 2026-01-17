# Linear Programming

This subfolder contains **linear programming (LP) models and case studies** drawn from classical **process systems engineering** and **industrial optimization** problems. Each notebook demonstrates how real-world engineering decision problems can be formulated as linear programs and solved efficiently using the **Gurobi Optimizer** via its Python interface (`gurobipy`).

The focus of this subfolder is on:
- translating process descriptions into mathematical optimization models,
- implementing LP formulations programmatically,
- solving them using a state-of-the-art commercial solver,
- and interpreting optimal solutions in an engineering and economic context.

---

## 📘 Contents

The subfolder currently includes the following linear programming examples:

### 🔥 Optimal Operation of a Thermal Cracker
This notebook implements **Example 14.1: Optimal Operation of a Thermal Cracker via Linear Programming**, adapted from *Optimization of Chemical Processes* (Edgar, Himmelblau, and Lasdon).  
The problem models the steady-state operation of a thermal cracking unit and determines optimal feed and product flow rates that maximize profit subject to material balances and capacity constraints.

### ⚡ Boiler–Turbogenerator System Optimization
This notebook models the optimal operation of a **boiler–turbogenerator system**, a classic energy systems optimization problem. The LP formulation captures steam generation, power production, and operational constraints, and identifies the economically optimal operating point.

---

## ⚙️ Methodology

Across all notebooks in this subfolder:
- Decision variables represent flow rates, production levels, or operating decisions.
- Objective functions are linear economic metrics (e.g., profit maximization or cost minimization).
- Constraints are linear equalities and inequalities derived from mass balances, capacity limits, and operational restrictions.
- All models are solved using **Gurobi**, ensuring globally optimal solutions.

The notebooks emphasize **clarity of formulation**, **solver transparency**, and **engineering interpretation of results**.

---

## 🎯 Purpose of This Subfolder

The goal of this subfolder is to:
- demonstrate proficiency in **linear programming modeling**,
- show how LP applies to **chemical and energy process optimization**,
- provide reproducible, well-documented examples suitable for learning and benchmarking,
- and serve as a foundation for more advanced optimization topics such as MILP, MIQP, and nonlinear programming.

These examples illustrate why linear programming remains a powerful and widely used tool in industrial optimization and decision-making.

---

