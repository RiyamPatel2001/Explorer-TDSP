# Explorer-TDSP
Explorer Transportation Data Science Project

# NYC Traffic Collision Analysis

## Overview

This project analyzes traffic collision data in New York City to identify patterns, trends, and key factors contributing to accidents. The goal is to extract insights that could potentially inform strategies for improving road safety.

## Data Source

The analysis uses the publicly available NYC traffic collision dataset.  The notebook includes snippets showing the data includes the following:
* Crash Date and Time
* Location information (Borough, Zip Code, Latitude, Longitude, Streets)
* Factors Contributing to the crash per vehicle
* Vehicle Types
* Number of persons injured/killed (pedestrians, cyclists, motorists)

## Data Cleaning and Preprocessing

*   **Handling Missing Values:** The notebook shows a detailed breakdown of missing values in each column and the percentage of missing data. Columns with high percentages of missing data for vehicle type and contributing factors were noted.
*   **Data Type Conversion:** Data types of columns such as 'CRASH DATE' and 'CRASH TIME' were checked.
*   **Geographic Data:** Latitude and longitude coordinates were used for location analysis.

## Exploratory Data Analysis (EDA)

The following EDA was conducted, based on the notebook contents:

*   **Summary Statistics:** Descriptive statistics (mean, median, std, min, max) were calculated for numerical columns like 'NUMBER OF PERSONS INJURED,' 'NUMBER OF PERSONS KILLED,' 'LATITUDE,' and 'LONGITUDE.'
*   **Casualties per Area:** The notebook calculates and analyzes casualties (injuries and fatalities) per square kilometer for each ZIP code, providing a density-based measure of accident impact.  This includes separate calculations for pedestrians, cyclists and motorists.

## Key Findings (Based on Snippets)

Based on the analyzed snippets, some potential findings include:

*   **High Missing Data:** A significant portion of the dataset contains missing values, especially in columns related to contributing factors and vehicle types (particularly for vehicles 3, 4, and 5). This needs to be considered when interpreting results.
*   **Casualty Density Variation:** There's considerable variation in casualty density across different ZIP codes in NYC. Some ZIP codes show significantly higher casualties per square kilometer. For example, a small snippet shows ZIP code `10007` has high casualties per square kilometer as compared to other ZIP codes.

## Next Steps (Potential)

The following steps could be taken to further enhance the analysis:

1.  **Advanced Spatial Analysis:** Conduct spatial clustering and hotspot analysis to identify areas with significantly higher collision rates.
2.  **Temporal Analysis:** Investigate trends in collisions over time (daily, weekly, monthly, yearly) to identify peak collision periods.
3.  **Factor Analysis:** Use statistical methods to determine which factors are most strongly associated with severe collisions.
4.  **Interactive Visualization:** Create interactive maps and dashboards to visualize collision data and insights.
5.  **Address Missing Data:** Further handling of the data and imputations of the missing datapoints.

## Technologies Used

*   Python
*   Pandas
*   Jupyter Notebook
*   Google Maps
*   Polygon
