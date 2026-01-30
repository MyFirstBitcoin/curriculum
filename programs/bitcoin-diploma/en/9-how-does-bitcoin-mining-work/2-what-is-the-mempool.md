# 9.2 What Is the Mempool?

The “mempool” or memory pool is like a waiting room for transactions in the Bitcoin network. When you make a transaction, it is first broadcasted to the mempool before it is verified, selected, and added to the blockchain.

Imagine you are waiting in line at a restaurant. Your name is added to a list of people waiting for a table. When a table becomes available, the host calls your name and seats you. Similarly, a bitcoin transaction is added to the mempool when it is made and is confirmed and added to the blockchain when a miner includes it in a block.

The **mempool** is where transactions wait to be confirmed into a block.

![ ](https://cdn.sanity.io/images/vje9ehw2/production/601fdb412519d6124cf0d88b8292f5464339deb8-188x105.svg)

When a node first receives a transaction from a peer, it has to verify that the transaction is legit. Nobody wants faulty or deceptive transactions.

The main purpose of the **mempool** is to:

1. Relay unconfirmed transactions
1. Provide miners transactions to mine


> **Callout**
>
> _Mempool synchronization_ allows nodes to share their transactions with other nodes by sending a message containing a list of **verified transactions** in the mempool.


##### How Are Transactions Verified and Added to the Mempool?

![ ](https://cdn.sanity.io/images/vje9ehw2/production/b92f229e8e7a41e22315e07e20a65f9048a24faf-169x102.svg)

When new transactions are broadcast to the Bitcoin network, nodes verify these transactions to make sure they are valid and that the funds have not been spent before. Once these transactions are verified, the nodes will add them to their mempool. The nodes will then share the transactions with other nodes to double check. Finally, if the majority of nodes agree, the transactions will be made available for miners to select and include them in a block. There are several reasons why a transaction might not be confirmed after 72 hours:

1. **Low Transaction Fees**: Transactions with low fees may not be processed quickly enough as miners are more likely to choose transactions with higher fees to include in their blocks.
1. **Network Congestion**: If the network is congested, there may be a delay in confirming transactions, even if they have a high fee.
1. **Double-Spend Attempt**: If a malicious actor attempts to double spend, their transaction will be rejected by the network.
1. **Incorrect or Incomplete Data**: If a transaction contains incorrect or incomplete data, it will be rejected by the network.
1. **Malformed Transaction**: If a transaction is malformed, it will be rejected by the network.

To avoid delays, it’s recommended to include a fee that is high enough to ensure the transaction is processed in a timely manner and to double check that all the data in the transaction is correct before sending it.


---


#### Activity: Exploring the Mempool

https://qr.myfirstbitcoin.org/mempool.pdf

**This activity exposes students to a free and open-source tool that does not require technical skills to use. It is useful for Bitcoiners at all levels, from beginner to experienced.**

##### Key Points

1. **Mempool** refers to the list of unconfirmed transactions maintained by each Bitcoin node, not a specific service or platform.
1. This is no single, universal mempool. Mempool.space is one of many.
1. [Mempool.space](https://mempool.space) is open-sourced and well known for being an easy-to-use visual block explorer. It provides real time data on unconfirmed transactions, fee rates, and other network activity.

##### Student Tip

Mempool.space does much more than visualize blocks. Explore other parts of the Bitcoin ecosystem: e.g., Lightning, mining, the hash rate, pools, and block space "goggles".


---
