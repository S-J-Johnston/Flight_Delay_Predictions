# Flight-Delay-Project

## Introduction
The purpose of this project is to create a predictive model to estimate the expected time delay on US commercial flights. 
The models are built using sampled data of all US air traffic from 2015-2019. 

## Data
Raw data was accessed from LHL private servers. Samples of the data can be found in the Data folder.

1. Flight Table:
    The departure and arrival information about flights in US in years 2018 and 2019
2. Passenger Table:
    The passenger totals on different routes from years 2015-2019 aggregated per month.
4. Weather:
    Was accessed through the [weatherAPI](https://www.weatherapi.com/). 

## Tech Stack
SQL, Pandas, Numpy, Matplotlib, Seaborn, SKlearn, Pickle 

## Process
The predictive model was built over multiple iterations. At each iteration additional features were applied to assess if there was any improvement in model performance.

![Alt text](Images/Development%20Process.png)

## Results
*To be added. Baseline model using linear regression showed the best performance. XGBosst showed suspect results which require further investigation. 

## Repository Table of Contents:

### ipynb files:
  - model_test.ipynb
      - Test Dataset predictions
  - Flights_EDA_&_Modelling_Pass_Flight_Feats.ipynb
      - Best preforming model and candiate model used for predictions on test dataset.
  - Flights_Modelling_Pass_Flight_Weather_Feats.ipynb
      - Test model using weather data.
  - Flights_Modelling_Pass_Feats.ipynb
      - Test model using passenger features.
  - Flights_EDA_&_Baseline_Modelling.ipynb
      - Test model using minimum features. No feature engineering.
  - Passenger_EDA_Feature_Eng.ipynb
      - EDA and Feature engineering for passenger table.
  
 ### model files:
  - finalized_lin_reg_model.sav
       - Exported model from Flights_EDA_&_Modelling_Pass_Flight_Feats.ipynb. Used for the flight delay prediction for the test dataset.
 
 ### Data Files
  - flight_delay_pred_model_submission.csv
      - The important one. Contains the model output for predictions on the test dataset.
  - route_keys.csv
      - Used to filter passenger data by routes present in Flight data
  - passenger_sample_50K.csv
      - sample data used for passenger EDA and feature engineering.
  - pass_route_features.csv
      - Output from passenger feature engineering. Imprted into models using passenger features.
  - output.csv
      - Weather API output.
  - flights_rnd_sample_50K.csv
      - Flights sample data
  - flight_test_100K.csv
      - sample flight test data
  - carrier_route_delay.csv
      - Aggregated features for flights
