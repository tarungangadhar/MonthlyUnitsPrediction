# Electricity Consumption Prediction & Billing Analysis

Website:- https://tarungangadhar.github.io/MonthlyUnitsPredictionWebsite/
Report:- 
Colab:- https://colab.research.google.com/drive/12EpFp8j5ocAuaBjxCUslVRxjsh1USMNL?usp=sharing

This project predicts monthly electricity consumption for ~190 quarters over 12 years of college data (2012–2023) and estimates bills using machine learning.

## Abstract
Using **linear** and **polynomial regression**, the system forecasts electricity usage and translates predicted units into electricity bills. Historical data was gathered from 144 monthly Excel files maintained by the college’s Maintenance Department. After cleaning (removing nulls, duplicates, and outliers), the dataset was structured into quarter-wise consumption records. The models achieved **~96% accuracy**, demonstrating ML’s potential in energy planning

## Method
- **Data collection**: 12 years of monthly readings (2012–2023).  
- **Cleaning**: handled nulls, duplicates, outliers.  
- **Feature prep**: Quarter number, year, units consumed.  
- **Models**: Linear regression (trend baseline), Polynomial regression (seasonal non-linearity).  
- **Billing**: Units mapped to real tariff slabs (2.90–7.80 Rs/unit + fixed + wheeling + taxes).  

## Results
- Example: Predicted units for Quarter 3, Jan 2025 = 395.7 → Bill ≈ Rs. 4003.99
- Achieved ~96% accuracy on held-out years.  

| Model               | Accuracy |
|----------------------|----------|
| Linear Regression    | 92–94%   |
| Polynomial (deg=6)   | 95–96%   |

![Forecast Example](assets/results_plot.png)
