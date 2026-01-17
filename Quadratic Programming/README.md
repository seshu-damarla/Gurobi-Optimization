# Quadratic Programming

This subfolder contains a collection of **quadratic programming (QP) and quadratically constrained programming (QCQP)** examples, implemented and solved using the **Gurobi Optimizer** via its Python interface (`gurobipy`). The problems in this folder focus on optimization models with **quadratic objective functions and/or quadratic constraints**, primarily involving **continuous decision variables**.

Quadratic programming extends linear programming by allowing second-order (quadratic) relationships, enabling more realistic modeling of engineering, economic, and physical systems where linear assumptions are insufficient.

---

## 📘 Scope of Problems

The notebooks and model files in this subfolder cover the following classes of problems:

### • **QP – Quadratic Programming**
Optimization problems with:
- a quadratic objective function,
- linear constraints,
- continuous decision variables.

### • **QCQP – Quadratically Constrained Quadratic Programming**
Optimization problems with:
- quadratic objective functions,
- quadratic and linear constraints,
- continuous decision variables.

Several of the included problems are **nonconvex**, meaning the quadratic terms are indefinite and the feasible region may be nonconvex. These problems require explicit nonconvex handling by the solver.

---

## 📂 Included Benchmark Instances

This subfolder includes benchmark problems drawn from the **QPLIB (Quadratic Programming Library)**, a standard repository used in optimization research and solver benchmarking. For example:

- **QPLIB_1703** — a continuous, nonconvex QCQP with a quadratic objective and multiple quadratic constraints.

Each problem is provided in solver-readable format (e.g., `.lp`) and solved using appropriate Gurobi settings.

---

## ⚙️ Methodology

Across the notebooks in this subfolder:

- Quadratic objective functions and constraints are modeled explicitly.
- Solver parameters are configured to handle **nonconvex quadratic structure** when required (e.g., `NonConvex = 2` in Gurobi).
- Models are solved to optimality when possible, or to the best feasible solution within solver limits.
- Final objective values, solution status, and selected variable values are reported and interpreted.

For continuous quadratic problems, the emphasis is on **correct model formulation** and **solver configuration**, rather than branch-and-bound progress analysis.

---

## 🎯 Purpose of This Subfolder

The objective of this subfolder is to:

- demonstrate practical implementation of **quadratic optimization models**,
- highlight the differences between linear and quadratic formulations,
- showcase experience with **nonconvex optimization problems**,
- and provide reproducible examples using **benchmark-grade test instances**.

These examples form a natural bridge between linear programming and more advanced mixed-integer and nonlinear optimization techniques.

---

## 📌 References

- **QPLIB – Quadratic Programming Library**  
  https://qplib.zib.de/

- **Gurobi Optimizer Documentation**  
  https://www.gurobi.com/documentation/

---

