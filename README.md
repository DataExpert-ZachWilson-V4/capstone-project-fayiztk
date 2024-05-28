## Capstone Project - Air Pollution across cities in India

### Objective:
The objective of this project is to develop a comprehensive and dynamic dataset which aims to provide a clean and aggregated view of air pollution trends in India over the years, while also reflecting the current pollution levels

Input data set of the project is:
- Historical data over the years in CSV
- Real time data which is getting refreshed every hours

### Data model
- State: India state name
- Area: Area from the state
- Area Type:  Type of the area. For example, industrial,residential,etc
- Pollutants measurement: Cumulative array which stores average measurement for pollutant for each month.
                          There will be separate column for each pollutant.
- Year: Year of the measurement


### Tools used:
- Create base dataset from historical data:

  Transformation:
    - spark for creating a silver layer if the dataset needs to be cleaned in deep
    - dbt for silver to gold layer
  
  Orchestration: Airflow
  
- Update base dataset with real time data: To be updated after realtime data processing classes
