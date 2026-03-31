# 7.1 The Lightning Network

The Lightning Network is a payment system that allows users to send and receive bitcoin quickly and inexpensively. It works by setting up a shared wallet where both parties store some of their bitcoin. They can then make unlimited transactions with each other without needing to record each one on the main blockchain. In doing so, they bypass the need to verify and include every single transaction in a block, which makes the process both fast and cost-eﬀective. The lower fees mean that the Lightning Network can be used for small payments which are not always viable on-chain. Once the parties decide to end their collaboration, only the final balance is recorded on the blockchain.

Picture a day working in a café. Planning to stay a while, you open a tab and prepay instead of paying for each order. At the end of the day, you and the owner review the tab to settle the bill. If your deposit is more than what you spent, you get the difference back; if you spent more, you pay what you still owe.

This scheme can scale to include more participants. For instance, on one of your visits to the café, you bring a friend who the bartender doesn’t know and can’t open a tab. You oﬀer your friends your existing tab to cover their expenses, and agree they will repay you privately. Now imagine thousands of people doing the same thing simultaneously, allowing others to use existing tabs to connect with even more individuals — that show the Lightning Network works!

With Lightning, you can make payments to anyone on the network, not just the person you share a direct tab with — provided a route between the two parties can be found. Your payment can navigate through the network until it reaches its destination, even if you don't have an open channel directly with the recipient.

Let’s take a look at the difference between on-chain and off-chain transactions.

##### On-Chain Transactions

These are transactions that happen directly on the Bitcoin blockchain. They take about 10 minutes to confirm, and the fees depend on the size of the transaction in virtual bytes. They are more secure slower, since they require the consensus of the network.

##### Lightning Network Transactions

These transactions happen on a separate network built on top of the Bitcoin blockchain. They settle faster and with lower fees. They are commonly used where considerations like the speed and cost of transactions are more important. Compared to on-chain transactions, they are less secure.


|  | Bitcoin Network | Lightning Network |
| --- | --- | --- |
| Definition | A decentralized digital network that uses cryptography to secure financial transactions. | A second layer payment protocol that operates on top of the Bitcoin blockchain, enabling faster and cheaper transactions. |
| Advantages | Decentralized and secure. No chargebacks or fraud. Can be used pseudonymously. Global acceptance. | Faster and cheaper transactions. Increased scalability. Off-chain transactions do not clog the blockchain. |
| Disadvantages | Slow transaction times. High fees for certain types of transactions. Complex for beginners. | Can require trust in the channel operators. Requires on-chain transaction to open and close channels. |
