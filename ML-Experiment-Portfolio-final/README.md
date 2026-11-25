# Machine Learning – Experiment Portfolio (Assessment 1)

Two machine learning experiments: one **regression** and one **classification**. Each folder has its notebook (saved with outputs) and its dataset.

| Folder | What it does | Model | Main result (test set) |
|---|---|---|---|
| [`01-Regression-HousePrices`](01-Regression-HousePrices/) | Predicts the median house value of California districts | Linear Regression | MAE ≈ $45,300, R² = 0.613 (Random Forest extension: R² = 0.787) |
| [`02-Classification-Churn`](02-Classification-Churn/) | Predicts which telecom customers will leave (churn) | Logistic Regression | Accuracy 80.7%; recall 56.7% → 78.6% with class weights; ROC-AUC 0.841 |

## How to run

Each notebook loads the CSV file that sits in the same folder, so keep them together.

- **Google Colab:** open the notebook, upload its CSV to the Files panel, then *Runtime → Run all*.
- **Your own computer:**
  ```bash
  pip install -r requirements.txt
  jupyter notebook
  ```
  Open the notebook from inside its folder and run all cells.
- **Kaggle:** add the dataset with *Add Input*, then change `data_path` in Section 2 to the path shown in the Input panel.

## Data sources
- California Housing Prices: https://www.kaggle.com/datasets/camnugent/california-housing-prices
- Telco Customer Churn: https://www.kaggle.com/datasets/blastchar/telco-customer-churn
