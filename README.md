# Gas Station Study – Deloitte Data Challenge

Team project with **Francesca Zen** (University of Padova, May 2022) for a data challenge set by Deloitte.
The goal was a data-driven strategy for an entrepreneur who wants to open a new petrol station in Italy:
where to open it, which fuels to sell, and what drives fuel prices.

## Data

* Italian Ministry of Economic Development (MISE) open data: the registry of petrol stations (location,
  brand, road type) and the prices they report for petrol, diesel, LPG and methane, for 2021.
* Brent crude prices and population density by province.

## Analysis

* **Price structure:** self-service vs. served prices, motorway vs. other roads, fuel types, brands
  ("flags") and provinces.
* **Price drivers:** regression models per fuel type with PyCaret, and feature importance to find the
  factors that matter most, for self-service and served prices separately.
* **Location choice:** provinces with high population density but few stations, excluding metropolitan
  cities where public transport lowers demand.

## Files

| Path | Contents |
|---|---|
| `Challenge_Deloitte.pdf` | Project report |
| `Pycaret Analysis/` | Modelling notebooks for self-service (`challenge_self_analysis.ipynb`) and served (`Challenge_notself_analysis.ipynb`) prices |
| `Visualisation/` | Exploratory plots for both price types |
| `Challenge_Deloitte.ipynb` | Web-page snapshot of the main notebook from the team repository. It is HTML, so it does not open in Jupyter. |

Requirements: `pandas`, `numpy`, `pycaret`, `scikit-learn`, `plotly`, `matplotlib`. The notebooks were
run on Google Colab.
