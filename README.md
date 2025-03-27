# Performance Benchmarking of Pandas Methods
## Overview
### This project benchmarks different Pandas methods (iloc, iterrows, itertuples, apply, and NumPy vectorization) to compare their execution times across different dataset sizes.

## Methods Compared
- iloc[]: Index-based row access.
- iterrows(): Row-wise iteration (returns index & Series).
- itertuples(): Row-wise iteration (returns named tuples, faster than iterrows).
- apply(): Function application to a column or row.
- NumPy vectorization: Uses NumPy's optimized operations for efficiency.
