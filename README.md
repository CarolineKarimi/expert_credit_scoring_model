# Expert Based Credit Scoring Model

*Karimi Gitari (November 2022)*


## Overview

Starting a digital lending company requires an expert scoring model before getting actual costomer data that is used to tune the expert model or phase it out and build a databased model. An expert based model is very risky and should be focused on lending the minimum amount posible as a means of buying actual customer data. Subsequent loan amounts an be gradually increased depending on customer repayment behavior. From the total funding available , the lender is advised to determine the amount they are willing to spend on buying customer data , establish a maximum amount they are willing to lend to each customer and tune the expert model so that it approves a maximum of 30% of that amount to the best customer scored. 10% of default should be assumed and planned for.

## Data Sources
* Customer Application Forms
* Telco's/ Banks
* Credit Reference Bureau 

## Data Points / Variables
* Customer Application Forms
  * Employment Status
  * Level of Education
  * Number of Dependants
 
It is important to collect as much customer demographic information as posible (gender , age , marital status , location...etc). While these variables aren't used during expert scoring , they will be correlated with loan repayments and help build the databased subsequent model 

* Telco - Mpesa Statement
  *  Monthly Disposable Income
  *  Average number of monthly loans
  *  Average monthly airtime expenditure
  *  Average monthly utility expenditure
  *  Average monthly betting expenditure
  *  Average monthly transport expenditure
  *  Average monthly salary amount paid in
  *  Average estimated monthly income
  *  share of total loan amount borrowed that is repaid
  *  Total numer of defaults
  *  Total amount of default penalties paid
  *  Average loan amount borrowed

This data could be extracted manually which is time consuming or automated using python or other programming languages (in this case the mpesa statement is uploaded and autoprocessed) 

* Credit Reference bureau data
  * CRB Score
  * Open Loan Contracts-Number
  * Estimated total borrowing per lender 
  * Open loan contracts-Average Installment amount value
  * Overdue balance sum (open loan contracts)
  * Max. no. of overdue installments last 12 months(open loan contracts)
  * Average amount borrowed monthly (closed),0 Arrears
  * Worst current Arrears
  * Worst arrears last 12 months
  * No. of enquiries, last 12 months
  * Monthly demonstrated affordability

## Credit Scoring 
* Variable Weighting - Some variables and datapoints are more important than others hence different weights need to be assigned. For example the CRB score could be assigned more weight compared to othe variables from credit reference bureau
* Variable Rating - One a scale of say 1-5 , rate each value or range of values in each variablle
* Total Client Score - The total client score is the sum of Variable Rating multiplied by their assigned weights
* Score Card - For each range of client score , there is an expert assigned  Client Grade , Probability of Default and Apporved Amount
* Total Amount to Disburse to Client - Using the predetermined interest rates and one-time fees , total fees to be accrued is determined and amount approved less the fees is disbursed to the client

  
  
  
  




