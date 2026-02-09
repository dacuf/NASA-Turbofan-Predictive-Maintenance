# NASA-Turbofan-Predictive-Maintenance
Remaining Useful Life (RUL) prediction for aircraft engines using Sensor Signal Processing &amp; Random Forest
### Project Overview
This project focuses on **Predictive Maintenance** for turbofan jet engines using the NASA CMAPSS dataset. 
The goal is to predict the **Remaining Useful Life (RUL)** of an engine based on multi-variate time-series data from 21 sensors (Temperature, Pressure, RPM).

This workflow simulates real-world engineering challenges such as **Sensor Noise Reduction**, **Signal Drift Analysis**, and **Failure Threshold Modeling**, which are critical in the automotive and aerospace industries.

### Engineering Approach
1.  **Data Processing:** Handled raw sensor data with significant noise and outliers.
2.  **Signal Processing:** Applied **Rolling Mean (Window=5)** to filter high-frequency noise.
    * Extracted true degradation trends from noisy sensor signals.
3.  **Feature Engineering:** Identified top critical sensors (Pressure & Temperature) correlating with physical wear.
4.  **Modeling:** Built a **Random Forest Regressor** to predict failure cycles.

### Key Results
* **Model Accuracy:** Achieved an **RMSE of ~40 cycles** on the test set.
* **Signal Analysis:** Successfully isolated the degradation trend from sensor noise.

> *Figure 1: Raw Sensor Signal (Gray) vs. Smoothed Signal (Red). The rolling mean technique effectively filters noise.*
<img width="1020" height="548" alt="28610336-90d6-496f-923e-53081f28b2f8" src="https://github.com/user-attachments/assets/eecbda07-be1b-4a81-806c-756b8401c3e1" />

> *Figure 2: Actual vs. Predicted RUL. The model tracks the degradation path closely.*
<img width="850" height="548" alt="6822eceb-1518-4dcb-ba97-f3c29df49e07" src="https://github.com/user-attachments/assets/fa7f5d7d-9872-42a8-8268-3e826c951a1f" />

### Technologies Used
* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn.
* **Concepts:** Time-Series Analysis, Signal Processing, Regression.
