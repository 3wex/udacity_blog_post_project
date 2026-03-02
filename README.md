# Decoding the Macroeconomic Drivers of the Arab World

## Motivation for the Project
This project is part of the Udacity Data Science Nanodegree. The goal of this analysis is to apply the CRISP-DM (Cross-Industry Standard Process for Data Mining) methodology to real-world macroeconomic data. Using dataset indicators from the World Bank, this project explores the unique economic drivers of the Arab World. 

Specifically, the analysis investigates the relationships between oil reliance, labor markets, and financial liquidity to understand what accelerates commercial expansion. It concludes with a predictive machine learning model to forecast infrastructure investment booms, applying a scenario specifically focused on the Saudi Arabian market.

## Libraries Used
The code is written in Python 3 and requires the following libraries:
* `pandas` for data manipulation and wrangling
* `numpy` for numerical computations
* `matplotlib` and `seaborn` for data visualization
* `scikit-learn` for data imputation and building the Random Forest Classifier

## Files in the Repository
* `macroeconomic_analysis.ipynb`: The main Jupyter Notebook containing the data gathering, assessment, cleaning, exploratory data analysis, and predictive modeling.
* `data/`: This directory contains the raw World Bank data used for the analysis.
* `README.md`: This file, providing an overview of the project.

## Summary of Results
The analysis addressed three core business questions:

1.  **How does a nation's reliance on oil revenues impact its ability to attract foreign investment and build physical infrastructure?**
    * Although the negative correlations are moderate (-0.28 for Foreign Direct Investment, -0.14 for infrastructure), they point to a significant trend. The data suggests that heavy dependence on oil rents can deter diverse foreign investment and coincides with slower overall development of physical infrastructure.
2.  **How does the disparity between male and female unemployment relate to a country's overall economic prosperity?**
    * The data reveals a moderate negative correlation (-0.27) between the gender unemployment gap and GDP per capita. Furthermore, the unemployment disparity varies drastically across the region—from under 1% in Comoros to over 14% in Saudi Arabia and Egypt—suggesting that bridging this employment gap is positively linked to a nation's broader economic wealth.
3.  **Which financial lever drives physical infrastructure the most: raw money supply or active bank lending to the private sector?**
    * The analysis indicates that active bank lending to the private sector (0.17) has a stronger positive correlation with infrastructure development than broad money supply (0.09). This suggests that direct credit access and targeted lending act as more effective financial levers for driving physical market growth than simply increasing the overall money in circulation.

**Predictive Modeling:**
A Random Forest Classifier was trained to forecast infrastructure growth based on the cleaned macroeconomic indicators. The model achieved an accuracy of ~66% on the testing set. Feature importance analysis revealed that Foreign Direct Investment (FDI) net inflows, Broad Money Growth, and female unemployment rates are the strongest predictive indicators of future infrastructure acceleration in the region.

## Acknowledgements
* **Data Source:** The data utilized in this project was sourced from the [World Bank Open Data](https://data.worldbank.org/) platform.
* **Guidance:** This project was completed as part of the Udacity Data Science Nanodegree program.
