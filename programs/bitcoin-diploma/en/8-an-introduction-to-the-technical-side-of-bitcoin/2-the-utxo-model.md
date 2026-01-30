# 8.2 The UTXO Model

##### What are UTXOs?

![ ](https://cdn.sanity.io/images/vje9ehw2/production/f34962a29b04842b5d9b38ba1cefcfd89d3ab2aa-233x159.svg)

Don't be scared of the strange name. You can think of UTXOs as diﬀerent "sizes" of bitcoin, just like thephysical bills or coins in your wallet represent diﬀerent amounts. For instance, at the story you pay for a $6 item with a $10 bill and get back $4 in change. UTXOs function similarly.

All the bitcoin you hold is divided into UTXOs of varying sizes. Each time you spend bitcoin you do it from one or several UTXOs, just like with physical cash, to cover the purchase's price.

That UTXO is then broken down into several smaller UTXOs: first, a new UTXO is created in the recipient's wallet, representing the value you transferred to your peer; second, if the value of the UTXO you spent from exceeds the value you sent, you will get the rest back as "change," creating a new UTXO in your wallet for that amount; finally, a small amount was deducted from the original UTXO to cover the fee necessary to compensate the miner.

The diﬀerence with physical cash is that UTXOs don't have set denominatios [m dash] such as $1, $5, $10 dollar bills. Instead, the numeric value of the UTXO is entirely determined by what remains unspent, which you get back as "change;" hence the name Unspent Transaction Output, or "whatever you get back after spending from a UTXO."

The balance of your Bitcoin wallet is the sum of all your UTXOs. So, the sum of your UTXOs is the sum of the amount of bitcoin you own.


> **Callout**
>
> It is important to note that you should not make others aware of your UTXOs because when someone knows them, they can track your bitcoin transactions in the network and will ultimately know how much money you own.


In conclusion, each time you make a transaction, you use one or more of your existing UTXOs to spend bitcoin and new UTXOs are created (for both you as the recipient).

![ ](https://cdn.sanity.io/images/vje9ehw2/production/d8bba28a93d04ba56a5ab494ae35ef7e32c6054e-500x137.svg)

When a transaction is made, the amount of bitcoin sent is divided into multiple outputs, each of which is associated with a new Bitcoin address (a new UTXO).

When sending bitcoin to someone, you will use one or more UTXOs as the source of the funds (input). These UTXOs will be combined, if necessary, to create new outputs that belong to both the recipient of the transaction and yourself. These new outputs, or UTXOs, will become the recipient’s property and your property. These UTXOs can then be used as inputs in future transactions. This chain of UTXOs creates a transparent, traceable history of all Bitcoin transactions on the ledger, starting from the very first block (January 3rd, 2009).



##### Here's an example of how this works:

![ ](https://cdn.sanity.io/images/vje9ehw2/production/629683a3eca4b29cf4831b571bd7e53e9d05310c-237x161.svg)

1. Alice wants to send Bob 5 BTC
1. She combines two of her UTXOs for a value of 6 BTC
1. From these UTXOs, 5 BTC go to Bob: he will see a new UTXO worth 5 BTC on his wallet's balance
1. Alice receives a new UTXO worth 0.99 BTC, which is her change after paying the 0.01 BTC transaction fee
1. After confirmation, the transaction is added to Bitcoin’s ledger, updating all the nodes that have a copy of the ledger

If Alice attempts to use one of her already spent outputs to make another transaction, it will automatically be rejected by the nodes. This is because the nodes maintain a copy of the Bitcoin ledger (and all its transactions), so they can easily check the rightful ownership of each UTXO on-chain, and verify that the transaction is not valid.

Below are screenshots of two real transactions. What observations can you make when you look at the two transactions below? Do the inputs match the outputs? Can you describe the details of the transaction? Is there a connection between the two screenshots? And which transaction occurred first?

![ ](https://cdn.sanity.io/images/vje9ehw2/production/c97a46bc952adc47b51df029a93ab664303d32d6-234x165.svg)

In this chapter you've learned more about the technical side of Bitcoin. You've gained a deeper understanding of the protocol's security through cryptography, learned what a hashing function is, and, finally, seen how transactions actually work in the UTXO-based model.

In Chapter 9, we will take a closer look at nodes, and specifically at a very special type of node: miners. Then, we will once again return to Bitcoin transactions to give the full account, from start to finish.
