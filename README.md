# Loan Data from Prosper Dataset Exploration
## by Isaac Mwendwa


# Loan Data from Prosper Dataset Exploration
## by Isaac Mwendwa


## Dataset

* The Loan Data from Prosper Dataset is a dataset of loans taken between 2005 and 2013 from Prosper
* The dataset contains 113,937 rows (loans) with 81 columns (loan variables) on each row
* The loan variables consist of qualitative (ordinal and nominal) and quantitative features
* In this exploratory analysis, we will be seeking to find insights on the relationships between the various loan variables e.g. 
> * Borrower's APR, Prosper Score, Income Range, Debt to Income Ratio, Employment Status, Stated Monthly Income, Loan Year, and Employment Duration

The main features of interest (response variables) in the dataset include:
> * Borrower's APR
> * Prosper Score
> * Debt to Income Ratio 

The variables that will support the investigation of the variables of interest are known as predictor features. The following predictor feautures will be used in the exploration:
> * Income Range
> * Employment Status
> * Stated Monthly Income
> * Loan Year
> * Employment Duration 



## Summary of Findings

### Findings from Univariate Exploration

Borrower APR
* The distribution of Borrower APR is largely multimodal, with small peaks around 0.1 and 0.3. There is a large peak around 0.2
* The unusual points noted in the Borrower APR are the big steep peak around 0.35

Loan Original Amounts
* The distribution of Loan Original Amounts is multimodal, with big peaks at around USD 5000, USD 10000, and USD 15000
* The distribution is also right skewed, with the majority of the Loan Original Amounts being lower than USD 30,000

Income Range
* Majority of the borrowers have an Income Range of USD 25k - 50k and USD 50k - 75k (Middle Class). This implies that Middle Class group are the greatest loan takers
* The least of the borrowers are in the group of USD 1 - 25k, "Not Employed", and USD 0
* This implies that the Unemployed and Low Income earners are at a lesser chance of being given loans; as compared to the Middle Class earner's

Employment Status
* The majority of the Borrowers have an Employment Status of "Employed"
* Conversely, the least proportion of Borrowers are in the "Other",, "Part-time", "Not employed", and "Retired" employment statuses
* This implies that lenders are more likely to give loans to employed persons, due to the security associated with employment 

Debt to Income Ratio
* The histogram is skewed right, implying that the majority of the debt to income ratios lay between 0 and 0.4
* This implies that lenders pay keen attention to ensure a borrower can service the loan, by ensuring that their debt-to-income ratio is low

Loan Year
* There is a tremendous increase in the number of loans originated from 2013,as compared to other years
* This can be attributed to the low interest rates imposed in that year; as compared to other years. Hence, the favourable interest rates spurred extensive borrowing
* Reference: [U.S. regional banks see loan growth in 2013](https://www.reuters.com/article/us-pncfinancial-results-idUSBRE90G0LD20130117)

The unusual distributions I noted include:
* There is a small irrecognizable difference between distributions of loan takers who are home-owners and those who are not. 
> This is contrary to the fact that home-owners are more likely to be given loans as compared to those who are not; as there is more security assured with the lending

* There is also a great discrepancy between the distributions of Stated Monthly Income and Income Range. 
* Majority of the borrowers have an Income Range of USD 25k - 50k; while majority of borrowers have a Stated Monthly Income of below USD 20k. 
* The two variables are closely related, hence their distributions should not be counter-intuitive


### Findings from Bivariate Exploration

Borrower APR vs. Loan Original Amount
* There is a weak negative correlation (-0.323) between the Loan Original Amount and the Borrower APR
* This implies that the more the loan amount borrowed, the lower the APR (interest) charged for the loan


Borrower APR vs. Employment Status
* Borrowers who have "Not Employed" and "Other" as their Employment Statuses have the highest Borrower APR's. 
* This can be attributed to the increased risk of lending such people money; which has to be countered by increasing the APR

Debt to Income Ratio vs. Stated Monthly Income
* There is a weak negative correlation (-0.164) between Stated Monthly Income and Debt to Income Ratio
* This implies that as the Stated Monthly Income increases, then the Debt to Income Ratio reduces

Loan Original Amount vs. Is Home-owners:
* People who are home-owners are able to borrow more; as compared to people who are not home-owners. 
* This can be explained in part by the security associated with having a home; which can be used as collateral in the loan

Loan Original Amount vs. Income Range: 
* There is a positive relationship between the Income Range and the Loan Original Amount.
* This implies that the more you earn, the more you can borrow


### Findings from Multivariate Exploration

Borrower APR vs. Loan Term and Prosper Rating (numeric)
* There is an inverse relationship between Borrower APR; and Term and Prosper Rating (numeric). Thus, Borrower APR decreases as the Loan Term and Prosper Rating (numeric) increase

Loan Original Amount vs. Loan Term and Prosper Rating (numeric)
* The Loan Original Amount; and Prosper Rating (numeric) and Term share a positive relationship. Hence, the Loan Original Amount increases as the Prosper Rating (numeric) increases, and also as the Loan Term increases 

Prosper Rating vs. Borrower APR and Loan Original Amount
* The plots show that the Loan Original Amount increase with an increase in the Prosper Rating (numeric) and a decrease in Borrower APR
* However, there is an interesting and surprising observation from the three features
* When the Prosper Rating (numeric) is above 6 (top ratings) and the Loan Original Amount increases; there is an abnormal behaviour of the Borrower APR increasing
* This can be explained in part by the propensity of people with better Prosper Ratings borrowing; which creates a high demand for the loans; and a corresponding increase in Borrower APR
* The anomalous observation can be attributed to the maximizing on loan profits by the lenders, going by the Law of Supply and Demand


## Key Insights for Presentation

> Select one or two main threads from your exploration to polish up for your presentation. Note any changes in design from your exploration step here.

> 
