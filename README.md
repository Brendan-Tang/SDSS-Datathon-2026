# ✈️ Airfare Markets Under Pressure
> A data science project analyzing domestic U.S. airfare dynamics using U.S. Department of Transportation data (2022–2025 Q2). 

**Event:** SDSS Datathon 2026

## Table of Contents
- [Overview](#overview)
- [What We Did](#what-we-did)
- [Key Findings](#key-findings)
- [Approach](#approach)
- [Tech Stack](#tech-stack)
- [Contributors](#contributors)

## Overview
This project was submitted as part of the SDSS Datathon 2026 for students in Data Science and Statistics. The competition challenged participants to rigorously analyze domestic U.S. airfare markets and translate findings into actionable insights for travelers, airlines, and policymakers.

- **Data Source:** U.S. Department of Transportation Domestic Airline Consumer Airfare Report
- **Period Covered:** 2022 – 2025 (Q2)

## What We Did
We explored domestic U.S. airfare markets to understand what drives ticket prices beyond the anecdotal advice consumers typically hear. Using route-based data from the U.S. DOT, we investigated the structural forces behind fare differences, including airline competition, hub dominance, low-cost carrier presence, and weather.

## Key Findings
- Cities with dominant carriers (>70% market share) show significant fare premiums, Charlotte (+15.8%), Salt Lake City (+13%), and Atlanta (+12.4%) command higher prices regardless of flight distance
- Distance alone explains ~48% of fare variation (R² = 0.4822), but this correlation has weakened year-over-year (0.654 in 2022 → 0.501 in 2025), meaning market structure is increasingly overtaking geography as the primary pricing driver
- Adding market structure variables increased R² from 0.4822 to 0.6815, explaining an additional 28 percentage points of fare variation
- Families and students are disproportionately affected in "Fortress Hub" markets where a single carrier dictates prices

## Approach

**Analysis highlights:**
- Conducted exploratory analysis on route-level fares, hub concentration, and carrier market share across 2022–2025
- Engineered market structure features including hub dominance index and low-cost carrier presence flags
- Trained and evaluated multiple models, with a final Random Forest / Gradient Boosting model achieving R² = 0.86 and a Mean Absolute Error of $18.47

## Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

## Contributors

| Name | Role |
|------|------|
| Brendan Tang | Visualization, Modeling, Design |
| James Shin | Visualization, Modeling, Insights |
| Alejandro Salazar Rueda | Feature Engineering, Visualization, Modeling |
| Dipon Roy | Visualization, Modeling, Storytelling |
