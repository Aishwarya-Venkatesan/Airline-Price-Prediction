# Airline-Price-Prediction

dataset: 
  source: Kaggle https://www.kaggle.com/code/anshigupta01/flight-price-prediction/data
  size: 10683 records
  varialbles (9): demographic(4) - Name, Source, Destination, total stops
                  numerical(5) - Date of Journey, Departure time, Arrival time, Duration of flight, Price (target).

Aim: Forecast Airline ticket pricing based on past history

#Preprocessing:
  1) Missing value handling: Price-Replacing with mean
  2) Changed datatypes of Date_of_journey, arrival_time, departure time IN PROPER datetime format.
  3) Categorical data handling:
     i) Label encoding - Total_stops
     ii) OneHot encoding - Airline, source, destination
4) Outlier in price variable replaced with median of price of respective airlines.

#Data-Visualization
     I. Airline vs Price: (Insight) Jet Airways are most costliest compared to the other airlines.
    II. Source vs Price: (Insight) Most of the flight starts from Bangalore.
   III. Destination vs Price: New Delhi has the most expensive and higher range of flights than any other cities.

#PREDICTION USING MACHINE LEARNING MODELS
i) Random Forest:  r2_score=0.812
ii) KNeighbour Regressor:  R2_score= 0.55
iii) Decisiontree regressor:  r2_score=0.690
iv) GradientBoost Regressor: r2_score=0.77
v) SVM regressor: r2_score = -0.8

Metrics used: R2_SCORE, MAE, MSE, RMSE

#Conclusion: A thorough investigation was conducted for this work using Kaggle
dataset collection, and the Random Forest Machine Learning model was
applied. We were able to identify the factors that have the greatest impact on
airline ticket pricing using visualisation. The results of the experimental
research show that the Random Forest Regression model has good accuracy.
The objective for the future is to improve model accuracy and feature
selection. In order to obtain more accurate airfares, we also intend to expand
the study by working with larger datasets and conducting additional
experiments on it. This will allow consumers to get an idea of how much
their next flight will cost and enable them to negotiate the best deal.
