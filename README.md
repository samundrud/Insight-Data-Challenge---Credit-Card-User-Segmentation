# Credit Card User Segmentation
___Insight Data Challenge___

This data challange was completed as part of the Insight Data Science Fellowship program (New York, YN, Summer 2020) by Sarah Amundrud.



# Table of Contents
1. [Problem](README.md#introduction)
2. [Data](README.md#data)
3. [Approach](README.md#approach)
4. [Outcome](README.md#outcome)
 
 
 
# Problem
You work as a data scientist at a credit card company. A senior VP is leading an effort to reduce costs associated with signup incentives by offering credit cards with carefully targeted benefits that will attract new cardholders. As a first step, she would like you to examine cardholder data collected over the last 6 months in order to understand the various kinds of users who use the company’s products. Sh/e is especially interested in getting an idea of which benefits to associate with each new card offering.


# Data

The Data The data consists of a csv file with 8950 rows (one for each cardholder) organized in columns with descriptive headers. Key to column labels:

    CUST_ID : Credit card holder ID
    BALANCE : Monthly average balance (based on daily balance averages)
    BALANCE_FREQUENCY : Ratio of last 12 months with balance
    PURCHASES : Total purchase amount spent during last 12 months
    ONEOFF_PURCHASES : Total amount of one-off purchases
    INSTALLMENTS_PURCHASES : Total amount of installment purchases
    CASH_ADVANCE : Total cash-advance amount
    PURCHASES_ FREQUENCY : Frequency of purchases (percentage of months with at least one purchase)
    ONEOFF_PURCHASES_FREQUENCY : Frequency of one-off-purchases
    PURCHASES_INSTALLMENTS_FREQUENCY : Frequency of installment purchases
    CASHADVANCE FREQUENCY : Cash-Advance frequency
    CASH_ADVANCE_TRX : Average amount of Cash-Advance transaction
    PURCHASES_TRX : Average amount per purchase transaction
    CREDIT_LIMIT : Credit limit
    PAYMENTS : Total payments (due amount paid by the customer to decrease their statement balance) in the period
    MINIMUM_PAYMENTS: Minimum payment required on statement (average?)
    PRC_FULL_PAYMENT: percent full payment (percent of balance they pay off each months?)
    TENURE: months (in the last year) they have been with company


 
# Approach

K Means Clustering




# Outcome

Business Insights
Description of customer type and targeted recommendations

Cluster 0: Credit Card Debtsters (24% of users)
    keep high balance
    only make minimum payments
Targeted Benefits to new customers:
    offer balance transfers with low introductory rates

Cluster 1: Installment Spenders (11% of users)
    high spenders
    use card primarily on recurrend installments (e.g., bills)
Targeted Benefits to new customers:
    offer recurrent bill payment incentives for the first year (e.g., points, travel, cash back, etc.)

Cluster 2: Credit Card Collectors (32% of customer base)
    they have a huge credit limit
    do not tend to use their card much, and always pay off their bill right away
    they likely use it as a back up card
Targeted Benefits to new customers:
    we don't want attrackt more of this type of customer, because they don't make us any money

Cluster 3: Shoppers (13% of customer base)
    high spenders (mostly on one-off purchases)
    low credit limit
Targeted Benefits to new customers:
    offer purchase incentives for the first year (e.g., points, travel, cash back, etc.)

Cluster 4: Cash Grabbers (23% of customer base)
    use card primarily for cash advances and not to make purchases
    low credit limit
Targeted Benefits to new customers:
    offer low introductory cash advance fee for the first yea


