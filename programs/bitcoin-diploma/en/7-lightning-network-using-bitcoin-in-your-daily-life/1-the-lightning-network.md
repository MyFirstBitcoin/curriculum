# 7.1 The Lightning Network

The Lightning Network is a payment system that allows users to send and receive bitcoin quickly and inexpensively. It works by setting up a shared wallet where both parties store some of their bitcoin. They can then make unlimited transactions with each other without needing to record each one on the main blockchain. In doing so, they bypass the need to verify and include every single transaction in a block, which makes the process both fast and cost-eﬀective. The lower fees mean that the Lightning Network can be used for small payments which are not always viable on-chain. Once the parties decide to end their collaboration, only the final balance is recorded on the blockchain.

Picture a day spent doing some work in a café. Anticipating a full day's stay, you open a tab and prepay some money instead of paying each time you order something. When you're ready to leave at the end of the day, you and the owner review the tab to settle the final bill. If your upfront deposit exceeds the total amount of your final bill, you will receive back whatever amount you did not spend; if you ended up consuming more than your deposit, you will have to pay the owner whatever the diﬀerence is to settle the tab.

This scheme can scale to include more participants. For instance, on one of your visits to the café , you bring a friend who the bartender doesn’t know and can’t open a tab. You oﬀer your friends your existing tab to cover their expenses, and agree they will repay you privately. Now imagine thousands of people doing the same thing simultaneously, allowing others to use existing tabs to connect with even more individuals — that show the Lightning Network works!

With Lightning, you can make payments to anyone on the network, not just the person you share a direct tab with — provided a route between the two parties can be found. Your payment can navigate through the network until it reaches its destination, even if you don't have an open channel directly with the recipient.

Let’s take a look at the diﬀerence between on-chain transactions (which we discussed in Chapter 6) and oﬀ-chain transactions (Lightning Network).

##### On-Chain Transactions

![ ]

These are transactions that happen directly on the Bitcoin blockchain. They take about 10 minutes to confirm, and the fees depend on the size of the transaction in virtual bytes. They are more secure slower, since they require the consensus of the network.

##### Oﬀ-chain Transactions (Lightning Network)

![ ]

These transactions happen on a separate network built on top of the Bitcoin blockchain. They settle faster and with lower fees.

They are commonly used where considerations like the speed and cost of transactions are more important. Compared to on-chain transactions, they are less secure.


| Payment Network | Bitcoin Network | Lightning Network |
| --- | --- | --- |
| Definition | A decentralized digital network that uses cryptography to secure financial transactions. | A second layer payment protocol that operates on top of the Bitcoin blockchain, enabling faster and cheaper transactions. |
| Advantages | Decentralized and secure. No chargebacks or fraud. Can be used pseudonymously. Global acceptance. | Faster and cheaper transactions. Increased scalability. Off-chain transactions do not clog the blockchain. |
| Disadvantages | Slow transaction times. High fees for certain types of transactions. Complex for beginners. | Can require trust in the channel operators. Not yet as widely adopted as Bitcoin. Requires on-chain transaction to open and close channels. |
