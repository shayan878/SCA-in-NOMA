# Optimization for Alpha = 1 and Alpha = ∞

This repository contains the implementation of optimization models for the article:

"Fair Resource Allocation in an MEC-Enabled Ultra-Dense IoT Network with NOMA" (ICC Workshop 2019)

In this article, we address the resource allocation problem in MEC-enabled ultra-dense IoT networks using Non-Orthogonal Multiple Access (NOMA). The article focuses on solving challenging non-convex optimization problems under different fairness constraints, specifically for Alpha = 1 (proportional fairness) and Alpha = ∞ (max-min fairness).

The models implemented in this repository optimize resource allocation for communication networks under these fairness conditions using successive convex approximation (SCA). The goal is to balance energy efficiency, computation efficiency, and fairness among users.

Files:

- alpha=1.py: Implements the optimization model for Alpha = 1, which targets proportional fairness among users.
- alpha=infinity.py: Implements the optimization model for Alpha = ∞, which maximizes the minimum rate for all users, achieving max-min fairness.

Usage:

- Set up the required parameters (e.g., channel gains, power limits, etc.).
- Call the respective function to build and solve the model using IPOPT or Gurobi solvers.
- Retrieve the optimized variables, including frequencies and offloading power
