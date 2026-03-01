# ✈️ Airfare Markets Under Pressure
> A data science project analyzing domestic U.S. airfare dynamics using U.S. Department of Transportation data (2022-2025 Q2). 

**Event:** SDSS Datathon 2026

## Table of Contents
- [Overview](#overview)
- [What We Did](#what-we-did)
- [Key Findings](#key-findings)
- [Approach](#approach)
- [Tech Stack](#tech-stack)
- [Contributors](#contributors)
- [AI Statement](#-ai-assistance)
- [Acknowledgements](#acknowledgements)
- [References](#references)

## Overview
This project was submitted as part of the SDSS Datathon 2026 for students in Data Science and Statistics. The competition challenged participants to rigorously analyze domestic U.S. airfare markets and translate findings into actionable insights for travelers, airlines, and policymakers.

- **Data Source:** U.S. Department of Transportation Domestic Airline Consumer Airfare Report
- **Period Covered:** 2022 - 2025 (Q2)

## What We Did
We explored domestic U.S. airfare markets to understand what drives ticket prices beyond the anecdotal advice consumers typically hear. Using route-based data from the U.S. DOT, we investigated the structural forces behind fare differences, including airline competition, hub dominance, low-cost carrier presence, and weather.

## Key Findings
- Cities with dominant carriers (>70% market share) show significant fare premiums, Charlotte (+15.8%), Salt Lake City (+13%), and Atlanta (+12.4%) command higher prices regardless of flight distance
- Distance alone explains ~48% of fare variation (R² = 0.4822), but this correlation has weakened year-over-year (0.654 in 2022 → 0.501 in 2025), meaning market structure is increasingly overtaking geography as the primary pricing driver
- Adding market structure variables increased R² from 0.4822 to 0.6815, explaining an additional 28 percentage points of fare variation
- Families and students are disproportionately affected in "Fortress Hub" markets where a single carrier dictates prices

## Approach

**Analysis highlights:**
- Conducted exploratory analysis on route-level fares, hub concentration, and carrier market share
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
![SHAP](https://img.shields.io/badge/SHAP-FF0000?style=for-the-badge&logo=python&logoColor=white)
![Statsmodels](https://img.shields.io/badge/Statsmodels-3776AB?style=for-the-badge&logo=python&logoColor=white)
<!-- ![XGBoost](https://img.shields.io/badge/XGBoost-189AE0?style=for-the-badge&logo=xgboost&logoColor=white) -->

### **Machine Learning Libraries**
- **[Scikit-learn](https://github.com/scikit-learn/scikit-learn)** (BSD-3 License) - Used for regression models and preprocessing.
<!-- - **[XGBoost](https://github.com/dmlc/xgboost)** (Apache 2.0 License) - Used for gradient boosting regression. -->
- **[SHAP](https://github.com/slundberg/shap)** (MIT License) — Used for model explainability and feature importance analysis.

### **Data Handling & Computation**
- **[Pandas](https://github.com/pandas-dev/pandas)** (BSD-3 License) - Used for data manipulation and analysis.
- **[NumPy](https://github.com/numpy/numpy)** (BSD License) - Used for numerical computing.
- **[Statsmodels](https://github.com/statsmodels/statsmodels)** (BSD-3 License) — Used for statistical modeling and regression analysis.

### **Data Visualization**
- **[Matplotlib](https://github.com/matplotlib/matplotlib)** (PSF License) - Used for data visualization.
- **[Seaborn](https://github.com/mwaskom/seaborn)** (BSD License) - Used for statistical data visualization.
  
### Environment
- **[Jupyter](https://github.com/jupyter/notebook)** (BSD-3 License) - Used for interactive notebook development and analysis.

## References

- **[U.S. DOT Domestic Airline Consumer Airfare Report](https://www.transportation.gov/policy/aviation-policy/domestic-airline-consumer-airfare-report)** — U.S. Department of Transportation. Primary dataset for route-level fares, passenger volumes, and carrier market shares.
- **[NOAA Climate Data Online (CDO)](https://www.ncei.noaa.gov/cdo-web/)** — National Centers for Environmental Information, National Oceanic and Atmospheric Administration. Used for weather data.

## Contributors

| Name | Role |
|------|------|
| Brendan Tang | Design, Visualization, Modeling |
| James Shin | Visualization, Modeling, Insights |
| Alejandro Salazar Rueda | Feature Engineering, Visualization, Modeling |
| Dipon Roy | Visualization, Modeling, Storytelling |

## 🤖 AI Assistance
This project was developed with guidance from **LLMs**.
- **Debugging** - identifying and resolving errors in data processing and modeling code

*All models and, outputs were developed, validated, and  interpreted by the team. AI tools were not used as academic sources; all references 
cite original papers, documentation, or official data sources.*

## Acknowledgements
We thank the organizers of the SDSS Datathon 2026 for hosting  SDSS Datathon 2026 and providing the opportunity to explore real-world transportation pricing dynamics.

Data for this project was obtained from the Domestic Airline Consumer Airfare Report published by the United States Department of Transportation.

