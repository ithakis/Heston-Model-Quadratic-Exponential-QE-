## Heston Model Analysis

This repository provides a comprehensive analysis of the Heston model, a widely-used stochastic volatility model for option pricing. The analysis focuses on implementing and comparing different numerical methods for simulating the Heston model, pricing options, and calculating implied volatilities. The primary methods explored include the Quadratic Exponential (QE) scheme and the Empirical Moments (EM) method.

### Objectives

1. **Simulate Heston Model Dynamics**: Implement the Quadratic Exponential (QE) scheme and the Euler-Maruyama (EM) method to simulate the dynamics of the Heston model.
2. **Bootstrap Implied Volatilities**: Calculate implied volatilities using bootstrapping techniques and compare the results from different methods.
3. **Moments Analysis**: Evaluate the analytical and empirical moments of the Heston model to assess the accuracy of the numerical simulations.
4. **Option Pricing**: Use the Fast Fourier Transform (FFT) method for pricing options under the Heston model and compare with Monte Carlo simulations.
## Repository Structure

- **Heston Model Quadratic Exponential.ipynb**: Jupyter Notebook containing the main analysis code for the Heston model.
- **Moments: QE Heston.csv**: CSV file containing moments data for the Quadratic Exponential method.
- **Moments: Simple Heston.csv**: CSV file containing moments data for the Simple Heston method.

## Requirements

- Python 3.x
- Required Python packages:
  - `numpy`
  - `matplotlib`
  - `py_vollib_vectorized`
  - [`tqdm`](command:_github.copilot.openSymbolFromReferences?%5B%7B%22%24mid%22%3A1%2C%22path%22%3A%22%2FUsers%2Falexanderithakis%2F.vscode%2Fextensions%2Fms-python.vscode-pylance-2024.7.1%2Fdist%2Ftypeshed-fallback%2Fstubs%2Ftqdm%2Ftqdm%2Fstd.pyi%22%2C%22scheme%22%3A%22file%22%7D%2C%7B%22line%22%3A33%2C%22character%22%3A6%7D%5D "../../../.vscode/extensions/ms-python.vscode-pylance-2024.7.1/dist/typeshed-fallback/stubs/tqdm/tqdm/std.pyi")

You can install the required packages using pip:  
```bash
pip install numpy matplotlib py_vollib_vectorized tqdm
```



## Usage

1. **Bootstrap Implied Volatility**:
   The `Bootstrap_IV` function in the notebook performs bootstrapping to calculate implied volatilities. It takes an array of terminal stock prices and returns the mean, standard error, and confidence intervals for the implied volatilities.

2. **Plotting Implied Volatility**:
   The notebook includes code to plot the implied volatilities for different methods (QE, EM, Analytical). The plots show the mean implied volatility along with confidence intervals.

3. **Moments Data**:
   The CSV files contain moments data for the QE and Simple Heston methods. These files include analytical and empirical values for various moments, along with confidence intervals and differences.

## Example

To run the analysis, open the `Heston Model Quadratic Exponential.ipynb` notebook in Jupyter and execute the cells. The notebook will generate plots showing the implied volatilities for different methods.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- The `py_vollib_vectorized` library is used for calculating implied volatilities.
- The analysis is based on the Heston model for option pricing.

For any questions or issues, please open an issue in the repository.

