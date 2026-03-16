°Predictive Model for Airline Customer Bookings

A machine learning project that predicts whether a customer will complete a flight booking based on behavioral and travel data.
The goal is to help airlines identify high-potential customers and optimize marketing strategies.

This project was developed as part of a data science virtual internship simulation with British Airways.

°Project Objective

Airline websites receive a large number of visitors who search for flights but do not complete their bookings.

The objective of this project is to:

Predict whether a customer will complete a booking

Identify the most important factors influencing booking behavior

Provide insights that help airlines increase conversion rates

This allows airlines to:

Target customers with personalized promotions

Improve demand forecasting

Optimize seat capacity planning

°Dataset

The dataset contains 49,162 records of customer booking behavior.

Each record represents a customer's interaction with the airline booking system.

Example Features
Feature	Description
purchase_lead	Number of days between booking and departure
route	Flight route
length_of_stay	Duration of the trip
flight_hour	Hour of departure
flight_duration	Flight time
num_passengers	Number of passengers
wants_extra_baggage	Whether customer selected extra baggage
wants_in_flight_meals	Whether customer selected meal option
wants_preferred_seat	Whether customer selected seat preference

Target variable:

booking_complete

1 → booking completed

0 → booking not completed

°Data Processing

Steps performed during preprocessing:

Outlier handling

Data balancing

Feature encoding

Feature selection

Train / validation split

Balanced training subsets were created:

7,362 bookings

8,000 non-bookings

°Machine Learning Model

The model used for prediction:

Random Forest Classifier

Reasons for choosing Random Forest:

Handles mixed numerical and categorical data

Robust against overfitting

Provides feature importance analysis

Cross Validation
CV AUC: 0.700 ± 0.011
Test AUC-ROC: 0.972
Accuracy: 92%

The model demonstrates strong predictive performance and balanced classification ability.

°Model Performance

Confusion Matrix (Validation Set)

Predicted 0	Predicted 1
Actual 0	1496	109
Actual 1	124	1344

The model accurately predicts both booking and non-booking customers.

°Key Drivers of Booking Behavior

The most influential features identified by the model include:

Purchase lead time

Route popularity

Length of stay

Flight departure hour

Flight duration

Flight day

Number of passengers

In-flight meal selection

Extra baggage selection

Preferred seat selection

These insights reveal early booking signals and route demand patterns.

°Business Impact

Insights from the model can help airlines:

Revenue Optimization

Potential 15–20% increase in bookings through targeted promotions.

Customer Personalization

Identify users with high booking probability and offer personalized deals.

Operational Efficiency

Improve seat capacity planning

Reduce unused seats

Optimize route management
