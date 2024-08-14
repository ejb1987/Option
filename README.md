# Option Pricing and Volatility Smile

This project provides a Python script to visualize the **Volatility Smile** for stock options. It retrieves option chains using the `yfinance` library and plots the implied volatility against the strike price for a given expiration date. The tool is useful for traders and financial analysts who want to examine the volatility structure of options.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)

## Installation

To run the code locally, you need to have Python 3.7+ installed. You can clone this repository and install the required packages using pip:

```
git clone https://github.com/ejb1987/option.git
cd option
pip install -r requirements.txt
```

### Required Packages
yfinance: To fetch stock data and option chains.
matplotlib: For plotting the volatility smile.

## Usage
You can use this script in a Jupyter Notebook or as a standalone Python script. Below is a guide on how to run the script.

### Running the Script
1. Open the Jupyter notebook Option.ipynb.
2. Run all the cells in the notebook.
3. Insert the option ticker to analyze it.

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

