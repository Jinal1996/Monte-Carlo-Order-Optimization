# Monte Carlo Simulation in Supply Chain: Order Optimization

## Overview

This repository explores the application of Monte Carlo simulation in supply chain management to determine the optimal order quantity that maximizes expected profit. The study involves utilizing Excel functions to model demand uncertainty and evaluate different order quantities.

## Concepts Learned

- Monte Carlo Simulation
- Demand Uncertainty Modeling
- Expected Profit Calculation
- Critical Ratio Analysis
- Excel-based Simulation and Data Analysis

## Excel Functions Used

- `RAND()`: Generates random numbers between 0 and 1.
- `NORMINV(probability, mean, standard_dev)`: Maps random numbers to demand values based on a normal distribution.
- Data Tables: Used to automate calculations for different order quantities.
- Graphing Tools: Helps visualize the relationship between order quantity and expected profit.

## Uses in Supply Chain

Monte Carlo simulation is widely used in supply chain management for:

- Demand forecasting under uncertainty.
- Determining optimal inventory levels.
- Risk assessment in procurement and logistics.
- Profit optimization in inventory decisions.

## Procedure Steps

### Step 1: Generate Random Demand

1. Generate 1,000 random numbers using the `RAND()` function.
2. Copy and paste these values as static to prevent changes.
3. Use the `NORMINV()` function with the given/calculated mean and standard deviation to transform random values into demand values.

### Step 2: Compute Expected Profit, Expected Total Cost, and Expected Service Level

1. Fix an order quantity, e.g., `Q = 30,000`.
2. Compute profit using:
   - **Overage cost** (excess inventory cost)
   - **Underage cost** (lost sales cost)
   - **Total cost** = Overage Cost + Underage Cost
3. Average the 1,000 profit values to estimate expected profit at `Q = 30,000`.

### Step 3: Analyze Different Order Quantities

1. Use an Excel Data Table to estimate expected profit across order quantities ranging from **1,000 to 84,000**.
2. Plot a graph with order quantity on the x-axis and expected profit on the y-axis.
3. Identify the order quantity that maximizes expected profit while maintaining an optimal **service level**.

## Conclusion

This study demonstrates how Monte Carlo simulation can be used to optimize order quantity decisions under demand uncertainty. The methodology helps businesses make data-driven inventory decisions, reducing risk and maximizing profitability.

## Repository Contents

- Excel file with Monte Carlo simulation model.
- Study Visual Graphs

## Future Enhancements

- Extend the model to consider multiple product types.
- Implement Monte Carlo simulation in Python for greater scalability.
- Explore additional probability distributions for demand modeling.

---

This repository serves as a learning tool for supply chain students and practitioners looking to apply simulation techniques to real-world inventory management problems.

