# Telco Customer Churn Survival Analysis

This project applies survival analysis techniques to model customer churn behavior and estimate Customer Lifetime Value (CLV) in a telecom setting. Using parametric and non-parametric models from the `lifelines` library, the analysis identifies at-risk customers and valuable customer segments to inform data-driven retention strategies.

## Key Components

- **Data Preprocessing**: Label encoding of categorical features and cleaning.
- **Modeling**: Fit multiple survival models including:
  - Kaplan-Meier Estimator
  - LogNormal AFT model (final model)
  - Weibull, Log-Logistic, Exponential, and Spline models
- **CLV Estimation**: Predict expected customer lifetimes and calculate CLV based on average monthly revenue.
- **Segmentation**: Explore CLV by region, customer type, income, internet usage, and more.
- **Retention Strategy**: Estimate an annual retention budget and suggest proactive actions based on at-risk groups.

## Files

- `Report.ipynb` – main notebook with all analysis
- `requirements.txt` – Python dependencies for reproducibility
- `telco.csv` – Telco customer data

## How to Run

1.  Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

2.  Open and run `Report.ipynb` in Jupyter or VSCode.

## Insights

- Final model: `LogNormalAFTFitter` based on statistical performance and business relevance
- Most valuable customers: Those with high service bundles and income levels
- Retention suggestion: Personalized offers to top segments and \$15–20K annual retention budget

---

**Author**: Gayane Hovsepyan
