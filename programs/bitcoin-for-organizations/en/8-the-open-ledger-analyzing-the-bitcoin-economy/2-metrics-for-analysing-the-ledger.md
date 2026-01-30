# 8.2 Metrics for Analysing the Ledger

Because Bitcoin’s transparency is unlike traditional financial systems — where much of the monetary flow happens behind closed institutional doors — it gives rise to a rich field of on-chain analytics, where network-level data becomes a lens for understanding user behaviour, monetary flows and long-term trends. These metrics can help answer specific queries, such as how actively the network is being used, whether coins are being accumulated or sold off, and whether the network is becoming more secure.

Understanding these metrics is helpful not only for Bitcoin users, but also for researchers or policymakers seeking insight into this uniquely transparent financial system.

This section contains some commonly used metrics for analysing Bitcoin activity grouped into sub categories. It is not a comprehensive list. Visit [www.bitcoinmagazinepro.com/charts](https://www.bitcoinmagazinepro.com/charts) for a fuller list and descriptions.



#### 8.2.1 Address Metrics

Address metrics are useful to monitor over time as they indicate the level of activity on the Bitcoin network. For instance, as Bitcoin becomes more adopted, the number of active addresses increases. We can examine this further by distilling the number of addresses that hold a minimum specified amount of Bitcoin, say 0.1 BTC, by a certain time period, such as one year. While this provides a view of Bitcoin adoption over time, it is imperfect since an individual can hold multiple Bitcoin addresses. Conversely, exchanges or ETFs may appear as single entities when holding funds for large numbers of individuals.

![Bitcoin: Addresses Hodling > X BTC by Year](Bitcoin: Addresses Hodling > X BTC by Year)

_Addresses Hodling Bitcoin > X BTC by Year. Source: Bitcoin Magazine Pro._

By comparing addresses with the current market price of BTC it is possible to view the percentage of overall Bitcoin addresses in profit. This allows us to track market sentiment as we can see what proportion of the market is holding on to BTC at a profit or loss.

For example, the **Percent Unrealised Profit** chart below shows the proportion of all ledger addresses with an unrealised profit measured in US dollars. Note that, since the chart below was taken at close to Bitcoin’s all-time high, the percentage of addresses showing an unrealised profit is close to one hundred per cent. We can also see that prolonged periods of Percent Unrealised Profit below one standard deviation from the mean are unusual. Therefore, a drop below this line may suggest a good entry point for buyers.

![Percent Unrealised Profit](Percent Unrealised Profit)

_Percent Unrealised Profit. Source: checkonchain.com_



#### 8.2.2 On-Chain Indicators

On-chain indicators are useful because they offer an insight into network behaviour, beyond what price and address metrics alone can show. They help analysts understand the actions and sentiment of different types of participants, such as long-term holders versus short-term traders by tracking how coins are being held, moved, or valued over time. These indicators draw on the transparent nature of the ledger to reveal hidden market dynamics like accumulation, distribution, or even investor conviction. This makes them particularly useful for identifying structural trends, assessing whether the market is overheated or undervalued, and anticipating turning points in a market cycle.

For instance, by examining the value of BTC holdings since they were last transacted, we can deduce whether or not the market is under distress (as it might be during a major cycle low). This metric is known as **Realised Price** and gives us an ‘average cost basis’ of all BTC in circulation. If the market price drops below Realised Price, this shows that on aggregate the majority of addresses are holding a paper loss.

By further grouping ledger data into age bands, we can show how the amount of BTC moves between addresses over time, which creates wave-like patterns on a chart known as **HODL waves**.

![Bitcoin HODL Waves](Bitcoin HODL Waves)

_Bitcoin HODL Waves. Source: Bitcoin Magazine Pro._

The HODL waves show what long-term, medium-term and short-term holders are doing with their BTC. For instance, in the chart above, short-term holders are shown in red and orange and we can see spikes in activity as this group rushes to buy near market tops. At the other end, we can see that very long-term holders (in purple and blue) are steadily increasing in overall share of the network, indicating high conviction among these groups. The chart is imperfect since some coins can move from old to new addresses under the control of the same user. However, it does provide an interesting view of the conviction of long-term holders.

Another way of examining the ‘smart money’ of long-term holders is to examine **Coin Days Destroyed** (CDD). The concept of ‘Coin Days’ is a multiple of the number of BTC multiplied by the days since the coins last moved. For instance, 5 BTC that has not moved for 100 days has accumulated 500 coin days and 10 BTC that has not moved for 10 days has accumulated 100 coin days. In this way, we give extra weighting to coins held for longer. When those coins are moved those coin days are ‘destroyed’. This indicator shows increases in CDD at times of significant price movements, which provides analysts with a way of separating routine market activity from meaningful shifts in longer-term holder sentiment.

Another metric that may help identify whether the market is undervaluing or overvaluing BTC is the Market-Value to Realised Value or **MVRV**. It is calculated simply as the ratio of Market Value (number of BTC in issue multiplied by the market price) divided by the Realised Value (the sum of all BTC since they were last moved). A high MVRV suggests more coins are in profit (often seen near market tops) and a low MVRV indicates many coins are held at a loss (seen near market lows).



#### 8.2.3 Mining Metrics

Mining metrics are useful for understanding the security, economic incentives and overall health of the Bitcoin network. Metrics such as hashrate, miner revenue, difficulty, and fee ratios reveal how much computational power is securing the blockchain and how well miners are being compensated for their activities.

The **Hashrate** of the Bitcoin network is perhaps the commonly referred to indicator of the network health and strength of security. Since the process of mining secures the network and confirms that transactions on the ledger are valid, the greater the level of computing (or hashing) power there is, the harder it would be for a malicious actor to overpower and attack the network.

![Bitcoin Hashrate](Bitcoin Hashrate)

_Bitcoin Hashrate. Source: Bitcoin Magazine Pro._

The chart above shows that, in May 2025, the total computing power of the network stands at around 900 TeraHash/s (900 Trillion cryptographic ‘hash’ calculations per second). If the hashrate is rising, it shows that the network is becoming more secure, which is reassuring for users.

The Puell Multiple (devised by David Puell) looks at the market cycle from the perspective of miners and their revenue. The metric is calculated by dividing the daily issuance of BTC (in USD) by the 365-day moving average of daily issuance value. The metric helps to identify periods of miner stress or relief. Historically, a multiple above 3 has preceded a decline in market value of BTC, since it indicates that miners are highly-profitable. A value below 0.5 indicates stress and has historically indicated market lows for the value of BTC.
