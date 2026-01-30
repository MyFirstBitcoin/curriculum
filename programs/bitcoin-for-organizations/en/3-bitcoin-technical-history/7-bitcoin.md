# 3.7 Bitcoin

After many years and failed attempts, the Cypherpunks had for the most part begun to lose interest in the idea of a digital permissionless currency, when Adam Back received an email linking to a draft white paper called ‘electronic cash without a third party’ from an anonymous person calling himself Satoshi Nakamoto.

To recap at this point, we have at least the ideas of:

* Cryptographic signatures that could provide a level of privacy and anonymity
* Concept of an unbacked currency (B-Money)
* Proposals (but no means) for limiting the issuance of new currency
* Digital coins whose ownership was attributed by public keys (B-Money) and could be moved by signing and reassigned based on recipient address (RPOW and Hashcash)
* All nodes maintain a copy of a totally distributed ledger (B-Money) (dismissed at the time as impractical)
* Time-stamping protocol– using Merkle tree hashing to provide a mathematically provable chronology of events that is difficult to falsify if all users kept the same records
* Proof of work to tie real world effort to the system (but using the hash itself as the currency)
* Totally decentralised networks where all peers are equal and could come and go from the network (BitTorrent)
* Concept of tying new hashes to previous hashes (Bit Gold and time-stamping)

What was lacking at this time included:

* A viable solution to solve the ‘Byzantine generals’ problem
* A method to limit the amount of money in circulation despite continuous hardware improvements
* Incentives scheme for people to participate (chicken and egg issue)

The other major difference between recent attempts and Bitcoin was that Satoshi had been working on the code for some time in the true ‘Cypherpunks write code’ original ethos before announcing it on the mailing lists, unlike Bit Gold and B-Money which were more conceptual.

What was the innovation that set Bitcoin apart from previous attempts at electronic cash ?

Proof of work would be used as a consensus mechanism and a way of providing security and immutability: Instead of using the hash as a form of money, it would be used by a new conceptual process called mining, where a node would batch together a set of transactions, add a random number and then apply the hashing to the ‘block’ of data. A valid block that met the hash requirement would then be advertised to the network. These blocks would be tied together using the hash of the previous block in each, and the longest blockchain would be used in the event of a tiebreaker where different nodes would validate and advertise different blocks at the same time to create chain splits. Proof of work became the distributed tie-breaker to resolve the Byzantine generals problem.

These miners were also given an incentive to provide the CPU required to carry out the proof-of-work by being allocated new bitcoin for each block. The amount of Bitcoin they are awarded is also programmed to go down approximately every 4 years until all Bitcoin has been created, creating a hard limit to the total Bitcoin that will ever be in circulation to 21M.

The most original idea was the way in which he resolved the issue of how much money is created as hardware improves and more power can be applied to the network. The timestamps of a set number of blocks (2016) would be averaged out, and if they are being created too quickly, the hash needed to create a new block would be made more difficult, if too slowly it would be made easier. This was built into the decentralised protocol that all nodes run and so any miner ignoring it would expend energy to mine a block for no benefit as it would be rejected by the rest of the network. This adjustment ensures that the creation of new blocks remains on the planned schedule of issuance, and provides incentives for miners to ‘play by the rules’.

####   
Summary

Many of the pieces of the puzzle of what it takes to build a decentralised peer to peer electronic cash system based on sound money principles were in place before Satoshi released his whitepaper and soon after the initial release of the code.

> The nature of Bitcoin is such that once version 0.1 was released the core design was set in stone for the rest of its lifetime  
_Satoshi Nakamoto_

Whilst many ideas for improvements (BIPs) have been proposed and adopted, Bitcoin has been working away in the background since 2009 following the protocol designed into the initial release and with barely any disruption. All improvements have been made whilst enabling backward compatibility with all previous versions.



##### Notes

1. For an explanation of the Byzantine Generals problem - see https://en.wikipedia.org/wiki/Byzantine_fault
