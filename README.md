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
   ```

2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

## Project Steps

### 1. Data Preprocessing

We clean the dataset by handling missing values, encoding categorical features, and splitting the data into training and testing sets.

### 2. Exploratory Data Analysis (EDA)

We perform exploratory analysis to understand the distribution of key features and their relationship with the target variable (`booking_complete`). Key insights include:

- More bookings are made through certain sales channels.
- The booking lead time plays a critical role in predicting booking completion.
  
### 3. Model Training

Several models were evaluated, including:

- Logistic Regression
- Random Forest
- XGBoost
- SVM
- KNN

### 4. Hyperparameter Tuning

The Random Forest model was fine-tuned using grid search and cross-validation to find the optimal parameters.

### 5. Model Evaluation

The **Random Forest** model was selected as the best model due to its superior performance. The final classification report for Random Forest showed:

- Precision: 0.93 (for class 0)
- Recall: 0.73 (for class 1)
- F1-Score: 0.72

## Results

After hyperparameter tuning, the Random Forest model achieved an **accuracy of 85.3%**. The key features influencing booking completion include:

- **Purchase Lead Time**: Longer lead times tend to result in higher booking completion.
- **Trip Type**: Round trips had a higher likelihood of conversion.
- **Sales Channel**: Direct bookings via the website performed best.

## Conclusion

By understanding the factors that contribute to customer booking behavior, airlines can proactively target customers with personalized marketing campaigns to increase conversions.

