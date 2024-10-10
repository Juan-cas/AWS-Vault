2024-10-06 20:11

Status:

Tags:
[[AWS Budgeting Index]]

# AWS Budgets

You can use AWS Budgets to track and take action on your AWS cost and usage. 

You can use AWS Budget to monitor your aggregated utilization and coverage metrics for your reserved instances.

You can also use AWS Budgets to enable simple-to-complex cost and usage tracking. Some examples include:

- setting a monthly cost budget with a fixed target amount to track all costs associated with your account. You can choose to be alerted for both actual (After accruing) and forecasted (Before Accruing) spends.

- Setting a monthly cost budget with a variable target amount, with each subsequent month growing the budget target by 5%. Then, you can configure your notifications for 80% of your budgeted amount and apply an action. For example, you could automatically apply a custom IAM policy that denies you the ability to provision additional resources within an account.

- Setting a monthly usage budget with a fixed usage amount and forecasted notifications to help ensure that you are staying within the service limits for a specific service. You can also be sure you are staying under a specific AWS Free Tier Offering.

- Setting a daily utilization or coverage budget to track your RI or Savings Plans, You can choose to be notified through email and Amazon SNS topics when your utilization drops below 80% for a given day.

`AWS Budget` information is updated up to 3 times a day. Updates typically occur 8-12 hours after the previous update. Budgets can track your un-blended, amortized and blended costs. Budgets can include or exclude charges such as discounts, refunds, support fees, and taxes.

References 
[First Steps into AWS Budgets](https://docs.aws.amazon.com/cost-management/latest/userguide/budgets-best-practices.html)
[what is AWS Budgets](https://docs.aws.amazon.com/cost-management/latest/userguide/budgets-managing-costs.html)