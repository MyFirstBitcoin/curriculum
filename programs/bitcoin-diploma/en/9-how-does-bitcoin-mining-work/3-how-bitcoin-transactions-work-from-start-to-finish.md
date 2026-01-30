# 9.3 How Bitcoin Transactions Work from Start to Finish

Now that you know about public/private key cryptography and the roles of nodes and miners in more detail, it's time to do a last review of how Bitcoin transactions actually work:

1. Adam wants to send bitcoin to Gerardo. He picks one of his UTXOs, creates a transaction, and adds all necessary details — including the amount of bitcoin he wants to send, Gerardo’s receiving address, and a suitable transaction fee.
1. After a final check to ensure all details are correct, Adam uses his private key to sign the transaction.
1. Adam broadcasts the transaction to the Bitcoin network.
1. The nodes in the network receive the transaction and verify its validity according to theconsensus rules (like checking if Adam’s signature is valid and whether he has suﬃcient funds to make the transaction).
1. The transaction is marked valid, and the nodes propagate it to other nodes in the network, adding it to the mempool.
1. Since Adam picked a high enough transaction fee, almost all miners include his transaction in their candidate blocks.
1. Proof of Work: Miners race to mine their block by finding the valid block hash. One of the miners finds the hash and broadcasts their block to the network.
1. The nodes receive the newly mined block and verify its validity. This includes validating all transactions within the block and ensuring that the Proof-of-Work requirement is met.
1. The majority of nodes agree that the block is valid and add it to the blockchain. Gerardo receives the confirmed bitcoin at his receiving address.
1. As additional blocks are progressively added to the blockchain, the number of confirmations for the transaction grows. As the number of confirmations for the transaction increases, Gerardo can rest assured of its success and irreversible nature.

![ ](https://cdn.sanity.io/images/vje9ehw2/production/d9b90fafe63546c337c4a1cb706036b3a15036fa-457x274.svg)


> **Callout**
>
> In summary, the sender signs the transaction with their private key, the nodes verify the transaction's UTXOs, and the miners add the verified transaction to the blockchain.
>
> Once a block is mined, all the transactions included in it are considered confirmed and the UTXOs used as inputs in these transactions are considered spent and will not be used again. Instead, when the receiver decides to spend their newly received bitcoin, they will spend from the new unspent output (UTXO) created as a result of that transaction.


As we wrap up this chapter, you've gained valuable insights into the fundamental concepts behind how Bitcoin works. So far, we've covered the essential aspects not only of Bitcoin and its technicalities, but also of money in general and what defines it.

Now, let's tie it all together in the next chapter. Chapter 10 awaits, where we'll delve into the significant question: "What kind of future can Bitcoin empower us to create?"
