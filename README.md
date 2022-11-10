# Expert Based Credit Scoring Model

*Karimi Gitari (November 2022)*


## Overview

Starting a digital lending company requires an expert scoring model before getting actual costomer data that is used to tune the expert model or phase it out and build a databased model. An expert based model is very risky and should be focused on lending the minimum amount posible as a means of buying actual customer data. Subsequent loan amounts an be gradually increased depending on customer repayment behavior. From the total funding available , the lender is advised to determine the amount they are willing to spend on buying customer data , establish a maximum amount they are willing to lend to each customer and tune the expert model so that it approves a maximum of 30% of that amount to the best customer scored. 10% of default should be assumed and planned for.

## Data Sources
* Customer Application Forms
* Financial Information from Telco's/ Banks
* Credit Reference Bureau 

## Data Points / Variables
* Customer Application Forms
  * Employment Status
  * Level of Education
  * Number of Dependants
 
It is important to collect as much customer demographic information as posible (gender , age , marital status , location...etc). While these variables aren't used during expert scoring , they will be correlated with loan repayments and help build the databased subsequent model 

* Financial Information - M-Pesa Statement Used
  *  Total Number of Loans - Count of all loans paid in
  *  Average Monthly Installment Loaned - Total paid in loan amounts/No. of months
  *  Average Monthyly installment-Repaid - Total withdrawn loan amounts/No. of months
  *  Average Monthly  Savings - Total withdrawn to saccos and banks/No. of months
  *  Average Monthly Electricity Bill - Total withdrawn to KPLC/No. of months
  *  Average amount spent on transport Monthly - Total withdrawn to taxi apps / No.of months
  *  Average bank credits Monthly - Total Paid in from bank accounts(B2C)/No. of months
  *  Average amount spent on betting Monthly - Total withdtraw to betting sites/No. of months
  *  Average Monthly Expenditure - Total Paid Out(Lipa na M-Pesa(Paybill+Buy goods))/No. of Months
  *  Average expenditure on Airtime - Total withdrawn for airtime/No. of month

This data could be extracted manually which is time consuming or automated using python or other programming languages (in this case the mpesa statement is uploaded and autoprocessed) 
  
  




