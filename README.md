# Data-visualization
this repository is about communicating key findings from an analysis
This project is about visualization which is a step following the data wrangling process. Before getting to the visualization the data is to be cleaned. In this project, I will make sure that the data are cleaned, tidiness and data quality will be verified, mostly for the key variables.
For this project, I suggest three main steps
step 1: review the datasets, to verify the quality of the data and the tidiness of the dataset and understand the data’s structure, oddities.
step 2: Exploratory data analysis on key variables, the exploration will focus on 15 variables. To select those 15 variables, we will create a sub datasets, the exploration will be conducted on this sub-dataset. I will use data visualization libraries to explore the dataset’s 15 variables patterns and relationships. The analysis will be structured, going from simple univariate relationships up through multivariate relationships.
step 3: I will take my main findings from the exploration step2, above, and convey them to others through an explanatory analysis. To this end, I will create a slide deck that leverages polished, explanatory visualizations to communicate my results. Two major paths in my exploration will be selected, while choosing relevant visualizations along that path, and then polishing them to construct a story for the readers to understand my findings.

Prosper Loans Data exploration¶
This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. The data set can be found from the udacity server here https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1554486256021000

Structure of my dataset¶
There are 113937 records in my dataset, with 81 features, however for the purpose of the project, I will consider 14 features : CreditGrade,LoanStatus,Borrower APR, LenderYield,ProsperRating,EmploymentStatus,ListingCategory,IsBorrowerHomeowner,CreditScorRangeLower,CreditScoreRangeUpper,AmountDelinquent,IncomeRange,LoanCurrentDaysDelinquent.
Most variables are numeric (continuous and discrete) and some are categoric.
numeric continuous variables: Borrower APR,LenderYield,CreditScorRangeLower,CreditScoreRangeUpper,AmountDelinquent, LoanOriginalAmount, LoanCurrentDaysDelinquent.
categoric variables: 1- ordinal : CreditGrade, ProsperRating, IncomeRange 2- nominal : LoanStatus, EmploymentStatus, ListingCategory, IsBorrowerHomeowner

The main feature of interest from my dataset
What factors affect a loan’s outcome status? I am looking for which features better explain loan's outcome status. In this extent, some key statistics like correlation will be useful. LoanStatus will be the dependant variable or y; such variables : CreditScoreRangeUpper,AmountDelinquent,DebtToIncomeRatio, LoanCurrentDaysDelinquant
What affects the borrower’s APR or interest rate?
Like other types of debt, the interest rates for personal loans depend on the lender, your credit scores and your credit history. An estimated range of interest rates on personal loans for consumers with fair to good credit is currently between 6% and 36%. APR, or annual percentage rate, is your interest rate stated as a yearly rate. An APR for a loan can include fees you may be charged, like origination fees. APR is important because it can give you a good idea of how much you'll pay to take out a loan
Borrower APR will be the dependant variable (y); x(CreditScorRangeLower,CreditScoreRangeUpper,CreditGrade
This rate describes how much in interest charges you will pay on the balance of your loan over a year period. The higher rate will be your APR.
An annual percentage rate (APR) is a broader measure of the cost of borrowing money than the interest rate. The APR reflects the interest rate, any points, mortgage broker fees, and other charges that you pay to get the loan. For that reason, your APR is usually higher than your interest rate.
Are there differences between loans depending on how large the original loan amount was? We will consider fondamental keys, to see how the original loan amount can affect APR for instance.
