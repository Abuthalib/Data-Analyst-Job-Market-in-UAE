# UAE Data Analyst Job Market Analysis

This repository contains a dataset and Power BI analysis exploring the Data Analyst job market in the United Arab Emirates (UAE). The data was collected through web scraping and subsequently cleaned using Python in Jupyter Notebook. The analysis aims to provide insights into salary trends, skills demand, and location-based differences in the UAE's data analytics sector.

## Table of Contents

- [Data Collection](#data-collection)
- [Data Cleaning](#data-cleaning)
- [Dataset](#dataset)
- [Power BI Analysis](#power-bi-analysis)
- [Key Insights](#key-insights)

## Data Collection

The data was collected by web scraping job postings from online job portals relevant to the UAE's data analytics sector. The specific sources and scraping methodology can be found in the `web_scraping.ipynb` (or similar) Jupyter Notebook.

## Data Cleaning

The raw data obtained from web scraping was cleaned and preprocessed using Python in a Jupyter Notebook (`data_cleaning.ipynb` or similar). The cleaning process included:

- Handling missing values.
- Standardizing text data (e.g., job titles, company names).
- Parsing and cleaning the "Skills Required" column.
- Removing duplicates.
- Data type conversions.

The cleaned dataset is stored in `uae_data_analyst_jobs.csv` (or similar).

## Dataset

The cleaned dataset (`uae_data_analyst_jobs.csv` or similar) contains the following columns:

- **Title:** Job title (e.g., Data Analyst, Senior Data Scientist).
- **Company:** Name of the company posting the job.
- **Location:** City in the UAE (Abu Dhabi, Dubai).
- **MIN_Experience:** Minimum years of experience required.
- **MIN_Salary:** Minimum salary offered (in AED).
- **MAX_Salary:** Maximum salary offered (in AED).
- **Skills Required:** List of skills required for the job (comma-separated).

## Power BI Analysis

The Power BI analysis (`uae_data_analyst_jobs.pbix`) provides visualizations and insights based on the cleaned dataset. Key areas of analysis include:

- **Salary Range Analysis:**
    - Average minimum and maximum salaries.
    - Overall salary ranges and their distribution.
    - Median salary as a measure of central tendency.
- **Experience Analysis:**
    - Average minimum experience required.
    - Distribution of experience levels.
    - Most common experience levels.
- **Location Analysis:**
    - Job posting counts in Abu Dhabi vs. Dubai.
    - Average salary ranges per location.
    - Experience requirements by location.
- **Skills Analysis:**
    - Most frequently required skills.
    - Word cloud visualization of skills.
    - Association of skills with salary and job titles.
- **Comparative Analysis:**
    - Salary vs. Experience correlation.
    - Salary vs. Location comparison.
    - Job title-based salary and skill analysis.
    - Company-specific salary and skill analysis.

**Key DAX Measures and Calculated Columns:**

- `Average Minimum Salary`
- `Average Maximum Salary`
- `Salary Range` (Calculated Column)
- `Average Salary by Job Title`
- Extracted Skills Column (Using M code for specific skills)

**Power Query Transformations:**

- Splitting and cleaning the "Skills Required" column.
- Extracting specific skills to a new column.

