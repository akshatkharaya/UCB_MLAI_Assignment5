# UCB_MLAI_Assignment5
This README file includes the summary of findings and link to notebook
Summary of findings:
(A) About the data 
For age column: Result is surprising that some values are age groups (e.g., below21) vs some values are ages (e.g., 46)
'car' variable is not a useful variable because it is missing for 12576/12684 (i.e., 99%+) of responses. The missing rate for visit frequency variables is pretty low (<2%). Decided to remove 'car' column and then dropna 
(B) Data analysis
Proportion of total observations that chose to accept the coupon is:  0.569
Bar coupon acceptance rate analysis shows that:
* People who visit bars often (4 or more times a month) are more likely to accept a coupon
* Passenger in the car and age affect the likelihood of accepting a coupon
* Visiting cheap restaurants and income may *not* be a good indicator of likelihood to accept a coupon

Independent investigation shows that:
(A) For overall data
* As expected, acceptance rate is higher if the destination is not an urgent place.
* Acceptance rate is inherently higher for carry out & take away and cheap restaurants.
* Temperature affects acceptance rate for coffee house and cheap restaurants. For both, increase in temperature increases the acceptance rate to a certain extent.

(B) For coffee house coupon group
* Similar to the overall population, the acceptance rate is higher for Coffee House coupon if the destination type is No Urgent Place.
* People who visit coffee house more often (4 or more times) are more likely to accept the coupon.
* Based on overall data, we already observed that temperate affects the acceptance rate for coffee coupons. Increase in temperature increases the acceptance rate to a certain extent. 
* Acceptance rate is higher if the passenger is friend(s) or partner as opposed to alone or kid.


NEXT STEPS AND RECOMMENDATIONS
Analysis so far has showed the differences in acceptance rate by sub-groups for different coupon types (e.g., bar, coffee house). To make this actionable/prescriptive, we need to build a decision tree model that predicts the probability of accepting the coupon.