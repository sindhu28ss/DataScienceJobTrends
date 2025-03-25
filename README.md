# Data Science Job Market: A Trend Analysis Across Related Roles

## Project Overview

This project investigates current trends in the data science job market by scraping job postings from LinkedIn and analyzing the data using Python. It focuses on roles such as Data Scientist, Data Analyst, and Machine Learning Engineer, with the goal of understanding demand patterns, salary insights, and opportunities across the United States.

By leveraging libraries like BeautifulSoup for scraping and Pandas, NumPy, Matplotlib, Seaborn, and Plotly for analysis and visualization, this project aims to deliver meaningful insights for job seekers, recent graduates, and industry professionals.

## Objectives

- **Analyze Current Trends:**  Examine job role demand, industry distribution, and geographic patterns across different states.
- **Explore Salary Trends:**  Analyze average salaries across industries for various data science roles and identify top-paying sectors and companies.
- **Target Entry-Level Insights:** Provide focused insights for graduate students by identifying companies and industries hiring for entry-level and associate positions.

## Methodology

The project follows a structured approach from data extraction to insight generation:

### Data Extraction:
- **Web Scraping:** Used `BeautifulSoup` to scrape job postings from LinkedIn.  
- **Source URL:** `https://www.linkedin.com/jobs-guest/jobs/api/seeMoreJobPostings/search?keywords={title}&location={location}&start={start}`
- Scraped job postings for roles like Data Scientist, Data Analyst, Data Engineer, Business Analyst, Machine Learning Engineer and related positions.
- Extracted key fields including Job Title, Company Name, Location, Salary ,Seniority Level and more.

### Data Preprocessing:
- Handled missing values and removed duplicate entries  
- Split location data into separate City and State columns  
- Extracted minimum and maximum values from salary range fields  
- Standardized and grouped job titles into clearly defined role categories  
- Classified industries based on U.S. Bureau of Labor Statistics (BLS) groupings  
  - 🔗 [BLS Industry Classification Reference](https://www.bls.gov/iag/tgs/iag_index_naics.htm)


### Exploratory Data Analysis (EDA): 
- **Average Salary by Job Title Category:** Highlights salary spread and outliers across roles.
- **Average Salary by Industry:** Shows which industries pay more (e.g., Media & Entertainment).
<p align="left">
  <img src="https://github.com/sindhu28ss/DataScienceJobTrends/blob/main/images/avg%20salary-title.png" width="500">
  <img src="https://github.com/sindhu28ss/DataScienceJobTrends/blob/main/images/avg%20salary-industry.png" width="500">
</p>

- **Salary Insights:** Top Companies and Industries Offering the Highest Pay
<p align="left">
  <img src="https://github.com/sindhu28ss/DataScienceJobTrends/blob/main/images/top%20companies.png" width="500">
  <img src="https://github.com/sindhu28ss/DataScienceJobTrends/blob/main/images/top%20industry.png" width="500">
</p>

- **Entry Level and Associate Roles – Deep dive:** 
<p align="left">
  <img src="https://github.com/sindhu28ss/DataScienceJobTrends/blob/main/images/entrycompanies.png" width="500">
  <img src="https://github.com/sindhu28ss/DataScienceJobTrends/blob/main/images/entry-industry.png" width="500">
</p>

## Recommendations

- **📈 In-Demand Roles:**  Data Scientist and Data Engineer roles are currently seeing the highest demand in the job market.

- **💰 Top Paying Opportunities:**  
  - **Companies:** Netflix, Databricks, Meta, Intuit, and others lead in offering competitive salaries.  
  - **Industries:** Media & Entertainment and Information Technology offer the highest compensation.

- **🎓 Entry-Level & Associate Roles:**  Graduates and early-career professionals should target sectors with abundant entry-level roles:  
  - Information Technology , Finance & Insurance, Healthcare

