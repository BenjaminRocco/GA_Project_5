# Fluctuating $\text{CO}_2$ Emissions and Changing Energy Sources: Regression Modeling and Time Series Applications

## General 

This project focuses on analyzing environmental data with social impact.

### Environmental Data from the Energy Information Administration and Kaggle scraped from the EPA and World Bank:

- https://www.kaggle.com/datasets/sogun3/uspollution
- https://www.kaggle.com/datasets/anshtanwar/global-data-on-sustainable-energy
- https://www.eia.gov/state/seds/seds-data-complete.php
- https://www.eia.gov/electricity/data/state/

### Problem statement:

Communities across the United States are facing the dangers of climate change and air pollution. To address the issue, we are surveying air pollution and renewable energy datasets to create predictive models that can be utilized by policymakers, economists, and civil society organizations. The goal of this research is to better aid our understanding on how air pollution is affecting our society as a whole. The model will be capable of predicting air pollution levels as a function of changes in renewable energy  and fossil fuel productions.

We explore changing energy sources and their impact upon carbon emissions in the United States by utilizing multiple regression models, time series models, and multivariable modeling to find meaningful relationships and correlations between our feature variables (energy sources) and the target variable (carbon emissions). We also do in depth research to explore trends in changing policies and natural phenomena that impact carbon emissions and other pollution metrics independent of human energy consumption and dependent upon human energy consumption as a result of the coronavirus pandemic. Many of these interpretations may be found in our notebooks and in the powerpoint presentation. Overall, by creating advanced Time Series models, predict that $\text{CO}_{2}$ levels will continue to drop, followed by a subsequent spike and continued fluctuation trending downwards as certain states decide to roll back emissions regulations and not all states implement renewable energy options. 

## Table of Contents

See `requirements.txt` file for versions of libaries and packages, easy install with pip and -r flag, type the following in your bash or terminal: `pip install -r requirements.txt` 

### `README.md`
### `Exploratory_Data_Analysis`
- Project_5_New_EDA_ben.ipynb
- Project_5_EDA_ben.ipynb
- Project_5_EDA_Dom.ipynb
### `Modeling`
- Project_5_Regression_Modeling_Ben.ipynb
- Project_5_Time_Series_Modeling_Ben.ipynb
- Project_5_Time_Series_Dan.ipynb
- Project_5_Modeling_Dom.ipynb
### `Visualizations`
- Project_5_Visuals.ipynb
- ARIMA_Powerpoint.png
- SARIMA_Powerpoint.png
- pacf_dan.png
- ts_lin_dan.png
- co2_dom.png
- coal_dom.png
- natural_gas.png
- nuclear_dom.png
- petroleum_dom.png
- renewable_dom.png
### `Powerpoint_Presentation`

### `Datasets_Link`
- Datasets for this project may be found here: https://github.com/BenjaminRocco/Project_5_Datasets/tree/main

---

## File Descriptions 

### `README.md`
### `Exploratory_Data_Analysis_Folder`
- Project_5_New_EDA_ben.ipynb: Includes data imports, cleaning, munging, and exploratory data analysis (EDA) of $\text{CO}_2$ data and energy source data. Energy sources: coal, natural gas, nuclear energy, petroleum and renewable energy. Renewable energy includes solar, wind, hydroelectric, and geothermal. Units for $\text{CO}_2$ data are (Per capita emissions in metric tons per person). Units for energy sources are British Thermal Units. Source: https://www.eia.gov/state/seds/seds-change/index.php/
- Project_5_EDA_ben.ipynb: Data from Kaggle website includes pollution metrics ranging from $\text{O}_3$, $\text{CO}$, $\text{SO}_2$, $\text{NO}_2$ in parts per billion and Air Quality Index (standard units) observed over a $23$ year period from 2000-2023 from states at a county and city level as well as energy values [Electricity from fossil fuels (TWh) generated from fossil fuels (coal, oil, gas) in terawatt-hours, Electricity from nuclear (TWh) generated from nuclear power in terawatt-hours, Electricity from renewables (TWh) generated from renewable sources (hydro, solar, wind, etc.) in terawatt-hours] at a nationwide level from 2000-2020. These were initially used for regression modeling but later were excluded from the process and relegated to creation of visual plots. 
- Project_5_EDA_Dom - Took cleaned state-level data and generated cleaned national average data. Cleaned national average data for all variables used for various time series models throughout group.
### `Modeling_Folder`
- Project_5_Regression_Modeling_Ben.ipynb: Exploration of various regression models evaluated based on $\textbf{R}^{2}$ score agreement amongst train and test sets and Root Mean Squared Error (RMSE). Best Regression models: Third: Linear Regression with Polynomial features: The train score was $0.9956$ while test score was $0.9941$ with RMSE values train $1.1213$ and test $1.371.$ Second: K Nearest Neighbors with a train score of $1.0$ and test score $0.99476$ with RMSE values $0.0$ for train and test $1.2920.$ First: Bagging Tree Regressor with train score $0.9989$ and test score $0.9953$ with RMSE values train $0.5586$ and test $1.2230.$ 
- Project_5_Time_Series_Modeling_Ben.ipynb: Time Series models with ARIMA and SARIMA algorithms. Results: ARIMA: AIC: $89.124$ RMSE $3.330.$ SARIMA (with smaller sample size for test): AIC $36.0$ and RMSE $0.4773.$ 
- Project_5_Time_Series_Dan: Utilized clean national average data to conduct EDA through plots for all variables and create a linear time series model. Linear model finds that, $\text{CO}_2$ emissions are forecasted to continue in a downward trend based on energy consumption levels. The $\textbf{R}^2$ for train was $0.997$ and for test was $0.8212$ while the AIC score was $-27.74$ and RMSE Score for test was $0.5009.$
- Project_5_Modeling_Dom - Utilized clean national average data to generate EDA graphs for all variables and create a multivariate time series model. Multivariate model found that, after a small increase to $\text{CO}_2$ emissions from their COVID era low, $\text{CO}_2$ emissions are forecasted to continue in a downward trend based on energy consumption levels.

### `Visualizations_Folder`

- Project_5_Visuals.ipynb: Visuals from `Project_5_EDA_ben.ipynb` datasets (initial datasets prior to further data collection). Purpose of this file was to gain deeper insights into multiple pollution index metrics as well as energy source trends from states and at a nationwide level from the 21st century only. Viewed natural disaster and anthropologic crisis event and other trends in data emblematic of the positive and negative correlation amongst variables in the study that necessitated multi-variable analysis.

Following were for use in presentation:
- ARIMA_Powerpoint.png
- SARIMA_Powerpoint.png
- pacf_dan.png
- ts_lin_dan.png
- co2_dom.png
- coal_dom.png
- natural_gas.png
- nuclear_dom.png
- petroleum_dom.png
- renewable_dom.png
### `Powerpoint_Presentation`
### `Datasets_Link`
- Datasets for this project may be found here: https://github.com/BenjaminRocco/Project_5_Datasets/tree/main

### Group Members:

Ben Moss, Daniel Kim, Dominic Martorano.

---

### Presentation Contents:

- Problem summary.
- Walkthrough of blueprint to find solution.
- Demonstration of solution.
- Summaries of models fit and their performance (Root Mean Squared Error). 
- Brief discussion of limitations in the process. (i.e. data collection issues, missing values)
- Discussion of next steps.
