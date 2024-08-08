# Prophet Challenge: Analysis of traffic and Stock Price trends for MercadoLibre
> Module 8 Homework
> Mercado Libre is a popular e-commerce site in Latin America. The Task is to analyze the company's financial and user data to find trends and formulate potential growth strategies. the code contains the initial analysis of > the company's search traffic  and stock closing prices and build a predictive model to predict fututre stock price changes. The code walks through this analysis in the following steps:

Step 1: Finding unusual patterns in hourly Google search traffic:

> The code here specifically focuses on the month of May 2020  as the cmpany released its financial results. Comparing the seach traffic for the month of May 2020 to the overall monthly median value shows  VALUE OF 1.08 INDICATING 

Step 2: Mine the search traffic data for seasonality:


> In this step the data was processed to review seasonality. There are a few significant patterns in terms of the best time where there is most traffic observed for MercadoLibre:
> On any given day, traffic peaks early in the monring (12:00 am - 2:00 am) and 8:00 pm - 12:00 am) this is typical of customers browzing outside of working hours that may likely contribute to the peaks
> Search trends are n an increasing pattern starting Monday and peak on Tuesdays. Searches then continue on a declining pattern between Wednesday and Saturday. Weekdays see more traffic than weekends.
> Traffic peaks during the first 3 weeks of the year. A second uptick is also observed - building upwards from week 40 and having the highest traffci around week 50. 

> There seems to be a significant uptick in the stock value of Mercadolibre, starting April 2020 and peaking through the end of June 2020. This is not the case with Web traffic during the same timeframe. Web traffic peaks > > went up to an avrage of >60 per day in the first 3 months of the year. There is an observed decrease in traffic starting April 2020 with peak traffic ranging around ~55 per day. While there is an uptick in traffic volume > > at the end of April 2020, we do see that the period between April and June does not pick back up to the peaks of ~60+ hits and hovers below 60. Based on these trends, web traffic does not seem to be the casue of the > > > > increase in stock value.

Step 3: Relate the search traffic to stock price patterns.

> Data procssed here shows there is a very low negative correlation between lagged search trends and stock volatility. There is no evidence of a predictable relationship between lagged search trends and the hourly stock > > > return as well , evidenced by the low positive correlation coefficient of 0.046.

Step 4: Create a time series model with Prophet.

> Phrophet was used in this step to create a timeseries model. The near term forcast shows a dip in web traffic trend post 2020-04. This is out of pattern with seasonality typycally observed during this time.The dip also > > > seems to be lower than the dips seen in prior years. The forecast seems to be fairly accurate given the Yhat upper and yhat lower bounds are tight around the forecasted values. stats were also gathered on usage trends and > show:
> 12:00 am shows the maximum web traffic. Traffic steadily increases from 10:00 am and is the highest during the evening hours and peaks at the end of the day
> Tuesdays show the maximum amount of traffic. trend build up to Tuesday and then steadily drop as the weekend approaches
> The lowest point of traffic in a calendar year occurs in mid October.
