# 7.4 Sending and Receiving Lightning Transactions

With a Lightning wallet, using Bitcoin is fast, cheap, and private, making transactions between two people easy. You can quickly send and receive bitcoin for everyday things like buying coffee or shopping.

Let’s look at a few examples of the Lightning Network in action.

###### Example 1

Both Marcia and Eve have 5 units of currency. Marcia wants to send 2 units to Eve. The payment travels through Jeff, who helps pass the payment along the Lightning Network. After the payment is completed, Eve has 7 units and Marcia has 3.

Jeff helps route the payment, but he cannot steal the funds. The Lightning Network uses cryptography to ensure that only the intended recipient can receive the payment. Jeff simply helps the payment move through the network.

This shows a key advantage of the Lightning Network: people can send payments quickly without trusting intermediaries like banks.

Node operators like Jeff can also earn small fees for helping route payments. By doing this, they help the network remain decentralized and efficient.

Compared to regular Bitcoin transactions:

* **On-chain transactions** happen directly on the Bitcoin blockchain. They are very secure but can be slower and more expensive.
* **Lightning transactions** happen off-chain and allow payments to move much faster and at a much lower cost.

Because of this, Lightning is useful for small, everyday payments, while on-chain transactions are often used for larger transfers or long-term storage.

###### Example 2

Mina loves eating out and often stops by her favorite local café. With so many different payment options available, she isn’t sure which one is the best choice. Luckily, she has learned a little about Bitcoin and the Lightning Network. After reviewing her options, Mina realizes that using a Lightning payment method is the best option.

Mina wants to buy a coffee, but paying with a regular Bitcoin transaction can sometimes take time and require higher fees. Instead, she decides to use the Lightning Network.

The Lightning Network allows people to send bitcoin instantly and with very low fees. This makes it ideal for small, everyday purchases like coffee.

To start using Lightning, Mina downloads a Lightning wallet on her phone. She then sends some bitcoin from her regular Bitcoin wallet to her Lightning wallet. This step uses a normal Bitcoin transaction on the blockchain. Once the funds are in her Lightning wallet, they can be used on the Lightning Network.

Now Mina can pay the café instantly using Lightning. The payment happens off the main Bitcoin blockchain, which is why it is much faster and cheaper than a regular on-chain transaction.


| Benefits | Lightning Network | Traditional Banking System |
| --- | --- | --- |
| Speed | Fast | Slow |
| Transparency | Transparent | Opaque |
| Security | Secure | Vulnerable |
| Transaction fees | Low | High |
| Financial inclusion | High | Limited |
| Scability | High | Low |
| Privacy | High | Moderate |
| Interoperability | High | Low |
| Legal compliance | Moderate | High |
| Cost-effectiveness | High | Moderate |


In simple terms, on-chain transactions happen directly on the Bitcoin blockchain and can take more time and fees. Lightning transactions happen off-chain, allowing fast and low-cost payments while still using bitcoin.


| Visa, Inc. | Bitcoin On-chain | Lightning Network |
| --- | --- | --- |
| Capacity of 65000 transactions per second. | Capacity of 7 transaction per second. | Capacity of millions transactions per second. |


![Lightning Network Map](https://cdn.sanity.io/images/vje9ehw2/staging/5a760247cf4c32074c62f40aea8dc21095882740-504x245.svg)

https://mempool.space/graphs/lightning/nodes-channels-map

This is a map of the entire Lightning Network. Thanks to thousands of Lightning node runners, you can send sats to any user with a Bitcoin Lightning wallet, wherever they are in the world. The payment will arrive in a few seconds and will only cost a few cents.

**Check it out for yourself!**


---


#### Activity: Lightning Relay Race

https://qr.myfirstbitcoin.org/lightning.pdf

**This is a hands-on exercise where students send and receive real sats using the Lightning Network.**

###### Key Points

1. Using a Lightning wallet will build your confidence to receive and send real sats.
1. Pay attention to units. Some wallets allow users to send bitcoin OR sats (1/100,000,000 of a bitcoin).
1. Lightning payments can sometimes get hung up in routing, especially for larger payments. Although possible, this kind of user experience is becoming less common as the network matures.

###### Student Tip

Verify with your instructor if/how current on-chain Bitcoin transaction fees will impact the specific Lightning wallet you use.
