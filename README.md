# Will a Customer Accept the Coupon?

## Background
Imagine driving through town and a coupon is delivered to your cell phone for a restaraunt near where you are driving. Would you accept that coupon and take a short detour to the restaraunt? Would you accept the coupon but use it on a sunbsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaraunt? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day?

Obviously, proximity to the business is a factor on whether the coupon is delivered to the driver or not, but what are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?


This project aims to analyze the factors that determine whether a driver will accept a coupon delivered to their cell phone while driving. The goal is to use visualizations and probability distributions to distinguish between customers who accepted the coupon and those who did not. The data used for this analysis was collected through a survey on Amazon Mechanical Turk and is available in the UCI Machine Learning repository.

## Overview
The project involves exploring the survey data collected related to Amazon Mechanical Turk and available via UCI Machine Learning repository. We will use different probability predictions and co-relations to understand if coupon are likely to be accepcted by customers. The analysis will also include plotting, statistical summaries, and visualizations using Python. And finally conclusions will be listed in a bried report.

## Data Description
The dataset contains various attributes related to users, contextual factors, and coupon attributes. The attributes include:

1. User attributes:
   - Gender: male or female
   - Age: below 21, 21 to 25, 26 to 30, and so on
   - Marital Status: single, married partner, unmarried partner, or widowed
   - Number of children: 0, 1, or more than 1
   - Education: high school, bachelor's degree, associate's degree, or graduate degree
   - Occupation: various categories such as architecture & engineering, business & financial, etc.
   - Annual income: different income ranges
   - Frequency of going to a bar, buying takeaway food, going to a coffee house, and eating at a restaurant with an average expense less than $20 per person

2. Contextual attributes:
   - Driving destination: home, work, or no urgent destination
   - Location of user, coupon, and destination: geographical information with distances and driving times
   - Weather: sunny, rainy, or snowy
   - Temperature: temperature ranges
   - Time: different time slots such as 10 AM, 2 PM, or 6 PM
   - Passenger: alone, partner, kid(s), or friend(s)
     
3. Coupon attributes:
   - Time before it expires: 2 hours or one day
   - 
## Deliverables
The deliverables for this analysis includes:

1. Exploratory data analysis: Use Python to analyze and visualize the data, exploring the differences between customers who accepted the coupons and those who did not.
2. Report: Compile the findings into a brief report highlighting the key differences and correlations identified in the analysis.
3. Related code & data files: Publish relevant code in repository.

## Code: [Jupyter Coupon Data Analysis Notebook](/User_Coupon_Acceptance.ipynb)

## Conclusion
After analyzing, cleaning and exploring coupon data for different coupon types, customer habbits and thier situation like kids, age, occupation etc we can observe follow conclusions :
- Data cleaning was needed as many columns had data issues
- Few columns were missing data and needed to be dropped
- Datatype of columns needed to be fixed also to allow calculations and easy filtering etc

### Overall Coupons Analysis 
- Most coupons were dilevered for Coffee house of which close to 50% were accepted
- Least coupon were delivered for Restaurant(20 -50)
- Only 2 categories for Restaurant(< 20) & Carry Out we see majority of coupons were accepted

### Bar Coupon Analysis Summary
- Overall Bar coupons have close to 50% acceptance rate
- There is only negligible variation in acceptance rate given younger population < 25 years or more > 25 years
- Students tend to accept most bar coupons from total bar coupon population
- Other groups like Business & Management also tend to accept coupons more than reject
- Therefore Occupation does play a role in coupon acceptance rate
- People who go to bar more than 3 times a month tend to accept more coupons V/s people are are infrequent which makes sense given higher freqency of bar visits
- Lower income groups tend to accept more coupon which also makes sense given they prefer spending less
- Having Kids in car does affect coupon acceptance rate

### Coffee House Coupon Analysis Summary
- Unemployed & Students are contributing accept most coffee house coupons
- Weather does not seem to be a factor in determining coupon acceptance
- Most coupons are accepted either around morning 10AM followed by evening around 6PM
- More coupons were also delivered for above times
- Therefore time of day is importance variable for coupon acceptance

### Further Analysis & Recommendations
- Driving destination data can be explored to understand if it factors in coupon acceptance
- Coupon expiration validity can also be explored further
- Missing contextual Traffic data for the location can be very useful here to understand how soon can customer reach the location given short expiring coupons < 2-4 hours etc
- Other coupon attributes like discount type, %discount, discount limits etc could be added to data to understand how acceptance behaviour changes based on how deep and attractive the coupons. 

The analysis provides valuable insights into customer behavior and preferences regarding coupon acceptance in various driving scenarios.
