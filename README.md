## Loan Default Risk Analysis Dashboard
# Project Overview

This project focuses on analyzing borrower data to identify patterns and risk factors associated with loan defaults. The dataset contains demographic, financial, and credit-related attributes of loan applicants, enabling the exploration of relationships between borrower characteristics and repayment behavior.

The primary goal of the analysis is to support data-driven decision-making in credit risk management by identifying key indicators that influence whether a borrower is likely to default on a loan.

## Dataset Structure


## Column	Description

- LoanID Unique identifier assigned to each loan.
- LoanAmount  Total amount borrowed by the customer.
- InterestRate	Interest rate applied to the loan.
- InterestRate Group	Categorized interest rate levels (Very Low, Low, Medium, High).
- LoanTerm	Duration of the loan in months.
- LoanTerm - Year	Loan duration expressed in years.
- Loan_Date_DD_MM_YYYY	Date the loan was issued.
- Age	Age of the borrower.
- Age-group	Categorized age range of borrowers.
- MaritalStatus	Borrower’s marital status.
- Education	Highest educational qualification of the borrower.
- Income	Annual income of the borrower.
- Income Grouping	Categorized income levels used for segmentation.
- EmploymentType	Employment classification (Full-time, Part-time, Self-employed, etc.).
- MonthsEmployed	Total number of months the borrower has been employed.
- MonthsEmployed Group	Categorized employment duration groups.
- CreditScore	Numeric score indicating borrower creditworthiness.
- CreditScore Grouping	Categorized credit score ranges (Low, Medium, High).
- NumCreditLines	Total number of credit lines currently held by the borrower.
- DTIRatio	Debt-to-Income ratio representing the proportion of income used to service debt.
- DTI Group	Categorized DTI levels (Low, Medium, High risk).
- HasMortgage	Indicates whether the borrower currently has a mortgage.
- HasDependents	Indicates whether the borrower has financial dependents.
- LoanPurpose	Reason for applying for the loan (Education, Business, Home, etc.).
- HasCoSigner	Indicates if a co-signer was involved in the loan agreement.
- Default	Indicates whether the borrower defaulted on the loan (Yes/No).

## Step taken

## Understanding the Dataset:

The first step was to explore the dataset to understand what each column represents and how the data can answer business questions.

At this stage, I focused on identifying:

- The target variable: Default (whether a borrower defaulted on the loan).

Important borrower characteristics such as:

- Age

- Income

- Credit Score

- Employment duration

- Loan amount

- Interest rate

- Debt-to-Income ratio.

Understanding these variables helped define the main objective of the dashboard, which is to analyze factors that influence loan default risk.

## Data Cleaning

Before building the dashboard, the dataset needed to be cleaned to ensure the analysis would be accurate.

The main cleaning steps included:

Removing Missing or Inconsistent Values

I checked for:

1. Blank fields

2. Missing values

3. Incorrect data formats

These were corrected or standardized to ensure consistency.

Standardizing Data Formats

Some columns required formatting adjustments, such as:

Ensuring dates followed the same format

Making sure numeric columns like Income, Credit Score, and Loan Amount were correctly recognized as numbers.

Cleaning the data ensured that the analysis and calculations would be reliable.



## Creating Useful Categories 

To make the analysis easier to understand, I created grouped categories from some numerical columns using power query.

Examples include:

- Age Groups

Borrowers were grouped into categories such as:

1. Young Adult (25-34)

2. Mid-Age Adult (35-44)

3. Mature Adult (45-54)

4. Senior Adult (55-69)

5. Youth (18-24)

This helps identify which age groups are more likely to default.

- Income Groups

Income values were grouped into ranges such as:

1. Below 50k

2. Below 100k

3. Above 100k

This makes it easier to analyze how income level affects loan repayment behavior.

- Credit Score Groups

Credit scores were grouped into levels like:

1. Exreme high score (300-579)

2. High score (580-699)

3. Moderate score  (670-789)

4. Low score (790-799)

5. Very low (800-849)


This grouping helps evaluate credit risk across borrower segments.

- Debt-to-Income Ratio Groups

DTI was categorized to identify borrowers with:

1. Low debt burden

2. Moderate debt burden

3. High debt burden

This is a key indicator used by lenders to evaluate repayment capacity.

- InterestRate grouping

InterestRate was categorized into :

1. Very low rate

2. low rate

3. Medium rate

4. High Rate

5. Very high rate



## Creating Pivot Tables

After preparing the dataset, I created pivot tables to summarize the data.

Pivot tables allowed me to analyze relationships such as:

- Age group vs loan default

- Income group vs loan default

- Credit score vs loan default

- Employment duration vs loan default

Using pivot tables made it easier to calculate:

1. Total borrowers

2. Total defaulters

3. Default rate by category.

These summaries became the foundation for the dashboard visuals.

## Building Visualizations

Once the pivot tables were created, I used charts to visually present the insights.

Some of the key visuals included:

Default Rate by Age Group

This visual shows which age segment contributes the most to loan defaults.

This helps lenders understand which demographic group carries higher risk.

Default Rate by Income Level

This chart helps evaluate whether borrowers with lower income levels default more frequently.

This insight can help financial institutions adjust loan approval criteria.

Credit Score vs Default

This visual highlights the relationship between creditworthiness and loan repayment behavior.

Typically, borrowers with lower credit scores tend to have higher default rates.

Employment Stability Analysis

This visual compares months employed against default rate.

Borrowers with shorter employment history may show higher financial instability.

Debt-to-Income Analysis

This analysis identifies borrowers whose existing financial obligations may make repayment difficult.

Higher DTI levels usually correspond with greater loan risk.

## Designing the Dashboard

After building the visuals, I organized them into a single dashboard layout to make the insights easy to understand.

The dashboard was designed to allow users to quickly see:

Overall loan default patterns

Key borrower risk factors

Segments with higher default rates

This makes the dashboard useful for credit analysts, risk managers, and decision makers.


