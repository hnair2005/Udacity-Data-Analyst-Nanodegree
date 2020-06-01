# Prosper Loan Data Exploration

## Dataset

The dataset taken for analysis is Udacity curated Prosper loan. 
The dataset contains loan data, Borrowers credit attributes and lender data at a loan listing level.
The total number of records in the dataset is 113937 and it has 81 columns(variables). 
There is a good mix of categorical and quantitative variables. 
However there are far too many in the dataset. We will limit our focus to 10 - 15 variables.


## Summary of Findings

In the exploration, I found that there was a strong relationship between the
Borrowers APR and Lender Yield. The relationship is very strong positively correlated. 
I found that there was a strong negative correlation between Borrowers APR and Prosper Score, and Credit Score.
There was somewhat a surprising negative correlation between Borrowers APR and loan amounts.
But after plotting additional visuals it was clear that these larger loan were requested by borrowers 
who fall under higher income and higher Prosper score.

Outside of the main variables of interest, I verified the relationship between
loan status and Income range. For the dataset given, 90% of borrowers were 
current or completed their loans. Borrowers with IncomeRange greater than $25k 
and less than $50k let their loans into delinquency. Borrowers with different 
ProsperScores were normally distributed suggesting overall risk is nicely balanced out.
The distribution of the loans by state closely follows the distribution of states 
with largest population. Majority of borrowers in the dataset have an income range between $25000 - $74999.
Most loans are taken for 36 months term. 88% borrowers incomes are verifiable.
More than half of the borrowers are home owners. Another interesting relationship
observed was  that over the years loan amounts have increased while the APR's have fallen.

## Key Insights for Presentation

For the presentation, I focus on the influence of the Prosper Score & Credit Score 
on Borrowers APR and leave out most of the intermediate derivations. I start by introducing the
APR variable, followed by the correlation plot between APR and Prosper Score & Credit Score.

Afterwards, I introduce the categorical variables one by one. To start,
I use the violin and Box plots to show how APR is distributed across Prosper Scores. 
I'm only looking at Prosper Scores now as they are custom calculated by prosper to manage risk
and hence closely associated with APR of the borrower. Then I look at APR for Prosper Scores 
using time series plot to check correlation at different points in time and overall trend. 
I then use binned credit ratings explore their correlation to APR over Years.