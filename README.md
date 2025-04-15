# 🌫️ Breathe India: A Data-Driven Exploration of Air Quality Patterns

This project was developed for the course **"Data Science Toolbox: Python Programming"** and focuses on analyzing real-time air quality data across Indian cities using Python.

---

## 📁 Dataset

**Source**: [data.gov.in – Real-Time Air Quality Index](https://www.data.gov.in/catalog/real-time-air-quality-index)

- Format: CSV
- Rows: 1000+
- Fields: City, Station, Pollutant ID, AQI, Pollutant Values, Timestamps, etc.
- Description: This dataset includes hourly updates on Air Quality Index and pollutant levels from different monitoring stations across India.

---

## 🧠 Project Objectives

We focused on 7 key objectives:

### 1. Clean and Process the Data
- Removed rows with missing `pollutant_avg`, `last_update`, and `station`.
- Converted timestamp strings to proper datetime format.
- Ensured all columns have consistent data types for analysis.

### 2. Which City Has the Highest Average AQI?
- Filtered data to only include AQI values.
- Grouped by city and calculated average AQI.
- Displayed results in descending order to rank the cities.

### 3. What Is the Correlation Between PM2.5 and PM10?
- Extracted PM2.5 and PM10 values city-wise.
- Merged them into a single DataFrame.
- Used `.corr()` and a heatmap to visualize their relationship.

### 4. How Does AQI Vary by Time of Day?
- Extracted hour from `last_update` column.
- Classified times into: Morning, Afternoon, Evening/Night.
- Grouped by time of day and calculated average AQI.
- Visualized it using a bar chart.

### 5. Outlier Detection in AQI Values
- Used the IQR (Interquartile Range) method to detect AQI outliers.
- Identified and printed stations with unusually high or low AQI readings.
- Used boxplots to visualize the spread and outliers.

### 6. Which Pollutants Contribute the Most to Poor AQI in Metro Cities?
- Focused on metro cities like Delhi, Mumbai, Chennai, etc.
- Filtered AQI > 200 to find periods of poor air quality.
- Counted how often each pollutant was associated with high AQI.
- Used bar plots to visualize pollutant contributions.

### 7. How Does Air Quality Vary Across States?
- Extracted state names from station/city data.
- Grouped by state and calculated average AQI.
- Visualized results using horizontal bar charts.

---

## 🔧 Tools & Libraries Used

- **Python**
- **Pandas** – for data cleaning and manipulation
- **NumPy** – for numerical operations
- **Matplotlib & Seaborn** – for data visualization
- **Jupyter Notebook** – for interactive coding

---

## 📊 Sample Visuals

- Correlation heatmaps for pollutants
- AQI trend bar charts (time of day)
- Boxplots for AQI outliers
- Bar charts for city/state-wise AQI analysis

---

## 📌 How to Run the Project

1. Download the dataset from [here](https://www.data.gov.in/catalog/real-time-air-quality-index) or use the included `air.csv`.
2. Open the `Air_Quality_Analysis.ipynb` in Jupyter Notebook.
3. Run all cells in order.
4. Explore the graphs and outputs for each objective.

---

## 🤝 Project Credits

- **Developed by**: [Aditya ranjan]
- **Subject**: Data Science Toolbox: Python Programming

---

## 📬 Connect With Me
- LinkedIn: [ (www.linkedin.com/in/aditya-ranjan00) ]

---

