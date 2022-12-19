# Heart_Disease_Prediction
603 Term Project


### download_data.py

1. Download four csv files from UCI database
    1. processed.cleveland.data
    2. processed.hungarian.data
    3. processed.switzerland.data
    4. processed.va.data

2. Merge the data into a single pandas dataframe + add column headers +  saves the data to a single csv file.

### Processing_data.ipynb
check dataset info
drop Na rows
converting columns from float to int, and then check datatypes

#### data preprocessing
One-Hot Encoding

Creating Dummy Variables for cp, thal and slope
Merge Dummy Variables to Main Data Frame 
drop unnecessary variables
save to new csv file (processed_data.csv)