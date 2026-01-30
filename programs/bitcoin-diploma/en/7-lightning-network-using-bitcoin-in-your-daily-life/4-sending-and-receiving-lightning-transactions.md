# 7.4 Sending and Receiving Lightning Transactions

With a Lightning wallet, using Bitcoin is fast, cheap, and private, making transactions between two people easy. You can quickly send and receive bitcoin for everyday things like buying coﬀee or shopping.

Let’s look at a few examples of the Lightning Network in action.

##### Example 1

Below, both Marcia and Eve have 5 units of currency each. Marcia wants to send 2 of her units to Eve but she doesn't have a direct channel with her, so she sends 2 units to Jeﬀ, who is well connected to the network. Jeﬀ then passes on the 2 units to Eve, who now has 7 units. Marcia now has 3 units. And that’s it! The transaction is done.

![ ](https://cdn.sanity.io/images/vje9ehw2/production/a45f29d32babb448dafec3d541203195e66b8293-1962x434.jpg)

Jeﬀ acts as an intermediary in this scenario, where Marcia and Eve can't transact directly: perhaps they don't want to open a direct channel because they don't intend to transact often, for instance if Marcia is visiting a diﬀerent town. The beauty of the Lightning protocol is that neither Marcia nor Eve need to trust that Jeﬀ will relay the funds: thanks to cryptography, only the intended, legitimate recipient can claim the funds; there is no way for Jeﬀ or any other node to intercept them in transit.

The key point here is that Marcia and Eve don't have to trust a third party with the ability to deny the transaction, such as a bank or other centralized intermediary. Jeﬀ is a key element in this peer-to-peer transaction process. As a node operator in a Lightning Network transaction, Jeﬀ benefits in several ways:

1. **Transaction fees**: Jeﬀ earns a small fee for each transaction that passes through his node, which compensates him for the time and eﬀort he puts into maintaining and running his node.
1. **Network participation**: By running a Lightning node, Jeﬀ is participating in the network and helping to increase its decentralization, security, and stability. This can increase Jeﬀ’s reputation and credibility as a reliable node operator, making him a more attractive intermediary for future transactions.
1. **Network growth**: As the Lightning Network grows and more people use it, the number of transactions passing through Jeﬀ’s node is likely to increase, which can result in increased income from transaction fees.
1. **Increased network security**: Jeﬀ’s role as an intermediary helps to increase the network's security by adding an additional layer of protection between Marcia and Eve. This can increase the users' confidence in the network, making it more attractive to new users and helping to drive growth.

Overall, being a node operator in the Lightning Network can provide Jeﬀ with a steady source of income, as well as the opportunity to contribute to the network's growth and development.

In summary, **on-chain transactions are slower but more secure, while oﬀ-chain (Lightning Network) ones are faster but less secure**. You should consider the trade-oﬀ between security and speed depending on your needs.

##### Example 2

Mina has a serious love for McDonald's: she goes there for breakfast, lunch, and dinner every day! But with so many diﬀerent payment options available, she’s not sure which one is the best choice. Luckily, she’s learned a little bit about Bitcoin and the Lightning Network. After comparing the tables below, Mina has no doubt that using a Lightning payment method is the way to go.


|  |  |  |
| --- | --- | --- |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |



|  |  |  |
| --- | --- | --- |
|  |  |  |


![ ](https://cdn.sanity.io/images/vje9ehw2/production/65141160d0eb5eebc56b684053dbd2e22607c9d2-438x226.svg)

Mina is also a fan of fast, secure, and cost-eﬀective transactions, so she decided to use Lightning for her purchases at McDonald’s. With Lightning, she can enjoy her meals even more knowing that her payments are processed instantly, securely, and with low fees. Plus, she doesn't need to open a bank account, which can be diﬃcult or inaccessible in remote areas. Through the Lightning Network, Bitcoin oﬀers financial inclusion to millions of unbanked individuals across the world!

To get started with Lightning, Mina first downloads a Lightning wallet on her phone. She then funds her wallet by sending some bitcoin from her regular Bitcoin wallet to her new Lightning wallet. This process is called “funding the wallet” or “funding a payment channel.” Mina can fund her wallet with any amount of bitcoin she is comfortable with, but it’s important to note that the amount of bitcoin she locks in her Lightning wallet cannot be used in her on-chain transactions.

Once her Lightning wallet is funded, she can use it to make payments to McDonald’s.

McDonald’s has a Lightning node, so Mina can open a payment channel with them by sending some of her bitcoin by making an onchain transaction that locks those funds, for as long as the Lightning channel is open. This moves her bitcoin from the Bitcoin blockchain to an oﬀ-chain channel on the Lightning Network.


> **Note**
>
> With the payment channel open, Mina can now make purchases at McDonald’s without having to open a new channel or pay high fees each time. The channel stays open as long as both Mina and McDonald’s want to use it. For example, if Mina funded the channel with 0.001 bitcoin and she buys a hamburger for 0.00005 bitcoin, the channel tracks that Mina now has 0.00095 bitcoin. And if she buys a milkshake for 0.00003 bitcoin the next day, the channel tracks that Mina now has 0.00092 bitcoin.


When Mina decides she wants to use her bitcoin balance for something else, she closes the channel with McDonald's. This is done by initiating a closing transaction in her Lightning wallet, and the transaction contains the final balance of the channel agreed to by both parties. The transaction is then broadcast to the Bitcoin blockchain and confirmed by a miner. Once the transaction is confirmed, the channel is closed, and the remaining bitcoin in the channel will be returned back to Mina and McDonald’s.

It’s important to note that getting confirmation on the blockchain for the closure of a channel can take some time. During this waiting period, the funds are still locked in the channel and cannot be used for on-chain transactions. Both Mina and McDonald's will receive a notification once the closing transaction is confirmed.

Now that we have set up our Lightning wallet and read about how to use the Lightning Network to send transactions, we are going to play a game where we send satoshis (the smallest unit of bitcoin) to other students in the class over the Lightning Network.

![Lightning Network Map](https://cdn.sanity.io/images/vje9ehw2/production/20a49be467bbe04f8108b38bbf25144522708c3b-504x245.svg)

https://mempool.space/graphs/lightning/nodes-channels-map

This is a map of the entire Lightning Network. Thanks to thousands of Lightning node runners, you can send satoshis to any user with a Bitcoin Lightning wallet, wherever they are in the world. The payment will arrive in a few seconds and will only cost a few cents.

**Check it out for yourself!**


---


#### Activity: Lightning Relay Race

https://qr.myfirstbitcoin.org/lightning.pdf

**This is a hands-on exercise where students send and receive real sats using the Lightning Network.**

##### Key Points

1. Using a Lightning wallet will build your confidence to receive and send real sats.
1. Pay attention to units. Some wallets allow users to send bitcoin OR sats (1/100,000,000 of a bitcoin).
1. Lightning payments can sometimes get hung up in routing, especially for larger payments. Although possible, this kind of user experience is becoming less common as the network matures.

##### Student Tip

Verify with your instructor if/how current on-chain Bitcoin transaction fees will impact the specific Lightning wallet you use.


---
