# 9.1 Bitcoin Nodes and Miners

Bitcoin nodes may sound technical, but they are simply software that keeps a copy of the Bitcoin blockchain on a computer. The blockchain is a shared record of all Bitcoin transactions.

When you run your own node, you verify Bitcoin transactions yourself instead of trusting someone else. This gives you more independence and helps keep the Bitcoin network decentralized.

You can think of a Bitcoin node as a digital traffic officer with a few important jobs.

First, it keeps a copy of the blockchain, which is the history of all Bitcoin transactions.

Second, nodes connect with other nodes around the world and share information. One example is the list of new transactions waiting to be confirmed, which is called the mempool.

Third, nodes check that every transaction follows Bitcoin’s rules. If a transaction is invalid, the node rejects it.

Nodes also help new nodes join the network by sharing the blockchain with them. However, every new node still checks all the rules independently.

Anyone can run a node by installing software such as Bitcoin Core and downloading the blockchain. Once it is set up, the node continues to receive new blocks roughly every 10 minutes and verifies them before adding them to its copy of the blockchain.

Running a node helps make the Bitcoin network more secure and decentralized, because more people are independently verifying the system.

#### What Is a Bitcoin Node?

> The purpose of mining is not the creation of new bitcoin; that’s the incentive system. Mining is the mechanism by which Bitcoin’s security is decentralized.  
_Andreas M. Antonopoulos_


> **Callout**
>
> Miners collect unconfirmed transactions, form a block, and use energy to find a key that adds and secures the block.


Miners compete to add the next block of transactions to the blockchain. To do this, they must find a special number that creates a valid block hash. You can imagine it like searching for the right key among billions of possibilities. The first miner to find the correct hash wins the race and earns the right to add their block to the blockchain.

When a miner finds a valid hash, they share their block with the network. Other miners quickly verify that the solution is correct. If it is, the block is added to the blockchain, helping keep Bitcoin’s public ledger secure.

Miners earn bitcoin in two ways:

* **Block rewards:** New bitcoin are created and given to the miner who successfully adds a block to the blockchain.
* **Transaction fees:** When people send bitcoin, they include a small fee. The miner who adds the block receives the fees from the transactions included in that block.

#### Bitcoin Halvings


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12.5 BTC | 6.25 BTC | 3.125 BTC |



> **Callout**
>
> Miners’ rewards for completing one block halve every 210,000 blocks, about every four years.


Bitcoin has a fixed maximum supply of 21,000,000 bitcoin, but all of them were not created when Bitcoin started. Instead, new bitcoin are gradually introduced into circulation through **mining**.

When miners successfully add a new block of transactions to the Bitcoin network, they receive a **block reward** in bitcoin. In the early days of Bitcoin, this reward was 50 bitcoin per block. This reward encouraged people to use computing power and electricity to help secure the network.

About every 210,000 blocks (roughly every 4 years), the block reward is cut in half. This event is called the **halving**. The halving slows down the creation of new bitcoin and helps ensure that the total supply will never exceed 21 million. Over time, this makes bitcoin increasingly scarce.


> **Definition – Circulating supply**
>
> **Circulating supply** refers to the total available amount of a currency. With Bitcoin, the total circulating supply is the number of coins that have been mined and are incirculation at any given time.



> **Definition – Bitcoin supply schedule**
>
> The **Bitcoin supply schedule** is the predetermined and public plan for the release of new bitcoin into circulation, designed to maintain Bitcoin’s scarcity over time.


![ Bitcoin Supply Schedule](https://cdn.sanity.io/images/vje9ehw2/staging/8184cb1c032cab6fd5219e903f8dddc20bdde779-292x200.svg)

After each halving event, the bitcoin reward that miners receive for adding a block is cut in half. This reduces the rate at which new bitcoins are created.

Miners still earn transaction fees from the transactions included in the block they mine. Over time, these fees are expected to become a larger part of miners’ income.

Halvings are built into the Bitcoin protocol and happen automatically about every four years. Because of this, Bitcoin’s supply schedule is predictable and transparent.

The table below shows upcoming halvings, including the approximate date, the block number when they occur, the new block reward, and the percentage of the total bitcoin supply that will have been mined.


| Event | Date | Block | Reward | Mined |
| --- | --- | --- | --- | --- |
| 5th Halving | 2028 | 1,050,000 | 1.5625 BTC | 98.44 % |
| 6th Halving | 2032 | 1,260,000 | 0.78125 BTC | 99.22 % |
| 7th Halving | 2036 | 1,470,000 | 0.390625 BTC | 99.61 % |


As more bitcoin are mined, the circulating supply keeps increasing until the maximum supply of 21,000,000 bitcoins is reached, which is expected around the year 2140. Because fewer new bitcoins are created over time, if demand increases, the price of Bitcoin can rise. This also encourages miners to keep securing the network by contributing their computing power.


---


#### What is a valid block hash in Bitcoin?

In Bitcoin, miners compete to find a special code called a **block hash**. This code identifies a block of transactions and allows it to be added to the blockchain.

Each block contains information about recent transactions and also includes the hash of the previous block. This links every block together, forming a chain from the very first block (the Genesis Block) to the most recent one.

A hash works like a **digital fingerprint** for the data in the block. If any information in the block were changed, the fingerprint would change as well. This makes it easy for anyone to verify that the blockchain’s transaction history has not been altered and helps keep the network secure.


> **Callout**
>
> Satoshi Nakamoto, the creator of Bitcoin, mined the Genesis Block, which unlocked a total of 50 bitcoin.


#### The Race to Mine a Block

Miners compete to find a valid block hash. The first miner to find one gets to add the new block to the blockchain and receive a bitcoin reward.

To be valid, the block’s hash must be lower than a number set by the network called the difficulty target. Because hashes are random, miners must keep trying different inputs until they find one that works.

If too many miners are competing, blocks would be found too quickly. If too few miners are participating, blocks would take too long to find. To keep the system running smoothly, Bitcoin automatically adjusts the difficulty every 2,016 blocks (about every two weeks).

This adjustment ensures that, on average, a new block is added to the blockchain about every 10 minutes.


> **Definition – Definition of difficulty level**
>
> The **difficulty level** in Bitcoin mining measures how hard it is to find a valid block hash. The network adjusts this difficulty every 2,016 blocks (about every two weeks) so that new blocks are added to the blockchain about every 10 minutes. The higher the difficulty, the harder it is for miners to find a valid block.



> **Info**
>
> By finding a valid block hash, a miner proves they have done the work required to add a new block to the blockchain. This process is called Proof of Work (PoW). It is the security mechanism that allows Bitcoin to confirm transactions and add new blocks to the blockchain. The miner who finds the valid hash first earns a reward in bitcoin, which includes the block reward and the transaction fees from the transactions included in that block.


Proof of Work (PoW) helps keep Bitcoin secure by making it extremely expensive for anyone to try to cheat or take control of the network. Instead, it is far more profitable to follow the rules.

Miners play four main roles:

1. **Collect transactions**: Miners choose transactions that have been sent to the network and place them into a candidate block.
1. **Perform Proof of Work**: Miners compete to solve a difficult mathematical puzzle by finding a valid block hash.
1. **Broadcast the block**: The first miner to find a valid solution shares the new block with the network.
1. **Earn rewards**: If the block is valid, it is added to the blockchain and the miner receives newly created bitcoin plus transaction fees.

Many miners around the world try to create the next block at the same time. When one miner finds a valid solution, the network checks the block. If everything is correct, it is added to the blockchain. Other competing blocks are discarded. This process keeps the network in agreement and prevents double-spending.

* Miners are computers that help maintain and update Bitcoin’s ledger.
* They collect transactions and group them into a block. Then they run the block’s data through a hashing algorithm to create a unique code called a hash.
* Miners repeat this process many times, searching for a hash that meets Bitcoin’s rules. The first miner to find a valid hash gets newly created bitcoin as a reward, and their block is added to the blockchain.
* Each block’s hash also connects it to the previous block. If someone tried to change a past transaction, the hashes would no longer match, and the network would reject the altered chain. This is what keeps Bitcoin’s ledger secure.
