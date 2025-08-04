# Just Money Ltd – Data Technician Project

## Scenario

You are a **Data Technician** at *Just Money*, a UK-based financial company.  
Your line manager has asked you to complete a data analysis task involving two datasets.

You are expected to:

- Extract and merge data from multiple sources
- Remove any corrupted or incomplete records
- Format the data for presentation
- Present the data both as a table and as a visual chart

---

## Data Files

You have been provided with two CSV files:

- `Loan Data.csv` – Contains loan request information
- `Personal Data.csv` – Contains personal details of applicants

---

## Tasks

### Task 1: Merge Selected Columns

- Import the following columns from `Personal Data.csv` into `Loan Data.csv`:
  - `Gender`
  - `Married`
  - `Dependant`
  - `Education`
  - `Self-employed`
- Use a shared ID field (e.g., `Applicant_ID`) for matching
- Use `VLOOKUP` or `XLOOKUP` to join the datasets
- Save the new combined worksheet as:  
  `Loan Request Data`

> Tip: Make sure column names match exactly in spelling and capitalisation.

---

### Task 2: Format Currency Columns

- Format the following as **currency with two decimal places**:
  - `Applicant Income`
  - `Loan Amount`

Steps:

1. Select the column
2. Right-click → Format Cells
3. Choose **Currency** with **2 decimal places**

---

### Task 3: Remove Blank Records

- Identify and delete any rows that contain blank cells
- Use filters or conditional formatting in Excel to highlight blanks

> Tip: Back up your file before deleting anything.

---

### Task 4: Apply Table Formatting

- Format the table for clear presentation:
  - Bold column headers
  - Apply gridlines and borders
  - Adjust column widths as needed
  - Highlight key values or totals if relevant

---

### Task 5: Add a New Column

- Insert a new column next to `Loan Amount Term`
- Name the column: `Monthly Payment`
- Format the header (bold) and cells (currency)

---

### Task 6: Add Monthly Payment Formula

In the new `Monthly Payment` column, calculate:

=IFERROR([@LoanAmount]/[@Loan_Amount_Term], "")

yaml
Copy
Edit

> Tip: Use structured references if you're working within a formatted Excel Table.

---

### Task 7: Count Applicants by Gender

In cells outside your table (e.g., `O2` and `O3`):

O2: =COUNTIF([Gender Range], "Male")
O3: =COUNTIF([Gender Range], "Female")

yaml
Copy
Edit

Make sure spelling and capitalisation match your dataset.

---

### Task 8: Create a Chart

Create a visual chart showing total loan amounts for:

- Married Male applicants
- Married Female applicants

Steps:

1. Filter dataset: `Married = Yes`
2. Use a Pivot Table to summarise loan amounts by `Gender`
3. Insert a Bar Chart or Column Chart

---

### Task 9: Write a Summary

Below the chart, write a brief summary of what the chart shows. Example points:

- Which gender requested higher loans
- Any trends between marital status and loan amounts
- Any outliers or interesting patterns

Use a short paragraph or bullet points.

---

### Task 10: Save the Completed File

Save your final file with a clear name:

Loan_Request_Analysis_Complete.xlsx

markdown
Copy
Edit

Make sure:

- Charts are still connected to data
- Formatting is preserved
- No filters or error messages remain

---

## Final Checklist

Use this to confirm your work before submitting:

- [ ] Personal data successfully merged with loan data  
- [ ] Currency columns correctly formatted  
- [ ] Blank records removed  
- [ ] Table visually formatted  
- [ ] Monthly payment column added and calculated  
- [ ] Gender counts calculated  
- [ ] Chart created for married male/female loan amounts  
- [ ] Summary written  
- [ ] Final file saved correctly
