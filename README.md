# Payment Funnel Analysis

## Executive Summary

This report analyzes the payment funnel to identify reasons for incomplete subscription payments. Through SQL-based data exploration, we assess user drop-off points, error frequencies, and conversion rates. Key findings indicate that user errors and payment processing failures are major bottlenecks. Recommendations include UI/UX improvements, better error handling, and enhanced follow-up strategies to improve payment completion rates.

### Business Problem:
Your finance team comes to you one day asking about why there are so many unpaid subscriptions. Lately, customers have been choosing or opting into a paid subscription plan, but many are not completing the process by paying for their subscription. When customers sign up for a subscription, we consider them to officially be a customer, but they aren’t considered “converted” into a paid plan until they actually pay for their subscription by completing the payment process. Because of this, the company has a less-than-desired conversion rate since many companies have started a subscription but haven’t actually paid yet. This is a huge issue for the company because we have customers who are signing up for our product but aren’t paying— which has resulted in a large loss in revenue. The finance team has reported a high number of unpaid subscriptions, negatively impacting revenue. While users initiate the subscription process, many do not complete the payment. Understanding the pain points in the payment funnel is critical to improving conversion rates and minimizing revenue loss.

### Skills:

1. SQL- CTEs, Joins, Case, aggregate functions 
2. Data Interpretation-Identifying user drop-off points and analyzing error frequencies.
3. Data Wrangling
4. Business Intelligence- Translating data insights into actionable recommendations.
5. Problem-Solving-Suggesting improvements to enhance payment completion rates.

### Data Exploration and Understanding

Dataset Overview-

We analyzed two key tables:
- payment_status_log: Tracks different payment statuses for each subscription.
- payment_status_definitions: Provides definitions for each status ID in the payment process.
By exploring this data, we identified trends in user payment behavior and the major drop-off points.

Payment Funnel Analysis-
Identifying Subscription Statuses

Subscriptions were categorized based on their progress through the payment funnel. This classification helped in understanding user drop-off points and pinpointing critical friction areas.

Breakdown of Funnel Stages-

The payment process was divided into key stages:

1. Payment Initiated – Users open the payment widget.
2. Payment Entered – Users input payment details.
3. Payment Submitted – Payment is sent for processing.
4. Processing Stage – Transaction is handled by the payment vendor.
5. Successful Payment – Transaction is completed.
6. Failed Payment – Errors encountered during payment.
   
or User never entered the payment process.

By analyzing the distribution of users across these stages, we identified where the most significant drop-offs occurred.
![image](https://github.com/user-attachments/assets/a4c0d4de-db95-4a40-81b9-03aee8e76ca6)


Conversion and Workflow Completion Rates-

Two critical performance metrics were calculated:

- Conversion Rate: The percentage of users who successfully completed payments.
- Workflow Completion Rate: The percentage of users who started payment and successfully finished it.

These metrics highlighted inefficiencies in the process, helping prioritize areas for improvement.

Error Frequency Analysis-

We examined the proportion of subscriptions affected by errors and categorized them as:
- User Errors (e.g., incorrect payment details)
- Vendor Processing Failures
  
Understanding these errors allowed for targeted recommendations to reduce failures and improve the overall experience.

### Key Findings:

A significant percentage of users start the payment process but do not complete it.

The most common friction points include:

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

-User Follow-up Strategies:

   - Send automated reminders to users who started payment but did not complete it.

   - Offer alternative payment methods to users facing issues.

### Conclusion

By analyzing the payment funnel, we identified key bottlenecks in the subscription payment process. Addressing these friction points can significantly improve conversion rates, reduce revenue loss, and enhance user experience. The next steps involve collaborating with the product and engineering teams to implement these recommendations and measure the impact over time.
