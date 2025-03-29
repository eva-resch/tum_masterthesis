# 📘 Master Thesis – Graphical Lyapunov Models on Intervention Data

Welcome to the repository for my Master's thesis: **Graphical Lyapunov Models on Intervention Data**, completed as part of the requirements for the MSc in Mathematics at Technical University of Munich (TUM).

This repository contains the Python code and Jupyter notebooks used to conduct the simulation studies for the thesis.

## 🧠 Thesis Overview

**🧭 Goal**: The objective of this thesis is to investigate how interventions can be systematically incorporated into the graphical Lyapunov model — a framework for modeling causal relationships in continuous-time stochastic systems with potential feedback-loops and cyclic dependencies. 
The focus lies in understanding how such interventions improve the identifiability and estimation of the system’s underlying structure.

**🛠️ Methodology**: The thesis extends the graphical Lyapunov model by introducing two types of interventions: shift interventions, which modify the equilibrium state without changing the causal structure, and hard interventions, which break incoming dependencies to selected variables. 
A mathematical framework is developed to integrate these interventions into the model. 
Estimation is carried out using an adapted version of the Direct Lyapunov Lasso (DLL), and extensive simulation studies are conducted to evaluate performance under various structural settings and intervention types.
Concretely, we examine the ability of recovering the matrix $M$ driving the process using the DLL, the frequency with which the irrepresentability conditions (an indicator for the ability to recover the structure of $M$) are fulfilled under shift intervention, and the influence the node subjected to the intervention has on these two aspects.

**📊 Outcome**: Results show that incorporating interventional data leads to significantly more accurate estimation of the system’s dynamics, especially when the true model includes cycles or when observational data alone are insufficient. 
The analysis also reveals how the effectiveness of interventions depends on graph structure and intervention location. 
The work provides both theoretical insights and practical tools for causal inference in complex dynamical systems.

## 📂 Repository Structure

<pre>
  📁 Irrepresentability/     # Simulations on frequency of irrepresentability conditions being fulfilled
  📁 Lasso/                  # Simulations on performance of the Lasso with and without interventions
  📁 Rank Condition/         # Study rank condition for matrix A_+ in shift intervention
  📄 requirements.txt        # Python dependencies
  📄 README.md               # This file 
</pre>

The folders ```📁 Irrepresentability/``` and ```📁 Lasso/``` contain the Jupyter notebooks conducting the simulations studies and creating the evaluation.
Each contains the folders ```📁 Experiments/``` where the results of all experiments are stored and ```📁 Evaluation/``` where the graphics for the evaluation are stored.
The folder ```📁 Outdated/``` contains files that I used for primary experiments and investigation of the effects of interventions on the Lyapunov model.

## 📦 Dependencies

To install all packages, run ```pip install -r requirements.txt```.

The project was developed using Python 3.12.3 and tested with the following key packages:

- numpy
- pandas
- scipy
- matplotlib
- scikit-learn
- sympy

## 📚 Reference

If you want to cite this work, use the following:

Author: Eva C. Resch

Title: Graphical Lyapunov Models on Intervention Data

University: Technical University of Munich

Year: 2025

## 📬 Contact

For questions or further information, feel free to contact me at:

📧 eva_resch@yahoo.com

🔗 [on LinkedIn](https://www.linkedin.com/in/eva-resch-43a0ab161/overlay/about-this-profile/?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base%3BiXggH8IMTqyBwmn9VYfHuQ%3D%3D)
