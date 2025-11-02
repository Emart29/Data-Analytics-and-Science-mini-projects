# Los Angeles Crime Data Analysis

## 📊 Project Overview
Exploratory data analysis of crime data from Los Angeles, focusing on identifying patterns in criminal behavior to support the LAPD in resource allocation.

## 🎯 Objectives
- Analyze crime distribution throughout the day
- Identify peak crime hours  
- Determine areas with highest nighttime crime activity
- Examine victim age distribution patterns

## 📈 Key Findings
- **Peak crime hour**: 12 PM (noon)
- **Area with most night crimes**: Central district
- **Night hours definition**: 10 PM - 3:59 AM (22:00 - 03:59)
- **Victim age distribution**: Shows normal distribution with some outliers

## 🛠 Tools Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## 📁 Files
- `EDA_crime.ipynb` - Main analysis notebook
- `crimes.csv` - Crime dataset from Los Angeles Open Data

## 🔍 Analysis Highlights
- Extracted hour information from military time data
- Created visualizations showing crime frequency by hour
- Identified temporal and geographic crime patterns
- Analyzed victim demographics including age distribution

## 📋 Data Description
The dataset contains 185,715 crime records with the following key columns:
- `DR_NO` - Division of Records Number
- `Date Rptd` / `DATE OCC` - Date reported and occurrence date
- `TIME OCC` - Time of occurrence (24-hour military time)
- `AREA NAME` - Geographic patrol division
- `Crm Cd Desc` - Crime description
- `Vict Age` - Victim's age
- `Vict Sex` - Victim's sex (F, M, X)
- `Vict Descent` - Victim's descent/ethnicity
- `Weapon Desc` - Weapon used
- `Status Desc` - Crime status
- `LOCATION` - Street address

## 💡 Insights for Law Enforcement
This analysis provides actionable insights for optimizing:
- Patrol schedules based on hourly crime patterns
- Resource deployment to high-crime areas, particularly Central district
- Staffing during peak crime hours (around noon)
- Focus areas for crime prevention strategies

*Data Source: Modified version of Los Angeles Open Data*
