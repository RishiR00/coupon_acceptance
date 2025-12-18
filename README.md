**Coupon Acceptance Data Analysis :**

**Summary:**

This git repository includes the analysis of customers coupon acceptance analysis. This is  part of my ML & AI course work.  

This source data ior this analysis s from the UCI Machine Learning Repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios, including the destination, current time, weather, and passenger, and then asks people whether they will accept the coupon if they are the driver. There are three possible answers people can choose from:

	•	“Right away”
	•	“Later, before the coupon expires”
	•	“No, I do not want the coupon”

The first two responses are labeled as “Y = 1,” and the third is labeled as “Y = 0.” There are five different types of coupons: Less expensive restaurants (under $20), coffee houses, carryout and takeaway, bars, and more expensive restaurants ($20–$50). The data structure is documented in the Jupyter notebook.

I performed the following analysis for Bar and Coffee House coupons.

**Data clean up:**

Review of the data identified, the following up are required for effective analysis.
	•	The column Car has 99% null values. Therefore, removed the column from the data frame. 
	•	Converted the Age column to numeric by chaining the values ‘lessthan 21’ to 20 and ‘greater than 50’ to 50. This helped me perform numerical operations on the Age column while analyzing the data.
	•	Changed the column name from “passenger’ io ‘passenger’

**Analysis performed:**

Performed the following analysis:

	•	Proportion of Bar coupon accepted.
	•	Acceptance rate between those who went to a bar 3 or fewer times a month to those who went more.
	•	Comparing the acceptance rate between drivers who go to a bar more than once a month and are over 
	    the age of 25 to the all others to understand the difference.
	•	Comparing the acceptance rate between drivers who go to bars more than once a month and had passengers that 
	    were not a kid and had occupations other than farming, fishing, or forestry.
	•	Comparing the acceptance rate between the following three categories of customers:
	⁃	customer going to bars more than once a month, had passengers that were not a kid, and were not widowed OR
	⁃	customer going to bars more than once a month and are under the age of 30 OR
	⁃	customer going to cheap restaurants more than 4 times a month and income is less than 50K.

Also, explored the ‘Coffee House’ coupons  and to determine the characteristics of passengers who accept the coupons. 


**Bar Coupon observations:**

Customers older than 25 years of age with less $50k income and visting the bar more frequently bar-goers tend to accept the coupons more frequently.

1. Customers who visit bars more than 3 times per month have roughly double the acceptance rate (76%) compared to other customers who go 3 or fewer times (~37%).

2. Among the Customers visiting the bar more than once, customers over the age of 25 tend to acceptance the coupons twice (~69%) as much as the customers below the age of 25 (~33%).

3. Customers visited the Bar at least once with no kid in the car and not from Farming Fishing & Forestry occupation has accepted the coupons more than twice (~71%) as much as the other categories of customers (~29%).

**Coffee House coupon observations:**

Customers with Friends and Partners in the car tend to accept the Coffee House coupons compared to customers alone in the car.

Similarly, customers with kids in the car tend to accept the coupons at a higher rate (~5%) compared to the customers alone.

Finally, the acceptance rate did not change much with drivers over 25 for the same categories.


Links
Worksheet: https://github.com/RishiR00/coupon_acceptance/blob/main/customer_coupon_acceptance_rate_analysis.ipynb Data: https://github.com/RishiR00/coupon_acceptance/blob/main/data/coupons.csv
