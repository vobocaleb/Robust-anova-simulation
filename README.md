# Robust ANOVA Simulation Study

This repository contains the R code used in the simulation study:

“Comparative Performance of Heteroscedasticity-Robust ANOVA Methods: A Simulation Study of Welch, Brown–Forsythe, and Permutation Tests.”


Overview

This study evaluates the performance of four one-way ANOVA procedures:
	•	Classical ANOVA (F-test)
	•	Welch’s ANOVA
	•	Brown–Forsythe test
	•	Permutation-based ANOVA

The methods are compared based on:
	•	Type I error rates
	•	Statistical power

under varying conditions:
	•	Balanced and unbalanced designs
	•	Equal and unequal variances
	•	Different distributions (Normal, Lognormal, and t)


Simulation Design
	•	Number of groups: k = 3
	•	Sample size configurations: (20, 20, 20), (10, 20, 30), (15, 15, 15)
	•	Variance structures: (1,1,1), (1,2,3), (1,4,9)
	•	Distributions: Normal, Lognormal, and t
	•	Number of simulations: 5000

Power analysis is conducted by introducing mean differences: (0, 0.5, 1)


How to Run the Code
	1.	Open R or RStudio
	2.	Set the working directory to this repository
	3.	Run the main script:
  
  source("run_simulation.R")
  
  This will:
	•	Run Type I error simulations
	•	Run power simulations
	•	Save results automatically

Repository Structure
	•	run_simulation.R → Main script to reproduce all results
	•	simulate_type1.R → Functions for Type I error simulations
	•	simulate_power.R → Functions for power simulations
	•	helper_functions.R → Supporting functions

Folders:
	•	/data → Stores simulation results
	•	/plots → Contains generated figures
	•	/results → Scripts for tables and visualizations


Output
	•	Type I error results → /data/type1_results.csv
	•	Power results → /data/power_results.csv
	•	Plots are saved in /plots


Reproducibility

A random seed is set within the scripts to ensure reproducibility of results.


Author

Vobo Godlove Watoh
Email: vobo.caleb@yahoo.com
LinkedIn: 

Notes

This repository is provided to ensure transparency and reproducibility of the results presented in the associated manuscript.

