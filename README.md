# coupon-survey
# Overview
Imagine driving through town and a coupon is delivered to your cell phone for a restaraunt near where you are driving. Would you accept that coupon and take a short detour to the restaraunt? Would you accept the coupon but use it on a sunbsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaraunt? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day?

The goal of this project is to distinguish between customers who accepted a driving coupon versus those that did not

# Data
This data is from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. Answers that the user will drive there ‘right away’ or ‘later before the coupon expires’ are labeled as ‘Y = 1’ and answers ‘no, I do not want the coupon’ are labeled as ‘Y = 0’. There are five different types of coupons -- less expensive restaurants (under $20), coffee houses, carry out & take away, bar, and more expensive restaurants ($20 - $50).

# Data Wrangling
The column "car" was missing more 99% of the data. Hence the column was dropped. The columns "Bar" , "CoffeeHouse", "CarryAway", "RestaurantLessThan20" and "RestaurantLessThan20" were missing 0.84%, 1,7%,1.2%,1% & 1.5% respectively. The rows missing data in these columns were dropped since the total missing data amounted to less than 5%.

# Results:

- 57% of the drivers accepted the coupons
- Coupons for coffee house were accepted proportionately higher compared to others catogories. Coupons for cheap restaurants has the second best acceptance rate
- 41% of the bar coupons were accepted
- Drivers visiting the bars more than 3 times in a month are more likely to accept the coupons
- Drivers less than age 25 accept coupons on a higher rate than other
- Drivers that are single or divorced are also most likely to accept the coupons
- Acceptance rate of drivers who went to a coffee house less than 3 times is 45% which is higher than Acceptance rate of drivers who went to a bar less than 3 times. So compared to bar coupons minimal visits are enough to accept coffee house coupons
- Acceptance rate for coffee house coupons is higher among drivers of age less than 25
- Acceptance rate for coffee house coupons is higher among drivers accompanied by partners and friends
- Bar coupons acceptance rate increases as temperature increases. Interestingly when the temperature is low , acceptance rate in the cheap restaurants is lower





