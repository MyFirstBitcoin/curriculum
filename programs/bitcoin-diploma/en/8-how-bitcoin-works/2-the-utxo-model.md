# 8.2 The UTXO Model

##### What are UTXOs?

Don’t be intimidated by the strange name. You can think of UTXOs as pieces of bitcoin, similar to the bills and coins in your wallet. For example, if you pay for a $6 item with a $10 bill, you receive $4 in change. Bitcoin works in a similar way.

All the bitcoin you own is made up of different UTXOs. When you send bitcoin, your wallet uses one or more of these pieces to make the payment.

If the piece you spend is larger than the amount you send, the remaining value comes back to you as change in the form of a new UTXO. At the same time, the recipient receives a new UTXO representing the bitcoin you sent.

Your wallet balance is simply the total value of all the UTXOs you control.


> **Callout – Privacy**
>
> It is important to note that you should not make others aware of your UTXOs because when someone knows them, they can track your transactions and will ultimately know how much money you own.


###### Example

1. Alice wants to send Bob 5 BTC.
1. Her wallet uses two of her UTXOs that together are worth 6 BTC.
1. The transaction sends **5 BTC to Bob**, creating a new UTXO in Bob’s wallet.
1. The remaining **0.99 BTC returns to Alice as change**, after paying a **0.01 BTC transaction fee**.
1. Once the transaction is confirmed, it is added to Bitcoin’s ledger and the UTXOs used by Alice are marked as spent, so they cannot be used again.

###### Resources


[▶ YouTube](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
