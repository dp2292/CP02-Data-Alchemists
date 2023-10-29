# CP-02 Data Alchemist
## Dataset - [Credit Risk Analysis](https://www.kaggle.com/datasets/rameshmehta/credit-risk-analysis)
## Team Id - 23
### Team Members:
| Name              | Student ID   | Contribution |
| ----------------- | ------------ | ------------ |
| [Prarthee Desai](https://github.com/Prarthee-Desai)   | [202001257](mailto:202001257@daiict.ac.in)    | EDA |
| [Devansh Patel](https://github.com/dp2292)     | [202001262](mailto:202001262@daiict.ac.in)    | Models for Term classification(Excl. SVC) |
| [Dhruv Patel](https://github.com/Dhruv0348)       | [202001271](mailto:202001271@daiict.ac.in)    | Models for Interest rate range Classification(Excl. SVC) and Default Prediction |
| [Krish Patel](https://github.com/KrishPatel452)       | [202001452](mailto:202001452@daiict.ac.in)    | SVC Models(Term classification, Default Prediction) and Documentation        |
| [Jaykumar Navadiya](https://github.com/jaynavadiya) | [202001465](mailto:202001465@daiict.ac.in)    | Early Research |

## Project Overview
The Credit Risk Analysis project is a comprehensive endeavor designed to harness the power of data-driven decision-making in the field of financial lending. At its core, the project aims to develop a sophisticated machine learning solution for the evaluation of credit risk, focusing on loan applicants and their creditworthiness. This initiative is founded on the utilization of the "Credit Risk Analysis" dataset, a rich source of information encompassing a wide range of attributes, such as personal and financial data, credit histories, employment records, and loan outcomes.

One of the primary objectives of this project is to empower lending institutions with predictive models that facilitate more precise loan approval or rejection decisions. By leveraging the dataset, we can optimize the lending process, mitigate the risk of loan defaults, and enhance the allocation of financial resources. Furthermore, our research transcends beyond traditional credit assessment. We delve into the intricate realm of financial risk management, encompassing the prediction of borrower behavior trends and the identification of high-risk applicants. In addition, the dataset enables us to assess how various borrower attributes impact loan performance, contributing to more effective portfolio management and fraud detection.

Ultimately, the project's implications extend to a range of applications within the financial sector. It provides lending institutions with valuable insights for making informed, data-driven decisions. The benefits are widespread, encompassing the optimization of lending practices, risk mitigation, and the enhancement of financial stability. By implementing predictive models and data analysis techniques, the Credit Risk Analysis project offers a holistic approach to addressing credit risk, underlining its significance in the ever-evolving landscape of financial services.

## Dataset Description

This dataset contains detailed information related to loan applications and their outcomes. Below is a description of each column in the dataset, grouped for convenience:

**Borrower and Loan Information:**
1. **id**: Unique LC assigned ID for the loan listing.
2. **member_id**: Unique LC assigned ID for the borrower member.
3. **loan_amnt**: Listed loan amount applied for.
4. **funded_amnt**: Total amount committed to the loan.
5. **funded_amnt_inv**: Total amount funded by investors.
6. **term**: Number of payments on the loan in months (36 or 60).
7. **int_rate**: Interest Rate on the loan.
8. **installment**: Monthly payment owed by the borrower.
9. **grade**: LC assigned loan grade.
10. **sub_grade**: LC assigned loan subgrade.
11. **emp_title**: Job title supplied by the borrower.
12. **emp_length**: Employment length in years.
13. **home_ownership**: Home ownership status (RENT, OWN, MORTGAGE, OTHER).
14. **annual_inc**: Self-reported annual income.
15. **verification_status**: Income verification status.
16. **issue_d**: Month in which the loan was funded.
17. **pymnt_plan**: Payment plan status.

**Loan Description and Purpose:** 

18. **desc**: Loan description provided by the borrower.
19. **purpose**: Category provided by the borrower for the loan request.
20. **title**: Loan title provided by the borrower.

**Location and Address Information:**

21. **zip_code**: First 3 numbers of the borrower's zip code.
22. **addr_state**: State provided by the borrower in the loan application.

**Credit and Payment History:**

23. **dti**: Ratio of monthly debt payments to income.
24. **delinq_2yrs**: Number of past-due incidences of delinquency.
25. **earliest_cr_line**: Month the earliest reported credit line was opened.
26. **inq_last_6mths**: Number of inquiries in the past 6 months.
27. **mths_since_last_delinq**: Months since the borrower's last delinquency.
28. **mths_since_last_record**: Months since the last public record.
29. **open_acc**: Number of open credit lines.
30. **pub_rec**: Number of derogatory public records.
31. **revol_bal**: Total credit revolving balance.
32. **revol_util**: Revolving line utilization rate.
33. **total_acc**: Total number of credit lines.

**Loan Status and Payment Information:**

34. **initial_list_status**: Initial listing status of the loan (W, F).
35. **out_prncp**: Remaining outstanding principal (total amount funded).
36. **out_prncp_inv**: Remaining outstanding principal (portion funded by investors).
37. **total_pymnt**: Payments received to date (total amount funded).
38. **total_pymnt_inv**: Payments received to date (portion funded by investors).
39. **total_rec_prncp**: Principal received to date.
40. **total_rec_int**: Interest received to date.
41. **total_rec_late_fee**: Late fees received to date.

**Recovery and Collection Information:**

42. **recoveries**: Post-charge-off gross recovery.
43. **collection_recovery_fee**: Post-charge-off collection fee.

**Payment Dates and Credit Pulls:**

44. **last_pymnt_d**: Last month payment was received.
45. **last_pymnt_amnt**: Last total payment amount received.
46. **next_pymnt_d**: Next scheduled payment date.
47. **last_credit_pull_d**: Most recent month LC pulled credit for this loan.

**Credit and Derogatory Information:**

48. **collections_12_mths_ex_med**: Number of collections in 12 months excluding medical collections.
49. **mths_since_last_major_derog**: Months since the most recent 90-day or worse rating.

**Policy and Application Details:**

50. **policy_code**: Publicly available policy code (1 for new products, 2 for not publicly available).
51. **application_type**: Indicates individual or joint application.
52. **annual_inc_joint**: Combined self-reported annual income for joint applications.
53. **dti_joint**: Ratio for co-borrowers' total monthly payments to income.
54. **verification_status_joint**: Income verification status for joint applications.

**Account and Credit Balances:**

55. **acc_now_delinq**: Number of accounts with current delinquency.
56. **tot_coll_amt**: Total collection amounts ever owed.
57. **tot_cur_bal**: Total current balance of all accounts.

**Recent Trade and Inquiry History:**

58. **open_acc_6m**: Number of open trades in the last 6 months.
59. **open_il_6m**: Number of open installment lines in the last 6 months.
60. **open_il_12m**: Number of installment accounts opened in the past 12 months.
61. **open_il_24m**: Number of installment accounts opened in the past 24 months.
62. **mths_since_rcnt_il**: Months since the most recent installment accounts were opened.
63. **total_bal_il**: Total current balance of all installment accounts.
64. **il_util**: Ratio of total current balance to high credit/credit limit on all installment accounts.
65. **open_rv_12m**: Number of revolving trades opened in the past 12 months.
66. **open_rv_24m**: Number of revolving trades opened in the past 24 months.
67. **max_bal_bc**: Maximum current balance owed on all revolving accounts.
68. **all_util**: Balance to credit limit on all trades.
69. **total_rev_hi_lim**: Total revolving high credit/credit limit.
70. **inq_fi**: Number of personal finance inquiries.
71. **total_cu_tl**: Number of finance trades.
72. **inq_last_12m**: Number of credit inquiries in the past 12 months.

**Loan Default Status:**

73. **default_ind**: Indicates loan default (1) or non-default (0).

This dataset provides valuable information for credit risk analysis, loan approval, and financial decision-making.


## Dataset Attributes

The table below summarizes the columns in the dataset, including their data types and descriptions:

|    Attribute                | Data Type        | Description                                                           |
|-----------------------------|------------------|-----------------------------------------------------------------------|
| id                          | int64            | Unique LC assigned ID for the loan listing.                           |
| member_id                   | int64            | Unique LC assigned ID for the borrower member.                        |
| loan_amnt                   | int64            | Listed loan amount applied for by the borrower.                       |
| funded_amnt                 | int64            | Total amount committed to the loan.                                   |
| funded_amnt_inv             | float64          | Total amount funded by investors for the loan.                        |
| term                        | object           | Number of payments on the loan in months (36 or 60).                  |
| int_rate                    | float64          | Interest Rate on the loan.                                           |
| installment                 | float64          | Monthly payment owed by the borrower if the loan originates.         |
| grade                       | object           | LC assigned loan grade.                                               |
| sub_grade                   | object           | LC assigned loan subgrade.                                           |
| emp_title                   | object           | Job title supplied by the Borrower when applying for the loan.       |
| emp_length                  | object           | Employment length in years (0 to 10).                                 |
| home_ownership              | object           | Home ownership status (RENT, OWN, MORTGAGE, OTHER).                   |
| annual_inc                  | float64          | Self-reported annual income provided by the borrower.                |
| verification_status         | object           | Indicates if income was verified by LC, not verified, or the income source was verified. |
| issue_d                     | object           | The month in which the loan was funded.                              |
| pymnt_plan                  | object           | Indicates if a payment plan has been put in place for the loan.      |
| desc                        | object           | Loan description provided by the borrower.                           |
| purpose                     | object           | A category provided by the borrower for the loan request.             |
| title                       | object           | The loan title provided by the borrower.                              |
| zip_code                    | object           | The first 3 numbers of the zip code provided by the borrower in the loan application. |
| addr_state                  | object           | The state provided by the borrower in the loan application.          |
| dti                         | float64          | A ratio calculated using the borrower's total monthly debt payments on the total debt obligations, excluding mortgage and the requested LC loan, divided by the borrower's self-reported monthly income. |
| delinq_2yrs                 | int64            | The number of 30+ days past-due incidences of delinquency in the borrower's credit file for the past 2 years. |
| earliest_cr_line            | object           | The month the borrower's earliest reported credit line was opened.   |
| inq_last_6mths              | int64            | The number of inquiries in the past 6 months (excluding auto and mortgage inquiries). |
| mths_since_last_delinq      | float64          | The number of months since the borrower's last delinquency.          |
| mths_since_last_record      | float64          | The number of months since the last public record.                   |
| open_acc                    | int64            | The number of open credit lines in the borrower's credit file.        |
| pub_rec                     | int64            | The number of derogatory public records.                             |
| revol_bal                   | int64            | Total credit revolving balance.                                      |
| revol_util                  | float64          | Revolving line utilization rate, or the amount of credit the borrower is using relative to all available revolving credit. |
| total_acc                   | int64            | The total number of credit lines currently in the borrower's credit file. |
| initial_list_status         | object           | The initial listing status of the loan (Possible values: W, F).       |
| out_prncp                   | float64          | Remaining outstanding principal for total amount funded.             |
| out_prncp_inv               | float64          | Remaining outstanding principal for the portion of the total amount funded by investors. |
| total_pymnt                 | float64          | Payments received to date for the total amount funded.               |
| total_pymnt_inv             | float64          | Payments received to date for the portion of the total amount funded by investors. |
| total_rec_prncp             | float64          | Principal received to date.                                           |
| total_rec_int               | float64          | Interest received to date.                                           |
| total_rec_late_fee          | float64          | Late fees received to date.                                          |
| recoveries                  | float64          | Post-charge-off gross recovery.                                      |
| collection_recovery_fee     | float64          | Post-charge-off collection fee.                                      |
| last_pymnt_d                | object           | Last month payment was received.                                     |
| last_pymnt_amnt             | float64          | Last total payment amount received.                                  |
| next_pymnt_d                | object           | Next scheduled payment date.                                        |
| last_credit_pull_d          | object           | The most recent month LC pulled credit for this loan.               |
| collections_12_mths_ex_med  | float64          | Number of collections in 12 months excluding medical collections.    |
| mths_since_last_major_derog | float64          | Months since the most recent 90-day or worse rating.                |
| policy_code                 | int64            | Publicly available policy code (1 for new products, 2 for not publicly available). |
| application_type            | object           | Indicates whether the loan is an individual application or a joint application with two co-borrowers. |
| annual_inc_joint            | float64          | The combined self-reported annual income provided by the co-borrowers during registration. |
| dti_joint                   | float64          | A ratio calculated using the co-borrowers' total monthly payments on the total debt obligations, excluding mortgages and the requested LC loan, divided by the co-borrowers' combined self-reported monthly income. |
| verification_status_joint   | object           | Indicates if the co-borrowers' joint income was verified by LC, not verified, or if the income source was verified. |
| acc_now_delinq              | int64            | The number of accounts on which the borrower is now delinquent.      |
| tot_coll_amt                | float64          | Total collection amounts ever owed.                                  |
| tot_cur_bal                 | float64          | Total current balance of all accounts.                               |
| open_acc_6m                 | float64          | Number of open trades in the last 6 months.                         |
| open_il_6m                  | float64          | Number of open installment lines in the last 6 months.               |
| open_il_12m                 | float64          | Number of installment accounts opened in the past 12 months.         |
| open_il_24m                 | float64          | Number of installment accounts opened in the past 24 months.         |
| mths_since_rcnt_il          | float64          | Months since the most recent installment accounts were opened.       |
| total_bal_il                | float64          | Total current balance of all installment accounts.                   |
| il_util                     | float64          | Ratio of total current balance to high credit/credit limit on all installment accounts. |
| open_rv_12m                 | float64          | Number of revolving trades opened in the past 12 months.             |
| open_rv_24m                 | float64          | Number of revolving trades opened in the past 24 months.             |
| max_bal_bc                  | float64          | Maximum current balance owed on all revolving accounts.              |
| all_util                    | float64          | Balance to credit limit on all trades.                               |
| total_rev_hi_lim            | float64          | Total revolving high credit/credit limit.                            |
| inq_fi                      | float64          | Number of personal finance inquiries.                                |
| total_cu_tl                 | float64          | Number of finance trades.                                            |
| inq_last_12m                | float64          | Number of credit inquiries in the past 12 months.                   |
| default_ind                 | int64            | Indicates loan default (1) or non-default (0).                       |

## Objectives

The primary objectives of this data mining project are as follows:

1. **Data Preprocessing**: Data preprocessing refers to the initial step in data analysis, where raw data is cleaned, transformed, and organized to make it suitable for further analysis and modeling. It involves handling missing values, dealing with outliers, standardizing data formats, and encoding categorical variables, ensuring the data is usable and consistent before applying data mining or machine learning techniques. Our dataset had 8,55,969 instances of data having 73 features, out of which we dropped few features.
2. **Exploratory Data Analysis (EDA)**: Exploratory Data Analysis (EDA) is visually and statistically analyzing a dataset to summarize its main characteristics, gain insights, and uncover patterns or anomalies. It involves techniques such as data visualization, summary statistics, and correlation analysis to understand better the data's structure, relationships between variables, and potential areas of further investigation in data analysis and modeling tasks. To visualize and understand the data, we have made boxplots, count plots, pie charts, bar graphs, point plots, violin plots,  etc.
3. **Feature Engineering**: Feature Engineering is the process of creating new, relevant, and informative features or transformations of existing ones from raw data to improve the performance of machine learning models. It involves selecting, combining, or transforming variables better to represent the underlying patterns and relationships in the data, ultimately enhancing the model's ability to make accurate predictions or classifications.
4. **Model Selection:**: Model Selection is the process of choosing the most suitable machine learning algorithm or model from a set of candidate models to best address a specific problem or task based on factors like performance, accuracy, and generalization ability. We implemented Logistic Regression, Artificial Nueral Network Model, Support Vector Machine Model, SGD Classifier, Random Forest Classifier.
5. **Model Training and Tuning**: Model Training and Tuning involves training a machine learning model on a dataset to learn patterns and relationships and then optimizing the model's hyperparameters to achieve the best possible predictive performance. This iterative process aims to find the most accurate and effective model configuration for a specific task. We have used gradient descent algorithm to perform model tuning.
6. **Evaluation Metrics**: Evaluation metrics are quantitative measures used to assess the performance or accuracy of a predictive model or algorithm by quantifying the degree of its predictions' agreement with the actual observed outcomes. These metrics help understand how well a model performs its intended task, whether predicting values, classifying data, or solving other machine learning and data mining tasks. Common evaluation metrics include Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), accuracy, precision, recall, and F1-score, depending on the specific task and context.

## Expected Outcome
- A classifier model which is capable of accurately classifying loan default prediction, loan term, loan interest rate range.
- Insight into the factors that most influences the loan lenders and borrower.
- Models can improve the user experience of both loan lender and borrower to lend or borrow the loan.

# Conclusion
## Loan Default
- In predicting the Loan Default Index, evaluating throughout all machine learning models it reveals that ANN model is most favorable than any other method used namely, Logistic regression, Random Forest Classifier, SGD Classifier, SVC. 
Insights of each model can be shown as below:

### Model Performance[Loan Default]

| Model             | Recall |
|-------------------|----------|
| ANN               | 0.98     |
| Logistic Regression | 0.89     |
| Random Forest     | 0.77     |
| SGD Classifier    | 0.89     |
| SVC Linear Kernel | 0.97     |
| SVC RBF Kernel    | 0.92     |

## Loan Term

- In predicting the Loan Term , evaluating throughout all machine learning models it reveals that ANN model is most favorable than any other method used namely, Logistic regression, SVC, XGBoost. 
Insights of each model can be shown as below:

### Model Performance[Loan Term]

| Model             | Accuracy |
|-------------------|----------|
| ANN               | 0.98     |
| Logistic Regression | 0.79     |
| SVC Linear Kernel | 0.79     |
| XGBoost    | 0.85     |

## Interest Rate Range

- In predicting the Interest Rate Range, evaluating throughout all machine learning models it reveals that ANN model is most favorable than XGBoost. 
Insights of each model can be shown as below:

### Model Performance[Loan Interest Rate range]

| Model             | Accuracy |
|-------------------|----------|
| ANN               | 0.90     |
| XGBoost    | 0.85     |