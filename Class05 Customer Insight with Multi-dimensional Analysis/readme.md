## To create Dashboard by Powerbi

Dataset: supermarket.csv [Link](https://github.com/Vvanit/BADS7105-CRM-Analytics/blob/e4cbf416a209bacd311f584d2d69f0846c38291c/Class05%20Customer%20Insight%20with%20Multi-dimensional%20Analysis/Supermarket%20Data.zip)

### Preparation
Create customer table

Dax: 

customer_table = SUMMARIZE('Supermarket Data','Supermarket Data'[CUST_CODE],'Supermarket Data'[CUST_LIFESTAGE]
,"CLV",SUM('Supermarket Data'[SPEND])
,"count_basket",DISTINCTCOUNT('Supermarket Data'[BASKET_ID])
,"last_purchase",max('Supermarket Data'[date])
,"first_purchase",min('Supermarket Data'[date])
)

### Dashboard

Contains 2 part

1. Sales information
![2021-12-17 23 55 04](https://user-images.githubusercontent.com/46345359/146580396-41217367-92bf-46ac-b172-3cfa99be73c0.png)

2. Customer insight (CLV, Cohort analysis)
![2021-12-17 23 56 51](https://user-images.githubusercontent.com/46345359/146581543-ad857b1a-82fb-44e0-a507-d76f3ef5e359.png)
