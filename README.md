# Energy Consumption Prediction Report

## 1. Problem Statement
The objective of this project is to develop a machine learning model that predicts the energy consumption of industrial equipment using sensor data. This will support facility managers in optimizing energy usage and reducing operational costs.

## 2. Approach

### a. Data Preprocessing
- Converted necessary features from object to numeric types
- Imputed missing values using median strategy
- Removed or capped outliers in features like humidity and wind speed
- Extracted time-based features from timestamps (if applicable)
- Scaled features using standardization

### b. Exploratory Data Analysis (EDA)
- Found correlations between environmental conditions and energy consumption
- Identified important contributors like temperature, humidity, and atmospheric pressure

### c. Modeling
- Applied multiple regression models including:
  - Linear Regression (baseline)
  - Random Forest Regressor
  - XGBoost Regressor
- Evaluated models using:
  - Mean Absolute Error (MAE)
  - Root Mean Squared Error (RMSE)
  - RÂ² Score

## 3. Key Insights

- *Zone Temperatures and Humidity*: Strong correlation with equipment energy use, suggesting internal environment plays a major role
- *Outdoor Conditions*: Variables like outdoor temperature and atmospheric pressure also had moderate influence
- *Lighting Energy*: Often associated with higher equipment energy usage, indicating combined operational loads

## 4. Model Performance

| Model               | MAE    | RMSE   | RÂ² Score |
|--------------------|---------|---------|----------|
| Linear Regression  | ~74.22  | ~147.97 | ~0.00    |
| Random Forest      | ~63.73  | ~128.33 | ~0.25    |
| XGBoost Regressor  | ~73.17  | ~146.21 | ~0.02    |


## 5. Recommendations

- *Zone Climate Control*: Maintain consistent and optimal zone temperatures and humidity levels.
- *Outdoor-Responsive Scheduling*: Adjust operational intensity based on weather forecasts to minimize energy waste.
- *Lighting Optimization*: Use energy-efficient lighting and automate control based on usage and time.
- *Sensor Calibration*: Ensure accurate sensor readings as some anomalies indicate potential data quality issues.

## 6. Conclusion
The predictive model effectively estimates equipment energy usage and highlights actionable factors to reduce energy consumption, offering clear benefits for operational efficiency and cost management.
