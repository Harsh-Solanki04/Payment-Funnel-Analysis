# Payment Funnel Analysis

##Executive Summary

This report analyzes the payment funnel to identify reasons for incomplete subscription payments. Through SQL-based data exploration, we assess user drop-off points, error frequencies, and conversion rates. Key findings indicate that user errors and payment processing failures are major bottlenecks. Recommendations include UI/UX improvements, better error handling, and enhanced follow-up strategies to improve payment completion rates.

###Business Problem:
Your finance team comes to you one day asking about why there are so many unpaid subscriptions. Lately, customers have been choosing or opting into a paid subscription plan, but many are not completing the process by paying for their subscription. When customers sign up for a subscription, we consider them to officially be a customer, but they aren’t considered “converted” into a paid plan until they actually pay for their subscription by completing the payment process. Because of this, the company has a less-than-desired conversion rate since many companies have started a subscription but haven’t actually paid yet. This is a huge issue for the company because we have customers who are signing up for our product but aren’t paying— which has resulted in a large loss in revenue. The finance team has reported a high number of unpaid subscriptions, negatively impacting revenue. While users initiate the subscription process, many do not complete the payment. Understanding the pain points in the payment funnel is critical to improving conversion rates and minimizing revenue loss.

###Skills:

1.SQL: CTEs, Joins, Case, aggregate functions
2.Data Interpretation: Identifying user drop-off points and analyzing error frequencies.
3.Business Intelligence: Translating data insights into actionable recommendations.
4.Problem-Solving: Suggesting improvements to enhance payment completion rates.

###Data Exploration and Understanding

Dataset Overview-

We analyzed two key tables:
-payment_status_log: Tracks different payment statuses for each subscription.
-payment_status_definitions: Provides definitions for each status ID in the payment process.



