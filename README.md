# Performance Benchmarking of Pandas Methods
## Overview
This project benchmarks different Pandas methods (iloc, iterrows, itertuples, apply, and NumPy vectorization) to compare their execution times across different dataset sizes.

## Methods Compared
- iloc[]: Index-based row access.
- iterrows(): Row-wise iteration (returns index & Series).
- itertuples(): Row-wise iteration (returns named tuples, faster than iterrows).
- apply(): Function application to a column or row.
- NumPy vectorization: Uses NumPy's optimized operations for efficiency.

## Experiment Setup
The script generates DataFrames of varying sizes (1,000 / 10,000 / 1,00,000 / 1,000,000 / 5000000 rows) and applies a simple function to each row using the above methods. The time taken by each method is recorded and visualized.

## Requirements
To run the script, install the following dependencies:
```pip install pandas numpy matplotlib```

## Usage
Run the script using:
```python benchmark_pandas.py```
This will generate a performance comparison plot showing execution times.

## Results & Key Findings
-NumPy vectorization is the fastest method.
-apply() performs well but is slower than vectorization.
-itertuples() is faster than iterrows().
-iterrows() is the slowest and should be avoided for large datasets.
