**London Bike Sharing Analysis and Forecasting 🚲📊**

This project explores and analyzes the London bike-sharing dataset. The dataset contains detailed information about bike rentals, weather conditions, and time-based data points, enabling data-driven insights and forecasts. The analysis includes data preparation, statistical summary generation, and preparation for visualization using Tableau.

**Table of Contents**

Introduction

Data Understanding

Data Preparation

Insights and Observations

Next Steps

**Introduction**

Bike-sharing systems play a significant role in urban mobility. This analysis leverages Python for data processing and prepares the dataset for visualization in Tableau. The goal is to uncover trends, patterns, and actionable insights about bike rentals in London.

**Data Understanding**

The dataset, london_merged.csv, contains 17,414 rows and 10 columns:

  time: Timestamp of the record.
  
  count: Number of bikes rented.
  
  real_tempature: Actual temperature in Celsius.
  
  feels_like_tempature: Perceived temperature in Celsius.
  
  humidity_percent: Humidity level as a percentage.
  
  wind_speed_kph: Wind speed in km/h.
  
  weather: Weather conditions (e.g., Clear, Rain, etc.).
  
  is_holiday: Whether the day is a holiday (0: No, 1: Yes).
  
  is_weekend: Whether the day is a weekend (0: No, 1: Yes).
  
  season: Meteorological season (e.g., Winter, Summer, etc.).
  
**Data Preparation**

Key steps taken to prepare the data:

1. Renaming Columns: Improved readability by renaming columns to more descriptive names.
2. Value Scaling: Converted humidity_percent to a scale between 0 and 1.
3. Mapping Values:
  Seasons (e.g., 3.0 → Winter).

  Weather conditions (e.g., 1.0 → Clear).
5. Data Type Conversion: Updated season and weather columns to string for proper mapping.
6. Statistical Summary: Generated descriptive statistics to understand the dataset's key metrics.
7. NULL Value Check: Confirmed there are no missing values.
   
**Insights and Observations**

Average Rentals: 1,143 bikes rented daily, with significant fluctuations (std: 1,085).
- Temperature Range: From -1.5°C to 34°C, representing all seasons.
- Humidity Impact: High average humidity (72.3%), potentially influencing bike rentals.
- Rental Patterns:
    Holidays: Rare in the dataset (~2% of days).
    Weekends: Comprise ~28% of the dataset.
- Peak Rentals: Maximum daily rentals reached 7,860, indicating high demand on busy days.
  
**Next Steps**
  
Visualization: The data has been saved as an Excel file (london_bikes_sharing_analysis.xlsx) for further visualization and exploration in Tableau.

You can view the interactive Tableau dashboard here: [Tableau Public Dashboard](https://public.tableau.com/views/LondonBikeSharingDashboard_17365424694300/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

Forecasting: Implement machine learning models to forecast bike rentals based on weather and temporal patterns.

**Tools Used**

Python: pandas, numpy, matplotlib for data processing.

Tableau: For interactive visualizations.

**How to Run**

1. Clone the repository:
```
git clone git@github.com:<your-username>/London-Bike-Sharing-Analysis-and-Forecasting.git
cd London-Bike-Sharing-Analysis-and-Forecasting
```

2. Install required Python libraries:

```
pip install pandas numpy matplotlib openpyxl
```
3. Run the Jupyter notebook or Python script to process the data.
4. Open _london_bikes_sharing_analysis.xlsx_ in Tableau to visualize insights.


Feel free to contribute, report issues, or suggest enhancements! 🚀

