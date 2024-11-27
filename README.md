# **Household-Level Day-Ahead Peak Electricity Demand Forecast**

This repository contains materials from my MSc Data Science dissertation, which was awarded a **Distinction** at the University of Manchester. The project focuses on developing machine learning models to forecast household-level day-ahead peak electricity demand using the Low Carbon London dataset and detailed London weather data.

## Abstract
- Objective: Develop machine learning models to forecast day-ahead peak electricity demand at the household level
- Research Questions:
  - How accurately can machine learning models predict day-ahead peak electricity demand at the household level?
  - What are the most significant factors influencing this demand?
  - How does the inclusion of household-specific survey data and dynamic pricing information impact forecast accuracy? 
- Methodology:
  - Used Low Carbon London project dataset and weather data
  - Applied XGBoost models with various feature sets
- Key Findings:
  - Optimal model achieved a test WAPE of 29.63% with 15 features
  - Recent consumption patterns were the most significant predictors
  - While marginally increasing model accuracy, household characteristics played a less prominent role than expected
- Key Insights:
  - Carefully selected feature subsets can achieve comparable performance to larger sets
  - Suggests potential for efficient, streamlined forecasting models
- Limitations:
  - Underestimation of high consumption events
  - Potential bias from opt-in recruitment
- Implications:
  - Highlights importance of high-quality recent consumption data for short-term forecasting
  - Provides directions for future research in energy sector modeling

## Key Components
### Dissertation
- The full dissertation is provided as `dissertation.pdf`, detailing the methodology, results, and implications of the study.

### Notebook
- `Model-Development-Cbrt-No-Scaler.ipynb`: Final XGBoost model development notebook
  - Demonstrates the optimal approach using the cube root transformation of the target variable
  - Showcases feature selection and model performance evaluation
  - Selects the best model and analyzes its performance in detail

  Note: Only the notebook related to the final model development is included to comply with data safeguarding policies.

### Supplementary Materials
- Key figures used in the dissertation are included in the `supplementary/key-figures` folder.
- Additional figures can be found in the `supplementary/additional-visualizations` folder.

## Data Sources
- Weather datasets used in this study are included in the `weather-data` folder. These were retrieved using [Visual Crossing](https://www.visualcrossing.com/weather/weather-data-services) and merged by me.
- The Low Carbon London dataset is not provided in this repository due to licensing restrictions. However, it can be accessed via the UK Data Service:  [Low Carbon London Dataset](https://beta.ukdataservice.ac.uk/datacatalogue/studies/study?id=7857).

## Repository Limitations
Due to data safeguarding policies, this repository contains only partial code and cannot be directly run. Full replication requires accessing the Low Carbon London dataset via the UK Data Service and following the methodology detailed in the dissertation.

## Acknowledgements
I would like to thank my supervisor, Dr. Fanlin Meng, for his invaluable guidance and encouragement throughout this project. Special thanks to my family, friends, and girlfriend for their support.

## Contact
For any questions about this project, feel free to contact me at rogerthant33@gmail.com

## License
This project is licensed under a Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License. See the `LICENSE` file for details. Additional permissions may be required from the University of Manchester.
