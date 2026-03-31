# 8.4 A Walk Through the Ledger: The Pizza Day Transaction

So far, this module has focused on using the open nature of the Bitcoin ledger to compile useful metrics from aggregated transaction data. However, it is possible to use ledger data and block explorers to examine real-world transactions and trace the movement of funds within the network.

Every year on the 22nd of May, the Bitcoin community acknowledges Laszlo Hanyecz, who became the first person reported to use bitcoin to purchase physical goods. On the 18th May 2010, Hanyecz announced on a Bitcointalk.org forum that he was looking for pizza and was willing to pay in BTC. He offered 10,000 BTC to anyone willing to enter into the transaction. He waited for several days, until 19-year-old student Jeremy Sturdivant obliged and sent two large pizzas.

The ’Pizza Day’ transaction can be viewed by anyone and has the following transaction ID:

**a1075db55d416d3ca199f55b6084e2115b9345e16c5cf302fc80e9d5fbf5d48d**

Entering this transaction ID into mempool.space reveals the following:

![Transaction](https://cdn.sanity.io/images/vje9ehw2/staging/d9b23ca4a14b433f0540a0920a1a1eb9662cad37-1126x268.png)



Date of time of the transaction: 22nd May 2010

Network transaction fee: 99,000,000 sats (at the time it equalled less than 1 US cent. In May 2025, this stands at $95,072.67)

The Block Height: 57,043

The Number of Confirmations: 838,645 (this is the number blocks added to the ledger after this transaction)

![Inputs & Outputs](https://cdn.sanity.io/images/vje9ehw2/staging/dde2d64b67678116d039740c63ba279c27cc8703-1149x571.png)



![Address](https://cdn.sanity.io/images/vje9ehw2/staging/c6d7be3be795a922e7850718408570234b206615-573x253.png)

Number of Transaction Inputs: 131

Number of Transaction Outputs: 1

Clicking on the output public key (ending in ‘XaxFyQ’) that we know was owned by Jeremy Sturdivant who received 10,000 BTC for two pizzas, reveals the following:

This address currently has a balance of 0.00257879 BTC (approx. $248.87) and it appears that it has been involved in 14 transactions, the most recent of which was on 13th December 2024.



#### 8.4.1 Activity: Group Discussion

1. Describe the benefits (e.g. auditing, accountability) or risks (e.g. privacy concerns) for individuals or businesses using such a transparent and open transaction system.
1. How might this kind of financial transparency affect industries like charity, government procurement, remittances or law enforcement?
1. Should traditional banking systems offer a similar level of visibility? Will they be forced to by the market?
