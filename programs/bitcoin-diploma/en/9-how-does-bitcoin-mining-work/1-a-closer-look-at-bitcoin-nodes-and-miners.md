# 9.1 A Closer Look at Bitcoin Nodes and Miners

![ ]

Bitcoin nodes may sound technical, but they are just software running a copy of the Bitcoin ledger on a piece of hardware. When you run your own Bitcoin node, you gain sovereignty over the validation of your own transactions, but also a voice in shaping the rules of the Bitcoin network.

Imagine this: if a group of people were to try to change how Bitcoin functions (say by altering the total supply of bitcoin) you, as a full participant in the network, would have a say. You can choose not to update your node to the new system and continue running the original version — like voting to enforce the rules of the network you support, except that the majority can't force you to run their version.

**Let’s think of a Bitcoin node as a digital traﬃc oﬃcer charged with some essential tasks:**

1. **Gatekeepers of Validation**: A Bitcoin node keeps an updated digital copy of the blockchain, which is like a shared ledger of all Bitcoin transactions. Many nodes around the world hold this same record.
1. **Communication Hub**: Nodes connect with one another, creating a vast communication network. They share information, especially the list of transactions waiting to be added to the blockchain, which is stored in a "digital waiting room" called the “mempool."
1. **Quality Checker**: Each addition to the blockchain undergoes careful scrutiny. Nodes ensure that transactions are valid, rejecting any that don't adhere to the rules of the Bitcoin network.
1. **Blockchain Informant**: Other software, like wallets, can ask a node for information about the blockchain, such as bitcoin balances. Nodes serve as an archive for the history of Bitcoin.
1. **New Node Welcomer**: When a new node first joins the network, existing nodes generously provide a copy of the blockchain. Still, the new node independently checks the validity of each transaction, emphasizing a trustless but collaborative system.

The Bitcoin Core software is the original implementation of the Bitcoin protocol, though there are now other options. Install it and give it some time to download the entire blockchain. Once ready, leave it running and, approximately every 10 minutes, a new block with transactions will arrive. Your node will check its validity and add it to your local copy of the blockchain.

Running a node provides sovereignty and independence. You don't rely on others; it's your own traﬃc oﬃcer. Unlike your Bitcoin wallet, which lacks a copy of the blockchain, a node ensures self-suﬃciency. Instead of trusting others with the state of the Bitcoin network and the rightful ownership of your and everyone else's bitcoin holdings, you can connect your wallet with your personal node, making your digital experience more secure, independent, and trustworthy.




[▶ YouTube](https://www.youtube.com/watch?v=xc_TxlByxeY)


**Resource**: [Download Bitcoin Core](https://bitcoincore.org/en/download/)



#### 9.1.1 What Is a Bitcoin Node and How Do I Set One Up?

> The purpose of mining is not the creation of new bitcoin; that’s the incentive system. Mining is the mechanism by which Bitcoin’s security is decentralized.  
_Andreas M. Antonopoulos_


> **Callout**
>
> _Miners_ collect unconfirmed transactions, form a block, and expend energy to look for a valuable key that will **add and secure the block’s spot in the blockchain**.


Miners are in a race with one another to add the next block to the blockchain. The sought-after prize is a “valid block hash,” cleverly hidden among billions of others. Picture a massive haystack filled with millions of keys, each representing a unique block hash. Whoever finds the correct key (valid block hash) first wins the race and gets to add the next block!

Once a miner finds the correct block hash, they share it with the network, along with their created block of new transactions. Other miners verify the solution to make sure it’s the right fit. If everything checks out, the block is added to the blockchain, creating a secure and public ledger.

**Miners earn rewards for their eﬀorts in two ways:**

1. **Block rewards**: Block rewards are new bitcoin released into circulation with each block added to the blockchain. Transaction fees are small bitcoin payments users make to have their transactions processed faster and prioritized by the miner. Miners can pick which transactions to include in the block they mine, usually giving preference to those with higher transaction fees.
1. **Transaction fees**: Every single Bitcoin transaction carries a fee, an amount of bitcoin paid to the miner who wins the race. On most wallets, users can select the fee they're willing to pay; miners, who pick which transactions to include in the block they mine, naturally give preference to those with higher transaction fees.

##### Bitcoin Halvings

**Miners' Rewards for sucessfully completing one block halve every 210 000 blocks, or an average of every four years.**


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12.5 BTC | 6.25 BTC | 3.125 BTC |


Bitcoin halvings are an essential part of the Bitcoin protocol that helps maintain its scarcity and value over time. As you now know, there is a fixed supply of 21,000,000 bitcoin in total. This supply wasn’t fully available from the day Bitcoin launched — in fact, the full supply has not yet reached circulation. Instead, this supply enters the Bitcoin ledger progressively, following a schedule the network agrees to. Satoshi Nakamoto cleverly designed the block reward system as a way to distribute new bitcoin little by little, without the need for a central authority. In Bitcoin’s early days, miners got a sweet 50 bitcoin reward for each block they mined! This incentive motivated early miners to invest in powerful equipment and electricity for their mining operations.

To keep the network stable and manage new bitcoin supply, the block reward is halved about every 210,000 blocks (about 4 years). This event, called “the halving,” decreases the number of new bitcoin entering circulation and continues to motivate miners to protect the network and uphold its decentralization. Historically, halving events have led to significant price increases in the Bitcoin market due to the reduced supply of new bitcoin making their way into circulation.


> **Callout**
>
> _Circulating supply_ refers to the total available amount of a currency. With Bitcoin, the total circulating supply is the number of coins that have been mined and are incirculation at any given time.


![ Bitcoin Supply Schedule]

After each halving event, miners receive a reduced bitcoin reward, which progressively lowers the issuance rate of new coins. This reduction doesn’t necessarily mean miners make less of a profit: they also earn the sum of the transaction fees for the block they mine and, additionally, Bitcoin's price tends to increase as the emission of new coins slows down—miners receive a smaller amount of bitcoin, but each unit is very likely to be worth more!

Halving events are pre-programmed into the Bitcoin protocol, making the supply schedule of bitcoin predictable and transparent.


> **Callout**
>
> The _Bitcoin supply schedule_ is the predetermined and public plan for the release of new bitcoin into circulation, designed to maintain Bitcoin’s scarcity over time.


The following table outlines the details of upcoming Bitcoin halvings, including the expected date of the next halving event, the block number at which it will happen, the block reward per mined block until the following halving, and the percentage of the total supply that will be mined.


| Event | Date | Block | Reward | Percentage Mined |
| --- | --- | --- | --- | --- |
| 5th Halving | 2028 | 1,050,000 | 1.5625 BTC | 98.44 % |
| 6th Halving | 2032 | 1,260,000 | 0.78125 BTC | 99.22 % |
| 7th Halving | 2036 | 1,470,000 | 0.390625 BTC | 99.61 % |


![ ]

As more bitcoin are mined, the circulating supply and the percentage of the total supply that has been mined will keep increasing until the total supply of 21,000,000 is reached — which will happen in the year 2140. The reduced new supply, combined with rising demand, can boost Bitcoin’s price (relative to fiat currency). This benefits early adopters and also motivates miners to continue securing the network and contributing their computing power and resources.



##### What is a valid block Hash in Bitcoin?

In Bitcoin, a valid block hash is like a special code that miners try to find. It's a unique number that helps keep track of each block in the blockchain that stores information about transactions. The blocks connect in a chain from the first one (the so-called Genesis Block) to the latest, making a public record of all transactions.

![ ]

This block hash is crucial because it links each block to the one before it, making it easy for anyone to check the complete history of transactions. It's a bit like a fingerprint for each block, ensuring the information is correct and secure. The block hash acts as a way to confirm that the data in the block hasn't been changed.

The blocks are “linked” together by enforcing a specific relationship between blocks. That is, a block must contain a “fingerprint,” which is a hash value of the data of the previous block. A hash function can condense an arbitrary message (the block information) to a fixed size (e.g., 160 bits) and produces a fingerprint of the message.


> **Callout**
>
> Satoshi Nakamoto, the creator of Bitcoin, mined the Genesis Block, which unlocked a total of 50 bitcoin.


##### The Race to Mine a Block

Miners engage in a competition to uncover a valid block hash. The first miner to successfully discover the correct block hash is granted the opportunity to add that block to the blockchain and assign it with the corresponding hash ID. This solution serves as validation for the block’s authenticity.

The valid block hash aligns with a special number set by the network called the difficulty target. Earlier we compared mining to finding one valid key in a massive haystack. But what if no one ever finds the key? In other words: What if the problem to solve is too hard and no new blocks are mined? The Bitcoin protocol addresses this issue through what is called the "diﬃculty adjustment."

The protocol automatically adjusts the diﬃculty of the problem to be solved every 2,016 blocks (or around 2 weeks). depending on the total computational power — or "hash rate" — deployed by miners. This ensures that each block continues to be mined approximately every 10 minutes, regardless of how much power is expended in mining.

Let’s say the target number set by the Bitcoin network is 1,000. The miners would have to use their computational power and energy to search for a block hash (a specific number) that is lower than 1,000. The first miner to find a block hash lower than 1,000 gets to add the new block to the blockchain and is rewarded with bitcoin.


> **Callout**
>
> The diﬃculty level in Bitcoin mining is a measure of how hard it is to find a valid block hash that meets the target set by the network. It is adjusted every 2,016 blocks, or roughly every two weeks, to ensure that blocks are added to the blockchain at a consistent rate — every 10 minutes on average. The difficulty level is expressed as a number: the higher the diﬃculty level, the more harder it is to find a valid block hash.


For example, consider two different hashes:

* **Hash 1**: 0000A1mINgF0RbL0cK5wItHth3hAy5tAcK
  * **Difficulty level**: 1
* **Hash 2**: 00000000A1mINgF0RbL0cK5wItHth3hAy5tAcK
  * **Difficulty level**: 2

In this example, Hash 2 has a higher diﬃculty level than Hash 1 because it is a longer hash with more zeros at the beginning. It's harder for miners to find Hash 2 because their computers would need to do more work.


> **Info**
>
> By finding a valid block hash, a miner demonstrates that they have done the work required to add the new block to the blockchain. This demonstration is referred to as Proof of Work (PoW), which is the most crucial security mechanism to validate transactions and add new blocks to the blockchain. Because the winning miner can demonstrate that they have done the necessary work, they are rewarded in bitcoin through both the block reward and the fees from the transaction included in that block.


PoW keeps Bitcoin safe by making it prohibitively expensive for anyone with malicious intentions to take control — you are far more likely to profit by being an honest miner or even simply by holding bitcoin than by attempting to undo the blockchain. **In summary, the miners' role consists of**:

1. **Bundling transactions into blocks**: While nodes verify newly created transactions that are waiting in the mempool, miners select a subset of these to include in their candidate block.
1. **Proof of Work**: Miners race with one another to find a valid block hash.
1. **Broadcast valid blocks**: After finding a valid blockhash, they broadcast the new block to the network.
1. **Earn Rewards**: Lastly, they receive newly created bitcoin according to the supply schedule as well as the transaction fees for successfully adding the block to the blockchain.

![ ]

Multiple miners can work on creating new blocks simultaneously. The first miner to discover a block hash that meets the target set by the network announces it to the network, and the nodes then check the transactions in that miner’s candidate block to make sure they are valid. If the transactions are indeed valid, the block is added to the blockchain. The other blocks created by the other miners at the time are not added and are discarded. This process helps maintain consensus within the network and prevents double-spending.


> **Callout**
>
> _A candidate block_ is a set of transactions considered for addition to the blockchain that has not been added yet.


* The **miners** — Computers working to maintain and update the ledger — gather all the latest transaction data.
* They select transactions and group them all together into a **block** to be added to the chain.
* Then they calculate a **hash** for that block: they run all the data through an algorithm that spits out a unique string. Then they do it again. And again. They’re Looking for a valid hash — one that begins with a long string of zeroes. The first miner to find one wins newly created bitcoin, and their block is added to the chain.
* This hash ensures no one tampers with the ledger. Changing a single number or letter anywhere in the chain will make every hash for every subsequent block unrecognizably different. Then other nodes will reject the compromised ledger.
