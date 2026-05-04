# 6 - How to Use Bitcoin

Duration: 90 minutes

Core Idea: Using Bitcoin on-chain teaches students how ownership, self-custody, and verification work in practice, turning theory into direct financial action.

#### Learning Objectives

By the end of this lesson, students should be able to:

* Identify common ways to acquire and exchange bitcoin, including peer-to-peer and centralized exchange methods.
* Explain the difference between self-custodial and custodial wallets, and why self-custody matters in Bitcoin.
* Describe the purpose of private keys, public addresses, seed phrases, and wallet interfaces.
* Compare different wallet types and evaluate their trade-offs based on security, convenience, privacy, and control.
* Set up a mobile Bitcoin wallet and explain the basic recovery process.
* Demonstrate how to receive and send an on-chain bitcoin transaction.

Apply the principle "Don't Trust, Verify" to wallet choice, transactions, and broader Bitcoin use.

#### Tools & Resources

##### Visual Aids

* Chapter 6 - How to Use Bitcoin

##### Support Library

* Vocabulary Reference Card — Chapter 6 — Terms: wallet, private key, public address, seed phrase, custodial, self-custodial, UTXO, transaction fee
* Comparison Charts & Reference Sheets — Wallet types comparison (custodial, mobile, hardware, paper)
* Technical Explainers & Deep-Dives — Public/private keys, UTXO model, transaction confirmation
* Private Key Security Deep-Dive — Seed phrases, key derivation, backup methods, attack vectors
* Transaction Anatomy Guide — Step-by-step example of how a Bitcoin transaction works
* Security Best Practices Checklist — Before you start, creating wallet, receiving, sending, phishing prevention

#### Activities

* Transactions in Action
* Lightning Relay Race
* Exploring the Mempool

#### Online Teaching

* Make it clear from the start whether students are watching a demo or setting up a wallet themselves.
* Use large, readable screenshots for each wallet setup step.
* Pause after each step and ask students to confirm understanding in chat before continuing.
* Give a direct warning before the seed phrase section and remind students never to share sensitive information online.

#### Preparation

* Download and test a mobile wallet app (Blue Wallet or Muun); prepare screenshots of key setup steps.
* Prepare wallet setup guide (download → create → backup seed → receive) for reference.
* Ensure network/WiFi is working; have a demo address and QR code ready to show.

#### Procedure

This lesson moves from theory into direct practice. It now matches the Diploma structure directly so that acquisition, wallets, setup, transactions, and verification appear under the same main headings as the student guide. Extra teaching support remains nested inside those sections.

##### 6.0 Introduction, 8 minutes

Start by connecting this chapter to the previous one:

* If Bitcoin is money, how do people actually get and use it?
* What does it mean to truly control your bitcoin?
* Why is using Bitcoin different from using a bank app?

Clarify that this chapter is about practical use. Students are no longer only learning what Bitcoin is, they are learning how to interact with it directly.

##### 6.1 Acquiring and Exchanging Bitcoin, 12 minutes

Explain that people can acquire bitcoin in different ways, including:

* getting paid in bitcoin
* mining bitcoin
* exchanging fiat for bitcoin in person
* exchanging fiat for bitcoin online

Then focus on the two main acquisition routes covered in the chapter:

* peer-to-peer, in person
* peer-to-peer, online
* centralized exchanges

Make the trade-offs clear.

For P2P in person, emphasize direct exchange without a bank or intermediary, but also mention the practical risks of meeting people for cash trades.

For P2P online, explain escrow in simple terms, as a way to reduce counterparty risk while still allowing direct exchange between peers.

For centralized exchanges, make clear that they are convenient, but they require users to trust a company, often share personal information, and leave funds under third-party control until withdrawn. This is a good place to reinforce that convenience often comes with trade-offs in privacy and sovereignty.

##### 6.2 An Introduction to Bitcoin Wallets, 35 minutes

**What a Bitcoin Wallet Actually Is**

Clarify a common misunderstanding right away: bitcoin is not stored inside the wallet app like physical cash in a bag.  
The bitcoin exists on the ledger maintained by the network. What the user controls is the ability to spend it through private keys.

Then explain the two things people often mean by "wallet":

* the private key system, from which addresses are generated
* the app or interface used to interact with the network

Use the chapter's email analogy if helpful:

* public address = like an email address you can share
* private key = like a password you must protect

Be very clear here: whoever controls the private keys controls the bitcoin. That is the core concept students must understand.

**Self-Custodial vs Custodial Wallets**

This is one of the most important parts of the chapter.

Explain the distinction clearly:

* Self-custodial wallet: the user controls the private keys
* Custodial wallet: a third party controls the private keys on the user's behalf

Then walk through the trade-offs:

Self-custodial

* full control over funds
* no approval process
* protection against arbitrary confiscation
* greater responsibility
* no easy recovery if the seed phrase is lost

Custodial

* easier recovery and support
* simpler for beginners
* more exposed to account freezes, hacks, and third-party control
* the user does not truly hold the bitcoin

This is the right moment to emphasize the phrase:

"Not your keys, not your coins."

Students should leave this section understanding not only the slogan, but what it actually means in practice.

**Different Types of Wallets and How to Choose One**

Introduce the wallet types covered in the chapter:

* online wallet
* mobile wallet
* desktop wallet
* hardware wallet
* paper wallet

Do not treat one as perfect. Instead, explain that each one involves trade-offs between:

* security
* privacy
* convenience
* compatibility
* fees
* control
* reputation

Also make clear that we recommends paying attention to whether wallet software is open-source, because open-source tools can be reviewed, audited, and continued by the community. This connects directly to the principle of verification in Bitcoin.

##### 6.3 Setting Up a Mobile Bitcoin Wallet, 10 minutes

Walk students through the basic process shown in the chapter:

* download the wallet
* create a new wallet
* generate and write down the recovery phrase
* confirm the recovery phrase
* add extra security if available
* open the wallet and find the receive function

Make the seed phrase warning very explicit:

* if the seed phrase is lost, access to the funds may be lost
* if someone else gets the seed phrase, they can take the funds

If students are doing this hands-on, the educator should pause at each step and check that everyone understands what they are doing. If the class is more conceptual, this section can be explained as a walkthrough rather than performed live. The recovery option shown in the chapter is also useful for explaining that wallets can be restored if the seed phrase was backed up correctly.

##### 6.4 Receiving and Sending Transactions, 17 minutes

**Receiving and Sending On-chain Transactions**

Now explain how on-chain transactions work.

For receiving bitcoin:

* open the wallet
* tap receive or deposit
* copy the address, share the link, or show the QR code

For sending bitcoin:

* open the wallet
* paste or scan the recipient's address
* enter the amount
* double-check all details
* broadcast the transaction
* wait for confirmation

Make these key points clear:

* the transaction transfers ownership, not physical coins
* transactions are irreversible
* nodes verify validity
* miners include transactions in blocks
* fees influence confirmation priority
* on-chain transactions are generally secure, but slower and often more expensive than Lightning transactions

The transaction flow diagram in the chapter is especially useful here, because it helps students visualize the path from wallet request to network confirmation.

**Transactions in Action and Role-Based Practice**

Use the cooperative exercise structure from the chapter to reinforce understanding. Explain the four roles involved:

* sender
* recipient
* miner
* node operator

A simple classroom approach is to assign roles and walk through one transaction step by step. This helps students see that a Bitcoin transaction is not magic, it is a coordinated process involving approval, verification, inclusion in a block, and ledger updates.

The goal here is not technical depth. It is helping students understand who does what in a transaction and why verification matters.

##### 6.5 Don't Trust, Verify, 8 minutes

Explain that this applies to:

* wallets
* exchanges
* apps
* transaction details
* claims about "easy profits"
* projects pretending to be like Bitcoin

Make clear that Bitcoin requires users to think critically, verify what they are using, and avoid blind trust. Also explain why open-source tools matter in this context: they make independent verification possible.

###### Wrap-Up and Check for Understanding

Close with a few quick questions:

* What is the difference between a custodial and self-custodial wallet?
* Why is the seed phrase so important?
* What happens when you send an on-chain transaction?
* Why are on-chain transactions slower than some other Bitcoin payments?
* What does "Don't Trust, Verify" mean in practice?

#### Educator Notes

This chapter is highly practical, so prioritize clarity, safety, and repetition.

Students do not need to master every wallet type in one class. The main goals are:

* understanding wallet basics
* understanding self-custody
* learning the basic transaction flow
* adopting a responsible verification mindset

Be especially careful when discussing seed phrases and wallet setup. Students should leave understanding that these are not small details, they are the basis of Bitcoin ownership.

The most useful visuals and activities in this chapter are:

* the self-custodial vs custodial comparison
* the wallet type trade-off table
* the step-by-step wallet setup exercise
* the transaction flow diagram
* the role-based transaction activity

##### What Good Looks Like

* It is important to have students actually set up a wallet or watch a careful demo, make the seed phrase the centerpiece with "This 12 words IS your Bitcoin," test scenarios like "What happens if you lose your phone?", and practice phishing recognition.
* Educators should be hands-on guides who have done this before, be security-conscious without paranoia, and be honest about the difficulty curve and learning required.
* Students feel they have learned an actual skill they can use, understand that the seed phrase is real and important rather than abstract, feel capable of holding their own Bitcoin, and understand that decentralization requires personal responsibility.
* Learning Outcomes should be met if students can set up a wallet and understand public versus private keys, understand custody trade-offs between custodial and self-custody wallets, explain how a transaction works including inputs, outputs, and fees, demonstrate security awareness including seed phrase protection, and ask critical questions about ownership and control.

##### Time Management

If time is short, prioritize:

* Understanding wallet basics
* Understanding self-custody
* Learning the basic transaction flow
* Adopting a responsible verification mindset

If ahead, take time on:

* Self-custodial vs custodial comparison table
* Wallet type trade-off table
* Step-by-step wallet setup exercise with live demo
* Transaction flow diagram with fee calculations
* Advanced security practices and hardware wallet considerations

##### If Students Struggle

* Seed phrases as "real" → "This phrase IS your bitcoin; no customer service."
* Public vs. private keys → Email analogy (address vs. password).
* Why it's hard → "You control it; you're responsible." Acknowledge trade-off.
