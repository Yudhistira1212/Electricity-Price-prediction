# Electricity Price Prediction

An AI-based electricity consumption and bill forecasting app built with Streamlit and an LSTM model. It is meant to predict 30-day electricity usage and estimate the monthly bill for households and industries.

> **Status: work in progress.** This is the initial upload and it has known bugs. It is open for contributions.

## What it is supposed to do

- Train an LSTM on daily consumption data
- Take user input: consumer type, forecast month, unit cost, daily usage
- Forecast consumption and calculate the estimated bill
- Show the results in a Streamlit web app (runs on Google Colab)

## Known issues (help wanted)

- [ ] Missing imports: `pandas` and `streamlit` are never imported
- [ ] Typo: `MinMaxScalerr` should be `MinMaxScaler`
- [ ] Code is cut off in the industrial input section (`step=50`)
- [ ] No forecast button, prediction output or bill calculation
- [ ] Model output is not scaled to the user's own daily consumption
- [ ] No safety limits, so predictions can be unrealistic
- [ ] Forecast is always 30 days, regardless of the month
- [ ] No charts for consumption and bill
- [ ] No landing page, summary cards, progress feedback or bill summary

## Tech stack

Python, Streamlit, TensorFlow/Keras (LSTM), scikit-learn, pandas, NumPy

## How to run

1. Open the code file in Google Colab
2. Run the cell
3. Open the public link printed at the end

## How to contribute

1. Fork this repository
2. Create a new branch (for example `fix-core-errors`)
3. Fix one of the issues above, or add a new feature
4. Commit with a clear message
5. Open a pull request against `main` of this repository

Please keep each pull request focused on a single change.
