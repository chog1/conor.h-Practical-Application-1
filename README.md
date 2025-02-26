# conor.h-Practical-Application-1

All workings can be found in file _prompt.ipynb_

Based on CRISP-DM Framework below is a brief report of data review:

1. **Business Understanding**
   The goal of this project is to use visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.
   
3.**Data Understanding**
  This data is from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The data consists of:
  - There are five different types of coupons -- less expensive restaurants (under 20), coffee houses, carry out & take away, bar, and more expensive restaurants (20 - $50).
  - User attributes: gender, Education, Occupation, Annual Income, Number of times that he/she goes to a bar etc
  - Contextual attributes
  - Coupon attributes: time before expires, accepted etc

5. **Data Preparation**
  - Brief review of columns and blank data info() & isnull()
  - drop car column with mostly blank data
  - copy of bar_coupons dataframe, removed text from age column and updated to float in order to simplify query on age (greater than, less than)
  - visual display of columns grouped by responses to identify categories for filtering purposes
  - visualize distribution through charts
    
7. **Modeling**
  - use query function to filter on appropriate values and return mean based on Y column (0,1) for acceptance rate

   
9. **Evaluation**
   ** Investigating the Bar Coupons**:
   - The acceptance rate of bar coupons is 41.00%
   - The acceptance rate for those who went to a bar 3 or fewer times a month is 52.74%
   - The acceptance rate for those that went more than 3 times a month is 76.88%
   - The acceptance rate for those who go to a bar more than once a month and are over 25 is 69.52%
   - The acceptance rate for all the others 26.10%
   - The acceptance rate for those who go to a bar more than once had no kids in the car and had occupations other than farming, fishing, or forestry 71.32%
   - Go to bars more than once a month, had passengers that were not a kid, and were not widowed 71.32%
   - Go to bars more than once a month and are under the age of 30 72.17%
   - Go to cheap restaurants more than 4 times a month and income is less than 50K 76.92%
   - hypothesize about drivers who accepted the bar coupons: Drivers that go to cheap restaurants more than 4 times a month and income is less than 50K are likely to accept bar coupon with 76.92% acceptance rate
  
    **resturant20_50_coupons**
   - A large number of coupons distributed were for those with a destination of Home. See chart 'Restaurant(20-50) Coupon Destination Distribution' in data folder
   - The highest propertion of acceptance is 6pm. see chart 'Histogram of time column and accepted' in data folder




