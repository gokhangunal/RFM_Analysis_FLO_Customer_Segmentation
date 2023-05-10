# RFM_Analysis_FLO_Customer_Segmentation
RFM, CRM, Customer Segmentation

An online shoe store called FLO wants to segment its customers and develop marketing 
strategies based on these segments. For this purpose, customer behaviors will be identified 
and groups will be formed based on the clustering of these behaviors.

-----------------------------------------------------------------------

**master_id:** Unique customer number

**order_channel:** The channel used for the purchase (Android, ios, Desktop, Mobile)

**last_order_channel:** The channel used for the last purchase

**first_order_date:** The date of the customer's first purchase

**last_order_date:** The date of the customer's last purchase

**last_order_date_online:** The date of the customer's last online purchase

**last_order_date_offline:** The date of the customer's last offline purchase

**order_num_total_ever_online:** The total number of purchases the customer has made online

**order_num_total_ever_offline:** The total number of purchases the customer has made offline

**customer_value_total_ever_offline:** The total amount paid by the customer for offline purchases

**customer_value_total_ever_online:** The total amount paid by the customer for online purchases

**interested_in_categories_12:** The list of categories in which the customer made purchases in the last 12 months

-----------------------------------------------------------------------

**1.** Read the data and create a copy of the dataframe.

**2.** Examine the first 10 observations, variable names, descriptive statistics, missing values, and variable types in the dataset.

**3.** Create new variables for the total number of purchases and spending for each customer, 
indicating omnichannel customers who have made purchases from both online and offline platforms.

**4.** Examine variable types. Convert date variables to date format.

**5.** Examine the distribution of the number of customers, total number of products purchased, and total spending across different shopping channels.

**6.** Rank the top 10 customers with the highest revenue.

**7.** Rank the top 10 customers with the highest number of orders.

**8.** Functionize the data preprocessing steps.

-----------------------------------------------------------------------

**1.** Define Recency, Frequency, and Monetary metrics.

**2.** Calculate Recency, Frequency, and Monetary metrics for each customer.

**3.** Assign the calculated metrics to a variable named "rfm".

**4.** Rename the metrics as recency, frequency, and monetary.

-----------------------------------------------------------------------

**1.** Convert Recency, Frequency, and Monetary metrics into scores between 1-5 using qcut function.

**2.** Save these scores as recency_score, frequency_score, and monetary_score.

**3.** Combine recency_score and frequency_score into a single variable called RF_SCORE.

-----------------------------------------------------------------------

**1.** Define segments for the created RF scores.

**2.** Convert the scores into segments using the seg_map.

-----------------------------------------------------------------------

**1.** Examine the averages of recency, frequency, and monetary for each segment.

**2.** Using RFM analysis, find the customers in the relevant profile for the following 2 cases and save their customer IDs as a csv file:

   **2a.** FLO is adding a new women's shoe brand to its portfolio. The prices of this brand's products are above the general customer preferences. 
      Therefore, they want to communicate with the customers who are interested in this profile and make special efforts to promote the brand and sell its products. 
      The loyal customers (champions, loyal_customers) and those who shop in the women's category will be the targeted customers for communication. 
      Save the customer IDs of these customers to a csv file.
      
   **2b.** A discount of nearly 40% is planned for men's and children's products. The company wants to target customers who are interested in these categories, 
      but haven't made a purchase in a long time, as well as new customers. Save the customer IDs of these customers who are in the appropriate profile to a csv file.
