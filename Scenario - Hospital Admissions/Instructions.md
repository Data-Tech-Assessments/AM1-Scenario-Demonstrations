# Scenario 1 – Data Gathering and Validation

## Overview

You are provided with two files:

- `Admissions.csv` – Contains patient admission data  
- `Hospitals.csv` – Contains hospital reference information

Your task is to import, validate, clean, and merge the datasets, and then classify BMI for each patient.

---

## Tasks

### Task 1: Import the Datasets

- Import `Admissions.csv` and `Hospitals.csv` using your preferred tool (e.g. Excel, Power BI, Python, etc.)
- Inspect the structure of both files to ensure they load correctly

---

### Task 2: Identify and Correct Issues

Check both datasets for:

- Data entry **errors** (e.g. typos, impossible values)
- **Inconsistencies** in column formats or naming
- **Missing or null values**
- Specific issues in:
  - `lengthofstay`
  - `pulse`

> Tip: Use filters, conditional formatting, or validation rules to highlight and correct these values.

---

### Task 3: Merge the Datasets

- Join `Admissions.csv` with `Hospitals.csv` using a common identifier (e.g. `Hospital_ID`)
- Make sure each admission now includes the correct `Hospital Name`
- Validate that all admissions are matched correctly

---

### Task 4: Classify BMI

Add a new column to classify BMI into the following categories:

| BMI Range           | Category         |
|---------------------|------------------|
| Less than 18.5      | Underweight      |
| 18.5 to 24.9        | Healthy weight   |
| 25 to 29.9          | Overweight       |
| 30 to 39.9          | Obese            |
| 40 or above         | Severely obese   |

Example formula in Excel (using nested `IF` statements):

=IF(BMI<18.5,"Underweight",IF(BMI<=24.9,"Healthy weight",IF(BMI<=29.9,"Overweight",IF(BMI<=39.9,"Obese","Severely obese"))))

yaml
Copy
Edit

> Tip: Use consistent BMI formatting (e.g. numeric, 1 decimal place) before applying the logic.

---

## Final Checks

- [ ] All errors in `lengthofstay` and `pulse` corrected  
- [ ] All columns checked for inconsistencies  
- [ ] Datasets merged correctly  
- [ ] BMI classification column added and verified  
- [ ] File saved with clear name, e.g. `Admissions_Cleaned.xlsx`

---
# Scenario 2 – Data Analysis

## Overview

Using the cleaned and combined dataset from Scenario 1, explore how **length of stay** varies across different factors.

---

## Analysis Tasks

### Task 1: Compare Length of Stay by Hospital

- Group data by `Hospital Name`
- Calculate average, minimum, and maximum `lengthofstay` for each hospital
- Display results in:
  - A summary table
  - A bar chart for easy comparison

---

### Task 2: Compare Length of Stay by BMI Category

- Use the BMI classification column from Scenario 1
- Calculate average `lengthofstay` for each BMI group
- Present data using:
  - A table
  - A bar or column chart

---

### Task 3: Compare Length of Stay by Gender

- Group patients by `Gender`
- Calculate and display average `lengthofstay` per gender
- Optionally break this down further by BMI or Hospital

---

### Task 4: Analyse Other Variables

Check for any relationships between `lengthofstay` and other numerical fields, such as:

- `Pulse`
- `Temperature`
- `Age` (if available)

Use:

- Correlation coefficients (if using software like Excel or Python)
- Scatter plots
- Trend lines

---

### Task 5: Summary and Presentation

Create a short summary of findings, including:

- Key insights and trends
- Any outliers or surprising patterns
- Possible explanations or next steps

Use a mix of:

- Tables
- Charts (bar, column, scatter)
- Bullet points or brief paragraphs

---

## Final Checks

- [ ] Length of stay analysed across hospital, BMI, and gender  
- [ ] Other numerical variables explored  
- [ ] Charts and tables created  
- [ ] Clear summary written  
- [ ] Final file saved and ready for submission
