# Cash Flow Forecast
- Develop cash flow forecast models to identify the Group Cash Flow impact from amounts due to vendors or suppliers for goods or services received that have not yet been paid for stemming from vendors in 5 key countries.
    This project is focused on forecasts for five key countries.
    - USA 
    - China 
    - Germany
    - Switzerland
    - Ireland

 - For different countries, the Account Payable and Cost are following different units. The aforementioned five key countries have different currencies so each country should have a separate unit. Specifically, USD (USA) / CNY (Yuan) / Euro (Germany/Ireland) / Switzerland (CHF). There is no standardized unit for all countries. 

# Dataset Anonymization
‘Z-score’ is used to anonymize the real data. For all the variables, following is the formula used to privatise the data:

            zi = (xi – μ) / σ
 
where zi = z-score of the ith value for the given variable

            xi  = actual value

            μ = mean of the given variable

            σ = standard deviation for the given variable

 
Other account and vendor names are replaced by their md5 values.

## Tech Stack
- [Anaconda Python3](https://www.anaconda.com/distribution/)


## Installation
### Installing Required modules in conda environment
```cmd
- pip install -r requirements.txt
- copy the training and test csv's into the data folder
- give the path anme in teh training-prediction jupyter notebook and run it
- this will create a output file in data folder with test_sheet.csv
```

## NOTES
- For guidelines,strategy and intuition involved follow the report.pdf .
- Exploratory Data Analysis is done in EDA jupyter notebook.
- Analysis of data trends and seasonality with smoothening and stationary checks and selecting the appropriate model is in analysis jupyter notebook.
- Prediction and Training of data and models is done in training-prediction jupter notebook

