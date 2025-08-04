# Scenario 1 – Data Gathering and Validation

## Overview

You are provided with three data files:

- `Happiness_data_2018.csv` – Happiness data for 2018
- `Happiness_data_2019.csv` – Happiness data for 2019
- `Population_data.csv` – Population by country

Each happiness file includes:

- Country name
- Happiness score
- GDP per capita
- Social support
- Healthy life expectancy
- Freedom to make life choices
- Generosity
- Perceptions of corruption

Your goal is to prepare a clean and combined dataset for analysis.

---

## Tasks

### Task 1: Import All Files

- Import all three CSV files using your preferred tool (e.g. Excel, Power BI, Python, etc.)
- Check for consistent column headers and data formats

---

### Task 2: Validate the Data

For each dataset:

- Check for:
  - Errors or typos in country names or metrics
  - Inconsistencies in column names between 2018 and 2019 files
  - Duplicates or null (missing) values

> Tip: Use sorting, filters, and data validation tools to assist in error checking.

---

### Task 3: Merge Happiness Data

- Combine `Happiness_data_2018` and `Happiness_data_2019` into one dataset
- Include a column to indicate the year for each row
- Ensure all variables are consistently named and formatted

---

### Task 4: Link Population Data

- Join the population data to the merged happiness dataset
- Use the country name as the key
- Ensure each country in the happiness dataset includes its correct population value

---

## Final Checks

- [ ] All three files imported  
- [ ] Column names standardised  
- [ ] Errors, inconsistencies, and duplicates resolved  
- [ ] Happiness data merged with year column  
- [ ] Population data successfully linked  
- [ ] Final file saved as e.g. `Happiness_Population_Combined.xlsx`
markdown
Copy
Edit
# Scenario 2 – Data Analysis

## Overview

Using the cleaned and combined dataset from Scenario 1, perform analysis to explore happiness trends and relationships with other factors.

---

## Tasks

### Task 1: Compare 2018 vs 2019 Happiness Scores

- For each country, calculate the difference in happiness score between 2018 and 2019
- Identify countries with:
  - Increased happiness
  - Decreased happiness

> Tip: Use a calculated column or a Pivot Table for year-over-year comparison

---

### Task 2: Average Happiness Rating

- Calculate the **overall average happiness score** for all countries
- Compare this average to the **United Kingdom’s** score for both years

---

### Task 3: G7 Country Comparison

- Identify the following countries:
  - Canada
  - France
  - Germany
  - Italy
  - Japan
  - United Kingdom
  - United States

- Calculate the **average happiness score** for G7 countries
- Compare with global averages

---

### Task 4: Happiness vs Population

- Create a scatter plot of:
  - Happiness score vs Population
- Check for any visible trends or correlations

> Tip: Use logarithmic scale if population sizes vary widely

---

### Task 5: Explore Other Variables

- Examine possible relationships between happiness score and:
  - GDP per capita
  - Social support
  - Healthy life expectancy
  - Freedom to make life choices
  - Generosity
  - Perceptions of corruption

Steps:

- Use correlation analysis or scatter plots
- Identify which variable(s) show the strongest relationship with happiness

---

## Final Checks

- [ ] Year-over-year comparisons complete  
- [ ] UK score compared to global average  
- [ ] G7 scores analysed  
- [ ] Population correlation visualised  
- [ ] Other variables reviewed for correlation  
- [ ] Summary of findings written  
- [ ] Final file saved and ready for submission
