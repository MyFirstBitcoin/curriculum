# 9.3 How Transactions Work

Now that you understand public and private keys, as well as the roles of nodes and miners, here’s how a Bitcoin transaction works from start to finish.

1. Adam wants to send bitcoin to Gerardo. He creates a transaction with Gerardo’s address, the amount to send, and a fee.
1. Adam signs the transaction with his private key to prove ownership.
1. He broadcasts the transaction to the Bitcoin network.
1. Nodes receive it and check that it follows the rules, including verifying the signature and that Adam has enough bitcoin.
1. If valid, the transaction is shared across the network and added to the mempool, where pending transactions wait.
1. Miners pick transactions from the mempool and include them in a block they try to mine.
1. When a miner successfully mines a block, it is shared with the network and checked by other nodes.
1. If valid, the block is added to the blockchain. Gerardo receives the bitcoin.
1. As more blocks are added, the transaction gains confirmations, making it more secure.

Once included in a block, the transaction is confirmed. Adam cannot spend that bitcoin again, and Gerardo can spend what he received in a new transaction.


> **Note**
>
> Transaction & fee selected → Signed by wallet and sent → Distributed by nodes → Miner adds transaction to block template → Miner wins Proof-of-Work contest → New block is validated → New block is distributed by nodes


###### Resources


[▶ YouTube](https://www.youtube.com/watch?v=xc_TxlByxeY)
