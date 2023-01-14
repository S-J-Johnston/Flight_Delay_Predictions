# Flight-Delay-Project


##The following document descibes the files in the currect directory.

## ipynb files:
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
  
 ## model files:
  - finalized_lin_reg_model.sav
       - Exported model from Flights_EDA_&_Modelling_Pass_Flight_Feats.ipynb. Used for the flight delay prediction for the Test dataset.
 
 ## Data Files
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
