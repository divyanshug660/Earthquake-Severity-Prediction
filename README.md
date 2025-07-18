# Earthquake-Severity-Prediction

This project is an end-to-end machine learning pipeline that classifies the severity of earthquakes based on geospatial and geological features. It uses historical earthquake data containing latitude, longitude, depth, and magnitude to predict whether an event is of low, moderate, or high severity.

The model is built using Python and scikit-learn, and includes all steps from data loading to model evaluation and artifact saving. It’s designed to be easy to understand, reproducible, and extendable for more advanced seismic prediction systems in the future.

# Problem Statement #

Earthquakes pose a serious threat to life and infrastructure. While seismic data is continuously recorded across the globe, manually interpreting this data is not scalable. This project aims to automate the classification of earthquake magnitude levels to support early risk assessment and further integration into alert systems.

# Objectives #

1. Load and clean raw earthquake data
2. Convert magnitude values into categorical severity levels
3. Train a classification model using Random Forest
4. Evaluate the model using standard performance metrics
5. Save the trained model and scaler for deployment or integration

# Dataset Structure #

The dataset include the following columns:

1. Latitude: The latitude coordinate of the earthquake epicenter
2. Longitude: The longitude coordinate of the earthquake epicenter
3. Depth: The depth of the earthquake in kilometers
Magnitude: The magnitude of the earthquake (used to classify severity)

# Classification Criteria #

Magnitude values are categorized into three classes:

- **Low**: Magnitude < 4.0
- **Moderate**: 4.0 ≤ Magnitude < 6.0
- **High**: Magnitude ≥ 6.0

These are then encoded as 0, 1, and 2 respectively for model training.

## Technologies Used

- Python 3.7+
- Pandas & NumPy
- Scikit-learn
- Seaborn & Matplotlib
- Joblib (for model persistence)
