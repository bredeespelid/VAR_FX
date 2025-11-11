# VAR_FX

A compact project for estimating and analysing Vector Autoregression (VAR) models on foreign-exchange and macroeconomic time series.

This repository contains data and example Jupyter notebooks used in a master's thesis. The aim is to demonstrate VAR and VARX modelling workflows: data preparation, estimation, diagnostics, impulse-response analysis and basic forecasting.

Contents
- data/var_monthly.csv — cleaned monthly time series used by the notebooks
- src/VAR.ipynb — core VAR modelling and diagnostics
- src/VARX.ipynb — VARX example (VAR with exogenous variables)

Getting started
1. Create a virtual environment and install dependencies from `requirements.txt`.
2. Start Jupyter and open the notebooks in `src/`.

Minimal commands (example, PowerShell):

	python -m venv .venv
	.\.venv\Scripts\Activate.ps1
	pip install -r requirements.txt
	jupyter notebook

Notes
- The notebooks are runnable end-to-end but may expect the `data/var_monthly.csv` file to be present.
- If you adapt the analysis, add new dependencies to `requirements.txt`.

License
This project is released under the MIT License — see the `LICENSE` file for details.
