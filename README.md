# Phase_5_FFTR
Structure of this repo:
notebooks folder contains all jupyter notebooks, final notebook summarizes all of the work done and should be read first.
images folder contains saved visualization files
data folder contains all data files

# Overview
In the fields of finance and macroeconomics the Federal Funds Target Rate (FFTR) is one of the most studied and important indicators of the state of 
the US economy. While there have been sucessful models of how the FFTR should move in the past using machine learning, they are outdated and do not 
account for special circumstances in the economy that arose following the 2008 financial crisis and the 2020 covid pandemic. In this notebook I will 
outline 2 main models that have the ability to predict changes in the FFTR months in advance with high accuracy. I will compare these models to 
models based on conventional macroeconomic knowledge to show that there is more that goes into the decision to change the FFTR than classic theory 
suggests.

# Business Question
How well can we predict changes in the Federal Funds Target Rate (FFTR) using past performance and macroeconomic indicators?

# Data Sources
The data used in this project was sourced from FRED (Federal Reserve Economic Database) which is maintained by the Federal Reserve Bank of St. 
Louis. The API requests used to gather the data can be seen in the pipeline construction notebook. Feature inclusions and preprocessing can be seen 
in the EDA_Cleaning notebook.

# Results
The best model (gradient boosted trees) was able to predict the FFTR 3 months out with a RMSE of .048, MAE of .0112, r2 of 99.967, and MAPE of .005.