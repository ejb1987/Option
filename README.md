# Stock Option Pricing and Volatility Smile

This repository contains a Jupyter Notebook that enables users to analyze and price stock options using two widely recognized methods: the Black-Scholes Model and Monte Carlo Simulation. Additionally, the notebook provides functionalities to calculate and plot Implied Volatility, a crucial metric for assessing whether an option is overvalued or undervalued in the market.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [Functionality Overview](#functionality)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Features
* Black-Scholes Model: Calculates the theoretical price of European-style call and put options, considering the continuous dividend yield.
* Monte Carlo Simulation: Estimates option prices by simulating future price paths of the underlying asset.
* Implied Volatility Calculation: Determines the implied volatility based on the current market price of the option.
* Volatility Smile Plot: Visualizes the relationship between strike prices and implied volatility, providing insights into market sentiment and conditions.

## Installation

To run the code locally, you need to have Python 3.7+ installed. You can clone this repository and install the required packages using pip:

```
git clone https://github.com/ejb1987/option.git
cd option
pip install -r requirements.txt
```
## Dependencies
The project relies on the following Python packages:

- `numpy`: For numerical computations and handling large arrays or matrices.
- `scipy`: Provides additional functionality for optimization, statistics, and more advanced mathematical functions.
- `yfinance`: To retrieve financial data.
- `matplotlib`: For data visualization.

To install the dependencies, run:

```bash
pip install numpy scipy yfinance matplotlib
```
## Usage
You can use this script in a Jupyter Notebook or as a standalone Python script. Below is a guide on how to run the script.

### Running the Script
1. Open the Jupyter Notebook Option.ipynb.
2. Run the cells in the notebook sequentially to perform stock option pricing, and implied volatility calculation, and to plot the volatility smile.

## Functionality Overview
1. get_option_data(option_ticker)
Fetches the underlying stock data and option-specific details such as strike price, expiration date, risk-free rate, and dividend yield.

2. black_scholes_price(...)
Computes the price of a call or put options using the Black-Scholes formula, taking into account the continuous dividend yield.

3. implied_volatility(...)
Estimates the implied volatility by minimizing the difference between the market price of the option and the price calculated using the Black-Scholes model.

4. monte_carlo_option_price(...)
Utilizes Monte Carlo Simulation to estimate the price of the option by simulating multiple future price paths of the underlying asset.

5. plot_volatility_smile(stock_ticker, expiration_date, option_type)
Plots the volatility smile, showing the relationship between different strike prices and their respective implied volatilities for either call or put options.

### Example Output
```
Implied Volatility Calculation
Underlying Price: $221.27
Strike Price: $255.00
Expiration Date: 2024-12-20
Option Type: Call
Risk-Free Rate: 5.07%
Option Price: $2.74
Dividend Yield: 0.45%
Calculated Implied Volatility: 21.94%
```
**Monte Carlo Simulation Price**
Monte Carlo Price: $2.60
Option Status: Overpriced (compared to the Monte Carlo estimate)
**Volatility Smile Plot**
The plot illustrates the implied volatility across different strike prices, helping to identify patterns such as the volatility smile or skew.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any enhancements or bug fixes.

### How to Contribute
1. Fork the repository.
2. Create a new branch: git checkout -b feature/your-feature-name.
3. Commit your changes: git commit -m 'Add some feature'.
4. Push to the branch: git push origin feature/your-feature-name.
5. Submit a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.

## Acknowledgements
* Yahoo Finance for providing real-time stock and options data.
* The Python community for developing the powerful tools utilized in this project.
