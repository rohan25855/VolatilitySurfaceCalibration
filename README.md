# Volatility Surface Calibration

Project builds and calibrates a smoothed implied volatility surface for NIFTY index options, using end-of-day option chain data from NSE.
  
Surface smoothing was performed using:
- Quadratic polynomial regression across strikes
- Exponential decay modeling across maturities

Key steps:
- Collected raw option chain data from NSE for 5 different maturities
- Fitted individual curves separately across strikes and maturities
- Combined both fits into a unified 3D implied volatility surface
- Validated model performance using RMSE and regional error heatmaps

**Files:**
- `Volatility_Surface_Smoothing.ipynb`: Full Jupyter Notebook (data cleaning, modeling, visualization)
- `Data_OptionChains.csv`: Processed option chain data used for modeling
- `Raw_Data/`: Folder containing raw option chain data directly downloaded from NSE

**Note:**  
This is a personal learning project targeted for practical understanding of volatility surface construction and basic smoothing techniques.
