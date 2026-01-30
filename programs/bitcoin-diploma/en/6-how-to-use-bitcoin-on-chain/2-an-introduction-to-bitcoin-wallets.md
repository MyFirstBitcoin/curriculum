# 6.2 An Introduction to Bitcoin Wallets

![ ]

Unlike physical money, bitcoin are not actually contained in a Bitcoin wallet. Instead, they live on the distributed ledger that the Bitcoin network constantly verifies and secures. So, how can you own bitcoin?

You have ownership of your bitcoin only if you control the private keys allowing you to sign transactions and transfer ownership of your bitcoin to someone else. This is the act of sending bitcoin.

With that in mind, let’s take a look at two concepts we refer to when using the term “**wallet**”:

* A master private key (like a password) from which your public keys (like email addresses) are generated [m dash] you can share your public address with others to receive and send bitcoin, but you must never share your private key!
* The mobile or desktop interface from which you can interact with the Bitcoin network to retrieve your bitcoin balance, send and receive transactions, and broadcast them to the network. Diﬀerent types of wallets, along with their benefits and tradeoﬀs, will be described in the next sections.

#### 6.2.1 Self-Custodial vs Custodial Wallets

Before detailing the diﬀerent types of Bitcoin wallets and their characteristics, let’s make an important distinction between self-custodial and custodial wallets, as shown in the table below. You can see the benefits and risks of using each wallet type and who controls the bitcoin in each case. Self-custodial means the user holds the private keys, which means they are in true possession of their bitcoin; with the second kind, a third party holds the bitcoin for the user.


| Wallet Type | Who controls my bitcoin? | Benefits | Risks |
| --- | --- | --- | --- |
| Self-Custodial | The user | Complete control over funds and transactions, no approval process or account freeze, no corporate or government control, protected against arbitrary confiscation, like keeping money at home. | No recovery if recovery phrase is lost, less customer support, full responsibility falls on the user. |
| Custodial Wallets | The third-party provider | Easy recovery if access is lost, easier customer support. | Funds are always connected to the internet, more vulnerable to hacking and breaches. Custodial control means the custodian can freeze accounts. |


In a self-custodial wallet (also called non-custodial wallet), you are the only one with the keys to the wallet and you have full control over what goes in and out. On the other hand, in a custodial wallet someone else holds the private key, giving them full access to move any bitcoin that provider controls on your behalf.

* Self-custody is like being your own bank. Transactions are not subject to the scrutiny and control
* Self-custody ensures that third parties cannot confiscate your bitcoin.
* Self-custody gives peace of mind in times of uncertainty, because you know your bitcoin is secure.

It’s important to choose the right type of wallet for each individual’s needs. Sometimes, people find it hard to distinguish whether they are installing a self-custodial or a custodial wallet. This table shows the diﬀerences in the installation process.


| Wallet Type | Step 1: Choose a Wallet | Step 2: Install the Wallet | Step 3: Create a New Wallet | Step 4: Secure Your Seed Phrase | Step 5: Start Using Your Wallet |
| --- | --- | --- | --- | --- | --- |
| Self-Custodial | Choose a self-custodial wallet provider | Follow the wallet provider's instructions | Generate a recovery phrase | Store the recovery phrase in a secure location | Start using the wallet to receive and send bitcoin |
| Custodial Wallets | Choose a custodial wallet provider | Follow the wallet provider's instructions | Create an account with the wallet provider | N/A (wallet provider holds the private keys) | Start using the wallet to receive and send bitcoin |


![Not your Keys not your Coins]

“Not your keys, not your coins” is a popular saying among bitcoin holders. It refers to the idea that if you don’t have direct control over the private keys associated with your Bitcoin wallet, you don’t have true ownership of the coins.

Whoever accesses your private keys has ownership of your bitcoin. This is why it is of the utmost importance to protect them by keeping them away from prying eyes! We’ll see a few ways you can do that later in the book.

For what follows, we’ll be talking about self-custodial wallets only, where the user owns their keys and has complete control over their bitcoin.

Don’t worry if it seems complicated or you don’t understand everything — this is a journey, and you will understand better the more you start using Bitcoin!

#### 6.2.2 Diﬀerent Types of Bitcoin Wallets

Depending on where your private key is created and stored, we commonly use diﬀerent names to describe Bitcoin wallets. If the keys are stored on your smartphone, we call it a “mobile wallet.” If they’re stored securely on a dedicated device, we call it a “hardware wallet.” If the key is only stored on paper, then it is called a “paper wallet.”

**The different names we give Bitcoin wallets depending on their structure:**


| Wallet Type | Description | Advantages | Disadvantages | Example User |
| --- | --- | --- | --- | --- |
| Online Wallet | A wallet accessed through a web browser | Accessible from any device with an internet connection | Less secure because it can be hacked or compromised | Someone who needs to access their wallet frequently and doesn’t have a lot of funds to store |
| Mobile Wallet | A wallet installed on a mobile device | Easy to use | Can be lost if the device is stolen or hacked | Someone who needs to make transactions on the go and doesn’t have a lot of funds to store |
| Desktop Wallet | A wallet installed on a desktop computer | Convenient and can be accessed from anywhere | Can be hacked if the computer is infected with malware | Someone who wants to store a large amount of bitcoin and is comfortable with using a desktop computer |
| Hardware Wallet | A physical device that stores bitcoin offline | More secure than online wallets and can be used offline | Funds could be unrecoverable | Someone who wants to store a large amount of bitcoin and is willing to pay for the added security of a hardware wallet |
| Paper Wallet | A physical record of a Bitcoin wallet's private and public keys | Very secure and can be used offline | Can be lost or stolen if the physical record is lost or stolen | Someone who wants to store a large amount of bitcoin and is willing to take the added precautions to ensure its security |


Because the keys can be moved from one device to another, the “status” of your Bitcoin wallet is not definitive. For example, if I generate the keys of my Bitcoin wallet on a computer and later upload them to my phone, the “desktop wallet” then becomes a “mobile wallet.”

When it comes to storing your bitcoin, it’s not just about who has control over the keys — there are many other risks to consider. That’s why it’s important to find a storage solution that is both secure and convenient.

When you analyze the trade-oﬀs of the various types of wallets, you will learn that there is no ideal wallet to satisfy all needs.

##### When choosing a Bitcoin wallet, there are several things you should consider:

* **Security**: Make sure the wallet has strong security measures in place such as two-factor authentication and secure password policies.
* **Privacy**: Consider whether the wallet allows you to remain anonymous or if it requires personal information to set up an account.
* **Ease of use**: Choose a wallet that is easy to use and navigate, especially if you are new to Bitcoin.
* **Compatibility**: Make sure the wallet is compatible with your device and operating system.
* **Fees**: Compare the fees charged by diﬀerent wallets to make sure you are getting the best deal.
* **Reputation**: Research the reputation of the company or developers to make sure they are trustworthy.
* **Control**: Some wallets give you more control over your private keys, which can be a security advantage.

Consider whether you want a wallet that gives you full control or one that is more user-friendly but may oﬀer less control.

#### 6.2.3 Open Source vs Closed Source

Another important factor to keep in mind when choosing a Bitcoin wallet is knowing if the application or software is open-source.

This is very important because open-source projects allow the community to review the code and fork or pick up the project, if the team were to stop working on it for instance.

Just as Bitcoin’s code is completely open for everyone to review, use, and modify, so should the code of the wallet you use to manage your bitcoin be.

#### Activity: Class discussion and evaluation of Bitcoin wallets on bitcoin.org

https://bitcoin.org/en/choose-your-wallet

Go to the following website:

[https://bitcoin.org/en/choose-your-wallet](https://bitcoin.org/en/choose-your-wallet)

and use your new knowledge of Bitcoin wallets to select the one best suited to your needs based on the criteria we discussed today.
