# Supply Chain Sourcing and Production Optimization

## Executive Summary

This project uses a 30-day linear optimization model in Excel Solver to determine the most profitable combination of internal production, outside-union milk purchases, and recombined milk. The model optimizes daily order quantities while meeting forecasted demand and accounting for production capacity, inventory availability, reserve requirements, and storage constraints.

## Business Problem

MAMD needed to satisfy daily milk demand while deciding how much supply should come from internal production, outside-union sourcing, and recombined milk. Each option had different costs and operational limits, creating a tradeoff between profitability, inventory usage, and service levels.

## Objective

Maximize total modeled profit by optimizing daily production and procurement quantities while maintaining full demand coverage.

## Tools and Methods

- Microsoft Excel
- Excel Solver
- Linear Programming
- Demand Planning
- Inventory Optimization
- Production and Sourcing Analysis

## Model Constraints

- Daily demand requirements
- Internal raw milk availability
- Five-percent reserve requirement
- Outside-union supply
- Skim milk powder inventory
- Butter inventory
- Storage capacity
- Daily storage cost
- Nonnegative decision variables

## Results

- Maximized modeled profit to approximately ₹24.30 million
- Fulfilled 8.96 million liters of demand
- Maintained zero demand shortages across the 30-day period
- Optimized approximately 1.69 million liters of outside-union purchases
- Selected approximately 18,954 liters of recombined milk
- Balanced internal production, external sourcing, inventory, and storage constraints

## Model Outputs

### Optimization Summary

![Optimization summary](opt%201.png)

### Daily Decision Variables

![Daily decision variables](opt%202.png)

### Daily Cost and Profit Results

![Daily cost and profit results](opt%203.png)

### Solver Configuration

![Solver configuration](opt%204.png)

## Skills Demonstrated

- Procurement and sourcing analysis
- Order quantity optimization
- Production planning
- Inventory management
- Constraint modeling
- Profit maximization
- Supply chain analytics
