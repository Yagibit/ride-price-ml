# Ride Price Estimation System

## Project Overview
This project builds a machine learning system to estimate ride prices based on trip and contextual features such as distance, duration, traffic, weather, and demand. The focus is on thinking like a practitioner: designing a dataset, preparing data, training models, and reflecting on results.

## Dataset Description
The dataset is synthetically generated with 200 rows and 7 input features. The target variable is `ride_price`, a continuous value representing the cost of a ride. Both numerical and categorical features are included.

## Features Used
- **distance_km** (numerical): Distance of the ride in kilometers. Longer distances increase price.  
- **duration_min** (numerical): Trip duration in minutes. Longer duration slightly increases price.  
- **time_of_day** (categorical): Morning, Afternoon, Evening, Night. Prices may vary during peak hours.  
- **traffic_level** (categorical): Low, Medium, High. High traffic increases price.  
- **weather** (categorical): Clear, Rainy, Foggy. Bad weather increases price.  
- **demand_level** (categorical): Low, Medium, High. High demand may trigger surge pricing.  
- **vehicle_type** (categorical): Standard, Premium, SUV. Premium or SUV vehicles cost more.

## Models Implemented
- **Linear Regression**: Predicts the exact ride price.  
- **Logistic Regression**: Classifies rides as high-cost or low-cost based on median price.

## Evaluation
- Regression is evaluated using **Mean Absolute Error (MAE)** and **R² Score**.  
- Classification is evaluated using **Accuracy** and **Confusion Matrix**.  

### Key Findings
- Distance (`distance_km`) is the most influential feature for pricing.  
- Linear regression accurately predicts ride price with reasonable error.  
- Logistic regression can classify high-cost rides effectively.  
- Data quality and feature design strongly influence model performance.

## Ethical Consideration
- Surge pricing may unfairly affect low-income users or during emergencies.  
- Synthetic dataset may not fully capture real-world pricing behavior.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/ride-price-ml.git
