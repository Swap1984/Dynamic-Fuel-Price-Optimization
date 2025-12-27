⛽ Dynamic Fuel Pricing Optimization System

A machine-learning–driven pricing system that recommends an optimal daily fuel price to maximize profit in a competitive retail petrol market, using historical data, competitor pricing, and business constraints.

📌 Problem Statement

A retail petrol company operates in an open market where competitors freely change prices daily.
The company can update its own price once per day and wants to maximize daily profit:

Profit
=
(
Price
−
Cost
)
×
Volume Sold
Profit=(Price−Cost)×Volume Sold

The key challenge is that demand depends more on relative pricing versus competitors than on absolute price.

Flow chart
Input (Today JSON)
      ↓
Feature Engineering
      ↓
XGBoost Demand Model
      ↓
Price Simulation
      ↓
Business Rules Filtering
      ↓
Profit Maximization
      ↓
Recommended Price

🧠 Key Insights from Data

Fuel demand is price-inelastic in absolute terms

Relative price vs competitors is the strongest demand driver

Day-of-week patterns exist; monthly seasonality is weak

Cost affects profit, not demand

Demand response is non-linear and asymmetric

These findings motivate a machine-learning + optimization approach rather than simple elasticity models.
