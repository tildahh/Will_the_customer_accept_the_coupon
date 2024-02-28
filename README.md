# Will a customer accept the coupon? 

The goal of this project is to distinguish between customers who accepted a driving coupon versus those that did not, using visualizations and statistical summaries to reveal underlying patterns.

The data comes is sourced from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios, including the destination, current time, weather, passenger, etc., and then asks people whether they will accept the coupon if they are the driver.

**The programming language used is Python, and the libraries used were: Pandas, Seaborn, Matplotlib, and numpy**

[Link to notebook used](https://github.com/tildahh/Will_the_customer_accept_the_coupon/prompt.ipynb)

## Data Summary

The dataset includes responses on five types of coupons: less expensive restaurants (under $20), coffee houses, carry out and take away, bars, and more expensive restaurants ($20–$50). Each entry corresponds to a survey response indicating acceptance ("Y = 1") or rejection ("Y = 0") of the coupon in a given driving scenario.

![Distribution of Coupon Types](/images/coupon_distribution.png)

## Methodology

Using Python for data plotting and statistical analysis, we:
- Examined the distribution of coupon types and acceptance rates.
- Analyzed correlations between acceptance and variables such as visit frequency, time until expiration, customer age, passenger type, and occupation.
- Generated visualizations to support our findings and hypothesis.

## Key Findings

- Coffee houses coupons were accepted at a rate of 50.14%, with a balanced distribution indicating no class imbalance.
- Coupon acceptance correlated with longer expiration times, higher visit frequencies to coffee houses, and the presence of friends or partners.
- Younger customers (below age 30) were more inclined to accept coupons, especially when visiting coffee houses more than once a month.

- https://github.com/tildahh/Will_the_customer_accept_the_coupon/tree/main/images

![Proportion of Coupon Acceptance](https://github.com/tildahh/Will_the_customer_accept_the_coupon/tree/main/images/all_coupon_acceptance.png)
![Number of Coupons Accepted per Category](https://github.com/tildahh/Will_the_customer_accept_the_coupon/tree/main/images/all_coupons_acceptance_ratio.png)
![Proportion of Bar Coupon Acceptance](https://github.com/tildahh/Will_the_customer_accept_the_coupon/tree/main/images/bar_coupon_acceptance.png)
![Bar Correlation Heatmap](https://github.com/tildahh/Will_the_customer_accept_the_coupon/tree/main/images/bar_correlation_heatmap.png)
![Acceptance Rate Based on Number of Bar Visits per Month (https://github.com/tildahh/Will_the_customer_accept_the_coupon/tree/main/images/bar_acceptance_rate_frequency_category.png)
![Proportion of Accepted Coffee Coupons](https://github.com/tildahh/Will_the_customer_accept_the_coupon/tree/main/images/coffee_coupon_acceptance.png)
![Acceptance Rate for Coffee House Visits](https://github.com/tildahh/Will_the_customer_accept_the_coupon/tree/main/images/coffee_acceptance_rate_frequency_detailed.png)
![Rejection Rate for Coffee House Visits](https://github.com/tildahh/Will_the_customer_accept_the_coupon/tree/main/images/to/coffee_rejection_rate.png)
![Coffee Coupon Acceptance by Time of Day](https://github.com/tildahh/Will_the_customer_accept_the_coupon/tree/main/images/to/coffee_acceptance_by_time.png)

## Hypothesis

We hypothesize that customers who are young, frequently visit coffee houses, and are accompanied by peers are more likely to accept driving coupons. This demographic represents a key target for marketing strategies aimed at increasing coupon acceptance rates.

## Actionable Recommendations

- **Optimize Expiration Times**: Adjust coupon validity periods to enhance acceptance.
- **Engage Frequent Visitors**: Focus promotions on customers with regular coffee house visitation habits.
- **Target Youth Demographics**: Direct marketing to younger age groups, who show higher engagement.
- **Capitalize on Social Visits**: Encourage coupon use during social outings with friends or partners.
- **Maximize Peak Times**: Leverage high-acceptance windows, particularly from 10am to 2pm, for coupon offers.

## Next Steps

The subsequent phase involves developing a machine learning model to validate our hypothesis. This model will test the predictive power of the identified factors and confirm the patterns observed in the pre-analysis.

---

For a more detailed exploration of our findings and methodology, please refer to the accompanying Jupyter Notebook which includes all data visualizations and statistical analyses conducted during the study.
