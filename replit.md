# Primer_212 - Financial Calculation Application

## Overview
This is a Python console application that performs financial calculations related to asset depreciation using two different methods. The application calculates depreciation values, displays tabular data using pandas, and generates visualization plots with matplotlib.

## Project Type
Console application - Python script

## Setup Date
October 6, 2025

## Project Structure
- `main.py` - Main application script containing:
  - Container for calculations (two depreciation methods)
  - Container for tabular output using pandas DataFrames
  - Container for visualization using matplotlib
- `requirements.txt` - Python dependencies (sympy, pandas, matplotlib)
- `README.md` - Basic project description

## Dependencies
- **sympy** - Symbolic mathematics library for calculations
- **pandas** - Data analysis and manipulation, used for creating data tables
- **matplotlib** - Plotting library for data visualization

## How to Run
The application runs automatically via the configured workflow. It performs calculations and outputs:
1. Lists of calculated values (Am_lst, C_ost_lst for both methods)
2. Pandas DataFrames showing Year, Cost, and Depreciation values
3. Line plots comparing the two depreciation methods

## Calculation Methods
The script implements two depreciation calculation methods:
1. **Method 1**: Linear depreciation using formula `Am = (C-L)/T`
2. **Method 2**: Accelerated depreciation using formula `Am = k * 1/T * (C - Aj)`

Where:
- C = Initial cost (100,000)
- T = Time period (5 years)
- L = Liquidation value (0)
- k = Acceleration coefficient (2)
- Aj = Accumulated depreciation

## Technical Notes
- The application is designed for console output
- Matplotlib plots use `plt.show()` which works in console mode
- Initial capital values: 20,000,000 (Method 1) and 2,000,000 (Method 2)
- Iteration count: 16 cycles, displaying first 5 years in tables

## Configuration
- **Python Version**: 3.11
- **Workflow**: "Run Application" - executes `python main.py`
- **Output Type**: Console
