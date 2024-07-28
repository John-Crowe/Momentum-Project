# Momentum Portfolio

For this momentum portfolio project, I will be using CRSP stock data to replicate the momentum decile returns in the 2016 paper, "Momentum Crashes" by Daniel and Moskowitz. The objective of this project is to determine the average annual returns for 10 different momentum portfolio deciles. Each decile categorizes every stock based on the total return for the last year of each stock. The bottom decile stocks provided the worst returns for the past year and the top deciles were the top performers of the past year. We also create the momentum portfolio outlined by Ken French (KRF) and compare it's returns to that of the Daniel and Moskowitz (DM) portfolio.

The risk free rate is from the French Fama numbers (not CRSP), which I download below. I combine the dlret and ret data for the stocks and create a new 'ret' column to encompass all returns for the stocks. I filter the stocks to only use the 10 and 11 sharecodes and the 1, 2 and 3 exchanges, per the French Fama website. 

# Relevant Libraries

* wrds
* pandas
* pandas_datareader
* datetime
* numpy

