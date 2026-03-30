### Cost-Based Optimisation of Heat Exchanger Configuration
A MATLAB-based engineering framework designed to determine the most cost-effective heat exchanger configuration (Shell-and-Tube vs. Plate-Frame) by balancing thermal performance, fluid dynamics, and economic constraints.

# Project Overview
Selecting the optimal heat exchanger is a multi-objective challenge. This project implements a computational framework that evaluates different geometries and flow arrangements. By integrating the \epsilon-NTU and LMTD methods with rigorous cost functions, the tool identifies configurations that maximize thermal effectiveness while minimizing pressure drop and total lifecycle costs.

# Core Methodologies
The framework utilizes two primary analytical approaches for thermal validation:
 * Log Mean Temperature Difference (LMTD): Used primarily for sizing and rating when inlet and outlet temperatures are known or specified.
 * Effectiveness-NTU (\epsilon-NTU): Applied to predict performance when only inlet temperatures are available, facilitating easier iteration during the optimization loops.

# Technical Features
 * Dual-Architecture Evaluation: Side-by-side comparison of Shell-and-Tube and Plate-and-Frame exchangers.
 * Cost-Model Integration: Includes equations for capital expenditure (CAPEX) based on material mass and surface area, alongside operational expenditure (OPEX) derived from pumping power requirements (pressure drop).
 * Pareto Analysis: Generates a Pareto frontier to visualize the trade-offs between thermal efficiency and economic investment.
 * Parametric Sensitivity: Studies the impact of fouling factors, flow arrangements (counter-flow vs. parallel-flow), and fluid property variations.

# Current Status: Phase 1 Complete
 * [x] Derivation: Mathematical models for \epsilon-NTU, LMTD, and pressure drop gradients completed.
 * [x] Manual Verification: Theoretical models and cost equations verified against textbook standards using spreadsheet-based manual calculations.
 * [x] Architecture Design: MATLAB framework structure defined for modularity (Fluid Props -> Thermal Model -> Cost Model -> Optimizer).

# Next Steps: Phase 2
 * [ ] Finalize the core MATLAB solver.
 * [ ] Implement the multi-variable optimization algorithm.
 * [ ] Integration of the Pareto Frontier visualization.
 * [ ] Documentation of specific case studies (e.g., HVAC vs. Industrial Process cooling).
