# Lending Club Case Study
### Business Understanding
You work for a consumer finance company which specialises in lending various types of loans to urban customers. When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:
* If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company
* If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company

The data given below contains information about past loan applicants and whether they ‘defaulted’ or not. The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.

 In this case study, you will use EDA to understand how consumer attributes and loan attributes influence the tendency of default.

When a person applies for a loan, there are two types of decisions that could be taken by the company:

* Loan accepted: If the company approves the loan, there are 3 possible scenarios described below:
  * Fully paid: Applicant has fully paid the loan (the principal and the interest rate)
  * Current: Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.
  * Charged-off: Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan 
* Loan rejected: The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface.
- Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'. 
- If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study. In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.  The company can utilise this knowledge for its portfolio and risk assessment. 

## Conclusions

Bank should consider the below factors identified in Bivariate Analysis before approving a loan

- Loan Amount: Higher loan amounts are more likely to be charged off. This suggests that the bank may need to reassess its risk assessment strategies for larger loans.
- Interest Rate: Loans with higher interest rates have a higher chance of default. The bank should consider adjusting interest rates based on risk assessment to mitigate defaults.
- Instalment Amount: Higher instalment amounts correlate with higher default rates. The bank might want to review its loan terms and conditions to ensure borrowers can comfortably afford repayments.
- Annual Income: Borrowers with higher annual incomes tend to default less. The bank may consider setting income thresholds for loan eligibility or adjusting loan terms based on income levels.
- Debt-to-Income Ratio (DTI): Higher DTI ratios are associated with higher default rates. The bank should carefully evaluate borrowers' DTI ratios when assessing loan applications.
- Loan Term: Loans with longer terms, particularly 5-year terms, have higher default rates. The bank may need to adjust its lending criteria for longer-term loans or closely monitor these loans for potential defaults.
- Loan Grade: Higher loan grades show higher default percentages. The bank should revisit its grading system and potentially tighten lending criteria for higher grade loans
- Purpose of Loan: Loans for small businesses, renewable energy, and education have higher default rates. The bank might want to reassess its risk assessment for these specific loan purposes.
- State of Residence: Applications from certain states like TN, NV, AK, HI, and SD are riskier. The bank should consider regional economic factors and adjust its lending policies accordingly.
- Public Record Bankruptcies: Individuals with a history of bankruptcies are more likely to default. The bank should factor in past financial history when assessing loan applications and consider additional measures for applicants with bankruptcy records.



## Technologies Used
- Pandas - version 1.4.2
- Numpy - version 1.24.4
- Matplotlib - version 3.7.1
- Matplotlib-inline - version 0.1.6
- Seaborn - version 0.12.2

## Contact
Created by [@govindbanura][@gauravemani] - feel free to contact me!
