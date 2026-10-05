# Sensory_Panel_Prediction
Data cleaning, descriptive analysis and modelling code for Master's thesis on predicting sensory panel scores of Cheddar cheese from physical, E-tongue, tribology and GC-MS measurements.

The thesis predicts sensory panel scores of twelve Cheddar samples from four
instrumental modalities and compares regularised linear models, PLSR and Random Forest
under nested leave-one-out cross-validation.

## Contents

| File | Purpose |
|---|---|
| `Sensory_Panel_Data_Cleaning.ipynb` | Cleans the raw sensory panel data and saves `panel_cleaned.csv` |
| `Sensory_Panel_Modelling.ipynb` | Descriptive analysis and all models reported in the thesis |

## How to run

1. Install the requirements listed below.
2. Set the file paths in the configuration cell of each notebook.
3. Run Notebook 1. It writes `panel_cleaned.csv`.
4. Run Notebook 2. It reads `panel_cleaned.csv` and the four instrumental datasets.
   The full run takes about 15 to 25 minutes.

## Input data

| Dataset | Used in |
|---|---|
| Raw sensory panel file (Excel) | Notebook 1 |
| Physical texture measurements (Excel) | Notebook 2 |
| E-tongue measurements (Excel) | Notebook 2 |
| Tribology measurements (Excel) | Notebook 2 |
| SPME GC-MS results (Excel, one sheet per trial) | Notebook 2 |
| Academy of Cheese Flavour Tree (Excel) | Notebook 2 |

The data belong to the data-providing company and are not included in this repository.

## Models

Taste and aroma models are labelled M1 to M12 and quality models N1 to N13, as in the
thesis. An overview table is given at the top of Notebook 2, and a summary of all
results at its end.

## Requirements

Python 3 with pandas, numpy, scikit-learn, matplotlib, seaborn and openpyxl.
