# Tate Museum Collection Analysis: Cultural Diversity & Historical Trends

## 📌 Project Overview
This project performs an Exploratory Data Analysis (EDA) on the official, open-source metadata collection from the **Tate Art Museum in London**. Transitioning from a Public Administration background, I utilized Python and Pandas to evaluate structural diversity, geographic representation, and historical tracking within the museum's registry.

## 🛠️ Tech Stack & Skills Demonstrated
- **Language:** Python
- **Libraries:** Pandas
- **Key Concepts:** Exploratory Data Analysis (EDA), Data Cleaning, Handling Missing Values (`NaN`), Data Storytelling

## 📊 Core Insights Uncovered

### 1. Geographic & Cultural Representation
- **The Indian Context:** Out of **3,532 total artists** recorded in the museum's database, only **2 artists** are from India. This highlights a significant historical and structural skew in collection diversity, presenting a clear case study for institutional representation.

### 2. Historical Baselines
- **The Collection Origin:** By cleaning and standardizing historical date strings using `pd.to_numeric()`, the absolute oldest recorded artist in the dataset was identified as **Hans Holbein, the Younger**, born in **1497** (Augsburg, Deutschland).

### 3. Institutional Gender Demographics
- **Male Artists:** 2,895
- **Female Artists:** 521

## 🧼 Data Cleaning Approach
Historical cultural datasets are notoriously incomplete. In this analysis, the `yearOfBirth` column contained non-numeric strings and missing entries. 
- Utilized `pd.to_numeric(..., errors='coerce')` to safely transform valid historical years into integers while handling missing values without breaking the execution pipeline.

## 📊 Key Insights & Geographic Distribution

Using Matplotlib to plot the top artist birthplaces revealed strong institutional biases and archival quirks:

* **Imperial Center Dominance:** London, United Kingdom is the overwhelming primary source of artists in the collection, exceeding 400 entries. 
* **Global Art Hubs:** Paris, France (No. 2) and New York, United States (No. 4) are the prominent international cities breaking into the top five, reflecting historic transatlantic art trade routes.
* **Granularity Inconsistency:** The dataset contains structural inconsistencies, treating specific municipal data (e.g., *Manchester*) interchangeably with broad regional data (e.g., *England, United Kingdom*).
