# Health Care Claims-Analysis

## Project Description
This project analyzes a sample of prospective May 2024 hospital claims from Stony Brook University Hospital to understand billing patterns, common clinical conditions, and payer relationships that drive revenue and compliance performance. Using three relational claims files, the work will focus on linking patient, encounter, and line-level detail to generate actionable insights for the compliance and revenue cycle teams.

The primary purpose is to profile provider billing behavior and identify trends that may affect reimbursement, denials, and regulatory risk. Findings will support operational decision-making around documentation improvement, coding accuracy, payer contracting, and workflow redesign in the hospital revenue cycle

## Data Source
The project consist of three csv files:
- Header: Contains provider information 
- Line: Contains procedure information
- Code: Contains diagnosis codes
Together it creates a relational database structure
Foreignkey: 'ProspectiveClaimId'

## How to Run
1. Clone this repository in your local machine
2. Ensure the three CSV files located in 'data' are in the same directory
3. Open Jupyter or Google Colab notebook.
4. Run all cells

## Key Findings
1. New York Spine and Brain Surgery records the most complex cases, averaging 9.23 diagnoses per claim, while SB Internists rank second with an average of 3.59 diagnoses per claim
2. Medicare is the largest payer, both by number of claims and by total charges submitted
3. The most common diagnosis code is J96.01, acute respiratory failure with hypoxia
4. Inpatient services account for 59.54% of all claims, with outpatient doctor office visits next at 34.02%
5. The most commonly billed procedure code is 99291, billing for the first 30-74 minutes of critical care services

## Required Libraries
```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```