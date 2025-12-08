# VAR_FX

A compact project for estimating and analysing Vector Autoregression (VAR) and VARX models on foreign-exchange (FX) and macroeconomic time series, developed as supporting material for a master’s thesis on EUR/NOK forecasting.

## Purpose
- Provide benchmark VAR/VARX specifications for **EUR/NOK level forecasting**.
- Demonstrate a full VAR workflow: data preparation, estimation, diagnostics, impulse-response analysis, and forecasting.
- Compare baseline VAR models to VARX extensions with exogenous/panel-style covariates.

## Repository Structure
- `data/` — cleaned and processed datasets used by the notebooks.
- `src/` — Jupyter notebooks implementing the modelling workflows.
- `LICENSE` — MIT License.

## Data
- **var_monthly.csv** — cleaned monthly time series used by the notebooks.  
  Link: [`data/var_monthly.csv`](data/var_monthly.csv)

## Notebooks
All notebooks are located in `src/` and are runnable end-to-end (assuming the data files are present).

### VAR Models (EN)
- **VARMacroMonthly.ipynb** — Core VAR model with macro-financial covariates, monthly frequency.  
  Link: [`src/VARMacroMonthly.ipynb`](src/VARMacroMonthly.ipynb)

- **VARMacroQuarterly.ipynb** — Core VAR model with macro-financial covariates, quarterly frequency.  
  Link: [`src/VARMacroQuarterly.ipynb`](src/VARMacroQuarterly.ipynb)

### VARX Models (EN-EX)
- **VARXPanelMonthly.ipynb** — VARX specification with exogenous/panel-style extensions, monthly frequency.  
  Link: [`src/VARXPanelMonthly.ipynb`](src/VARXPanelMonthly.ipynb)

- **VARXPanelQuarterly.ipynb** — VARX specification with exogenous/panel-style extensions, quarterly frequency.  
  Link: [`src/VARXPanelQuarterly.ipynb`](src/VARXPanelQuarterly.ipynb)

## Getting Started
1. Create a virtual environment and install dependencies from `requirements.txt`.
2. Start Jupyter and open the notebooks in `src/`.

Example (PowerShell):

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
jupyter notebook
