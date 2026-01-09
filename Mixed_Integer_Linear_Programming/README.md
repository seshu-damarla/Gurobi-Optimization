# Mixed Integer Linear Programming (MILP) – MIPLIB 2017 Benchmarks

## 📌 Overview

This subfolder contains a curated set of **Mixed Integer Linear Programming (MILP)** benchmark problems selected from **MIPLIB 2017**, a widely used public library of challenging real-world optimization instances.

The goal of this collection is to:
- Practice solving **industry-grade MILP problems** using Gurobi
- Analyze solver behavior across **different variable compositions**
- Study branch-and-bound performance, integrality gaps, and convergence patterns
- Build a **reproducible optimization portfolio** based on standard benchmarks

All models are provided in **MPS format**, which is commonly used in industrial optimization pipelines.

🔗 Reference: https://miplib.zib.de/tag_collection.html

---

## 🧠 Problem Categories Covered

The selected instances span multiple MILP structures based on the **composition of decision variables**:

| Category | Description |
|-------|------------|
| Binary–Continuous | Binary decisions coupled with continuous variables |
| Binary–Integer | Binary decisions with general integer variables |
| Pure Binary | All decision variables are binary |
| Integer–Continuous | General integer and continuous variables |
| Mixed (Binary + Integer + Continuous) | Full mixed-integer structure |

This diversity allows systematic comparison of solver performance under different combinatorial and numerical characteristics.

---

## 📂 Instances Included

### 🔹 Binary–Continuous MILP
- **`binary_continuous_pk1.mps`**  
  A benchmark MILP with binary decision variables interacting with continuous variables.  
  Useful for studying integrality gaps and relaxation strength.

---

### 🔹 Binary–Integer MILP
- **`binary_integer_enlight8.mps`**  
  Combines binary and general integer variables.  
  Emphasizes discrete feasibility and combinatorial complexity.

---

### 🔹 Pure Binary MILP
- **`binary_pb-market-split8-70-4.mps`**  
  A purely binary decision problem, representative of selection or market-splitting formulations.

---

### 🔹 Integer–Continuous MILP
- **`integer_continuous_flugpl.mps`**  
  General integer variables coupled with continuous variables.  
  Typical of capacity planning or flow-based models.

---

### 🔹 Fully Mixed MILP
- **`mixed_integer_continuous_noswot.mps`**  
  A fully mixed formulation involving binary, integer, and continuous variables.  
  Closely resembles large-scale industrial optimization models.

---

## ⚙️ Solution Methodology

All problems in this folder are solved using:

- **Gurobi Optimizer**
- Python interface (`gurobipy`)
- Standard **branch-and-bound / branch-and-cut** algorithms

For selected instances, solver progress is analyzed using:
- **Callbacks** to track incumbent objective values
- **Best bound evolution**
- **Objective convergence vs time and node count**

---

## 📊 Analysis Performed

Depending on the instance, the following analyses are conducted:

- Model size inspection (variables, constraints, nonzeros)
- Identification of binary vs integer vs continuous variables
- Solver log interpretation
- Objective convergence plots
- Integrality gap analysis
- Export of solutions and parsed LP models

---

## 📁 Outputs

Typical outputs generated per instance:
- `solution.sol` — optimal solution values
- `model_parsed.lp` — solver-parsed LP formulation
- Objective convergence plots (`.png`)
- Optional CSV logs of solver progress

---

## 🎯 Learning Outcomes

Through these benchmark problems, this subfolder demonstrates:

- Practical experience with **standard MILP benchmarks**
- Ability to work with **solver-native formats (MPS)**
- Understanding of **MILP difficulty sources**
- Proficiency in **Gurobi callbacks and diagnostics**
- Reproducible optimization experimentation

---

## 🔮 Future Extensions

- Benchmark comparisons across multiple solvers (SCIP, HiGHS)
- Parameter tuning experiments (cuts, heuristics, branching)
- Automated batch-solving of MIPLIB collections
- Feature extraction for ML-guided optimization

---

## 🏷️ Tags

`#MILP` `#MIPLIB2017` `#Gurobi`  
`#OperationsResearch` `#OptimizationBenchmarks`  
`#CombinatorialOptimization` `#IntegerProgramming`

---


