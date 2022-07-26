# Predictive Value of Graduation Rate on Home Prices
## Potential Impact of Additional Investments in Education
King County, Washington
June 2022

## Project Overview
**Stakeholder:** Washington State Board of Education - https://www.sbe.wa.gov/our-work/education-system-health\

**Situation:** Variability in graduation rates across school districts in King County demonstrate a need for\ additional school resources to reach and engage all students.\

**Problem:** There are limited funds available to increase resources in King County.

**Objective:** The goal is to identify if an increase in property taxes can be justified by associating graduation rate with home sales price.

## The Data
### Years of Analysis
- 2014 Home Sales based on King County Dataset 
- 2014/15 Academic Year

### Graduation Rate based on
- 4 year completion of high school
- Public schools in King County

### Method of Analysis
<img width="904" alt="Screen Shot 2022-07-26 at 10 05 58 AM" src="https://user-images.githubusercontent.com/100314469/181028925-6f15161e-f4af-4825-b9e1-9563d508846a.png">

### Merged Data File
- Joined Housing and Graduation Rate data on Zip Code 
- Dataframe: df_housing_wgrade - N =21,597

## Prepare for Regression Model
### Variables selected for analysis:

**Target:** Sales Price 

**Predictors:**
- Graduation Rate
- SQFT
- Zipcode
- Grade
- Condition


**Ordinal variables ranked:**
- Grade
- Condition

**Categorical variables encoded:**
- Zipcode

**Numeric variables scaled:**
- SQFT

## Output of Model
 - The output of the model on the Train dataset showed an R squared of .86. When run on the Test dataset, the R squared was also .86.
 - Graduation rate had the largest coefficient among all of the predictive variables. 

### Subsequent iterations of the model will include:
- Running a simple linear regression with graduation rate as the only predictor
- Identify zip codes for which graduation rate has the highest interaction in terms of prediction
