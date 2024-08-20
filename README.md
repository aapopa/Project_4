# Project_4

The primary objective of this project is to develop a predictive model that accurately forecasts the purchase status of customers. The analysis aims to identify key factors influencing purchase decisions and provides actionable insights for marketing strategies. By understanding and predicting whether a customer is likely to make a purchase, businesses can enhance their marketing strategies, personalize customer interactions, and improve overall sales performance. 

The dataset comprises of 1500 customers and various attributes related to customer purchase behavior, including age, gender, annual income (USD), number of purchases, product category (clothing, home goods, beauty, sports), time spent of website, loyalty program, discounts availed, and the response variable, purchase status. There was 112 duplicate rows, so those rows were removed. Removing NAs or immputation was not necessary because the data contains no missing values.

Before beginning to fit our model, we created some hypotheses on how different factors would help our model in predicting Purchase Status. We believed that variables like age, number of purchases, and time spent on website would improve the model. For age, the older customers are likely to have more disposable insome, increasing the likelihood of making purchases. We believed that Number of Purchases would be an obvious indicator in Purcahse Status because the higher the number of purchases made in the past the likelihood of buying more later would be higher. Also, with time spent of website, we thought the longer a customer spent browsing, the higher their interest in the products, leading to a higher likelihood of making a purchase. 

The initial logistic regression model built used all the variables in the dataset. We split the data into testing and training, where our training data contained 1041 rows and testing contains 347 rows. When using all variables, the overall the accuracy is 81%. Looking deeper into the results, we see that the model has better precision for the cases of customers whose purchase status is true with 83%, whereas the recall is higher for purchase status false with 87%.

Although our inital model produced a high accuracy, we still wanted to improve upon this. To refine the model, we used stepwise selection to identify the most significant variables. This process found that Age, Annual Income, Number of Purchases, Time Spent on Website, Loyalty Program, and Discounts Availed were the predictors that most improved the model. This refined model achieved perfect precision, recall, F1-scores, and an overall accuracy of 100%.

The predictive model indicates that businesses can leverage customer attributes such as age, income, purchase history, and website engagement to predict purchase behavior. By identifying customers likely to make purchases, businesses can design targeted marketing campaigns and retention strategies, offering personalized promotions to those predicted to be less likely to purchase and engaging at-risk customers with loyalty rewards.


https://www.kaggle.com/datasets/rabieelkharoua/predict-customer-purchase-behavior-dataset/data.

Link to PowerPoint/Visualizations:
https://docs.google.com/presentation/d/1XG2OAX9YYntooxdoQPU2VrMwmBRurXXUZhefmsOfs1E/edit?usp=sharing
