# Urban-Traffic-Optimization-
This is data analysis project exploring the vehicle and pollution patterns at different location in Prayagraj.
**Dataset**
The dataset used for project is [DATA VISION original set.xlsx](https://github.com/user-attachments/files/20966000/DATA.VISION.original.set.xlsx). It contains the following columns:-
 * Timestamps
 * Intersection details (ID, name, coordinates)
 * Vehicle counts (total, car, bus, truck, motorcycle)
 * Average speed
 * Traffic signal timings (cycle, green, yellow, red)
 * Weather conditions
 * Day of the week, holiday status
 * Special events
 * Pollution levels

**Methodology**
1. Data Loading
   Load the dataset from the Excel file using Pandas.
2. Data Cleaning:
  * Address missing values using appropriate strategies (median for numerical, mode for categorical, interpolation for timestamp, ffill for record ID).
  * Handle outliers in average_speed using the IQR method with capping and flooring.
3. Exploratory Data Analysis (EDA):
  * Analyze traffic volume and speed patterns across different intersections, times, days, and weather conditions.
  * Investigate the impact of holidays and special events.
  * Examine correlations between vehicle count, average speed, and pollution levels.
4. Feature Engineering:
  * Encode categorical features (day_of_week, weather_condition) using Label Encoding for model training.
  * Extract features like hour from the timestamp.
  * Calculate total_vehicles and percentage distributions.
5. Model Training:
  * Select relevant features for prediction.
  * Split the data into training and testing sets.
  * Train a RandomForestRegressor model to predict vehicle_count.
  * Evaluate the model using MAE, MSE, and RMSE metrics.
**Technology Used**
  * Programming Language: Python
  * Data Manipulation & Analysis: Pandas, NumPy
  * Machine Learning: Scikit-learn
  * Development Environment: Google Collab
  * Data Visualization: Matplotlib/Seaborn (within notebook), Power BI
  * Data Storage: Excel (.xlsx)
