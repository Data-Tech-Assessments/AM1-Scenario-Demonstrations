# Scenario 1 – Data Gathering and Validation

## Overview

You are provided with two datasets:

- `Employment by industry – men.csv`
- `Employment by industry – women.csv`

Your task is to import, validate, and combine the data into a single clean dataset ready for analysis.

---

## Tasks

### Task 1: Import the Data

- Import both CSV files using a tool of your choice (e.g. Excel, Power BI, Python, etc.)
- Review column names, formats, and structures to ensure both files are compatible

---

### Task 2: Merge Datasets

- Combine the men’s and women’s employment datasets into a single dataset
- Ensure:
  - Consistent column names
  - A new column identifying gender if not already included

---

### Task 3: Validate and Clean the Data

Check the merged dataset for:

- **Errors** — such as negative values, misspellings, or incorrect dates
- **Inconsistencies** — including differences in naming conventions across datasets
- **Duplicates** — remove any repeated rows
- **Unnecessary data** — drop any irrelevant columns or rows not needed for analysis
- **Correct data types** for each field:
  - Dates as date format
  - Employment numbers as numeric
  - Industry names as text

---

### Task 4: Standardise the Date Field

- Convert the quarter field into a full date using the last date of the quarter  
  - Example:  
    - `Jan-Mar 1995` → `31/03/1995`  
    - `Apr-Jun 2002` → `30/06/2002`

> Tip: Use lookup tables or conditional formulas to map quarter names to end-of-quarter dates

---

## Final Checks

- [ ] Datasets merged correctly  
- [ ] Data validated and cleaned  
- [ ] Date field converted to last day of quarter  
- [ ] All data types checked and corrected  
- [ ] Clean file saved as `Employment_Cleaned.xlsx` or equivalent
markdown
Copy
Edit
# Scenario 2 – Data Analysis

## Overview

Using the cleaned employment dataset, carry out detailed analysis to explore trends, gender comparisons, and future projections.

---

## Tasks

### Task 1: Sector Analysis (1997–2023)

Using filters or slicers to select the relevant time range (1997–2023), analyse:

- Employment trends in:
  - **Public sector**
  - **Private sector**
- Create tables and charts to show changes over time
- Summarise with key statistics (e.g. average, maximum, minimum employment levels)

---

### Task 2: Industry Focus – Mining, Energy, Water Supply

- Extract employment data for:
  - Mining
  - Energy
  - Water Supply sectors
- Visualise trends from 1997 to 2023 using line charts or bar charts
- Compare male vs female employment in these sectors

---

### Task 3: Gender-Based Employment Comparisons

- Compare employment trends for men and women over the full time range
- Analyse by:
  - Overall employment levels
  - Specific sectors (e.g. manufacturing, education, healthcare)
- Use:
  - Side-by-side bar charts
  - Line graphs showing growth/decline trends

---

### Task 4: Identify Trends and Patterns

- Look for any of the following:
  - Seasonal patterns
  - Sudden increases or drops (e.g. economic crises, policy changes)
  - Convergence or divergence in gender employment over time
- Summarise any observations in brief bullet points or paragraphs

---

### Task 5: Correlation Analysis

- Explore relationships between employment levels across sectors  
  - Example: Is a rise in private sector jobs related to a drop in public sector jobs?
- Use:
  - Correlation matrices
  - Scatter plots
  - Conditional formatting in Excel or statistics tools

---

### Task 6: Forecast Employment to 2028

- Use existing data trends to forecast future employment levels for the next 5 years
- Suggested tools:
  - Linear regression
  - Excel’s Forecast Sheet
  - Power BI forecasting visuals
- Forecast by:
  - Overall employment
  - Selected industries or sectors

---

## Final Checks

- [ ] Public and private sector trends visualised  
- [ ] Sector-specific charts created (Mining, Energy, Water Supply)  
- [ ] Gender comparisons analysed  
- [ ] Trends and patterns summarised  
- [ ] Correlations explored and described  
- [ ] Forecasts generated for 5 years ahead  
- [ ] Final file and visuals saved and ready for presentation
