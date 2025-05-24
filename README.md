Overview
This project analyzes battery performance using Electrochemical Impedance Spectroscopy (EIS) and charge-discharge data from metadata.csv. It includes creating a Nyquist plot, training a machine learning model to predict capacity, performing Incremental Capacity Analysis (ICA), and visualizing aging effects in 3D, as part of a ThinkClock job assignment.
Tasks Completed

Nyquist Plot: Generated a Nyquist plot for battery B0047 at 24°C, showing Re(Z) vs. -Im(Z) in kΩ across cycle ranges (0-50, 51-100, 101-150, 151-200), with impedance increasing over cycles, saved as nyquist_plot.png.
Capacity Prediction: Trained a Random Forest model to predict battery capacity from EIS features (Re, Rct, test_id), achieving an MAE of ~0.05 Ah and R² of ~0.89, with results visualized in capacity_predictions.png.
Incremental Capacity Analysis (ICA): Derived <math xmlns="http://www.w3.org/1998/Math/MathML"><semantics><mrow><mfrac><mrow><mi>d</mi><mi>Q</mi></mrow><mrow><mi>d</mi><mi>V</mi></mrow></mfrac></mrow><annotation encoding="application/x-tex"> \frac{dQ}{dV} </annotation></semantics></math> vs. V plot from simulated charge-discharge data, identifying electrochemical peaks, saved as ica_plot.png.
3D Aging Visualization: Created a 3D surface plot showing how ICA peaks shift with cycle count, highlighting battery degradation, saved as ica_3d_aging.png.

Conclusions

The Nyquist plot indicated increasing impedance with cycle count, reflecting battery degradation.
The Random Forest model accurately predicted capacity from EIS data, outperforming Linear Regression.
ICA and 3D visualization revealed electrochemical peak shifts, confirming capacity loss with aging.

