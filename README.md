#   **Dynamic-Trading-Algorithm**
Our motivation for this project was to see if we could create an algorithm that would effectively at reading the market & create a profitable model which could the potential for chat bot integration. 
## **Finding Data**
--- 
We first used an alpacas API to bring in over a decade of market data as we found early on would be critical as our models/algorithm won't act with short term data sets.

## **Data Preparation** 
---
Once we brought in the data, we then needed to format it, and we decided to bring in the data using a 50/200 moving day split. If the value was higher after 200 moving days compared to the 50 moving day data set it will trigger a sell signal. Similarly, if the data brought in is lower after 200 moving days compared to the 50 moving day data set, it will trigger a buy signal. 
## **Model Training & Evaluation**
---
We then trained the data using 2 seperate models, one of which being SVM, and the other logistical regression. Once we plugged the data set into the models we found that the the though the models produced similar results, the drawback of the logistical regression model resulted in a riskier outcome than SVM.



## **Trading & Profit**
---
Using the SVM model, we plug the model into the trading algorithm of which uses the data set that was put into a DataFrame from the model, to decide when to buy/sell based on the capital price of the share compared to the historical data.

## **Summary**
---
We created a profitable algorithm that could bring in market data through an API, and evaluate the data sets based on different models. Given more time, we would've like to integrate lambda utilize a chat bot UI, along with test/integrate different models.
# **Trading Bot Demo**
Initialize the bot with a welcome message and using some of the options to demo the bot.
[Wake up the bot](https://github.com/ZacharyWilkinson/Dynamic-Trading-Algorithm-/blob/1c7191cbb7487b63ffb97310f1f6c13c8eb9fe0d/Images/snapbot1.PNG),[ then select what you'd like to do](https://github.com/ZacharyWilkinson/Dynamic-Trading-Algorithm-/blob/1c7191cbb7487b63ffb97310f1f6c13c8eb9fe0d/Images/snapbot2.PNG)
.[When selecting a strategy, choose which model you'd like to use](https://github.com/ZacharyWilkinson/Dynamic-Trading-Algorithm-/blob/1c7191cbb7487b63ffb97310f1f6c13c8eb9fe0d/Images/snapbot3.PNG)
[and select the ticker you would like to use.](https://github.com/ZacharyWilkinson/Dynamic-Trading-Algorithm-/blob/1c7191cbb7487b63ffb97310f1f6c13c8eb9fe0d/Images/snapbot4.PNG)
[Finally, view the results.](https://github.com/ZacharyWilkinson/Dynamic-Trading-Algorithm-/blob/1c7191cbb7487b63ffb97310f1f6c13c8eb9fe0d/Images/snapbot5.PNG)