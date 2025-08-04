# Scenario 1 – Data Gathering and Validation

## Overview

You are provided with a Titanic dataset that includes:

- A **Comments** tab explaining column names
- A **Passengers** tab with the data itself

Your task is to import, validate, and clean the data to prepare it for analysis.

---

## Tasks

### Task 1: Import the Data

- Import the **Passengers** tab using your preferred tool (e.g. Excel, Power BI, Python, etc.)
- Review the **Comments** tab to understand the data structure and column meanings

---

### Task 2: Validate the Data

Check for:

- Errors (e.g. negative ages, typos)
- Inconsistencies in formats or values
- Incorrect data types (e.g. text in numeric fields)

> Tip: Use filters, sorting, and data profiling tools to identify issues.

---

### Task 3: Clean the Dataset

Make the following changes:

1. **Rename Columns**:
   - Rename `Sex` to `Gender`
   - Rename `Pclass` to `Passenger Class`

2. **Split Name Column**:
   - Extract `Title`, `First names`, and `Last names` from the `Name` column
   - Example: `Mr. John Smith` → `Title = Mr.`, `First names = John`, `Last names = Smith`

3. **Create Survival Column**:
   - Add a new column called `Survival`
   - Use logic:
     - If `Survived = 1`, then `Survival = Survived`
     - If `Survived = 0`, then `Survival = Died`

4. **Add Family Size Column**:
   - Use formula:
     ```
     Family Size = SibSp + Parch + 1
     ```

5. **Replace Embarked Values**:
   - Replace:
     - `S` with `Southampton`
     - `C` with `Cherbourg`
     - `Q` with `Queenstown`

6. **Remove Unused Columns**:
   - Delete the following:
     - `Ticket`
     - `Cabin`

7. **Remove Rows with Null Values**:
   - Drop any rows containing missing values in any column

---

## Final Checks

- [ ] Columns renamed correctly  
- [ ] Name column split accurately  
- [ ] Survival and Family Size columns added  
- [ ] Embarked codes replaced  
- [ ] Unused columns removed  
- [ ] All null rows removed  
- [ ] File saved, e.g. `Titanic_Cleaned.xlsx`
markdown
Copy
Edit
# Scenario 2 – Data Analysis

## Overview

Now that the Titanic dataset has been cleaned, perform the following analysis to explore patterns and insights, especially related to survival.

---

## Tasks

### Task 1: General Statistics

1. **Average Age**:
   - Calculate the average age of all passengers

2. **Highest Fare**:
   - Identify the passengers who paid the highest fare

3. **Embarkation Percentages**:
   - Calculate the percentage of passengers who embarked from:
     - Southampton
     - Cherbourg
     - Queenstown

---

### Task 2: Explore Patterns in Survival

Use charts, tables, or summary statistics to explore the relationship between survival and:

1. **Family Size**:
   - Compare survival rates across different family sizes
   - Use bar charts or grouped statistics

2. **Passenger Class**:
   - Compare survival by `Passenger Class` (1st, 2nd, 3rd)
   - Consider stacked bar charts or pivot tables

3. **Gender**:
   - Compare survival rates for male and female passengers

4. **Age**:
   - Create age groups or use a histogram to compare age vs. survival
   - Look for trends (e.g. were children more likely to survive?)

---

## Final Checks

- [ ] Average age calculated  
- [ ] Highest fare payers identified  
- [ ] Embarkation percentages calculated  
- [ ] Survival analysed by family size  
- [ ] Survival analysed by passenger class  
- [ ] Survival analysed by gender  
- [ ] Survival analysed by age  
- [ ] Charts/tables created and clearly labelled  
- [ ] Insights summarised in brief comments or bullet points
