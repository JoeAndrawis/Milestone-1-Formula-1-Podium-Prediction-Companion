# Formula 1 Podium Prediction Companion - Milestone 1

**Student:** Youssef Samy (ID 40-20092) - GUC

Predicts whether a driver finishes on the podium (`positionOrder <= 3`) using only information available after qualifying and before the race starts.

- **Notebook (run-all):** `f1_podium_prediction.ipynb`
- **Kaggle notebook:** [add Kaggle link]
- **Dataset:** https://www.kaggle.com/datasets/rohanrao/formula-1-world-championship-1950-2020
- **Report:** `F1_Milestone1_Report_FINAL.pdf`

## How to run
Open the notebook on Kaggle with the dataset attached, restart the session, and press Run All. The notebook installs `shap` and `lime`, so internet must be enabled.

## Contents
Audit and cleaning, three data-engineering questions, leakage-safe features, chronological split (train <= 2016, validation 2017-2020, test 2021-2024), four models plus two baselines, feature-group ablation, preprocessing-order experiments, SHAP / permutation / LIME explanations, and an inference function.

## Final model
Shallow neural network (one hidden layer of 32 units), decision threshold 0.435 chosen on validation.
