# 3.4 Hashcash

Hashcash was created by Adam Back, another of the early innovators in this space. Adam had a strong interest in free markets and privacy on the internet, and came across the Cypherpunks mailing list which he joined and became an active participant of.

He was very interested in digital money, and made some suggestions of how the group could potentially work more closely on DigiCash with Chaum, but these didn’t go anywhere. He then turned his attention to another emerging problem – email spam. He and the rest of the Cypherpunks wanted to find a solution to the problem of spam, where it was trivial for spammers to create and send thousands of emails that clog up networks. His innovative solution was based on hashing – the capability with cryptography to turn any piece of data into a unique and random string of a specific length, to create the equivalent of a digital ‘stamp’ that needed to be added to the email for it to be considered valid and transmitted across the network. A trivial cost for a genuine email, but prohibitive to a spammer.

The key innovation that Hashcash created was tying real world resources- computational power – to a digital network. Whilst digital resources up until this point could be replicated without limits, the number of ‘hashcash’ created was limited by how much energy people were willing to invest in it.

Although the solution met some of the criteria that Adam believed was needed in a digital cash system; it was anonymous, resilient and trustless, each hashcash was not reusable and not truly scarce. He suggested other ways that these issues could be addressed using external third parties.

##### BItGold

Nick Szabo built on the concept of Hashcash and proof of work to propose an alternate solution, which he described in a mailing list a year after Hashcash was published, in 1998.

Whilst moving closer to a solution, this proposal still had several challenges.

* Who would run the Registry of hash ownership and how can they be trusted?.
* Hashing would generally get cheaper over time, a challenge for HashCash too.

As the linked hashes would be time-stamped, he proposed some form of historical tracking of the difficulty of hashing at the time; an earlier hash would require more processing costs than a later one as costs have come down. Unfortunately, this meant that hashes would not be ‘fungible’ i.e. of equal value, considered a key attribute of digital money. To help resolve this Nick suggested some form of ‘free banking’ working on top of BitGold that could aggregate different groups of hashes that would be valued the same.

##### B-Money

Soon after the Bit Gold proposal, Wei Dai proposed a similar solution. He had already developed several other tools for the Cypherpunks, and had his own ideas about digital money.

His proposal resembled Bit Gold in that it used digital signatures to transfer cash, and the records of transactions would be stored on a ledger, containing public keys and the amount of currency units attributed to each. As with Bit-Gold, trusted third parties were considered security holes, and the belief was that an electronic cash system should not rely on a single entity to track balances, transactions or to prevent double spend.

Wei-Dai proposed several solutions to these issues, one of which was that instead of a central entity(ies) maintaining the ledger, ALL nodes would maintain a copy. If all users checked their own ledger and the validity of each transaction, as long as all nodes remain up to date then the ledgers should remain synchronised across the network. This highly distributed system would be difficult to corrupt.

Wei Dai recognised that this didn’t solve the Byzantine generals problem (1), as nodes could easily lose synchronisation or simply lie. He suggested alternate methods such as having a subset of ‘trusted’ servers that maintain the ledger, and creating financial incentives to keep these servers honest.

For monetary policy, he proposed pegging purchasing power of B-Money to some form of external consumer price index. He wanted the same amount of B-Money to be able to buy an equal share of the index over time, providing some price stability. So, anybody could generate new currency units by providing a valid hash, but the difficulty of generating a hash may change over time based on CPU costs and the price index, so that each unit would be ‘immutable’.
