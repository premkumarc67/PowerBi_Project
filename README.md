# 📊 Data Professional Survey Analysis

<img width="1419" height="795" alt="image" src="https://github.com/user-attachments/assets/5dd157a0-6b90-4e1d-88a1-d923383b217d" />

## 📖 Project Overview
This project analyzes a dataset of over 600 data professionals to identify trends in salaries, job satisfaction, work-life balance, and programming language preferences. Using **Power BI**, I transformed raw survey data into an interactive dashboard that provides a snapshot of the current data job market.

## 📂 Dataset
The dataset consists of survey responses from professionals in the data industry.
* **Format:** CSV
* **Key Attributes:** Job Title, Salary Estimates, Programming Language, Satisfaction Ratings, and Demographics.

## ⚙️ Data Cleaning & Transformation (ETL)
The raw data required significant cleaning in **Power Query Editor** before visualization. Key steps included:

1.  **Column Standardization:** Renamed complex survey questions (e.g., *"Q1 - Which Title Best Fits your Current Role?"*) to clean headers like `Job Title`, `Salary`, and `Industry`.
2.  **Salary Parsing:** The raw salary data was in ranges (e.g., *"106k-125k"*).
    * Removed non-numeric characters (Isolating specific text).
    * Split the column by delimiters to separate the lower and upper bounds.
    * Created a custom column to calculate the **Average Salary** for each respondent to enable aggregation.
3.  **Data Type Validation:** Ensured all numerical columns (Age, Salary) and text columns were correctly formatted.
4.  **Handling Duplicates & Nulls:** Filtered out incomplete responses and standardized "Other" categories for cleaner visuals.
5.  **Grouping:** Created age groups or other categorical bins where necessary for better segmentation.

## 💡 Key Insights

Based on the dashboard analysis, here are the major findings:

* **Python is King:** Python is the most popular programming language among data professionals, vastly outperforming R and other languages.
* **Salary Expectations:** The average salary across the surveyed dataset is approximately **$54,000** (global average), with significant variation based on role and location.
* **Demographics:** The average age of the data professional in this survey is **29.9 years old**, indicating a relatively young workforce.
* **Work-Life Balance vs. Salary:**
    * Respondents generally rated **Work/Life Balance (5.74/10)** higher than their **Salary Satisfaction (4.27/10)**.
    * This suggests that while professionals enjoy the flexibility of the field, many feel undercompensated relative to market rates.
* **Ease of Entry:** A large portion of respondents rated breaking into the data field as "Neither easy nor difficult" to "Difficult," highlighting a moderate barrier to entry for newcomers.
* **Geographic Distribution:** The majority of survey takers originated from the **United States**, followed by India, the UK, and Canada.

## 📊 Dashboard Features
The Power BI report includes:
* **KPI Cards:** Displaying total survey takers, average age, and average salary.
* **Treemap:** Visualizing the country of origin distribution.
* **Bar Charts:** Comparing average salary by job title and favorite programming languages.
* **Donut Chart:** Illustrating the perceived difficulty of breaking into the data field.
* **Gauges:** Visualizing average satisfaction ratings for Salary and Work/Life balance.

## 🛠️ Technology Stack
* **Microsoft Power BI Desktop:** For Data Cleaning (Power Query), Data Modeling, and Visualization.
* **Microsoft Excel:** Initial data inspection.

## 🚀 How to Use
1.  Download the `.pbix` file from this repository.
2.  Open the file in **Power BI Desktop**.
3.  Interact with the slicers to filter data by Job Title or Region.

---
*Created by Prem*
