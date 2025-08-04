# Scenario 1 – Data Gathering and Validation

## Overview

You are an analyst for a technology firm that sells computers and smartphones in:

- France
- United Kingdom
- China

You have been provided with the following files:

- `Jake.csv` – Sales data from France
- `Liam.csv` – Sales data from the UK
- `Nick.csv` – Sales data from China
- `Exchange Rates.csv` – Currency exchange rates into EUR

Your task is to validate and prepare this data for analysis.

---

## Tasks

### Task 1: Import All Files

- Import all four datasets using a tool of your choice (e.g. Excel, Power BI, Python, etc.)
- Review headers and formats to ensure files load correctly

---

### Task 2: Validate Data

Check each dataset for:

- Errors or typos
- Inconsistent formatting (e.g. date formats, number separators)
- Missing or null values

> Tip: Use filters, conditional formatting, and data validation tools to highlight problems.

---

### Task 3: Merge Sales Files

- Combine the `Jake.csv`, `Liam.csv`, and `Nick.csv` files into one dataset
- Ensure all columns are aligned (e.g. headers must match)
- Add a new column if needed to identify the country or representative

---

### Task 4: Add Exchange Rates

- Merge the `Exchange Rates.csv` file with the combined sales data
- Use the `Currency` field as the key to match exchange rates
- Only select rates from **December 2018**

> Tip: Use `VLOOKUP`, `XLOOKUP`, or merge functions in your analysis tool to join the data.

---

## Final Checks

- [ ] All three sales files merged into one clean dataset  
- [ ] Exchange rate data from December 2018 merged correctly  
- [ ] All formatting consistent  
- [ ] Data saved in a working file, e.g. `Combined_Sales_2018.xlsx`
markdown
Copy
Edit
# Scenario 2 – Data Analysis

## Overview

Now that the sales data and exchange rates have been combined, your task is to perform a series of calculations and produce an analysis of sales performance.

---

## Tasks

### Task 1: Calculate Unit Price in Euros

- Create a new column: `Unit Price EUR`
- Use the formula:

Unit Price EUR = Unit Price (Local Currency) / Exchange Rate

yaml
Copy
Edit

Make sure:
- Exchange rates are matched by currency
- Decimal formatting is consistent (e.g. 2 decimal places)

---

### Task 2: Calculate Revenue

- Create a new column: `Revenue`
- Use the formula:

Revenue = Unit Price EUR * Quantity

yaml
Copy
Edit

> Tip: Double-check for any null values in Quantity or Unit Price EUR

---

### Task 3: Analyse Performance

Use tables, charts, and summary statistics to identify:

- The **best performing sales representative** (based on total revenue)
- The **product that generated the most revenue**
- The **average revenue for each product**

Suggested methods:

- Pivot Tables (in Excel or Power BI)
- Bar or column charts
- Summary tables with totals and averages

---

## Final Checks

- [ ] `Unit Price EUR` calculated and formatted  
- [ ] `Revenue` column added  
- [ ] Total revenue per representative analysed  
- [ ] Top-selling product identified  
- [ ] Average revenue per product calculated  
- [ ] Visuals and summary clearly presented  
- [ ] Final file saved and ready for submission
