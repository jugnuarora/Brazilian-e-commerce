# Brazilian-e-commerce #

Olist had made it's data public for the timeframe 2016 to 2018. Its features allows viewing an order from multiple dimensions: from order status, price, payment and freight performance to customer location, geolocation data, product attributes and finally reviews written by customers.

Olist connects small businesses from all over Brazil to channels without hassle and with a single contract. Those merchants are able to sell their products through the Olist Store and ship them directly to the customers using Olist logistics partners.

The Data is present in [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce?select=olist_order_reviews_dataset.csv)

In 2019, Olist chief executive and founder Tiago Dalvi said the company plans to expand the number of sellers it serves to 100,000 in two years from current 7000. We have data from 2016 to 2018 and will be analysing it from this perspective. The increase in sellers means increase in the commissions to Olist from the sales.

Main questions for analysis are:
  1. How is the growth in revenue (main KPI) in this timeframe?
  2. How to increase the seller base?
  3. Seller Segmentation
  4. Are there any regions where sellers might be not sufficient? How is it impacting the customers?
  5. Which products needs more attention?
  6. What could be the predicted revenues?

How the Olist business works?
  1. Customer orders and it creates an order in orders dataset with status 'created'
  2. Order is approved and it creates the record in order_items dataset and the status is changed to 'approved'
  3. Order is processed and the status is changed to 'processing'
  4. Order is handed to logistics of Olist and the status is changed to 'shipped'
  5. Order is delivered to customer and the status is changed to 'delivered'
  
Data Quality:
  1. Data is 98% accurate.
  2. For the 2% records, the values in date fields are not in sync. For example, in shipping limit date, there is date for 2020 which is far ahead of actual deleivered to carrier date and since our data is for until 2018, it is absurd.
  3. For records with order_status as invoiced, processing, shipped, unavailable and approved, there are null values in deleivered carrier date and delivered customer date. We checked the reviewes dataset and these packages were actually missing. 
  
 Watch this section for further updates as the project progresses.
