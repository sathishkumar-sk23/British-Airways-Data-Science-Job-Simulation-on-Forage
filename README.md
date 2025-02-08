# British-Airways-Data-Science-Job-Simulation-on-Forage
# Customer Buying Behavior Prediction

This repository contains the code and analysis for predicting customer buying behavior using machine learning models. The goal of this project is to identify the factors that influence customers to purchase flights or holidays and predict whether they will complete a booking based on historical data.

## Project Overview

The project involves:

1. **Data Cleaning**: We preprocess and clean customer booking data to ensure it's ready for modeling.
2. **Exploratory Data Analysis (EDA)**: We analyze the dataset to uncover insights about the customer behavior and features influencing purchases.
3. **Modeling**: Several machine learning models were trained and evaluated to predict customer buying behavior.
4. **Hyperparameter Tuning**: We fine-tuned the Random Forest model to improve its predictive performance.
5. **Final Model**: The Random Forest model was selected as the best model based on its performance metrics.

## Dataset Description

The dataset contains 50,000 customer records with the following columns:

- `num_passengers`: Number of passengers travelling.
- `sales_channel`: The channel through which the booking was made.
- `trip_type`: Type of the trip (Round Trip, One Way, etc.).
- `purchase_lead`: Number of days between booking and flight.
- `length_of_stay`: Duration of stay at the destination.
- `flight_hour`: Departure hour.
- `flight_day`: Day of the week of flight departure.
- `route`: Flight route (origin -> destination).
- `booking_origin`: Country from where the booking was made.
- `wants_extra_baggage`: Whether the customer wants extra baggage.
- `wants_preferred_seat`: Whether the customer wants a preferred seat.
- `wants_in_flight_meals`: Whether the customer wants in-flight meals.
- `flight_duration`: Flight duration in hours.
- `booking_complete`: Target variable indicating if the customer completed the booking (1 = completed, 0 = not completed).

## Installation

To run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/customer-buying-behavior-prediction.git
