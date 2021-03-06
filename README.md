
![лого](https://user-images.githubusercontent.com/104389384/166113023-8a07fb9d-2f11-4a5f-9563-320b949fbcf9.PNG)


## AUTOTRADER – automated trading solution for crypto exchanges and it's analysis. The Bot supports unlimited number of connected accounts. It is a powerful tool for professional traders, on the other hand, it is easy to use for beginners. Algorithm of AUTOTRADER suggests long term trading strategies and provides the result minimum within a month of working. This bot uses technical analysis to identify a buy/sell entry points and is capable of watching several assets simultaneously. In order to verify customized settings, you can use simulation option where any trading strategy may be tested. At the moment Bot provides trading algorithms for Binance and Kucoin exchanges (other platforms are coming soon). Algorithm works with 1 hour timeframe (other timeframe options are coming soon). Create simulations/testing environments to proof your strategy and launch it on real crypto market. Trading bots are profitable for as long as you can configure them properly. AUTOTRADER generates profits 1 - 100 % per month depending on settings and the market. Set custom automated trades and never miss a rally or get caught in a dip. AUTOTRADER obsessively seeks out effective market indicators to enable smart allocation of funds while putting you in control of your trading machine.

# Download
https://github.com/autotraderbot/AUTOTRADER/releases/tag/1.0.1


# Notifications

AUTOTRADER allows to turn on telegram notifications of trading signals for customers.

# Backtest

AUTOTRADER supports running trading simulations. Backtesting is the general method for seeing how well a strategy or model would have done ex-post. Backtesting assesses the viability of a trading strategy by discovering how it would play out using historical data. If backtesting works, traders and analysts may have the confidence to employ it going forward. **Backtest strategy** function reproduces the same behavior of the bot as if it was trading during the simulation period. Trailing option is considered only during real traiding.

![res2021-01-0100-00-00-2021-01-3123-00-00](https://user-images.githubusercontent.com/66214013/164999191-aaf8feb5-c2ae-4725-a4d2-435d0d34a339.png)


# Market analysis

AUTOTRADER's functionality provides live technical analysis of price data of any trading asset and this is absolutely free! You can ensure bot's efficiency simply by following it's signals. 

![testXTZ](https://user-images.githubusercontent.com/104389384/165693293-b53bad5e-5867-4fb0-8a47-99d04ee5d12a.png)


# Settings
Initial settings are conservative and provide 10 % per month as an average income. Flexibility of settings allows to tune trading algorithm with respect to different market trends (bullish, bearish). Once bot is launched it creates data.pkl file and data folder in the same directory with bot. data.pkl contains all the settings parameters and data folder stores csv data. 


## API keys
Bot uses API keys to connect to your account on exchanges. It can be settled in the settings menu. You can find your API and secret keys in your exchange API settings.


## Indicators

### Trend lines

Trend lines is an indicatopr based on ‘Support’ and ‘resistance’ levels which are terms for two respective levels on a price chart that appear to limit the market’s range of movement. The support level is where the price regularly stops falling and bounces back up, while the resistance level is where the price normally stops rising and dips back down. The levels exist as a product of supply and demand – if there are more buyers than sellers, the price could rise, and if there are more sellers than buyers, the price tends to fall. Bot allows to add as many trading lines as you want. The parameters that define trends are **period** which is defined in hours, **tl_low** and **tl_high** are defined in pecents relative to total distance between support and resistance levels. For example you can use small periods (10-48 hours) to define main trading channels and long periods (720 hours ~ 1 month) to define an antisqueeze mechanism. **Dynamic trend lines** parameter enables to trace trends with taking into account latest hours, this feature works good in bullish scenario and must be switched off during bearish period.

![TLXRPperiod48](https://user-images.githubusercontent.com/104389384/165706402-87a7d874-747f-4060-9e0e-d07fe825e4d1.png)

### MACD
Moving average convergence divergence (MACD) is a trend-following momentum indicator that shows the relationship between two moving averages of a security’s price. The MACD is calculated by subtracting the 26-period exponential moving average (EMA) from the 12-period EMA. In MACD setting section you are able to define a **trend length** parameter which indicates how many hours must be passed scince previous intercection of EMAs. Algorithm finds an ongoing intersection in stead of using allready occured intersection in order to increase effectiveness.

![macdATOM](https://user-images.githubusercontent.com/104389384/165700345-e2ed8e8f-b512-4686-b136-e64dc0dc416d.png)

### RSI
The relative strength index (RSI) is a momentum indicator used in technical analysis that measures the magnitude of recent price changes to evaluate overbought or oversold conditions in the price of a stock or other asset. Default **period** of RSI is 14 but you can increase it in order to find a better extremum points. Also there are **overbought level** and **oversold level** parameters which have standart values 30 and 70 respectively.
![RSIATOM](https://user-images.githubusercontent.com/104389384/166115719-9870b214-ae36-4af4-9529-db555a792b36.png)




## Trailing

A trailing is a modification of a typical order that can be set at a defined percentage or dollar amount away from a security's current market price. For a buy position, an investor places a trailing below the current market price to buy at lower price. For a sell position, an investor places the trailing stop above the current market price to sell at a higher price. Trailing is supported only for real trading and is not considered in backtests.

## Grid settings

**Number of averagings** define a number of nodes in your grid. As far as a grid total size is defined automaticaly acording to previous month volatility a **Grid stretching** parameter has default value = 1. If you suggest that the next month volatility would be 2 times greater in comparison with previous one than you should put  **Grid stretching** = 2.

## Additional settings

**Coin list** defines a coins which are allowed to trade.\
**Comparison symbol** defines a traded asset. \
**Take profit** defies a percent of desired profit as a signal to sell.\
**Stop loss** defines a percent to sell with minimum lesion.\
**Coin num** defines a number of coins which can be traded at the same moment.\
**Tg bot API** defines telegram bot token to notify you. tg bot token may be obtained thru https://t.me/Bott_Father. \
**User list** is a list of telegram user's id to notify with telegram bot. Use tg bot @userinfobot to find your telegram id. \
After the definition of **Tg bot API** and **User list** you have to press /start command at tg bot. 


## DISCLAIMER 
AUTOTRADER does not provide financial, investment, legal or any other professional advices. AUTOTRADER provides the software. AUTOTRADER - is not a broker, a financial consultant, an investment consultant or a portfolio manager. Nothing in the software should be interpreted as investment recommendations (for example, recommendations regarding whether to purchase currency or other tools). You recognize and agree that AUTOTRADER is not responsible for using any information that you receive inside the software. Your decisions based on the technologies within the software or services in the software, or your interpretations of data found in the software are your own strategy for which you are fully responsible.





