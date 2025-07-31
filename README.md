## england-house-prices

[![Lint](https://github.com/0xnu/england-house-prices/actions/workflows/lint.yaml/badge.svg)](https://github.com/0xnu/england-house-prices/actions/workflows/lint.yaml)
[![Release](https://img.shields.io/github/release/0xnu/england-house-prices.svg)](https://github.com/0xnu/england-house-prices/releases/latest)
[![License](https://img.shields.io/badge/License-Modified_MIT-f5de53?&color=f5de53)](/LICENSE)

Predict house prices for the next five years across all English local authorities. It is built like a professional investment tool, featuring advanced risk analysis and decision support.

> [!WARNING]
> Disclaimer: It is an experimental system; do not use it for actual investment decisions.

### What It Does

The system takes house price data and creates predictions for every local authority in England. It tells you:

+ Which areas will have the best price growth
+ How risky each investment might be
+ What could go wrong in different economic situations
+ Which areas to buy, hold, or avoid

### Key Features

#### 🔮 Smart Predictions

+ Multiple Models: Uses 3 different prediction methods and combines them
+ Economic Factors: Includes interest rates, GDP growth, and housing supply
+ 5-Year Forecasts: Shows year-by-year predictions from 2025 to 2030
+ Risk Analysis: Calculates confidence intervals and downside risks

#### 📊 Professional Analysis

+ Monte Carlo Simulation: Runs 500+ scenarios to test uncertainty
+ Stress Testing: Shows what happens in recessions or market crashes
+ Statistical Validation: Checks if the models are working properly
+ Performance Tracking: Measures how accurate the predictions are

#### 💼 Investment Tools

+ Investment Grades: Rates each area from A+ (excellent) to D (avoid)
+ Portfolio Builder: Creates balanced investment portfolios
+ Screening Tools: Finds areas that match your requirements
+ Risk-Return Analysis: Shows the best risk-adjusted opportunities

#### 📈 Professional Charts

+ Price Distributions: Shows how prices vary across regions
+ Risk Profiles: Visualises uncertainty and confidence levels
+ Comparison Charts: Compares different investment strategies
+ Dashboard: One-page summary of key insights

### Install Dependencies

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install following

```sh
## Prerequisites
python3 -m venv .venv
source .venv/bin/activate
uv pip install -r requirements.txt
python3 -m pip install --upgrade pip
```

### Data Requirements

The system needs a CSV file with these columns:

+ `Local authorities`: Names of English local authorities
+ `May 2025`: Current house prices (with £ symbol)
+ `May 2024`: Previous year prices (with £ symbol)
+ `Difference`: Annual percentage change

The data (UK House Price Index England: May 2025) is from [HM Land Registry](https://www.gov.uk/government/statistics/uk-house-price-index-for-may-2025/uk-house-price-index-england-may-2025).

### Run the System

Click the `Run` button to run the individual cell of the [Jupyter Notebook](./england_house_prices_predictor.ipynb).

### License

This project is licensed under the [Modified MIT License](./LICENSE).

### Copyright

(c) 2025 [Finbarrs Oketunji](https://finbarrs.eu). All Rights Reserved.