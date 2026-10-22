# Electricity Price Prediction (WattWise)

An AI-based electricity consumption and bill forecasting app built with Streamlit and an LSTM model. It predicts daily electricity usage for a chosen month and estimates the monthly bill for households and industries.

> **Status:** open source project, built through community pull requests.

## Features

- LSTM model trained on daily consumption data
- Inputs: consumer type, forecast month, unit cost, daily usage
- Forecast scaled to the user's own consumption with safety limits
- Real calendar days for the selected month (28, 29, 30 or 31)
- Daily forecast table, consumption chart and bill chart
- Monthly bill summary
- Landing page, summary cards and progress feedback
- Runs on Google Colab with a public link

## Known issues (all solved through pull requests)

- [x] Missing imports: `pandas` and `streamlit` are never imported
- [x] Typo: `MinMaxScalerr` should be `MinMaxScaler`
- [x] Code is cut off in the industrial input section (`step=50`)
- [x] No forecast button, prediction output or bill calculation
- [x] Model output is not scaled to the user's own daily consumption
- [x] No safety limits, so predictions can be unrealistic
- [x] Forecast is always 30 days, regardless of the month
- [x] No charts for consumption and bill
- [x] No landing page, summary cards, progress feedback or bill summary

## Tech stack

Python, Streamlit, TensorFlow/Keras (LSTM), scikit-learn, pandas, NumPy

## How to run

1. Open the code file in Google Colab
2. Run the cell
3. Open the public link printed at the end

## Contributors

[![Contributors](https://contrib.rocks/image?repo=Yudhistira1212/Electricity-Price-prediction)](https://github.com/Yudhistira1212/Electricity-Price-prediction/graphs/contributors)

| Contributor | Contribution | PR |
|---|---|---|
| [@Agent-A345](https://github.com/Agent-A345) | Fixed imports, scaler typo and cut-off code, added forecast button and bill calculation | #1 |
| [@Yash-Dhekne](https://github.com/Yash-Dhekne) | Scaled predictions to user input with safety limits | #2 |
| [@Tanmay7007](https://github.com/Tanmay7007) | Added real month dates, charts and cleaner industry limits | #3 |
| [@Omkar-A555](https://github.com/Omkar-A555) | Added WattWise landing page, summary cards, progress bar and bill summary | #4 |

Maintained by [@Yudhistira1212](https://github.com/Yudhistira1212)

## Changelog

- **v0.1:** Initial upload (original version with bugs)
- **v0.2:** Core errors fixed (PR #1)
- **v0.3:** Predictions scaled to user input (PR #2)
- **v0.4:** Month-based dates and charts (PR #3)
- **v1.0:** WattWise landing page and bill summary (PR #4)

## How to contribute

1. Fork this repository
2. Create a new branch (for example `fix-core-errors`)
3. Make your change
4. Commit with a clear message
5. Open a pull request against `main` of this repository

Please keep each pull request focused on a single change.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
