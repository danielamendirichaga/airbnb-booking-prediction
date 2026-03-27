# Final Project Submission

This submission contains the final report, the end-to-end notebook, and the data needed to reproduce the analysis for the project:

**Can machine learning predict whether a Los Angeles Airbnb listing-night is booked rather than open using a panel built from repeated Inside Airbnb snapshots?**

## Main Files

- `Report_FinalProject_DMM.pdf`: final report
- `DMM_final_project_v2.ipynb`: final end-to-end notebook

## Folder Structure

- `data/raw/`: raw input data used in the project
- `data/processed/`: processed inputs and notebook-generated outputs
- `images/figures/`: figures exported by the notebook
- `images/tables/`: tables exported by the notebook

## Reproducibility

The notebook was developed in Python 3 and relies on the following core packages:

- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`
- `xgboost`

To reproduce the analysis, open `DMM_final_project.ipynb` and run the cells sequentially from top to bottom from the project root directory. The notebook:

1. Loads the raw Airbnb, holiday, weather, and event data.
2. Builds the curated listing-night panel and target variable.
3. Constructs the event proxy features within the notebook workflow.
4. Creates train, validation, and test splits using a chronological design.
5. Trains and evaluates the L1-logistic and XGBoost models.
6. Runs the event-controls and weather-controls robustness checks.
7. Exports the processed outputs, figures, and tables used in the report.

## Notes

- The final report is exactly 20 pages.
- The project is predictive rather than causal.
- Some files in `data/processed/` and `images/` are generated notebook outputs included for transparency and convenience.
