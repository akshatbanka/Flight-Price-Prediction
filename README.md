# Flight Price Prediction

## Overview
The **Flight Price Prediction** project predicts flight ticket prices based on user inputs such as travel date, time, source, destination, and airline. The project uses a machine learning model trained in Python, deployed via a Flask web application, with an HTML-based frontend for user interaction.

## Features
- Predicts flight ticket prices using a trained machine learning model.
- Interactive web interface for entering flight details.
- Provides real-time predictions and displays the result on the frontend.

## Technologies Used
- **Python**: Backend development and machine learning.
  - Libraries: `scikit-learn`, `pandas`, `numpy`, `flask`.
- **HTML**: Frontend for user interface.
- **Flask**: Framework to deploy the model as a web application.
- **Pickle**: For saving and loading the trained model.

## Workflow
### 1. Machine Learning Model
- The machine learning model is trained using a dataset of flight details.
- Preprocessing steps include:
  - Date-time extraction for departure and arrival times.
  - Encoding of categorical variables (e.g., airlines, source, destination).
  - Calculation of travel duration.
- The trained model is stored as `flight_rf.pkl` using Pickle.

### 2. Backend (Flask Application)
- **File**: `app.py`
- Key features:
  - Accepts user inputs such as departure and arrival times, stops, airline, source, and destination.
  - Processes inputs and predicts the price using the machine learning model.
  - Renders predictions on the HTML frontend.

### 3. Frontend
- **File**: `home.html`
- Interactive web page allowing users to input flight details.
- Displays the predicted flight price based on the user-provided details.

## Usage
1. Enter the required flight details:
   - Date and time of departure and arrival.
   - Number of stops.
   - Airline, source, and destination.
2. Submit the form to get the predicted flight price.

### 4. Deployment

Hosted on Heroku for public access.
