# Gurobi Optimization

This repository showcases a collection of **practical optimization models and solutions implemented using the Gurobi Optimizer** with Python (`gurobipy`). It is designed to demonstrate how real-world decision problems from engineering, process systems, and mathematical optimization can be formulated, solved, and analyzed using commercial-grade optimization software.

The repository is organized into subfolders covering:
- **Linear Programming** – classic LP models from chemical and energy systems.
- **Mixed Integer Linear Programming** – optimization problems with discrete decisions.
- **Quadratic Programming** – continuous and nonconvex quadratic optimization.
- **Mixed Integer Quadratic Programming** – mixed discrete–continuous quadratic problems.

Each section contains self-contained Jupyter notebooks that:
- formulate the optimization problem clearly,
- interface with Gurobi via its Python API,
- solve the problem efficiently,
- and interpret the resulting optimal decisions.

Gurobi is one of the world’s leading optimization solvers, capable of handling:
- linear programming (LP),
- mixed integer linear programming (MILP),
- quadratic programming (QP),
- mixed integer quadratic programming (MIQP),
- and quadratically constrained problems such as MIQCP. :contentReference[oaicite:0]{index=0}

---

## 📂 Repository Contents

### Linear Programming
Industrial examples formulated as linear programs, such as the **optimal operation of a thermal cracker**, demonstrating material balances and economic objective optimization.

### Mixed Integer Linear Programming
Classic MIP instances solved with Gurobi, including formulations with binary and integer decision variables and callback-based progress tracking.

### Quadratic Programming
Continuous and nonconvex quadratic programming models, including QCQPs with quadratic objectives and constraints.

### Mixed Integer Quadratic Programming
Benchmark MIQPs from QPLIB with both quadratic structure and integer variables, showing advanced solver configuration and handling of nonconvex models.

---

## 🧠 Purpose & Learning Outcomes

This repository is intended to:

- Provide self-contained examples of optimization modeling using Python and Gurobi.
- Illustrate how real decision problems can be expressed as mathematical optimization problems.
- Demonstrate the use of Gurobi’s advanced solver features, including:
  - nonconvex problem handling (`NonConvex = 2`),
  - callback functions for solution monitoring,
  - solver parameter configuration.
- Serve as a **portfolio of optimization projects** suitable for learning, teaching, and demonstration.

Whether you are a student, researcher, or practitioner, this repository shows how optimization models can be structured and solved for real and benchmark problems.

---

## 🧩 Dependencies

This repository assumes:
- Python (3.7+),
- Gurobi Optimizer installed with an academic or commercial license,
- `gurobipy` Python package,
- Jupyter Notebook support for interactive exploration.

---

## 🚀 Getting Started

To run the notebooks:
1. Clone the repository:
   ```bash
   git clone https://github.com/seshu-damarla/Gurobi-Optimization.git

