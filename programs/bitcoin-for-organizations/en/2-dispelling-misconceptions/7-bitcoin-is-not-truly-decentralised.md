# 2.7 Bitcoin is not truly decentralised

> Crypto’s complexity arises from attempts at decentralisation—by distributing power and governance in the system, there is theoretically no need for trusted intermediaries like financial institutions. That was the premise of the initial Bitcoin white paper, which offered a cryptographic solution intended to allow payments to be sent without involving any financial institution or other trusted intermediary. However, Bitcoin became centralized very quickly and now depends on a small group of software developers and mining pools to function  
_International Monetary Fund_

As the quote above from a fairly recent post by the International Monetary fund shows, the mainstream financial industry continues to claim that Bitcoin is not decentralised, as well as confusing Bitcoin with other crypto assets.

##### Introduction

![Trilemma](https://cdn.sanity.io/images/vje9ehw2/staging/ff9d3a607afc6bf60f358eef412a749ce3e47c40-161x167.svg)

Decentralisation is a critical aspect of Bitcoin. The ability to maintain the rules of the protocol such as scarcity and distribution without a central authority ensures that it can act as permissionless money for a global society.

As Satoshi noted in his online correspondence, decentralised services such as BitTorrent were ‘holding their own’ against Government clampdowns, in comparison to services with identified owner(s) and decentralised servers. He was clearly concerned about the potential risk of Governments or other interests shutting down or otherwise adversely affecting Bitcoin.

In this context, we are interested in decentralisation of:

* The development and management of the code running the protocol; who is allowed to change the rules?
* The mining function that created new blocks in accordance with the rules and validates against double-spend
* The nodes that validate transactions for validity and keep a copy of the blockchain

##### Developers

Bitcoin is an open-source protocol that anyone is free to look at, download, copy or suggest changes to. It is available in a GitHub library, the source code having been launched originally in 2009 By Satoshi Nakamoto. Anyone is free to download the code and run a node, the majority of which run the original Bitcoin core software, which has been updated over time.

![How Does an idea Make Its Way Into Bitcoin Core?](https://cdn.sanity.io/images/vje9ehw2/staging/49f70d059c9dbe19a6e4500e9abd8db66ca97bff-1300x1439.png)

_Source: https://river.com/learn/what-is-bitcoin-core/_

Bitcoin Core development follows the best practices of open source development. At any time, there can be any number of developers writing or reviewing code changes. They need to listen to the concerns of the node operators and miners, as well as the user base before making any critical change to the code, which will be reviewed and agreed on as shown in the above flowchart before finding their way into the code.

The rules of Bitcoin are then encoded in this Bitcoin Core software, which runs on each node. Anyone can suggest a change to the rules – the rules are code, but they are not _just_ code, they are _agreed-upon_ code. If changed unilaterally, the new code is no longer part of consensus and is no longer part of Bitcoin. Changing something with Bitcoin and remaining in consensus is tricky. Suggested changes to the code fall into one of three categories:

* Within existing rules: Minor upgrades such as spelling errors, nicer UI or data management may fall into this category and are relatively trivial to gain approval for.
* Adding a new rule that adds restrictions to the rules – such as reducing the block size. This is referred to as a ‘soft fork’. Nodes that choose not to implement the code change and stay on the old release will still be able to take part in the network.
* Adding a new rule that breaks the current rules, e.g. an increase in block size. Nodes that do not upgrade to the new code will dismiss a block created in the larger size as invalid. This is referred to as a ‘hard fork’ and will create a chain split between the nodes running the original and new code and creates a new coin. This has happened previously but has not led to any long-term success for the new coin as the majority of the nodes decided to keep to the original code.

Therefore, a single party or group of people cannot unilaterally change the Bitcoin code without gaining a consensus agreement, or they risk a chain split and the creation of a new coin following a different set of rules.

##### Mining

The mining function validates the transactions just like any other node on the network, but it will then expend the energy required to create a new block which meets the consensus rules in the code. Success enables the miner to gain the rewards in the form of transaction fees and Bitcoin rewards (at the time of writing 3.125 coins per block).

Mining is normally carried out by mining ‘Pools’ where people consolidate the mining power or hash rate together to increase the chances of successfully mining a block and sharing the rewards. There is a danger that one or more of these mining pools could combine together to achieve a 51% dominance in mining and essentially overrule the network validation protocol in their favor to double spend coins. This would require a massive amount of resources to achieve at great cost, and individual miners can very easily move to a different mining pool at any time. Such an attack would also likely collapse the value of bitcoin, since it would be obvious that the network integrity had been compromised. An attacker would therefore have to convert any bitcoin gained quickly to fiat before the value erodes. This would make it even more difficult to sustain an attack for a long period, and therefore makes it more profitable for a miner or a pool operator to adhere to the rules and attempt to mine valid blocks.

The geographic distribution of the mining function is also important to avoid governments for example taking over mining capacity or shutting it down. For example, a recent ban on mining by China demonstrated the ability for Bitcoin to adapt and survive such government intervention, adapting and recovering quickly from the resultant loss of hash power.

##### Nodes

Unlike mining, which requires a significant financial investment to effectively compete in the race to mine new blocks, or code development which requires coding expertise, running a node is something that anybody interested in helping to maintain the decentralisation of Bitcoin can do.

Nodes run the Bitcoin Core software and enforce the rules that the code includes to ensure that the miners don’t cheat, for example by allocating themselves a greater block reward than is allowed. They also enforce the 21 million supply cap, which is critical to maintain the scarcity of Bitcoin. For any government or bad actor to stop Bitcoin, it would have to destroy every single copy of the blockchain, currently running in thousands of nodes distributed globally, an almost impossible task.

##### People

Another aspect of potential centralisation is people. Every other ‘alt-coin’ has a figurehead- someone that could be potentially coerced into advocating for changes not in the best interest of Bitcoin. Satoshi Nakamoto stayed around long enough to ensure that Bitcoin was on a path to success before disappearing for good, leaving it in the hands of others to enhance and adapt the software.

What about holders of large amounts of Bitcoin? Early investors, that have held their coins and not lost them, will be extremely wealthy at this point. It is important to note that this may well be the case, but that doesn’t give them any more influence on the system than anyone else, unlike the ‘proof of stake’ coins where the early adopters who are already wealthy in that coin gain advantages in decision making and distribution of future coins. This has or will inevitably lead to centralization over time.

##### Conclusion

What are the potential threats that decentralisation can try to mitigate?

* Government shutting down or banning Bitcoin
* Unwanted changes to the code that favors one set of interests in Bitcoin, e.g. increasing the block reward
* Coercion of the protocol by government or bad actors to influence the direction of the protocol
* Ability for a pool of miners to take over the network and ‘double-spend’ Bitcoin – a 51% attack

As we can see, the combination of nodes, code developers and miners, as well as the use of the ‘proof of work’ mechanism, decentralises Bitcoin to a sufficient level where these potential threats are not considered to be of great concern. The community will need to continue to monitor the situation to ensure this remains the case.
