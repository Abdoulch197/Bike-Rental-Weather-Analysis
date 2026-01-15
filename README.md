# Bike Rental Weather Impact Analysis

## Overview
This project analyzes Citi Bike ridership data mixed with NOAA daily weather data to understand how weather conditions affect bike rental demand. The goal was to design a PostgreSQL database  that is ready for analysis and create SQL views and schemas that  would allow users to quickly draw conclusion on weather impacts.

---

## Data Sources
- **Citi Bike Trip Data (2016)**  
  Monthly bike rental data including trip duration, start and end stations, user type, and rider demographics.
- **NOAA Weather Data (Newark Airport, 2016)**  
  Daily weather metrics including temperature, precipitation, snowfall, and wind speed.

---

## Tools & Technologies
- Python (pandas, Jupyter Notebook)
- PostgreSQL
- SQL (views, aggregation, joins)
- GitHub

---

## Project Workflow

### 1. Data Cleaning & Preparation
- Standardized column names and data types
- Parsed timestamps and created analytical fields (trip date, start hour, trip duration)
- Filtered invalid trips and cleaned demographic data
- Reduced weather data to relevant daily metrics

### 2. Database Design
- Created separate tables for trips and daily weather data
- Used appropriate data types and constraints for analytics
- Loaded cleaned CSVs into PostgreSQL using bulk import

### 3. Analytics-Ready Views
Several SQL views were created to support analysis:
- **Trips with Weather** – combines individual trips with daily weather conditions
- **Daily Trips & Weather Summary** – aggregates daily demand and average trip duration
- **Weather Impact Summary** – groups days by rainfall level to compare demand
- **Hourly Demand View** – shows how ridership changes by hour of day

---

## Key Findings
- Bike usage is highest on days without precipitation
- Average daily trips decrease as rainfall intensity increases
- Temperature alone does not explain demand the way precipitation does

---

## Example Insight
On days with no rain, average daily trips were significantly higher than on heavy rain days, showing that precipitation has a strong negative impact on bike rental usage.

---

## Project Takeaways
This project demonstrates the ability to:
- Clean and transform real-world datasets
- Design and implement a relational PostgreSQL database
- Create reusable SQL views for analytics
- Translate data into meaningful business insights

---

## Future Improvements
- Add station-level geographic analysis
- Incorporate hourly weather data
- Build visual dashboards using SQL query outputs


