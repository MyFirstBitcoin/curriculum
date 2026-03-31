# 6.4 Receiving and Sending Transactions

A Bitcoin transaction is a transfer of ownership of bitcoin to a new owner. Note that it is not the actual coins that are transferred, but ownership of them: in other words, the right to spend them. Every time a transaction is accepted into a block, all the nodes in the network update their local copy of the public ledger to reflect the change ownership. In this respect, a Bitcoin transaction is more akin to a real estate (or other property) transaction than to a cash transaction.

To "send" bitcoin, the sender signs a message with their private key, signaling to the network that the rightful owner of the bitcoin has transferred its ownership to the recipient.

The bitcoin will now be tied to the recipient's address, giving them ownership of the bitcoin, so that only the new owner can spend them by using their private key.

New Bitcoin transactions are initiated from wallets around the world, but there is no central payment processor. Instead, miners compete to record transactions in the ledger.

Let’s say Jim owes Eliana 0.5 BTC and is ready to pay her back. Both have digital wallets.

1. Eliana shares her address with Jim.
1. Jim uses his wallet software to create the transaction, which includes Eliana’s address, the amount to be transferred (0.5 BTC), and a fee for the miner. Higher fees make it more likely that a miner will include the transaction in the next block.
1. After signing the transaction, it is broadcast to the network, where it is verified by nodes. They check whether Jim has enough funds and is the rightful owner of the coins he means to spend. If he does not, they reject the transaction immediately.
1. Once the transaction is verified, miners choose whether to add the transaction to the next block, usually based on the selected fee. Once the transaction makes it into a block, it is added to the blockchain and the funds are transferred to Eliana's address.
1. Ownership has been transferred to Eliana. She can now use her private key to spend the received funds.

_It’s important to note that once the transaction is complete, it cannot be reversed._


> **Note – How a Bitcoin Transaction Works**
>
> 1. Someone requests a transaction
> 1. Transaction broadcast to P2P computers (nodes)
> 1. Miners verify the transaction
> 1. Transactions combined to form a data block
> 1. New block added to the existing blockchain
> 1. The transaction is complete



> **Note – Receiving Bitcoin Transactions**
>
> To receive bitcoin, you will need to provide the sender with a Bitcoin public address. This is a unique string of letters and numbers that represent your wallet and is used to identify it on the Bitcoin network.
>
> You can find your public address by opening your Bitcoin wallet and looking for an option to “Receive” or “Deposit” bitcoin.
>
> You can then share your Bitcoin address in one of several ways:
>
> 1. **Copy and paste the address**: You can copy the address by highlighting it and pressing "Copy", then paste it into an email or message.
> 1. **Share a link to your Bitcoin wallet**: Some Bitcoin wallets allow you to create a link to your wallet that you can share with the sender. They can then click on the link to access your wallet and send bitcoin.
> 1. **Share a QR code**: If the sender has a smartphone with a Bitcoin wallet app installed, they can scan the QR code to get your Bitcoin address.


Once the sender has your address, they can send you bitcoin by entering your address and the amount they want to send. The bitcoin is then sent from their wallet to your wallet.

The transaction is confirmed by the Bitcoin Network and usually takes about 10 minutes. For greater security, it is recommended to wait for two confirmations, which takes about 20 minutes.


> **Note – Sending Bitcoin Transactions**
>
> To send bitcoin, you will need a few things: a Bitcoin wallet, the recipient’s public address, and the amount of bitcoin you want to send.
>
> 1. Open your Bitcoin wallet.
> 1. Navigate to the “Send” button and paste the recipient's address in the "To" field. Alternatively, you can also scan the QR code if the recipient provides one.
> 1. Enter the amount of bitcoin you want to send in the “Amount” field.
> 1. Double-check the recipient’s address and the amount to be sent. Remember transactions are irreversible!
> 1. Before clicking “Confirm and Send”, we recommend you double-check the transaction details one more time to ensure that you are sending the correct amount of bitcoin to the correct address.
> 1. Broadcast the transaction and wait for the network to confirm the transaction.
>
> Now you know how to evaluate, select, and set up a self-custodial Bitcoin wallet. Sending and receiving bitcoin on the Bitcoin network are referred to as “on-chain” transactions. This is because the transactions occur on the main Bitcoin network and are recorder in the blockchain.
>
> On-chain transactions are the safest way to transact with bitcoin because of the decentralized verification provided by the network.
>
> However, on-chain transactions are slower and can be significantly more expensive than other options (which we will discuss in Module 7) due to the miner fee.



---


#### Activity: Transactions In Action

https://qr.myfirstbitcoin.org/transactions.pdf

**This is a cooperative exercise simplifying the basic roles of people involved in a Bitcoin transaction.**

###### Key Points

1. There are four types of participants in every bitcoin transaction: the sender, the recipient, miners, and node operators.
1. The sender must approve (cryptographically sign) the **amount of bitcoin** to send AND the **specific address** to send to.
1. The recipient must provide a **valid address** to the sender AND verify the transaction was successfully confirmed on the blockchain.
1. Miners ensure all criteria are valid before adding transactions to future blocks.
1. Node operators verify mined blocks are valid before updating their version of the blockchain (the ledger).

###### Student Tip

Rotate through all four roles to experience what each participant does.
