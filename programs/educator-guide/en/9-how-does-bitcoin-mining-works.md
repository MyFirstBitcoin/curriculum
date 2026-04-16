# 9 - How Does Bitcoin Mining Works

Duration: 90 minutes

Core Idea: Bitcoin mining and node validation work together to secure the network, confirm transactions, and enforce the rules of the system through Proof of Work.

#### Learning Objectives

By the end of this lesson, students should be able to:

* Explain the difference between the role of Bitcoin nodes and the role of Bitcoin miners.
* Describe how nodes validate transactions, share information, and help enforce Bitcoin's rules.
* Explain what miners do, including selecting transactions, building candidate blocks, and competing to find a valid block hash.
* Define the mempool and explain why it works like a waiting room for unconfirmed transactions.
* Describe how transaction fees influence miner selection and confirmation speed.
* Explain Proof of Work as the mechanism that secures Bitcoin by making attacks expensive.
* Describe how difficulty adjustment helps maintain an average block time of about 10 minutes.
* Walk through the full life cycle of a Bitcoin transaction, from creation and signing to confirmation in a block.

#### Tools & Resources

##### Visual Aids

* Chapter 9 - How Does Bitcoin Mining Work?

##### Support Library

* Vocabulary Reference Card — Chapter 9 — Terms: mining, Proof of Work, hash puzzle, difficulty adjustment, block reward, mempool, 51% attack
* Misconceptions Libraries — Chapter 9 — Address: "miners create Bitcoin from nothing," "miners control Bitcoin," "more mining = less secure"
* Comparison Charts & Reference Sheets — Mining economics: revenue, costs, incentive alignment; difficulty adjustment
* Technical Explainers & Deep-Dives — Proof of Work security; why attacking is expensive; 51% threshold

#### Activities

* Exploring the Mempool
* Transactions in Action

#### Online Teaching

* Use one clear transaction flow diagram from wallet signing to confirmation.
* Keep nodes and miners visually separated on screen throughout the lesson.
* Use mempool.space or a screenshot of it to show unconfirmed transactions and fee pressure.
* Pause after each stage of the mining process and ask one short comprehension question.

#### Preparation

* Prepare mining process diagram (mempool → transaction selection → block creation → difficulty adjustment) for display.
* Bookmark mempool.space or blockchain.com mining page; prepare screenshots of current mining stats and difficulty adjustments.
* Create visual explanation of Proof of Work as the security mechanism; show difficulty adjustment over past 3-6 months.

#### Procedure

This lesson takes a closer look at how Bitcoin transactions move through the network and become part of the blockchain. It now follows the Diploma structure directly so the main sections align with the student guide while still preserving the fuller educator explanation inside each section.

##### 9.0 Introduction, 8 minutes

Start by connecting this chapter to the previous one:

* If a user signs a transaction with a private key, what happens next?
* Who checks whether that transaction is valid?
* How does it get added to the blockchain?
* Why does Bitcoin need both nodes and miners?

Clarify that this chapter explains how the network processes transactions in practice and how mining secures the system without a central authority.

##### 9.1 Bitcoin Nodes and Miners, 47 minutes

**Nodes and Miners, Different Roles**

Begin by clearly separating the two roles.

Bitcoin nodes:

* keep a copy of the blockchain
* verify whether transactions follow the rules
* share information with other nodes
* help wallets and other software access blockchain data
* can reject invalid transactions or invalid blocks

The chapter describes nodes as gatekeepers of validation, and expands that with the "digital traffic officer" analogy. That is helpful because it shows nodes as checkers and coordinators, not rulers. The diagram also reinforces that many nodes keep copies of the ledger around the world.

Bitcoin miners:

* gather valid transactions
* assemble candidate blocks
* compete to find a valid block hash
* broadcast valid blocks when they win
* receive block rewards and transaction fees

A key teaching point from the chapter is that the purpose of mining is not simply to create new bitcoin, but to decentralize Bitcoin's security. The new bitcoin is the incentive, while the mining process itself is the security mechanism.

**What Nodes Actually Do**

Build on the node section with the chapter's list of node functions:

* Gatekeepers of validation: they check that transactions and blocks follow the rules
* Communication hub: they connect with one another and share transaction data
* Quality checker: they reject invalid information
* Blockchain informant: they provide data to other software such as wallets
* New node welcomer: they help new nodes obtain the blockchain, while each new node still verifies the data independently

This is a good moment to emphasize that running a node gives the user more independence. Instead of depending entirely on outside services to tell them the state of the network, they can verify it for themselves. makes this point clearly, including the mention of Bitcoin Core as one implementation users can run.

**What Miners Actually Do**

Now explain mining more carefully.

Miners:

* collect verified but unconfirmed transactions
* group them into a candidate block
* repeatedly hash block data while searching for a valid block hash
* broadcast the winning block to the network
* earn rewards if the block is accepted

Use the chapter's "massive haystack of keys" analogy if it helps. It gives students a concrete image of the mining race. The main idea is not that miners solve a useful math problem in the ordinary sense, but that they prove they expended real-world energy and computation to secure the system.

This is also the right place to explain miner rewards:

* block reward: newly issued bitcoin
* transaction fees: fees attached to transactions users want confirmed

Clarify that miners usually prioritize transactions with higher fees, because those increase their reward. The chapter also explains halvings here, so you can briefly note that the block reward decreases every 210,000 blocks, about every four years, according to Bitcoin's public supply schedule. Pages 5 and 6 include the supply schedule and upcoming halving table, which can help reinforce Bitcoin's predictable issuance.

**Valid Block Hash, Proof of Work, and Difficulty Adjustment**

This section is the core of the chapter.

Explain that miners are searching for a valid block hash, meaning a block hash that meets the network's target. The chapter explains this as finding a number lower than the target set by the network.

Then explain Proof of Work clearly:

* miners must do repeated computational work
* the first one to find a valid hash proves they did that work
* this makes it expensive to rewrite or attack the ledger
* nodes then verify the block before accepting it

A strong line for teaching is:

Proof of Work secures Bitcoin by making dishonesty expensive and verification easy.

Also explain difficulty adjustment:

* the network adjusts mining difficulty every 2,016 blocks
* this happens roughly every two weeks
* the goal is to keep average block time close to 10 minutes
* if more hash power joins the network, difficulty rises
* if less hash power is present, difficulty falls

Pages 7 and 8 explain this process and show how harder targets require more work. This helps students understand that Bitcoin's timing is not controlled by a central authority but by protocol rules that respond automatically to network conditions.

##### 9.2 What Is the Mempool?, 15 minutes

Now move to the mempool.

Explain that the mempool is the waiting room for valid, unconfirmed transactions. When a user broadcasts a transaction, nodes first verify it. If it is valid, they add it to their mempool and share it with other nodes. Then miners can select from those waiting transactions when building a block. Pages 10 and 11 explain this process directly.

Important points to emphasize:

* the mempool is not the blockchain
* transactions there are still unconfirmed
* each node maintains its own mempool
* there is not one single universal mempool
* higher-fee transactions are more likely to be selected sooner

The chapter also explains common reasons a transaction might stay unconfirmed for a long time:

* low fee
* network congestion
* double-spend attempt
* incorrect or incomplete data
* malformed transaction

If useful, mention the activity with mempool.space as a practical way to visualize unconfirmed transactions and fee rates. Also make clear that mempool.space is just one explorer, not the mempool itself.

##### 9.3 How Bitcoin Transactions Work, 20 minutes

Now bring everything together using the chapter's step-by-step sequence.

A clear classroom version is:



1. The sender selects a UTXO and creates a transaction
1. The sender adds the recipient address and fee
1. The sender signs the transaction with their private key
1. The transaction is broadcast to the network
1. Nodes verify it and add it to their mempools
1. Miners select it for a candidate block
1. Miners compete through Proof of Work
1. One miner finds a valid block hash and broadcasts the block
1. Nodes verify the block and add it to the blockchain
1. The transaction receives confirmations as more blocks are added
1. Make the final point explicit:
1. once the transaction is included in a valid block, it is confirmed
1. the spent inputs are no longer usable
1. the receiver now controls new UTXOs created by that transaction

The summary diagram is especially useful here because it visually connects the whole process from wallet signing to miner inclusion to node validation and block distribution.

###### Wrap-Up and Check for Understanding

Close with a few quick questions:

* What is the difference between a node and a miner?
* What is the mempool?
* Why do some transactions confirm faster than others?
* What does Proof of Work prove?
* Why does Bitcoin adjust mining difficulty?
* What are the main steps between sending a transaction and receiving confirmation?

#### Educator Notes

Keep the main teaching thread clear: nodes verify, miners compete, Proof of Work secures, and the mempool holds valid transactions until they are confirmed.

This chapter can feel technical, so use analogies and diagrams often.

Avoid making mining sound like "creating bitcoin out of nowhere." Be precise that the reward is the incentive, while the mining process secures the network.

The strongest points to prioritize, if time is short, are:



1. Node vs miner roles
1. Mempool as waiting room
1. Proof of Work
1. Difficulty adjustment
1. Transaction flow from signing to confirmation

##### What Good Looks Like

* It is important to immediately clarify that Miners ≠ Nodes, show mining as economic activity with real hardware costs and electricity expenses, use difficulty adjustment and Proof of Work to explain the security mechanism, and test understanding with scenarios about network changes.
* Educators should use real numbers to ground discussions, be crystal clear and repetitive about the Miners versus Nodes distinction, be realistic about centralization concerns with mining pools, and respect the genuine sophistication involved.
* Students understand that mining is smart people doing complex work because they earn Bitcoin, recognize that incentives drive honest behavior because miners' profits depend on Bitcoin succeeding, see the system self-regulating through automatic difficulty adjustment, understand that mining is a real business not charity, and appreciate that Bitcoin's security costs real electricity and money.
* Learning Outcomes should be met if students can distinguish miners who create blocks from nodes who validate them, understand Proof of Work as a security mechanism that makes attacks exponentially expensive, recognize difficulty adjustment keeps block time at approximately 10 minutes, understand miners' incentives around block rewards and fees, explain why a 51% attack fails to work, and see mining as an economic activity with real costs and benefits.

##### Time Management

If time is short, prioritize:

* Node vs miner roles (the critical distinction)
* Mempool as waiting room
* Proof of Work mechanism
* Difficulty adjustment (self-regulating system)
* Transaction flow from signing to confirmation

If ahead, take time on:

* Mining economics and hardware specifics
* Mining pool dynamics and centralization concerns
* 51% attack scenarios and why they mathematically fail
* Long-term security through incentive alignment

##### If Students Struggle

* Miners vs. nodes (confusion) → "Nodes validate, miners propose; referees vs. players."
* Proof of Work wasteful → "Expensive security prevents attacks; makes them pointless."
* Difficulty adjustment → "More miners = faster blocks = difficulty rises; system breathes."
