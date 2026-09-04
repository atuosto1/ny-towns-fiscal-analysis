# Public Spending in New York Towns Study
An empirical investigation into whether local government spending across New York towns is driven more by local tax revenue or intergovernmental aid, measured across three distinct spending categories.

## Overview
This project examines the determinants of local government spending across 914 New York towns over a ten year period from 2013 to 2023. Using panel data from the New York State Comptroller's Office, I estimate the causal impact of federal aid, state aid, and local tax revenue on three spending outcomes — general government spending, public safety, and social services — while controlling for unobserved town and time level heterogeneity through two-way fixed effects. Results suggest that the primary driver of spending varies meaningfully across categories, with intergovernmental aid dominating general government and social services spending while local taxes are the primary driver of public safety expenditures.

## Data
### Source: 
Office of the New York State Comptroller, Local Government Data (Financial Data for Local Governments) [Link to Data](https://wwe1.osc.state.ny.us/localgov/findata/financial-data-for-local-governments.cfm) 
For definitions of certain expenditures I used the corresponding [Glossary](https://wwe2.osc.state.ny.us/transparency/LocalGov/LocalGovGlossary.cfm)
### Time Period: 
2013 to 2023 (11 measured years)
### Sample Size: 
9,981 observations across 914 NY Towns
### Key Variables (refer to presentation for additional descriptive examples): 
#### Town Income:
**fed_aid -** total federal aid received by town (Sanitation, Economic Development, Transportation)
**state_aid -** total state aid received by town (Education, Health, Public Safety)
**local_taxes -** total local tax revenue (Property, Sales, and Non-Property taxes)
#### **Town Expenditures**:
##### gen_gov - total expenditures on general government needs (Administration, Zoning/Planning, Operations)
##### public_safety - total expenditures on public safety services (Police, Fire, EMS)
##### social_services - total expenditures on public assistance programs (Medicaid, Financial Assistance, Youth Services)


## Methodology
### Step 1: Panel Data Construction
##### Appended annual, cross-sectional files into a single panel dataset in STATA. Panel showed each entity's (town) income and expenditure data over 11 years. Since it was only 11 files I decided to convert each .csv file to .dta files by hand, however I would create a loop if expanding this project again.
<img width="1059" height="573" alt="image" src="https://github.com/user-attachments/assets/d6bd2d46-e134-4098-8648-1e8ef6509363" />

### Step 2: Encoding Variables
Explain here
<img width="1059" height="573" alt="image" src="https://github.com/user-attachments/assets/d070e96a-0067-416b-8a73-2110b75fd600" />
<img width="1059" height="285" alt="image" src="https://github.com/user-attachments/assets/02453c6c-314f-45b3-adb5-884e4f3b654b" />

### Step 3: Collapse/Reshape Data
Explain
<img width="1059" height="227" alt="image" src="https://github.com/user-attachments/assets/8e38dead-4dfd-4d70-b6b0-844adf34e186" />

### Step 4: Create Necessary Variables & Declare Panel
Explain
<img width="1059" height="358" alt="image" src="https://github.com/user-attachments/assets/45817ad7-6ae9-4042-8ed5-00966534332c" />

### Step 5: Random Effects Regression
Explain

### Step 6: Fixed Effects without and with cluster Standard Errors
Explain

### Step 7: Remaining Regressions
Explain

### Step 8: Graphs
Explain


## Findings
##### Explain here

## How to Reproduce
### REQUIREMENTS:
##### Stata requirements

## Planned Extensions
##### Explain

This project was conducted as a final for ECO 385 at Pace University (Dyson College of Arts and Sciences). Data sourced from the Office of the New York State Comptroller Local Government Bulk Data portal.



This is my first big econometrics project that I actually recorded. (https://wwe1.osc.state.ny.us/localgov/findata/financial-data-for-local-governments.cfm) was where I got my data, its the office of the state comptroller which looks at financial data for all NY town from 1995-2023. In "detailed account-level data" (Scroll down on the link) I selected "Revenue, Expenditure and Balance Sheet Data" then, "Single Class of Government for All Years" and then "Town" in the dropdown menu, after which I downloaded all of the data in a zip file.
