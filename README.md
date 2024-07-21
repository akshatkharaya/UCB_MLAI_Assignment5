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
* As expected, acceptance rate is higher if the destination is not an urgent place.
* Acceptance rate is inherently higher for carry out & take away and cheap restaurants.
* Temperature affects acceptance rate for coffee house and cheap restaurants. For both, increase in temperature increases the acceptance rate to a certain extent.
