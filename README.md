# StockPred_LSTM
Take in stock information and make a prediction on whether the stock will decrease by 5%, decrease by 2%, increase by 2%, increase by 5%, or remain unchanged. Please don't use this for actual day trading. I am not responsible for any losses or gains. 


**What is the motivation behind StockPred_LSTM?**

Predicting the exact stock price is difficult, and doing so in a short period of time is unfeasible because a normal person will never have access to the resources of a investment firm or trading company. Therefore, I predict whether the price will fluctuate within some range over the course of a week. This way, you are not competing against large firms with infinitely more resources.

**How does StockPred_LSTM work?**

We take in stock data, which is correlated in time to a certain extent, and feed it into a LSTM. The output is the exact price for the next 5 days, but we classify those predictions into 5 bins. -5% change, -5%:2% change, -2%:2% change, +2%:5% change, and +5% change.

<img width="304" alt="image" src="https://user-images.githubusercontent.com/111892527/221701542-888a046b-424a-4853-9cdb-c2ba1e3ac658.png">


**What can we do with StockPred_LSTM?**

Download any stock price and predict the following 5 days. Some stock predictiosn are more accurate than others.

<img width="207" alt="image" src="https://user-images.githubusercontent.com/111892527/221702139-432ad6d6-5ed7-4488-acf0-5e8dab614000.png">

For example VZ stock has a class accuracy of close to 70%.
