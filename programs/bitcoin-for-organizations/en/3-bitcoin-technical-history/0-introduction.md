# 3.0 Introduction

> **Info – The Bitcoin White Paper Abstract**
>
> **A purely peer-to-peer version of electronic cash** would allow online payments to be sent directly from one party to another without going through a financial institution. **Digital signatures provide part of the solution**, but the main benefits are lost if a **trusted third party** is still required to prevent double-spending. We propose a solution to the double-spending problem using a **peer-to-peer network**. The **network timestamps transactions** by hashing them into an ongoing chain of **hash-based proof-of-work,** forming a record that cannot be changed without redoing the **proof-of-work**. The longest chain not only serves as proof of the sequence of events witnessed, but proof that it came from the largest pool of CPU power. As long as a majority of CPU power is controlled by nodes that are not cooperating to attack the network, they'll generate the longest chain and outpace attackers. **The network itself requires minimal structure. Messages are broadcast on a best effort basis, and nodes can leave and rejoin the network at will**, accepting the longest proof-of-work chain as proof of what happened while they were gone.


Bitcoin didn’t appear in a vacuum but rather it built on the work of many in the previous decades. This chapter will explore the foundations of the internet that Bitcoin builds upon, as well as the research and development acknowledged in the whitepaper.

In the 70’s, a group of individuals looked at how the US Government in particular was trying to restrict access to cryptography, and set about ensuring that this technology would be made available for all people to protect their privacy online. Some of these early pioneers were also focused on the potential benefits of a digital ‘sound money’ system that could be used to store and exchange value over the emerging internet. Friedrich Hayek – a leading contributor to Austrian economics - envisioned what an ideal currency based on free market competition would look like well before the days of the internet, but decided that it was technically and politically infeasible. As well as digital privacy, this group, which evolved to become the Cypherpunks, attempted to realise Hayek’s vision for digital money, but these attempts had failed until Satoshi published his ideas on the mailing list.

* TCP/IP protocol (1976)
* Protocols for Public Key Cryptosystems - Ralph Merkle (1980)
* Digicash - David Chaum (1989)
* Digital Timestamping (90's)
* Hashcash - Adam Back (1997)
* BitTorrent - Bram Cohen (2001)
* Reusable POW - Hal Finney (2004)
* Bitcoin Whitepaper - Satoshi Nakamoto (2008)

A key influence on the development of Bitcoin was the emergence of this Cypherpunk movement in the 1990’s. They developed several cryptographic technologies including public-key cryptography to allow users to securely and privately communicate and share information. Many of the developments described here and the people involved were part of this group.

The need for digital cash was also identified and several attempts were made to create it, but these had limitations which stopped them from being successful. The genius of Satoshi Nakamoto was to pull these capabilities together, and along with some innovations of his own, built on them to create the Bitcoin protocol in use today. In the next sections we will explore some of these developments and explain how they helped inform the design of Bitcoin. We will also discuss what the missing pieces of the puzzle were that Satoshi managed to solve.
