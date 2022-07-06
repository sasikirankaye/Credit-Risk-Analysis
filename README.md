# Credit-Risk-Analysis

One of the leading banks would like to predict bad customer while customer applying for loan. This model also called as PD Models (Probability of Default)

Credit scoring is perhaps one of the most "classic" applications for predictive modeling, to predict whether or not credit extended to an applicant will likely result in profit or losses for the lending institution. There are many variations and complexities regarding how exactly credit is extended to individuals, businesses, and other organizations for various purposes (purchasing equipment, real estate, consumer items, and so on), and using various methods of credit (credit card, loan, delayed payment plan). But in all cases, a lender provides money to an individual or institution, and expects to be paid back in time with interest commensurate with the risk of default. Credit scoring is the set of decision models and their underlying techniques that aid lenders in the granting of consumer credit. These techniques determine who will get credit, how much credit they should get, and what operational strategies will enhance the profitability of the borrowers to the lenders. Further, they help to assess the risk in lending. Credit scoring is a dependable assessment of a person’s credit worthiness since it is based on actual data.<>

A lender commonly makes two types of decisions: first, whether to grant credit to a new applicant, and second, how to deal with existing applicants, including whether to increase their credit limits. In both cases, whatever the techniques used, it is critical that there is a large sample of previous customers with their application details, behavioral patterns, and subsequent credit history available. Most of the techniques use this sample to identify the connection between the characteristics of the consumers (annual income, age, number of years in employment with their current employer, etc.) and their subsequent history.

Typical application areas in the consumer market include: credit cards, auto loans, home mortgages, home equity loans, mail catalog orders, and a wide variety of personal loan products.

DATA AVAILABLE: Bankloans.csv The data contains the credit details about credit borrowers: Data Description:

age - Age of Customer
ed - Eductation level of customer
employ: Tenure with current employer (in years)
address: Number of years in same address
income: Customer Income
debtinc: Debt to income ratio
creddebt: Credit to Debt ratio
othdebt: Other debts
default: Customer defaulted in the past (1= defaulted, 0=Never defaulted)

Objective

To Predct whether the customer is defaulter or not

## Important insights
### Default

<img src="https://github.com/sasikirankaye/Credit-Risk-Analysis/blob/main/Images/default.png">
The default class is indicated by 1 and non-default class is indicated by 0

### Whisker_plots

<img src="https://github.com/sasikirankaye/Credit-Risk-Analysis/blob/main/Images/whiskerplot.png">
1. Age- It depicts that the customers with lower age group tends to default more than higher age group
2. Creddebt - It depicts that customers having higher creddebt tends to default more 
3. Debtinc - People with higher debt ratio tends to default more  often
4. employ - People with recently employed tends to default more than senior people

### Distribution_plots

<img src=https://github.com/sasikirankaye/Credit-Risk-Analysis/blob/main/Images/distribution_plot.png">
Above density graphs depicts that the otherdebts,credebts,ed doesnt have any considerable impact on the customer default situation in respect to the other variables

### Correlation

<img src="https://github.com/sasikirankaye/Credit-Risk-Analysis/blob/main/Images/correlation.png">
The above plot depicts that there is a strong correlation between default ~ debtinc,employ,creddebt

# Predictive Modelling results
In order to find a decent model to predict sales we performed an extensive search of various machine learning models available in Python. In the end, however, models from the sklearn package yielded the best results for this task. In particular Logistic regression(Statistical approcah).

# model_id	& AUC_Score  

### LogisticRegression	0.731 


