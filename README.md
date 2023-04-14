# Store Sales insight
### Breakdown of how different factors impact the product sales.
Jake Cho

The project aims to explore how few factors influence store sales by analyzing a dataset of sales across several stores. The project involves data preprocessing and exploratory data analysis. By identifying the most significant factors that impact store sales, the project provides insights into how businesses can optimize their sales strategies and improve their bottom line.

## Dataset

Original source: https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/

There are 12 columns and 8,523 rows.

## Data Dictionary

![image](https://user-images.githubusercontent.com/61045591/225922676-4d77eb7c-8933-48ed-919a-9ec3ffe01aff.png)

#### To prepare for analysis, data was cleaned by dealing with missing data points and inconsistent categorization 

## Exploratory Visuals

![image](https://user-images.githubusercontent.com/61045591/225922808-d1e45e58-16df-464a-b265-251e1a7572f5.png)

This is a histogram of the Item_MRP, which shows the range of maximum retail price for the products sold in the stores. 

![image](https://user-images.githubusercontent.com/61045591/225922857-3147cb19-fc25-4bff-8b36-492f7507ed9c.png)

This box and whisker plot shows the ranges of the Item Max Retail Price is for each individual store. You can notice that they have a very similar range among the 10 stores. This shows that all the stores have similar price range of items and the only determining factor of their sales is how much they sell, not the price range of items.

![image](https://user-images.githubusercontent.com/61045591/225922904-bd022fa8-25cc-4772-945a-8c31b51a1d33.png)

This is a heatmap among the quantifiable data to see the correlation between each factors. There is almost no correlation between the different factors. This means that there are no linear corelationship between the variables. However, it could mean they could have nonlinear relationships.

## Explanatory Visuals

![image](https://user-images.githubusercontent.com/61045591/225923015-f8c5c530-6c45-4791-a69e-83e43e8a7065.png)

This graph shows which type of items are contributing to the sales among all the outlets. 

The top three are

Fruits and Vegetables    2.82M

Snack Foods              2.73M

Household                2.06M

The bottome three are

Others                   326K

Breakfast                232K

Seafood                  148K

![image](https://user-images.githubusercontent.com/61045591/225923081-1be074eb-e92b-4ac8-a7a9-3cd4b290854a.png)

This graph shows which outlets have the most sales. This shows that OUT010 and OUT019 show very little sales compared to the most of them while OUT027 is outperforming by a lot. OUT027 had sales of 3.45M dollars while OUT019 had sales of 180K dollars


## Modeling results

Using both linear regression and decision tree, experiment tries to determine which is the better model to determine Item_Outlet_Sales. 

Results for Linear Regression testing data:
  - R^2 = 0.566
  - MAE = 803.616
  - MSE = 1196985.954
  - RMSE = 1094.069

Results for Decision Tree testing data:
  - R^2 = 0.216
  - MAE = 1028.277
  - MSE = 2162786.358
  - RMSE = 1470.641
  
Looking at the results, the linear regression model is a better model due to larger R2 and smaller values for MAE, MSE and RMSE.


## Recommendation:

# Store insights: 

It would be wise to start focusing more sales for certain products since they have the most sales. Also, since two of the stores are very underperforming, it might be better to make big changes to those two stores or reestablish the store elsewhere.

# Model performance:

It would be wiser to have more different factors to tune out the model more. Linear Regression model was better, but it's not great enough to help most people's cases.

## Limitations and Next Steps
From here, we would have to know how much money is being invested into these stores and how much of the sales are actually profitable. Two underperforming stores could be more profitable, if the investment is even lower. 
