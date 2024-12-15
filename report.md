
### Insights and Recommendations

**Analysis on User Details , Cooking Sessions ,Order Details**:

**Summary on OrderDetails df1 are**
- there are no missing values
- it consists of 10 rows and 9 columns
- there are no missing values
- there are total of 10 unique users/customers and their details


**Summary on cookingsessions df2 are**
- there are no missing values
- same  users order different orders on different days over the week.
- highest meal type ordered was dinner spaghetti (4 times)
- highest ordered users are 1 and 2
- maximum duration taken was grilled chicken it takes 45 mins
- minimum duration was oatmeal takes 10 mins


**Summary on OrderDetails df3 are**
- there is a missing value in Rating column and its in float datatype and the reason for the no rating is the order has been cancelled.
- from the order date feature engineering can be done(extracting day,month and year) since its a weeks data extracting day would be sufficient
- also two orders has been cancelled so there is no ratings for them(missing values)
- there are 6 different dishes in this week data
- highest orders are at night
- maximum amount spent is 15 dollars(spaghetti)
- minimum amount spent is 7 dollars(oatmeal)
- we can remove the cancelled orders or we can fill the ratings based on their avg which is for Grilled chicken is 4.7 and oatmeal is 4.0

**Summary on Merged Data**:
-since there is repition of columns[user_id,dish name,mealtype] we can remove it from either of the datasets.
-no need for the columns(session start, session end) we have already extracted the time as durations
-converted the merged data into excel file
-the merged data has 16 rows and 20 columns there is no loss of data and now we move on to visualisation.


1. **Relationship Between Cooking Sessions and Orders**:
   - We can clearly see that there were no orders placed by user 9 and 10
   - maximum orders placed is by user003 of 45 orders
   - minimum orders placed is by user008 of 5 orders
   - Popular dishes have higher session and order ratings.
   - Cooking sessions directly influence user ordering patterns.
   - dishes order for Breakfast are Oatmeal and Pancakes
   - for lunch is Caesar salad and Veggie Burger
   - for dinner is Grilled chicken and spaghetti

2. **Popular Dishes**:
   - Identified the popular dishes by sorting it in descending order with order count where grilled chicken and spaghetti tops the list.

3. **Demographic Factors**:
   - Age and location impact user preferences and spending habits.
   - Chicago placed maximum orders of 45 and followed by los angeles 35
   - Also from the above inference till now there was no orders placed by user 9(dallas) and 10(phoenix) in the year 2024 but they have total orders of 6 and 8 respectively and hence we can see the data is missing or not updated.

### Recommendations:
- Promote popular dishes more prominently in marketing.
- Offer location-specific deals and promotions.
- Encourage cooking sessions for underperforming dishes to boost orders.
