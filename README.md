# **Household-Level Day-Ahead Peak Electricity Demand Forecast**

This repository contains materials from my MSc Data Science dissertation, which was awarded a **Distinction** at the University of Manchester. The project focuses on developing machine learning models to forecast household-level day-ahead peak electricity demand using the Low Carbon London dataset and detailed London weather data.

## Abstract
This study develops and evaluates machine learning models for forecasting day-ahead peak 
electricity demand at the household level, addressing a gap in the literature by integrating 
diverse household-level data sources. Using the Low Carbon London project dataset and 
weather data, the research applies XGBoost models with various feature sets. The optimal 
model achieves a test WAPE of 29.63% with 15 features. Recent consumption patterns 
emerge as the most significant predictors, while household characteristics play a less 
prominent role than hypothesized. The study reveals that carefully selected subsets of features 
can achieve comparable performance to larger feature sets, suggesting potential for efficient, 
streamlined forecasting models. Limitations include underestimation of high consumption 
events and potential bias from opt-in recruitment. The findings have implications for data 
collection strategies and model development in the energy sector, emphasizing the 
importance of high-quality recent consumption data for short-term forecasting. Future 
research directions are proposed to address limitations and further refine forecasting 
techniques.

## Key Components
### Dissertation
- The full dissertation is provided as `dissertation.pdf`, detailing the methodology, results, and implications of the study.

### Notebook
- `Model-Development-Cbrt-No-Scaler.ipynb`: Optimized model with cube root transformation of the target variable. <br>

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
