## Answering Business Request
### Pakistan's Largest E-Commerce Dataset
### Source: [Kaggle](https://www.kaggle.com/datasets/zusmani/pakistans-largest-ecommerce-dataset)

The data used is data originating from Kaggle: Pakistan's Largest E-Commerce Dataset with some changes.

The price listed has been converted to 1 Rupee equal to IDR 58. The explanation of the dataset is as follows:

**order_detail:**
|variable                       |class     |description |
|:------------------------------|:---------|:-----------|
id          |object|    unique number of order / order_id
customer_id |object|    unique number of the customer
order_date  |object|    the date when the transaction was made
sku_id |object| unique number of the product (sku is stock keeping unit)
price |int64| the price stated on the price tag
qty_ordered |int64| the number of goods purchased by customers
before_discount |float64| total price value of the product (price * qty_ordered)
discount_amount |float64| total product discount value
after_discount |float64| the total price value of the product when it has been reduced by discounts
is_gross |int64| indicates the customer has not paid for the order
is_valid |int64| shows the customer has made a payment
is_net |int64| indicates the transaction is complete
payment_id |int64| unique number of the payment method


**sku_details:**
|variable                       |class     |description |
|:------------------------------|:---------|:-----------|
id |object| unique number from the product (can be used as a key when joining)
sku_name |object| name of the product
base_price |float64| the price of the item stated on the price tag
cogs |int64| cost of goods sold / total cost to sell 1 product
category |object| product category


**customer_detail:**
|variable                       |class     |description |
|:------------------------------|:---------|:-----------|
id |object| unique number of customers
registered_date |object| the date customers start registering as members


**payment_detail:**
|variable                       |class     |description |
|:------------------------------|:---------|:-----------|
id |int64| unique number of the payment method
payment_method |object| payment method used
