#Cryptocurrency Arbitrage Automation
Overview
This automated trading bot leverages Triangular and Exchange Arbitrages to identify and capitalize on arbitrage opportunities within the cryptocurrency market. The bot continuously scans for disparities in prices across various exchanges, executing trades to generate profits. The bot's versatility extends to multiple cryptocurrency pairs through straightforward configuration.

#Commencing with an initial investment of a Grand, the bot experienced periods of success, yielding around $40 per day for several weeks using Triangular Arbitrage on Bittrex. However, the escalating market volatility subsequently poses challenges, hindering the capacity to consistently surpass the impact of rapid price fluctuations.

#Supported Exchanges
The bot currently supports the following exchanges:
Bittrex
Bitfinex
Bitstamp
Kraken
Gatecoin (Deprecated due to minimal trading volume)

##Installation
If required, install Python 2 from https://www.python.org/downloads/.
Execute pip install grequests.
Duplicate or rename the .key_sample files in the keys directory to .key files, and insert the corresponding API keys. For example, establish a bittrex.key file. It's crucial not to disclose any API keys or the .key file.
Adjust the arbitrage_config.json file to accommodate additional ticker pairs or exchanges.
Usage
##Triangular Arbitrage: Run python main.py -m triangular.
##Exchange Arbitrage: Execute python main.py -m exchange.
By default, the bot operates in mock mode, which identifies and displays potential arbitrage opportunities without executing actual trades. To deactivate mock mode and transition to production mode, include the -p argument.
Challenges

The predominant hurdle involves trading fees, with most exchanges imposing a 0.25% fee. Reducing this fee could significantly augment profits.
On occasion, not all placed orders are executed, necessitating manual intervention for rebalancing. The bot should possess the capability to address such scenarios, such as implementing market orders instead of solely canceling open orders.
Future Enhancements
Integrate exchange rebalancing strategies.
Strategically manage open orders.
Undertake code refactoring to enhance efficiency.
Given the extreme price volatility observed recently, I am temporarily suspending this project. My aspiration is that this endeavor proves beneficial to individuals sharing similar interests.
