# Bank Project

Just last month, I was sitting in the passenger seat of my husband's car, grading math exams, while he was inside a Chipotle waiting to pick up his next delivery. Having grown up in a small town where delivery was virtually non-existent, I marveled at the customer who ordered a singular burrito to be delivered all the way across town. This customer ultimately paid more in delivery charges than for the food itself! I started to wonder: Who are the customers placing these orders? What drives them to spend money on takeout? Does educational background play a role in their spending habits?

So, I sat at my computer and dug into the details. Here's what I learned:

Customers who hold a high school diploma as their highest level of education spend only 0.31% of their income on delivery, while those with a Ph.D. spend 1.15%.

46% of all purchases are made in-store, while 33% occur online, and catalog purchases account for only 21%, with similar trends found among all educational backgrounds.

Customers who hold a bachelor’s degree are 2x as likely to complain about their order as those with a master’s degree, and almost 6x more likely than those with a Ph.D.

High school graduates are almost 2x as likely to use a coupon as those with all other educational backgrounds.

⬇️Keep reading to learn how I came to these conclusions⬇️ 


Dataset Details
In its original form, the dataset I used in this analysis included 2,205 lines of customer records, with each entry containing 36 different attributes. After cleaning and removing 184 duplicate entries, the final dataset included 2,021 unique customer profiles.

For this analysis, I aggregated customer data by educational background and then further explored categories such as:

Income level

Total amount spent on takeout

Spending categories

Number of complaints filed in the past two years

Number of coupons used

Purchase platforms

*Note this project is modified from an iFood job interview case study given by the Brazilian equivalent of DoorDash, iFood. The data is 98% real, but has been slightly modified for educational purposes.

Click here to see the original dataset.


Analysis
Data Cleaning – I started by examining and removing inconsistencies and missing values. 

Segmentation and Aggregation – I grouped the data by educational demographics, choosing to remove those with unknown backgrounds. 

Visualization – I utilized pivot tables and other functions in Excel to create graphs and charts that demonstrated spending patterns. 

Data Interpretation – I interpreted the graphical and numerical results to highlight consumer trends.



Maximize image
Edit image
Delete image

Figure 1. An example Excel formula used to accurately categorize and label an individual customer's education background based on given binary information columns. 
Visuals and Insights
Maximize image
Edit image
Delete image

Graph 1. A bar chart that displays the distribution of educational backgrounds among consumers.
With 50% of customers holding a bachelor's degree and only 2.42% holding a high school diploma as their highest level of education, I knew that I would not be able to derive actionable insights from observing pure counts in further analysis. Therefore, for the majority of my analysis, I will be using percentages to more accurately assess trends among consumers. Additionally, the data contains 183 users of an unknown educational background. Since I am interested in identifying patterns relating to educational background, I will not be including those in the unknown category for the rest of my analysis.

Total Spending Trends
Maximize image
Edit image
Delete image

Graph 2. A bar chart showing the average income compared to the average total spending (on separate axes) across educational demographics.
Income level and average spending increase drastically between high school graduates and college graduates, but then increase slowly from college graduates onward.

Customers holding a high school diploma are significantly more frugal, spending only 0.31% of their total income on takeout, which equates to $61 per customer on average, totaling $2,997 annually.

Those holding a bachelor’s or a master’s degree equally spend 1.1% (about $576 on average), which totals $582,133 and $194,042, respectively. The larger percentage of bachelor's degrees accounts for the discrepancy in the totals.

Customers with a Ph.D. spend the most, equivalent to 1.15% of their total income, or $632 per year on average, totaling $277,242 annually.

Spending Categories
Minimize image
Edit image
Delete image

Graph 3. A horizontal bar chart detailing the percentage of the total spending budget allocated to different product categories, by educational background.
Wine sales account for a significant portion (47% - 66%) of all total spending, excluding those holding a high school diploma (where wine only accounts for 8% of their overall spending).

High school graduates spend 76% of their total budget on fish, fruit, and sweets, compared to those holding a Ph.D., who allocate just under 10% for the same categories combined.

Educational background and wine spending show a strong positive relationship, as further investigated below.

Maximize image
Edit image
Delete image

Graph 4. A bar chart showing the percentage of the total spending budget allocated to wine purchases and the associated logarithmic trendline. 
This graph shows the strong logarithmic relationship between educational background and the percentage of the total budget spent on wine purchases. The calculated R^2 value of 0.9615 indicates that roughly 96% of wine purchases can be confidently explained by the educational background of the consumer.

I created the following aggregated pivot table to further investigate the spending discrepancy on wine between educational levels by investigating how age factors in.

Maximize image
Edit image
Delete image

Table 1. An aggregated data table summarizing the average percent of their overall spending budget that customers allocate to wine purchases, aggregated by educational background and age bracket.
This table shows that the age group of 51-65 dedicates the largest percentage of their overall spending budget to wine purchases compared to all other age groups across all educational backgrounds.

Purchase Platforms
Minimize image
Edit image
Delete image

Graph 5. A bar chart showing the relationship between preferred purchase platforms based on educational background.
In-store purchases account for 46% of all purchases made, indicating a strong preference for in-store purchases across all educational backgrounds.

Online orders account for 33% of purchases, while catalog purchases account for only 21%.

Educational background does not drastically affect preferences for purchase platforms.

Advertising Campaign Response
Minimize image
Edit image
Delete image

Graph 6. A bar chart depicting how educational backgrounds responded to six different advertising campaigns.
Overall, Campaign 6 was the most effective (resulting in 55% of users responding across all backgrounds), while Campaign 2 was the least effective (resulting in only 4% of users responding across all backgrounds).

While educational demographics do not show much trend among campaign response, it is worth noting that customers holding a high school diploma did not show any response to Campaigns 1, 2, 4, and 5 but showed a resounding response of 10% to Campaign 3, and a 4% response to Campaign 6.

Complaint Trends
Maximize image
Edit image
Delete image

Graph 7. A bar chart showing the percentage of customers who have filed a complaint in the past two years, aggregated by educational background.
Customers who hold a bachelor’s degree are 2x as likely to complain about their order as those with a master’s degree, and almost 6x more likely than those with a Ph.D.

While the data shows a 0% complaint rate for high school graduates, it is important to note that this metric is only considering complaints filed in the past two years and does not reflect the conclusion that these customers will never file a complaint.

Coupon Purchases
Maximize image
Edit image
Delete image

Graph 8. A bar chart showing the percentage of customers who used a coupon to make a purchase, aggregated by educational background.
High school graduates are almost 2x as likely to use a coupon as those with all other educational backgrounds.


Main Takeaways
This project set out to answer the following question: How does educational background influence spending on takeout? Using a real-world customer sales dataset, I uncovered patterns that provide intriguing insights and actionable takeaways for business stakeholders.

Here’s what the data says:
Customers who hold at least a bachelor’s degree spend more, on average. 

Customers with higher degrees allocate more of their budget towards wine purchases, specifically.

Customers in the age range of 36-50 make up the largest population across all educational backgrounds, while the largest spenders are those 66+. 

In-store purchases are the preferred platform across all educational backgrounds.

High school graduates are most likely to use coupons compared to all other educational backgrounds.

What this means for stakeholders:
The company should dedicate more resources to gaining and keeping customers with higher educational backgrounds.

The company could use this information to run targeted ad campaigns for wine pairings, to increase food purchases alongside wine.

The company could focus on recruiting the older demographic to increase sales.

Depending on the company's focus, they could either run promotions to drive online and catalog purchases to help bridge the gap between those and in-store orders, or they could solidify in-store as their main purchase platform by running campaigns specifically for brick-and-mortar shops. 

The company might want to rethink its coupon strategy to appeal more to those with a higher educational background, since those groups spend more.

Reflection
Analyzing this dataset was eye-opening and educational in and of itself. I began by wanting to uncover what role an educational background plays in the purchasing habits of consumers, and ultimately turned my curiosity into action items. Takeout and delivery companies (like DoorDash or iFoods) can use these main takeaways to drive sales, increase profits, and maximize advertising campaign efficacy.  


Stay in Touch
If you have thoughts on my findings or if you know of a job where this kind of information would be beneficial, I’d love to connect with you on LinkedIn! 
