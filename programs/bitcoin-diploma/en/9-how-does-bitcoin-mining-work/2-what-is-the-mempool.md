# 9.2 What Is the Mempool?

The **mempool**, short for “memory pool,” is like a waiting room for Bitcoin transactions. When you send bitcoin, your transaction is first broadcast to the network and placed in the mempool.

You can think of it like waiting in line at a restaurant. Your name goes on a list, and you wait until a table is available. In the same way, your transaction waits in the mempool until a miner includes it in a block.

Bitcoin nodes check each new transaction to make sure it is valid and that the bitcoin being spent has not already been used. If the transaction is valid, it stays in the mempool until it is confirmed.

Miners choose transactions from the mempool and include them in new blocks. Usually, transactions with higher fees are chosen first.

Once a transaction is included in a block, it becomes confirmed and is permanently recorded on the Bitcoin blockchain.


---


#### Activity: Exploring the Mempool

https://qr.myfirstbitcoin.org/mempool.pdf

**This activity exposes students to a free and open-source tool that does not require technical skills to use. It is useful for Bitcoiners at all levels, from beginner to experienced.**

###### Key Points

1. **Mempool** refers to the list of unconfirmed transactions maintained by each Bitcoin node, not a specific service or platform.
1. This is no single, universal mempool. Mempool.space is one of many.
1. [Mempool.space](https://mempool.space) is open-sourced and well known for being an easy-to-use visual block explorer. It provides real time data on unconfirmed transactions, fee rates, and other network activity.

###### Student Tip

Mempool.space does much more than visualize blocks. Explore other parts of the Bitcoin ecosystem: e.g., Lightning, mining, the hash rate, pools, and block space "goggles".
