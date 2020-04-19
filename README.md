# Description
This research project aims to find the most predictive features for countries living in extreme poverty. We used the World Bank's definition of having a GNI of less then 1.9$ per day per person on average. From this data further conclusions may be made about ways of fighting extreme poverty and finding means to overcome it.

# Structure
## ./data/
contains input and intermediate data
```unesco_poverty_dataset.csv``` Unesco Institute for Statistics (UIS) dataset: "Demographic & socio-economic" data.
```continents.csv``` List of countries and respective continent 
```transformed.csv``` transformed unesco_poverty_dataset.csv for easier handling & machine learning 
```feature_descriptions.csv``` transformed.csv column descriptions & statistics
```unesco_metadata.pdf``` metadata provided by UIS.
## ./src/
contains all the code in form of streamlit notebooks
```data_prep.py``` data cleaning and wrangling (streamlit notebook)
```question.py``` data imputation and machine learning models (streamlite notebook)
```plots.py``` visualization module - not a streamlit notebook
## ./tex/
contains the latex data necessary to build the report on this project.
```usecase.pdf``` the final version of the report.

# How to run
## used libraries
pandas
numpy
sklearn
plotly
seaborn
matplotlib
streamlit

... install them with pip (cd into src/ first)
```pip install -r requirements.txt```

## Execution
run this command in src/
```streamlit run <notebook_file.py>```