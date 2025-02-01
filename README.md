# Payment Funnel Analysis
(Note- Check Payment Funnel Analysis.pdf for SQL code and discussion)
## Executive Summary

This report analyzes the payment funnel to identify reasons for incomplete subscription payments. Through SQL-based data exploration, we assess user drop-off points, error frequencies, and conversion rates. Key findings indicate that user errors and payment processing failures are major bottlenecks. Recommendations include UI/UX improvements, better error handling, and enhanced follow-up strategies to improve payment completion rates.

## Business Problem:
The finance team comes up one day asking about why there are so many unpaid subscriptions. Lately, customers have been choosing or opting into a paid subscription plan, but many are not completing the process by paying for their subscription. When customers sign up for a subscription, we consider them to officially be a customer, but they aren’t considered “converted” into a paid plan until they actually pay for their subscription by completing the payment process. Because of this, the company has a less-than-desired conversion rate since many companies have started a subscription but haven’t actually paid yet. This is a huge issue for the company because we have customers who are signing up for our product but aren’t paying— which has resulted in a large loss in revenue. Understanding the pain points in the payment funnel is critical to improving conversion rates and minimizing revenue loss.

![image](https://github.com/user-attachments/assets/b1f4eba4-bfc5-46c9-b9b6-635c2797db1b)

## Methodology:
- Exploratory Data Analysis(EDA)
- Payment Funnel Analysis
- Data Visulisation   

## Skills:

1. SQL- CTEs, Joins, Case, Subqueries, Window functions, aggregate functions 
2. Data Interpretation-Identifying user drop-off points and analyzing error frequencies.
3. Data Wrangling
4. Business Intelligence- Translating data insights into actionable recommendations.
5. Problem-Solving- Suggesting improvements to enhance payment completion rates.
6. Data Science Notebook
7. Snowflake Data Warehouse

## Results and Recommendations:

### Results:
- A significant percentage of users start the payment process but do not complete it.
- The error rate among users is 17% and conversion rate is 20%.
- The most common friction points include:
   - Users failing to enter payment details correctly.
   - Payment processing failures from third-party vendors.

![image](https://github.com/user-attachments/assets/85677e46-ab45-4c63-a6e0-e798d08c792f)



The error rate among users is high, indicating a need for better validation and guidance.

The conversion and workflow completion rates suggest a need for process optimization.


### Recommendations

- Improve UI/UX for the payment portal:

- Add real-time validation for credit card fields to prevent user errors.

- Implement clear error messages and guidance for users encountering issues.

- Optimize third-party payment processing:

   - Investigate vendor-side failures and explore alternative payment processors.

   - Implement retry mechanisms for failed transactions.

- User Follow-up Strategies:

   - Send automated reminders to users who started payment but did not complete it.

   - Offer alternative payment methods to users facing issues.

### Conclusion

By analyzing the payment funnel, we identified key bottlenecks in the subscription payment process. Addressing these friction points can significantly improve conversion rates, reduce revenue loss, and enhance user experience. The next steps involve collaborating with the product and engineering teams to implement these recommendations and measure the impact over time.
