# Lending Club - EDA Case Study
> Outline a brief description of your project.
The assignment is to help understand how real business problems are solved using EDA. In this case study, apart from applying the techniques learnt in EDA, the case study also helps in developing  a basic understanding of risk analytics in banking and financial services and understand how data is used to minimise the risk of losing money while lending to customers.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Lending Club company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface. 
- Background :
    When a person applies for a loan, there are two types of decisions that could be taken by the company:
        - Loan accepted: If the company approves the loan, there are 3 possible scenarios described below:
        - Fully paid: Applicant has fully paid the loan (the principal and the interest rate)
        - Current: Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.
        - Charged-off: Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan 
    Loan rejected: The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)
 
- Business Objective
     When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile.Two types of risks are associated with the bank’s decision:
    - If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company
    - If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company
    In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.  The company can utilise this knowledge for its portfolio and risk assessment, applying EDA learning to understand how consumer attributes and loan attributes influence the tendency of default.
- Data Set
    - Data File : "loan.csv"
        Data File contains the complete loan data for all loans issued through the time period 2007 t0 2011.
    - Data Dictionary : Data_Dictionary.xlsx
        Data Dictionary provides the explaination of the data columns.
    

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Data Cleaning:
    - Removal (Dropping) of Columns with all null values
    - Removal (Dropping) of Columns with only one data value.
    - Removal of Outliers
- Data Handling :
    - Creation (adding) of Derived Columns
    - Creation (adding) of Category Columns, based on the analysis of the Category and Series data columns.
    - Conversion of the Data Types
    - Creation of Dataframe for Charged Off Loans.
 - Univariate Analysis Observations / Conclusions
     The analysis of Sanctioned loans and the analysis of Charged Off Loans indicate that the applicant with following characteristics are likely to default the loan repayment.
    - Applicants reside in rental homes
    - Applicants who have mortagaged their homes
    - Applicants Applying for loan with purpose of Debt Consolidation, i.e. applicants who use the loan to clear other debts
    - Applicants who receive interest at the rate of 13-17%
    - Applicants who have an income of range 30k - 75k
    - Applicants with employement length of 10
    - When investor funding is between 5000-10000
    - Loan Funded request is between 5k - 10k
    - Dti is between 12-18
    - When monthly installments works out between 145-274
    - Applicants who avail shorter term of 36 months
    - When the loan status is Not verified and Source of Income is not verified
    - When the number of derogatory public records and bakruptcy records is 0
    - Grade is 'B' or 'C', especially with sub-grades 'B5' and 'C1'
    - Loan Applicant applying in last 3 months of the year.
    - Loan Applicant residing in California State.
 - Conclusion :
     Following are observations based on the analysis of charged off loans. The probability of defaulting is high when:
    - Applicants are availing loan for Home Improvement and have high Annual Income Range (60K - 70K)
    - Applicants with Annual Income range between 35k - 70k and availing loan for Debt Consolidation.
    - Higher Annual Income Range applicants are disbursed loans with higher interest rates.
    - Higher Loans amounts are disbursed with higher interest rates (>= 14%).
        - Note: Fully Paid Loans across all Annual Income Range, Grades are arougn 10% - 12%
    - Loan applicant with Home Ownership is Mortgage and avail higher loan amount (>=14K) with high interest rate (>14%)
    - Loan Applicants with Grade F or G, and are sanctioned higher loan amount (> 14K) with high interest rate (>14%)
        - Note: Important to take note of the Grades, as loan applicants with smaller loan amount and interest are also in these Grade but have fully paod loans. But it is likely that if same applicant requests for higher loan amount (>=14k), the loan sanctioned will be with higher interest rate (>14%)
    - Loan Applicants with Verified status and with loan sanction is >=14K
    - Loan Applicant in Grade G and high interest rate (>15%)
    - Loan Applicants with >10 years of experience and sanction higher loan amount (> 10K) with high interest rate (>14%)
    - Loan Applicants with purpose of Debt Consolidation or Small Business, and when santioned higher loan amount (>=14K) with high interest rate (>14%)
    

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Jupyter Notebook
- Python
- Libraries
    - numpy
    - Matplotlib
    - seaborn
    - plotly (tried applying - but not used)


<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- References 
    - https://campus.datacamp.com
    - https://www.wikipedia.org/
   
- This project was based on combination of the reading from various programmer friendly sites and manuals / help guide.


## Contact
Created by [@ShashankPawas] - feel free to contact me!
