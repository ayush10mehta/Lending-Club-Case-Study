 # Project Name
> Lending Club Case Study


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Information

### About The Project
- A consumer finance company that specialises in providing urban customers with various forms of loans. When a company receives a loan application, it must decide whether or not to approve the loan based on the applicant's profile. The bank's decision is related with two sorts of risks:
If the applicant is likely to repay the loan, the company will lose business if the loan is not approved.
- Approving the loan may result in a financial loss for the company if the applicant is unlikely to repay the loan, i.e. if he or she is likely to default.
- The data pertains to previous loan applicants and whether or not they 'defaulted.' The goal is to find patterns that can be used to make decisions.

### Problem Statement
- This firm is the world's largest online loan marketplace, allowing personal loans, commercial loans, and medical procedure funding. Through a quick internet interface, borrowers can readily acquire cheaper interest rate loans.
- Lending to 'risky' applicants, like most other lending organisations, is the most common source of financial loss (called credit loss). The amount of money lost by the lender when a borrower refuses to pay or flees with the money owed is referred to as credit loss. In other words, defaulting borrowers do the most financial harm to lenders. - The 'defaulters' are the consumers who have been labelled as 'charged-off.' If these problematic loan applicants can be identified, the size of the loan can be reduced, reducing the amount of credit loss.
- The goal of this case study is to identify such applications using EDA. In other words, the organisation needs to know the reasons (or driver variables) that cause loan default, i.e. the variables that are significant predictors of default. This knowledge can be used to the company's portfolio and risk assessment.
- To gain a better understanding of the field, you should perform some independent study on risk analytics.

### About The Data
- The data set used is the loan.csv data set. It have 39717 rown and 111 columns. Explaining the columns which has been most used for the analysis purposes.
- loan_amnt: The listed amount of the loan applied for by the borrower. If at some point in time, the credit department reduces the loan amount, then it will be reflected in this value.

1. term: The number of payments on the loan. Values are in months and can be either 36 or 60.
2. int_rate: Interest Rate on the loan
3. installment: The monthly payment owed by the borrower if the loan originates.
4. grade: LC assigned loan grade
5. sub_grade: LC assigned loan subgrade
6. emp_length: Employment length in years. Possible values are between 0 and 10 where 0 means less than one year and 10 means ten or more years. 
7. home_ownership: The home ownership status provided by the borrower during registration. Our values are: RENT, OWN, MORTGAGE, OTHER.
8. annual_inc: The self-reported annual income provided by the borrower during registration.
9. verification_status: Indicates if income was verified by LC, not verified, or if the income source was verified
10. issue_d: The month which the loan was funded
11. loan_status: Current status of the loan
12. purpose: A category provided by the borrower for the loan request. 
13. addr_state: The state provided by the borrower in the loan application

### The Process
- ![Folw Diagram](link)


## Technologies Used
- numpy version - 1.22.3
- pandas version - 1.4.2
- matplotlib version - 3.3.2
- seaborn version - 0.11.2
- missingno version - 0.4.2
- plotly version - 5.1.0



## Conclusions
- Count of defaulters can be high for any category as the number of loan taken from any category is high which will not give us the correct information. Finding default rate is needed as analysing only the count will not give us the correct insights.
- Interest rate increases as per the grade. May be this is one of the reason for the increase in the defaulters in the grade G as the interest rate is highest for this grade 20-25%. We need to reconsider the rate of interest according to some different factors not by the grades.
- There should be through analysis of the people who are applying loans for opening small business. The background check is usually be done but we also need to do the detail analysis of the business plans which the one is asking loan for because from our analysis mostly defaulters belongs to this category and from our bivariate analysis we can clearly see that mostly high grade people apply for this type of loan so majoritly there backgroud is great but not there plans for the business which ultimatly leads to the loss.
- It should be strict to mention there employment lenght as most of the defaulters are coming from the one who haven't mentioned there employment length and also a detail background check of there employbility as there can be cases where the show fake employment.
- Either stop or be very carefull before taking any application from the state NE, it has the highest defaulters rate and all apply for only 36 months terms.
- It has been seen that loan are provided at high interests to low grade people as compared to the high grade people.
- The most number of defaulters count are from 36 months term. But the defulters are most likely to be the one from 60 months term as the average rate of defaulters is the highest for this 22%.
- The rate of defaulters for grade A has been decreased in a span from 2007 to 2011 and the number of A grade people taking loan has been increased.
- There is much more raise in defaulters for grade C & E as compared to the number of people taking loans.

### Interesting facts
- For sub grade A1 who has taken loan for 60 months terms are least likely to be defaulters with 0% defaulters.
- For sub grade G3 who has taken loan for 36 months terms are most likely to be defaulters with 100% defaulters.
- For grade G who has not mentioned there employment length are most likely to be defaulters with 100% defaulters.



## Acknowledgements
- We have taken the references of data computation methods from some of the python libraries.
1. Numpy: https://numpy.org
2. Pandas: https://pandas.pydata.org
- We have taken the references of data visualization from some of the python libraries.
1. Plotly: https://plotly.com
2. Seaborn: https://seaborn.pydata.org
3. Matplotlib: https://matplotlib.org


## Contact
Created by [@ayush10mehta] - feel free to contact me!
Created by [@abalajis] - feel free to contact me!
