# Excel - AI, ML, Data salaries Analysis

## Introduction:
Having access to salary and job information helps individuals, companies, policymakers, and researchers make informed decisions that contribute to the growth and success of the AI, ML, and data analysis fields.



## Purpose of the Analysis:
The purpose of this analysis is to showcase my expertise in data analytics using Excel. I will employ techniques such as Pivot Tables, Pivot Charts, hyperlinks, and VLOOKUP to analyze the data and uncover insights related to the following questions:

1. What is the average salary for AI, ML, and data analyst jobs based on employment type?
2. What is the average salary for AI, ML, and Data Analyst jobs based on experience level and employment type?
3. Which job titles have the highest and lowest average salaries?
4. What is the distribution of AI, ML, and Data Analyst jobs based on remote work ratios by year?
5. Do larger companies offer higher salaries compared to smaller companies?
6. How does the salary for AI, ML, and Data Analysts vary across countries?
7. What are the most common job titles for entry-level, mid-level, senior, and executive roles in AI, ML, and data analyst positions?
8. Is there a difference in salary for data analysts working remotely and those based in a physical office?


## Data Source and Description:
The data utilized in this analysis is available to the public and is in the public domain. I obtained the data from the following source: [AI, ML, and Data Analyst Salaries Dataset](https://www.kaggle.com/datasets/cedricaubin/ai-ml-salaries).

The data source includes a single CSV file. This file is presented in CSV format and features a single table. After converting the comma-separated text into columns, I labeled this table as "Salaries-RowData."

Furthermore, I generated a separate sheet that outlines the variables and their descriptions. I derived this information from [AI Jobs Salaries Directory](https://ai-jobs.net/salaries/download/).


## Data Cleaning and Preparation:
The dataset contains 3006 entries for data-related jobs from 2020 to 2023. 
There are 11 variables that provide information about employees'  records. The majority of these variables are categorical. However, only two variables report the numerical amount of salary.
 
 
| Variable          | Description                                                           |
|-------------------|-----------------------------------------------------------------------|
| work_year         | The year the salary was paid.                                        |
| experience_level  | The experience level in the job during the year with possible values: EN: Entry-level / Junior MI: Mid-level / Intermediate SE: Senior-level / Expert EX: Executive-level / Director |
| employment_type   | The type of employment for the role: PT: Part-time FT: Full-time CT: Contract FL: Freelance |
| job_title         | The role worked in during the year.                                  |
| salary            | The total gross salary amount paid.                                  |
| salary_currency   | The currency of the salary paid as an ISO 4217 currency code.        |
| salary_in_usd     | The salary in USD (FX rate divided by avg. USD rate for the respective year via fxdata.foorilla.com). |
| employee_residence| Employee's primary country of residence during the work year as an ISO 3166 country code. |
| remote_ratio      | The overall amount of work done remotely, with values: 0: No remote work (less than 20%) 50: Partially remote 100: Fully remote (more than 80%) |
| company_location  | The country of the employer's main office or contracting branch as an ISO 3166 country code. |
| company_size      | The average number of people that worked for the company during the year: S: less than 50 employees (small) M: 50 to 250 employees (medium) L: More than 250 employees (large) |

No missing values are present. Additionally, I identified duplicated rows. In addressing this, I chose to eliminate them. Although data could have come from various sources, I conducted this step to ensure accuracy and enhance the reliability of my analysis. This action demonstrates my skill in data cleansing methods and my dedication to providing precise analysis results. As a result, 864 rows were removed, leaving 2162 observations for analysis.

I also chose to conduct a Univariate Analysis, which involves examining the most crucial variables individually. This analysis revealed that the sample seems suitable for further examination, considering its substantial size and the relatively consistent central tendency measures.

The variable "salary" displays a positive (or right-skewed) histogram. This observation indicates that only a small number of employees earn notably higher salaries. Additionally, the relatively close proximity of the mean, median, and mode implies that the data might not be significantly impacted by extreme outliers. More details about the univariate analysis can be found in my Excel analysis file.

## Key Findings
- This data indicates that contract-based ($134,871) and full-time ($130,949) positions typically yield higher average salaries than freelance roles ($52,009) and part-time jobs ($39,535). The fewer hours worked in freelance and part-time roles compared to contract-based and full-time positions may contribute to these findings. Additionally, it's crucial to factor in other aspects such as benefits, work flexibility, and job responsibilities when assessing the overall appeal of different employment types.

- Upon analyzing the experience levels, it becomes evident that Executive-level/Director employees command the highest average salaries. Specifically, they earn an average of $416,000 in contract-based positions and $185,211 in full-time roles. However, it's important to note that there's no available data regarding Part-time and Freelance employment for this particular experience level.

- After examining job titles with at least 30 observations, it's evident that the role of "Data Science Manager" stands out with the highest average salary among the given choices, at $182,687.

- From 2021 to 2023, the remote work trend decreased from 51% to 36%. In contrast, the percentage of people working on-site increased from 20% to 61%. However, since 86% of the observations are for the years 2022 and 2023, it's crucial to separately compare these two years. The results indicate that onsite work increased from 39% to 61%, while fully remote work decreased from 56% to 36%. These findings demonstrate a consistent trend when considering the entire dataset.

- The data clearly indicates that larger companies, categorized as "M" (Medium) and "L" (Large), tend to offer higher salaries compared to smaller companies categorized as "S" (Small). The findings support the idea that there is a positive correlation between company size and salary levels.

- In terms of the country of the company's location, Portugal takes the lead with the highest average salary at $167,500, followed by the United States at $150,232, Russia at $140,333, Sweden at $130,000, and Canada at $126,448.

- The disparity in average salaries between employees who work completely remotely and those who do not work remotely is not significant (around $9,000). However, the salary of individuals who work in a hybrid manner (here 50) is exceptionally lower than the other options ($76,523). 



