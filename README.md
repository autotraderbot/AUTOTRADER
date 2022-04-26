

       /   | / / / /_  __/ __ \/_  __/ __ \/   |  / __ \/ ____/ __ \       
      / /| |/ / / / / / / / / / / / / /_/ / /| | / / / / __/ / /_/ /       
     / ___ / /_/ / / / / /_/ / / / / _, _/ ___ |/ /_/ / /___/ _, _/        
    /_/  |_\____/ /_/  \____/ /_/ /_/ |_/_/  |_/_____/_____/_/ |_|

## AUTOTRADER is a tool for automated trading on crypto exchange. This bot uses technical analysis to identify a buy/sell entry points. In order to check your settings you can use simulation option where any trading strategy may be tested. Bot provides trading on binance and kucoin (other platforms are coming soon). Algotithm works with 1 hour timeframe (other timeframes are comming soon). Once bot is launched it creates data.pkl file and data folder in the same directory with bot. Make simulations of trading to check your strategy and launch it on real crypto market! Trading bots are profitable for as long as you can configure them properly. This bot may have profits 1 - 100 % per month depending on settings and market. DO NOT CONSIDER AUTOTRADER AS A MAGIC BOX, USE IT WISELY AND MAKE BACKTESTS OF YOUR SETTINGS BEFORE TO TRADE IN REAL MARKET!!!

# Download

https://github.com/autotraderbot/AUTOTRADER/releases/tag/1.0.0

# Backtest

AUTOTRADER supports running trading simulations. Backtesting is the general method for seeing how well a strategy or model would have done ex-post. Backtesting assesses the viability of a trading strategy by discovering how it would play out using historical data. If backtesting works, traders and analysts may have the confidence to employ it going forward.

![изображение](https://user-images.githubusercontent.com/66214013/164999174-0e45d185-ddd9-43bc-8ffb-2c22838d6423.png)
![res2021-01-0100-00-00-2021-01-3123-00-00](https://user-images.githubusercontent.com/66214013/164999191-aaf8feb5-c2ae-4725-a4d2-435d0d34a339.png)



# Settings
Initial settings are conservative and provide 10 % per month as an average income.
## Test

Test is an option that enables to visualise entry points which trigger the bot to open and close positions.

![testETH](https://user-images.githubusercontent.com/66214013/165062969-5db45ed2-99f2-4d36-ad9c-958833b093b8.png)



## API keys
Bot uses API keys to connect to your account on exchanges. It can be settled in the settings menu. You can find your API and secret keys in your exchange profile API settings.

## Indicators
### RSI
The relative strength index (RSI) is a momentum indicator used in technical analysis that measures the magnitude of recent price changes to evaluate overbought or oversold conditions in the price of a stock or other asset. Default **period** of RSI is 14 but you can increase it in order to find a better extremum points. Also there are **overbought level** and **oversold level** parameters which have standart values 30 and 70 respectively. You can find more at https://www.investopedia.com/terms/r/rsi.asp.

### MACD
Moving average convergence divergence (MACD) is a trend-following momentum indicator that shows the relationship between two moving averages of a security’s price. The MACD is calculated by subtracting the 26-period exponential moving average (EMA) from the 12-period EMA. In MACD setting section you are able to define a **trend length** parameter which indicates how many hours must be passed scince previous intercection of EMAs. Algorithm finds an ongoing intersection in stead of using allready occured intersection in order to increase effectiveness.

![изображение](https://user-images.githubusercontent.com/66214013/164996909-7e972a67-e74d-4e9d-9cc6-22998d98161f.png)


### Trend lines

Trend lines is an indicatopr based on ‘Support’ and ‘resistance’ levels which are terms for two respective levels on a price chart that appear to limit the market’s range of movement. The support level is where the price regularly stops falling and bounces back up, while the resistance level is where the price normally stops rising and dips back down. The levels exist as a product of supply and demand – if there are more buyers than sellers, the price could rise, and if there are more sellers than buyers, the price tends to fall. Bot allows to add as many trading lines as you want. The parameters that define trends are **period** which is defined in hours, **tl_low** and **tl_high** are defined in pecents relative to total distance between support and resistance levels. For example you can use small periods (10-48 hours) to define main traiding and long periods (720 hours ~ 1 month) to define an antisqueeze mechanism.

![изображение](https://user-images.githubusercontent.com/66214013/164997884-c3ec5944-f408-4116-ad6a-549b19e194ab.png)


## Trailing

A trailing is a modification of a typical order that can be set at a defined percentage or dollar amount away from a security's current market price. For a buy position, an investor places a trailing below the current market price to buy at lower price. For a sell position, an investor places the trailing stop above the current market price to sell at a higher price. Trailing is supported only for real trading and is not considered in backtests.

## Grid settings

**Number of averagings** define a number of nodes in your grid. As far as a grid total size is defined automaticaly acording to previous month volatility a **Grid stretching** parameter has default value = 1. If you suggest that the next month volatility would be 2 times greater in comparison with previous one than you should put  **Grid stretching** = 2.

## Additional settings

**Coin list** defines a coins which are allowed to trade.\
**Comparison symbol** defines a traded asset. \
**Take profit** defies a % of desired profit as a signal to sell.\
**Stop loss** defines a % to sell with minimum lesion.\
**Coin num** defines a number of coins which can be traded at the same moment.\
**Tg bot API** defines telegram bot token to notify you.\
**User list** is a list of telegram user's id to nitify with telegram bot.

# Pricing

AUTOTRADER is free to download with it's backtest feature but real trading on exchanges costs 500 $ per 3 month subscribtion period.
