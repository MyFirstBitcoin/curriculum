# Use Bitcoin in Daily Life

Duration: 90 minutes

Core Idea: The Lightning Network makes Bitcoin more practical for everyday payments by enabling faster, cheaper transactions while keeping Bitcoin as the foundation.

#### Learning Objectives

By the end of this lesson, students should be able to:

* Explain what the Lightning Network is and why it was built on top of Bitcoin.
* Compare on-chain and Lightning transactions in terms of speed, cost, and security trade-offs.
* Distinguish between custodial and self-custodial Lightning wallets, and explain why self-custody matters.
* Set up a Lightning wallet and describe the role of the seed phrase in wallet recovery.
* Demonstrate how Lightning payments move through the network, even when two users do not share a direct channel.
* Identify real-world ways Bitcoin can be used in everyday life through Lightning, including coffee, groceries, merchant payments, and local spending.
* Explain how tools like BTCPay Server, BTCMap, and gift cards help expand Bitcoin usage in practice.
* Describe what a Bitcoin circular economy is and why Lightning makes it more viable.

#### Tools & Resources

##### Visual Aids

* Chapter 7 - Using Bitcoin in Daily Life

##### Support Library

* Vocabulary Reference Card — Terms: Lightning Network, payment channel, routing, Layer 2, circular economy, remittance
* Real-World Examples & Case Studies Library — El Salvador, Austin circular economy, Lightning merchant adoption stories
* Comparison Charts & Reference Sheets — On-Chain vs. Lightning comparison; Fee & Speed comparison across payment methods
* Lightning Network Simplified Explainer — How payment channels work without jargon; routing; security; use cases
* Payment Scenario Walkthroughs — Step-by-step: send to friend, receive payment, remittances, accept as freelancer
* Fee & Speed Comparison Tool — When to use Lightning vs. on-chain vs. banking (with cost examples)

#### Activities

* Lightning Relay Race

#### Online Teaching

* Use a side-by-side comparison slide for on-chain and Lightning payments.
* Start with a real-life use case like coffee or remittances so students understand why Lightning exists.
* Use a simple three-person routing diagram so the network explanation stays clear.
* Keep channel mechanics light unless the class already has a strong foundation.

#### Preparation

* Download Lightning wallet and prepare screenshots showing on-chain (slow) vs. Lightning (fast) transaction speeds side-by-side.
* Research 2-3 real merchants or communities using Lightning; bookmark BTCMap.org for reference.
* Prepare on-chain vs. Lightning comparison chart (speed, fees, security, use case) for distribution.

#### Procedure

This lesson shows students how Bitcoin becomes practical for everyday payments through the Lightning Network. The guide now follows the Diploma structure directly so the main Lightning sections correspond to the student guide, while comparisons, merchant tools, and circular economy material stay nested where they belong.

##### 7.0 Introduction, 8 minutes

Start by connecting this chapter to the previous one:

* If Bitcoin works on-chain, why was another layer needed?
* What happens when people want to make many small payments quickly?
* What kind of payment system would work better for coffee, groceries, or paying a friend?

Clarify that this chapter focuses on Bitcoin for everyday use, especially when speed and low fees matter. Make clear that Lightning is built on top of Bitcoin, not separate from it.

##### 7.1 The Lightning Network, 25 minutes

**What Is the Lightning Network**

Explain that the Lightning Network is a payment system built on top of Bitcoin that allows users to send and receive bitcoin quickly and inexpensively. It works by moving many small payments off the main blockchain and only settling the final result back on-chain later.

A helpful way to explain it is with the café tab analogy from the chapter:

* instead of paying for every item one by one on-chain
* two parties open a channel
* they update balances as they transact
* only the final balance is recorded on the blockchain when they close the channel

That makes Lightning faster and cheaper for frequent small payments. Also clarify that Lightning payments can route through the network, so users do not need a direct channel with every person they pay.

**On-chain vs Lightning**

Now make the contrast very clear.

On-chain transactions

* happen directly on the Bitcoin blockchain
* are generally slower
* depend on block inclusion and confirmation
* tend to be more secure
* can be more expensive depending on fees

Lightning transactions

* happen on a second layer built on top of Bitcoin
* settle much faster
* usually cost much less
* are useful for small and frequent payments
* involve trade-offs compared to on-chain settlement

Keep the main point simple: on-chain is stronger for final settlement, Lightning is stronger for speed and low-cost everyday use. The comparison is especially useful here.

##### 7.2 Different Types of Lightning Wallets, 10 minutes

Explain that a Lightning wallet performs the same basic function as a Bitcoin wallet, receiving and sending bitcoin, but it is designed for use on the Lightning Network. Then walk through the chapter's main wallet distinctions:

* self-custodial: the user controls the keys
* custodial: someone else controls the keys

Clarify the core trade-off:

* custodial wallets may feel easier and more convenient
* but the user depends on someone else's permission and control
* self-custodial wallets give more ownership and sovereignty

Also reinforce the chapter's recommendation to prefer open-source wallets, because open-source tools can be reviewed, improved, and verified by the community.

##### 7.3 Setting Up a Bitcoin Lightning Wallet, 10 minutes

Walk students through the basic setup flow:

* download a Lightning wallet
* create a new wallet
* write down the recovery phrase
* confirm the words in the correct order
* add extra security if the wallet allows it
* begin using the wallet

Be especially clear about the seed phrase:

* it is what allows the user to recover access
* if it is lost, access to funds may be lost
* if another person gets it, they can control the funds

This section should strongly reinforce responsibility and safe handling, just like in the on-chain chapter.

##### 7.4 Sending and Receiving Lightning Transactions, 17 minutes

**How Lightning Transactions Work in Practice**

Use the Marcia, Jeff, and Eve example to explain routing. Marcia does not need a direct channel with Eve. Her payment can move through Jeff, who is connected to the network, and still reach Eve securely.

Make these points clear:

* Lightning payments can move through intermediaries
* those intermediaries help route payments
* the routing process does not mean users are trusting a bank or centralized payment processor
* the network uses cryptography so the payment reaches the intended recipient

This helps students understand that Lightning is still peer-to-peer, even when payments move through a broader network structure. If useful, point out that the chapter also mentions node operators can earn fees and help strengthen the network by routing payments.

**Funding Channels and Using Lightning Repeatedly**

Explain the Mina example further:

* Mina moves bitcoin from her on-chain wallet into her Lightning wallet
* this funds a payment channel
* she can then make repeated payments without reopening the process each time
* when the channel closes, the final balance is settled back on-chain

Make one important limitation clear: funds locked in an active channel are being used for Lightning and are not freely available for separate on-chain use at the same time. This helps students understand that Lightning is powerful, but it involves a different payment structure.

##### 7.5 Buying Coffee and Groceries with Bitcoin, 20 minutes

**Everyday Use Cases**

Shift from mechanics to real life.

Explain that Lightning is especially useful for:

* buying coffee
* groceries
* shopping
* paying friends
* everyday small transactions

The chapter's Mina example helps show why Lightning is a better fit than traditional payment rails for many situations: it is fast, low-fee, borderless, and accessible even to people who may not have bank accounts. The comparison table and the payment-processing diagram are strong teaching aids here, especially for showing how many intermediaries exist in traditional card payments.

**Merchant Tools and Spending Bitcoin in the Real World**

Now explain how businesses and users can make Lightning practical in daily life.

Cover the three main tools or paths in the chapter:

BTCPay Server

* open-source payment processor
* lets merchants accept bitcoin directly
* no middleman controlling funds
* useful for online and in-person business payments

BTCMap

* helps users find merchants and communities that accept bitcoin
* lets people search locally
* can be updated by the community

Gift cards and vouchers

* transitional tools for spending bitcoin where direct acceptance does not yet exist
* help bridge the gap while adoption grows

This section is important because it shows students that Bitcoin use is not only theoretical. There are already real tools people can use today.

**Circular Economies and Bitcoin as a Medium of Exchange**

Close the main content by explaining that a circular economy is a community where participants try to buy from and sell to one another as much as possible. Applied to Bitcoin, this means merchants, workers, and users choose to transact in bitcoin and support each other economically.

Make clear why Lightning matters here:

* payments are near-instant
* fees are low
* small payments become practical
* local trade becomes easier to sustain

You can mention that the chapter points to examples such as Arnhem and Bitcoin Beach, showing that circular economies are not hypothetical. They already exist and continue to grow. The visual timeline is especially useful here

###### Wrap-Up and Check for Understanding

Close with a few quick questions:

* Why was the Lightning Network built?
* What is one major difference between on-chain and Lightning payments?
* Why does self-custody matter in a Lightning wallet?
* How can someone receive a Lightning payment without a direct channel to every person?
* What is a Bitcoin circular economy?

#### Educator Notes

Keep the main teaching thread clear: Bitcoin is the base layer, Lightning helps make everyday payments faster and cheaper.

This chapter should feel practical and concrete, not overly technical.

Prioritize understanding over deep channel mechanics.

The strongest points to prioritize, if time is short, are:

* what Lightning is
* on-chain vs Lightning trade-offs
* wallet custody and setup
* real-world payments
* circular economies

The most useful visuals in this chapter are:

* the on-chain vs Lightning comparison
* the wallet distinctions
* the routing example with Marcia, Jeff, and Eve
* the comparison table and capacity chart
* the traditional payment-processing diagram
* the circular economy timeline

##### What Good Looks Like

* It is important to start with the pain point "Bitcoin takes 10 minutes and costs $2," explain Lightning as a fast lane on top of Bitcoin, use real examples from merchants and remittance corridors, and create decision trees for when to use on-chain versus Lightning.
* Educators should be pragmatic about what Lightning actually solves, share stories from the field where Bitcoin is being used, be clear about specific trade-offs, and remain realistic about adoption while excited about possibilities.
* Students experience seeing Bitcoin actually working for real payments in real places, understand that speed and cost matter for payments, envision a circular economy where Bitcoin stays local, recognize that Lightning ≠ Bitcoin (different tools for different purposes), and become curious about economic systems built on Bitcoin payments.
* Learning Outcomes should be met if students can explain Lightning Network as a layer on top of Bitcoin, understand payment channels and routing basics, see real use cases for Lightning payments, compare on-chain versus Lightning for different scenarios, understand the circular economy concept, and recognize the specific trade-offs of each approach.

##### Time Management

If time is short, prioritize:

* What Lightning is
* On-chain vs Lightning trade-offs
* Real-world payments
* Circular economies

If ahead, take time on:

* Payment channel mechanics and routing
* Fee and speed comparison tool
* El Salvador and Austin circular economy case studies
* Practical Lightning payment scenario walkthroughs

##### If Students Struggle

* Why Lightning exists → Compare: 10 min/$2 vs. seconds/fraction cent.
* Payment channels → Café tab analogy; settle internally then on Bitcoin.
* Why it matters globally → "What if no bank but have Bitcoin?"
