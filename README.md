# Public Spending in New York Towns Study
##### An empirical investigation into whether local government spending across New York towns is driven more by local tax revenue or intergovernmental aid, measured across three distinct spending categories.

## Overview
##### This project examines the determinants of local government spending across 914 New York towns over a ten year period from 2013 to 2023. Using panel data from the New York State Comptroller's Office, I estimate the causal impact of federal aid, state aid, and local tax revenue on three spending outcomes — general government spending, public safety, and social services — while controlling for unobserved town and time level heterogeneity through two-way fixed effects. Results suggest that the primary driver of spending varies meaningfully across categories, with intergovernmental aid dominating general government and social services spending while local taxes are the primary driver of public safety expenditures.

## Data
### Source: 
##### Office of the New York State Comptroller, Local Government Data (Financial Data for Local Governments) [Link to Data](https://wwe1.osc.state.ny.us/localgov/findata/financial-data-for-local-governments.cfm) 
##### For definitions of certain expenditures I used the corresponding [Glossary](https://wwe2.osc.state.ny.us/transparency/LocalGov/LocalGovGlossary.cfm)
### Time Period: 
##### 2013 to 2023 (11 measured years)
### Sample Size: 
##### 9,981 observations across 914 NY Towns
### Key Variables (refer to presentation for additional descriptive examples): 
#### Town Income:
##### fed_aid - total federal aid received by town (Sanitation, Economic Development, Transportation)
##### state_aid - total state aid received by town (Education, Health, Public Safety)
##### local_taxes - total local tax revenue (Property, Sales, and Non-Property taxes)
#### **Town Expenditures**:
##### gen_gov - total expenditures on general government needs (Administration, Zoning/Planning, Operations)
##### public_safety - total expenditures on public safety services (Police, Fire, EMS)
##### social_services - total expenditures on public assistance programs (Medicaid, Financial Assistance, Youth Services)


## Methodology
### Step 1: Panel Data Construction
##### Appended annual, cross-sectional files into a single panel dataset in STATA. Panel showed each entity's (town) income and expenditure data over 11 years. Since it was only 11 files I decided to convert each .csv file to .dta files by hand, however I would create a loop if expanding this project again.
<img width="1251" height="516" alt="image" src="https://github.com/user-attachments/assets/d2e1d833-dc05-4ec7-9de6-c7689d6980ba" />

### Step 2: 




This is my first big econometrics project that I actually recorded. (https://wwe1.osc.state.ny.us/localgov/findata/financial-data-for-local-governments.cfm) was where I got my data, its the office of the state comptroller which looks at financial data for all NY town from 1995-2023. In "detailed account-level data" (Scroll down on the link) I selected "Revenue, Expenditure and Balance Sheet Data" then, "Single Class of Government for All Years" and then "Town" in the dropdown menu, after which I downloaded all of the data in a zip file.
