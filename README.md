### Assignment for UC Berkeley Professional Certificate in Machine Learning and Artificial Intelligence.

**Overview**

The goal of this project is to use what you know about visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.

**Data**

This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. Answers that the user will drive there ‘right away’ or ‘later before the coupon expires’ are labeled as ‘Y = 1’ and answers ‘no, I do not want the coupon’ are labeled as ‘Y = 0’.  There are five different types of coupons -- less expensive restaurants (under \$20), coffee houses, carry out & take away, bar, and more expensive restaurants (\$20 - \$50).

**Deliverables**

Your final product should be a brief report that highlights the differences between customers who did and did not accept the coupons.  To explore the data you will utilize your knowledge of plotting, statistical summaries, and visualization using Python. You will publish your findings in a public facing github repository as your first portfolio piece. 

### Final Observations and Conclusion
Based on the univariate, bivariate feature analysis and the plotted visualizations, the following hypothesis can be drawn on the conditions when a customer would or would not generally accept the coupons.

**Customers would generally accept the coupons if:**
* Carry out & Take away or Inexpensive Restaurants (average expense less than $20) coupons are offered
* Coffee House coupons offered to customers who have been to a Coffee House in past a few times (generally 4 or more)
* Coupons with 1 day expiry are offered instead of 2 hour expiry
* Coupons are offered when they aren't going to any Urgent Place
* Carry out & Take away or Inexpensive Restaurants or Coffee House coupons are offered when they are driving with Friend(s) around 6PM in warm weather (Sunny, 80°F)
* Coupons were offered for inexpensive restaurants where they have been in past at least few times (generally 4 or more).
* Carry out & Take away coupon offered in cold weather (Snowy, 30°F)

**Customers would not generally accept the coupons if:**
* Coupons are offered for Expensive Restaurants (average expense between \$20 and \\$50) to customers who have never visited them in past
* Coffee House coupons offered to customers who have never visited them in past
* Bar coupons offered to customers with kid(s)
* Bar and Expensive Restaurant coupons offered to customers in cold weather (Snowy, 30°F) or late night (10PM)
* Any coupons other than Carry Away are offered to customers in cold weather (Snowy, 30°F)
* Bar coupons sent to customers early in the day (7AM, 10AM, 2PM)

The jupyter notebook can be located in this repository here - https://github.com/jaiomrana/ucb_ai_ml_assignment_5_1/blob/main/coupon_acceptance_analysis.ipynb

**Next Steps**

The next step would be to continue to build the model, identify an alogorithm and complete the predictive analysis as we move forward to learn all these concepts in the program.
