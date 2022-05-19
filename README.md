# Project-1 Technical Analysis - Stocks vs Crypto
**FinTech Group Assessment 1**

- Raelyn Sangil (L)
- Parvinder Rakhra
- Kurt Cullerton


## Project Description

### The Scope

Cryptocurrency (henceforth referred to as crypto) is a digital currency that has been designed to work a medium of exchange through a computer network that is not reliant through on any central authority (government or bank) to uphold and maintain it. [<sup>1</sup>](#reference-list) 

This project provides an analysis of 5 Crypto and 5 Stocks, all high in market values as of 05/05/2022. This analysis will be useful to help beginner traders. It will highlight different elements to consider when performing due diligence prior to purchasing on the Stock Market. 

The project aims to help beginner investors *save* money and *make* money.

### Our Sample

<ins> Crypto Sample - We chose the 5 High Market Price Crypto of 05/05/2022. </ins>

[Source: https://www.coingecko.com/en/api/](https://www.coingecko.com/en/api/)

<ins> Bitcoin *BTC* </ins> - Created and released by Satoshi Nakomoto, this crypto has a limited supply of 21 million and works on a blockchain ledger. It is easily moved from one exchange account or digital wallet to another and easily transferred from one user to another or merchant. Many experts believe that these factors give the Bitcoin the value that it currently has today.[<sup>2</sup>](#reference-list)

<ins> Ethereum *ETH* </ins> - Via blockchain technology, Ethereum is the largest and most well-established, open-ended decentralized software platform. It enables the development of smart contracts and decentralized applications to be built and run without any downtime, fraud, control, or interference from a third party. Ether (ETH) is the fuel used to run commands in the Ethereum platform and is used by developers to build and run applications on the platform.[<sup>3</sup>](#reference-list)

<ins> Litecoin *LTC* </ins> - Litecoin was developed to be a compliment to Bitcoin. Satoshi Nakomoto saw that a major drawback of Bitcoin would be the speed in which it adds blocks. Litecoin has improved speed (2.5 minutes per block on average) and accessibility when compared to Bitcoin. However, this currency has a higher limited supply of 84 million. Litecoin was made to be a more practical and scalable medium than Bitcoin. It is now one of the most recognized, trusted and used blockchain-based payment networks in the world.[<sup>4</sup>](#reference-list)

<ins> Ripple *XRP* </ins> - Ripple is a technology that acts as both a crypto and a digital payment network for financial transactions. It was first released in 2012 and was co-founded by Chris Larsen and Jed McCaleb. Ripple's main process is a payment settlement asset exchange and remittance system, similar to the SWIFT system for international money and security transfers, which is used by banks and financial middlemen dealing across currencies.[<sup>5</sup>](#reference-list)

<ins> Cardano *ADA* </ins> - Other than being a crypto, every ADA holder also holds a stake in the Cardano network. ADA stored in a wallet can be delegated to a stake pool to earn rewards (to participate in the successful running of the network ) or pledged to a stake pool to increase the pool's likelihood of receiving rewards. In time, ADA will also be usable for a variety of applications and services on the Cardano platform. [<sup>6</sup>](#reference-list) 


<ins> Stock Sample - We chose the 5 High Market Price Stocks of 05/05/2022. </ins>

[Source: https://data.nasdaq.com/tools/api](https://data.nasdaq.com/tools/api)

<ins> Apple *AAPL* </ins> - Apple, Inc. engages in the design, manufacture, and sale of smartphones, personal computers, tablets, wearables and accessories, and other variety of related services. [<sup>7</sup>](#reference-list)

<ins> Microsoft *MSFT* </ins>  - Microsoft is the world’s largest software maker. The company, founded by Bill Gates and Paul Allen in 1975, is best known for its software products, including Microsoft Windows operating systems, the Microsoft Office suite, and the Internet Explorer web browser. Microsoft is also known for its hardware products such as the Microsoft Surface touch screen personal computer and the Xbox series of video game consoles.[<sup>8</sup>](#reference-list)

<ins> Google *GOOGL* </ins>  - Google LLC is an American multinational technology company that focuses on artificial intelligence,[10] search engine, online advertising, cloud computing, computer software, quantum computing, e-commerce, and consumer electronics.[<sup>9</sup>](#reference-list)

<ins> Tesla *TSLA* </ins>  - Tesla is a US company involved in car manufacturing and energy. Best described as a battery company, Tesla is best known for its electric cars. The company is also known for specialising in solar panels and Lithium-ion battery energy storage.[<sup>10</sup>](#reference-list)

<ins> Amazon *AMZN* </ins>  - Amazon.com, Inc. is an American multinational technology company which focuses on e-commerce, cloud computing, digital streaming, and artificial intelligence.[<sup>11</sup>](#reference-list)

## Data Cleaning

### Dependancies

- Basic Libraries - os, requests, pandas, dotenv numpy
- Libraries for Pulling Data - alpaca_trade_api, csv, json, datetime
- Libraries for Visualization - plotly.express, hvplot.pandas, matplotlib.pyplot, panel, pn.extension('plotly'), panel.interact, plotly.tools, seaborn
- Libraries for Data Analysis - MCForecastTools
- New Libraries used - yfinance, warnings, warnings.filterwarnings("ignore")

### Clean- up and exploration

We used Alpaca API to import the Stock Market data. Yfinance was used specifically for importing the S&P500 data. Once imported, we chose to use the closing prices for our analysis and then dropped nulls, columns and headings and sorted data where applicable.

All the data sourced from Coingeko came in UNIX datetime format for dates so we had to convert that over. To fix tickers we used .droplevel(axis, level).

Sadly, we noticeed too late that there were inconsistencies between Crypto and Stock data.

## Analysis

> *"There's one golden investment rule that you should always keep in mind: Never invest money that you can't afford to lose. The Market can be rewarding, but it does test you.  Always Do Your Own Research - DYOR"*

Stock Market analysis helps the investors to identify whether the worth of security is valued in the market. If a stock performs poorly, an investor will make a loss. If a stock performs well, an investor can make a profit.[<sup>12</sup>](#reference-list)

There are many ways to complete this due diligence. Reviewing past performance, checking correlations and analysing risk are just a few to mention.

Below are the finds of our analysis.

### Performance of Crypto over the last 5 years

<ins> Bitcoin *BTC* </ins>

![Performance of BTC over the last 5 years](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Performance%20of%20BTC%20over%20the%20last%205%20years.jpg)

<ins> Ethereum *ETH* </ins>

![Performance of ETH over the last 5 years](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Performance%20of%20ETH%20over%20the%20last%205%20years.jpg)

<ins> Litecoin *LTC* </ins>

![Performance of LTC over the last 5 years](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Performance%20of%20LTC%20over%20the%20last%205%20years.jpg)

<ins> Ripple *XRP* </ins> 

![Performance of XRP over the last 5 years](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Performance%20of%20XRP%20over%20the%20last%205%20years.jpg)

<ins> Cardano *ADA* </ins>

![Performance of ADA over the last 5 years](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Performance%20of%20ADA%20over%20the%20last%205%20years.jpg)

### Performance of Stocks over the last 5 years

<ins> Apple *AAPL* </ins>

![Performance of AAPL over the last 5 years](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Performance%20of%20AAPL%20over%20the%20last%205%20years.jpg)

<ins> Microsoft *MSFT* </ins>

![Performance of MSFT over the last 5 years](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Performance%20of%20MSFT%20over%20the%20last%205%20years.jpg)

<ins> Google *GOOGL* </ins>

![Performance of GOOGL over the last 5 years](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Performance%20of%20GOOGL%20over%20the%20last%205%20years.jpg)

<ins> Tesla *TSLA* </ins>

![Performance of TSLA over the last 5 years](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Performance%20of%20TSLA%20over%20the%20last%205%20years.jpg)

<ins> Amazon *AMZN* </ins>

![Performance of AMZN over the last 5 years](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Performance%20of%20AMZN%20over%20the%20last%205%20years.jpg)

### Profit of Each Investment after 5 years

![Profit of Each investment After 5 years](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Profit%20of%20Each%20investment%20After%205%20years.jpg)

### Daily Returns - Crypto

![Daily Returns - Crypto](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Daily%20Returns%20-%20Crypto.jpg)

### Daily Returns - Stocks

![Daily Returns - Stocks](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Daily%20Returns%20-%20Stocks.jpg)

### Return after 5 years with 30 days as Weighted Average

![Return after 5 years with 30 days as Weighted Average](https://github.com/RaelynSangil/Project-1/blob/15658b9010a95dd98898a01592cca2cd233dde6e/Graphs/Return%20after%205%20years%20with%2030%20days%20as%20Weighted%20Average.jpg)

### Return after 6 years

![Return after 6 years](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Return%20after%206%20years.jpg)

### Daily Returns% Change over 5 years

![Daily Returns% Change over 5 years](https://github.com/RaelynSangil/Project-1/blob/15658b9010a95dd98898a01592cca2cd233dde6e/Graphs/Daily%20Returns%20percentage%20Change%20over%205%20years.jpg)

### Correlation Heatmap

![Correlation Heatmap](https://github.com/RaelynSangil/Project-1/blob/15658b9010a95dd98898a01592cca2cd233dde6e/Graphs/Correlation%20Heatmap.jpg)

### Monte Carlo

<ins>Stocks Simulation</ins>

![Monte Carlo 1a](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Monte%20Carlo%201a.jpg)
![Monte Carlo 1b](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Monte%20Carlo%201b.jpg)

<ins>Crypto Simulation</ins>

![Monte Carlo 2a](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Monte%20Carlo%202a.jpg)
![Monte Carlo 2b](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Monte%20Carlo%202b.jpg)

### Sharpe Ratios

![Sharpe Ratios](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Sharpe%20Ratios.jpg)

### Volatility

![Volatility to Blackswan event Covid-19](https://github.com/RaelynSangil/Project-1/blob/15658b9010a95dd98898a01592cca2cd233dde6e/Graphs/Volatility%20to%20Blackswan%20event%20Covid-19.jpg)
![Volatility to Market Uncertainty](https://github.com/RaelynSangil/Project-1/blob/15658b9010a95dd98898a01592cca2cd233dde6e/Graphs/Volatility%20to%20Market%20Uncertainty.jpg)

### Blackswan Event - Covid-19

<ins>How Covid-19 Affected the Crypto and Stock Market in context</ins>

![How Covid-19 Affected the Crypto and Stock Market in context](https://github.com/RaelynSangil/Project-1/blob/15658b9010a95dd98898a01592cca2cd233dde6e/Graphs/How%20Covid-19%20Affected%20the%20Crypto%20and%20Stock%20Market%20in%20context.jpg)

<ins>How Covid-19 Affected the Crypto and Stock Market zoom</ins>

![How Covid-19 Affected the Crypto and Stock Market zoom](https://github.com/RaelynSangil/Project-1/blob/15658b9010a95dd98898a01592cca2cd233dde6e/Graphs/How%20Covid-19%20Affected%20the%20Crypto%20and%20Stock%20Market%20zoom.jpg)

### Blackswan Event - Russia vs. Ukraine War

<ins>How The Russia vs. Ukraine War Affected the Crypto and Stock Market in context</ins>

![How The Russia vs. Ukraine War Affected the Crypto and Stock Market in context](https://github.com/RaelynSangil/Project-1/blob/15658b9010a95dd98898a01592cca2cd233dde6e/Graphs/How%20The%20Russia%20vs.%20Ukraine%20War%20Affected%20the%20Crypto%20and%20Stock%20Market%20in%20context.jpg)


<ins>How The Russia vs. Ukraine War Affected the Crypto and Stock Market zoom</ins>

![How The Russia vs. Ukraine War Affected the Crypto and Stock Market zoom](https://github.com/RaelynSangil/Project-1/blob/15658b9010a95dd98898a01592cca2cd233dde6e/Graphs/How%20The%20Russia%20vs.%20Ukraine%20War%20Affected%20the%20Crypto%20and%20Stock%20Market%20zoom.jpg)

### Weighted Portfolio Comparisons

<ins>Scenario 1 - Portfoloio: 50% Crypto and 50% Stocks</ins>

![Portfoloio 50 Crypto and 50 Stocks](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Portfoloio%2050%20Crypto%20and%2050%20Stocks.jpg)

<ins>Scenario 2 - Portfoloio: 100% Crypto</ins>

![Portfoloio 100 Crypto](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Portfoloio%20100%20Crypto.jpg)

<ins>Scenario 3 - Portfoloio: 100% Stocks</ins>

![Portfoloio 100 Stocks](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Portfoloio%20100%20Stocks.jpg)

<ins>Scenario 4 - Portfoloio: 40% Crypto and 60% Stocks</ins>

![Portfoloio 40 Crypto and 60 Stocks](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Portfoloio%2040%20Crypto%20and%2060%20Stocks.jpg)

<ins>Scenario 5 - Portfoloio: 60% Crypto and 40% Stocks</ins>

![Portfoloio 60 Crypto and 40 Stocks](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Portfoloio%2060%20Crypto%20and%2040%20Stocks.jpg)

<ins>Portfolio Distribution Analysis - Overlay</ins>

![Portfolio Distribution Analysis - Overlay](https://github.com/RaelynSangil/Project-1/blob/821c1fc0b6e90282845b0d9de267b96740476487/Graphs/Portfolio%20Distribution%20Analysis%20-%20Overlay.jpg)

## Conclusion of Analysis

- We found that, of the crypto, BTC has the maxiumum standard deviation and GOOGL has the least over the last 5 years.
- We found that, of the stocks, XRP has the maxiumum standard deviation and AAPL has the least over the last 5 years.
- Our rolling standard deviation indicated volatility in the sample.
- We found that crypto had a consistently higher correlation with all the other stocks over the last 4 years.
- We found that crypto was more volatile than stocks.
- We found that Crypto reacts negatively to major macro economic factions: Covid-19.
- On a long term perspective, crypto assets gave better returns.
- Our portfolio analysis found that the scenario that most efficiently distributed investment funds was to distribute the allocated funds at a 40% Crypto and 60% Stocks split.

## Room for Improvement

### Difficulties

![UNIX Issue](https://github.com/RaelynSangil/Project-1/blob/a0c818ba114b35578dda984b6c9f57023eeb7448/UNIX%20issue.JPG)

- <ins> Coingecko provided dates in UNIX </ins> - As we began cleaning our data for our crypto samples, we noticed that dates were a long string of unknoen numbers. We soon found out it was UNIX datetime format. We googled for example coding and found that the reason we were having difficulty was because the UNIX format was going down to the millisecond and not second as most of the sample code online was suggesting.

- <ins> Some crypto weren't old enough </ins> - As we began cleaning our data, we noticed that LUNA and SOL were not at least 5 years old. As most of our analysis looked at how our sample had faired over a 5 year period, we needed to change these two crypto out for older ones. We chose LTC and XRP. We then had to extend our data cleaning time.

- <ins> Branch pushing </ins> - We had difficulty all the way to presentation day with pushing our branches to the main.

- <ins> Matplotlib graphs </ins> - these graphs were unable to be added to the dashboard. They would not interact.

### Future opportunities

1. **Adjust code so that a user could review any item on the Stock Market** - This would allow the project to go from an analysis to a product or tool. We were unable to make this change due to time constraints.
2. **Analyse how our sample faired on a Day by Day basis** - This would allow our project to introduce the concept of Day Trading to our target audience and analyse our sample on another level. We were unable to make this change due to time constraints.
3. **Analyse how our sample was affected by Twitter comments** - This would have been a great example of how social media can affect the Stock Market. Part of our sample, Tesla would have been great to analyse in relation to Elon Musk tweets. We were unable to make this change due to time constraints and coding skills (data mining).

# Reference list

- [<sup>1</sup> https://en.wikipedia.org/wiki/Cryptocurrency](https://en.wikipedia.org/wiki/Cryptocurrency)
- [<sup>2</sup> https://time.com/nextadvisor/investing/cryptocurrency/why-do-bitcoins-have-value/#:~:text=Limited%20supply%3A%20Bitcoin's%20maximum%20supply,one%20can%20counterfeit%20a%20Bitcoin.](https://time.com/nextadvisor/investing/cryptocurrency/why-do-bitcoins-have-value/#:~:text=Limited%20supply%3A%20Bitcoin's%20maximum%20supply,one%20can%20counterfeit%20a%20Bitcoin.)
- [<sup>3</sup> https://www.investopedia.com/articles/investing/031416/bitcoin-vs-ethereum-driven-different-purposes.asp#:~:text=Ethereum%20Basics,-Blockchain%20technology%20is&text=Ethereum%20enables%20the%20deployment%20of,interference%20from%20a%20third%20party.](https://www.investopedia.com/articles/investing/031416/bitcoin-vs-ethereum-driven-different-purposes.asp#:~:text=Ethereum%20Basics,-Blockchain%20technology%20is&text=Ethereum%20enables%20the%20deployment%20of,interference%20from%20a%20third%20party.)
- [<sup>4</sup> https://www.gemini.com/cryptopedia/litecoin-vs-bitcoin-blockchain#section-litecoin-is-a-complement-to-bitcoin-not-a-competitor](https://www.gemini.com/cryptopedia/litecoin-vs-bitcoin-blockchain#section-litecoin-is-a-complement-to-bitcoin-not-a-competitor)
- [<sup>5</sup> https://www.investopedia.com/terms/r/ripple-cryptocurrency.asp](https://www.investopedia.com/terms/r/ripple-cryptocurrency.asp)
- [<sup>6</sup> https://cardano.org/what-is-ada/#:~:text=Ada%20is%20a%20digital%20currency,recorded%20on%20the%20Cardano%20blockchain.](https://cardano.org/what-is-ada/#:~:text=Ada%20is%20a%20digital%20currency,recorded%20on%20the%20Cardano%20blockchain.)
- [<sup>7</sup> https://www.forbes.com/companies/apple/?sh=7bec23605355](https://www.forbes.com/companies/apple/?sh=7bec23605355)
- [<sup>8</sup> https://fortune.com/company/microsoft/#:~:text=Microsoft%20is%20the%20world's%20largest,the%20Internet%20Explorer%20web%20browser.](https://fortune.com/company/microsoft/#:~:text=Microsoft%20is%20the%20world's%20largest,the%20Internet%20Explorer%20web%20browser.)
- [<sup>9</sup> https://en.wikipedia.org/wiki/Google](https://en.wikipedia.org/wiki/Google)
- [<sup>10</sup> https://techmonitor.ai/what-is/what-is-tesla-4939228](https://techmonitor.ai/what-is/what-is-tesla-4939228)
- [<sup>11</sup> https://en.wikipedia.org/wiki/Amazon_(company)](https://en.wikipedia.org/wiki/Amazon_(company))
- [<sup>12</sup> https://blog.skillsuccess.com/why-is-stock-market-analysis-so-important/#:~:text=Investors%20rely%20on%20stock%20analysis,stock%20market%20as%20a%20whole.](https://blog.skillsuccess.com/why-is-stock-market-analysis-so-important/#:~:text=Investors%20rely%20on%20stock%20analysis,stock%20market%20as%20a%20whole.)
- [<sup>13</sup> https://medium.datadriveninvestor.com/the-sharpe-ratio-with-python-from-scratch-fbb1d5e490b9#:~:text=Evaluating%20a%20Stock's%20Risk%20with%20Python&text=Any%20Sharpe%20Ratio%20above%201.00,3.00%20is%20considered%20very%20good.](https://medium.datadriveninvestor.com/the-sharpe-ratio-with-python-from-scratch-fbb1d5e490b9#:~:text=Evaluating%20a%20Stock's%20Risk%20with%20Python&text=Any%20Sharpe%20Ratio%20above%201.00,3.00%20is%20considered%20very%20good.)
- [<sup>14</sup> https://corporatefinanceinstitute.com/resources/knowledge/trading-investing/exponentially-weighted-moving-average-ewma/](https://corporatefinanceinstitute.com/resources/knowledge/trading-investing/exponentially-weighted-moving-average-ewma/)
