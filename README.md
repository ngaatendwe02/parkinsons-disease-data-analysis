# Parkinson’s Disease Voice Measurements — Exploratory Data Analysis

An exploratory Python analysis of voice measurements and Parkinson’s symptom scores in a supplied 100-row sample.

## What this project explores
- Data quality, missing values, and potential outliers
- Distributions of `motor_UPDRS` and `total_UPDRS`
- Pearson correlations between voice features and `total_UPDRS`
- A scatterplot of the strongest observed voice-feature association

## Key result
`Shimmer:APQ3` has the highest absolute Pearson correlation with `total_UPDRS` among the voice features in this sample (**r ≈ 0.217**). This is a **weak** positive linear association, not evidence of diagnostic or predictive accuracy.

## Files
- `Parkinsons_Voice_EDA.ipynb` — reproducible analysis with charts and interpretation
- `parkinsons_sample.csv` — supplied 100-row sample used by the notebook

## How to run in Google Colab
1. Open `Parkinsons_Voice_EDA.ipynb` in Colab.
2. Upload `parkinsons_sample.csv` using the left-side **Files** panel.
3. Select **Runtime → Run all**.

Alternatively, run the notebook locally with `pandas`, `numpy`, `matplotlib`, and `seaborn` installed, keeping the CSV in the same directory.

## Limitations
The provenance and sampling procedure of this specific CSV have not been verified. Results are exploratory and cannot be generalized or used for medical diagnosis. Repeated subject measurements may affect statistical independence.

## Dataset context
[UCI Parkinsons Telemonitoring dataset](https://archive.ics.uci.edu/dataset/189/parkinsons+telemonitoring) (broader dataset reference; not verified as the exact source of this sample).
