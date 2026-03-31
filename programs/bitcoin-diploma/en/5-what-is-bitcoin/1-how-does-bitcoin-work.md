# 5.1 How Does Bitcoin Work?

#### The Nakamoto Consensus Mechanism

So, how does Bitcoin work? Bitcoin has lots of features, and the rabbit hole goes deep — very deep. Fortunately, if you're entering the Bitcoin world for the first time, you do not have to perfectly understand how it works to start using it.

The same is true for the internet: most people do not know how the TCP/IP protocol works, yet they send emails and messages, and post content on their social media every day. It's just like driving a car — most people do not know exactly how a car works, yet they do know how to drive.


> **Callout – Bitcoin is not widely adopted yet**
>
> Bitcoin is not widely adopted yet. It is still a pretty new technology, like the internet was during the 90s. Because of this, it can be helpful to focus on the fundamentals of Bitcoin, rather than on its technical aspects.


The key idea behind how Bitcoin operates can be condensed into one sentence: Bitcoin is a common set of rules agreed to by all network participants. You can think about it as playing a board game with friends. In a game like Monopoly, you are in agreement with the other players about specific rules. One of the rules of Monopoly is that only special “Monopoly bills” are to be accepted. If James (one of the players) decided against the rules to use toilet paper instead of Monopoly bills to buy a house, the other players would tell James he is a cheater and would simply stop playing with him. In short, to play the game, you need consensus on a set of rules and to agree with each other not to deviate from those rules, or you will be rejected.

This is essentially how Bitcoin works. Bitcoin is a network of people that agree on the same set of rules. These rules are mathematically bound, written in computer code, and accepted directly by everyone who runs the Bitcoin software. The rules of Bitcoin apply to all participants equally, which means that each player either follows the rules of the game or cannot play because the network will reject them.

For example, one of the rules of Bitcoin is "There will never be more than 21 million bitcoin." If someone were to create a million extra bitcoins for themselves, it would be of no use to them, because they would automatically be identified and rejected by everyone else. This is what makes Bitcoin so robust.


> **Info**
>
> It does not matter who you are or where you come from: if you enter the Bitcoin world, you must play by the same set of rules as everyone else.


This also applies to all the people and entities with disproportionate influence in the fiat world. In the Bitcoin world, there is no room for cheating or sabotage — everyone is treated equally, and no one can change that.


> **Callout**
>
> Did you know that, since 2009, Bitcoin has withstood tens of thousands of attempts to hack, tamper with, or alter it? Bitcoin has consistently proven that nobody can stop, control, or manipulate it.


#### The Players of the Game

To better understand the decentralization of Bitcoin, we need to dive deeper into the diﬀerent roles within the network. In the Bitcoin world, various participants play distinct yet harmonious roles, contributing to the protocol's seamless functioning.

##### 1. Miners: The Architects of Security

![ ](https://cdn.sanity.io/images/vje9ehw2/staging/e9d1728c47b7f769af79edbeeba097c9de253aa0-164x164.svg)

Miners are the backbone of Bitcoin. They work behind the scenes to maintain and secure the network through a mechanism called Proof-of-Work (PoW).

These players are armed with special computers that boast heavy computational power. They make this power available to the Bitcoin network, competing with each other in a worldwide lottery to add new blocks of transactions to Bitcoin’s decentralized ledger (the blockchain). Their commitment ensures the the ledger's immutability and guards against malicious attacks.

The decentralized nature of mining means that anyone can participate — in practice, however, competition is fierce. As a reward for their contribution, the first miner who solves the puzzle is rewarded in the form of new bitcoin, an incentive known as the block reward.

Bitcoin miners are distributed all over the world, safeguarding the network against centralization and ensuring Bitcoin's security stays robust and distributed.

##### 2. Nodes: Gatekeepers of Validation

![Bitcoin Nodes](https://cdn.sanity.io/images/vje9ehw2/staging/aaca4f0fcdedbbf9fd2bfb064ee70b480bc966d3-267x138.svg)

Bitcoin nodes are run by ordinary people across the planet. These participants serve as the Bitcoin network's gatekeepers by running Bitcoin software on their computers on which they keep a copy of the entire ledger. Nodes validate transactions and ensure that all participants adhere to the consensus rules.

By distributing the responsibility of validation across a network of nodes, Bitcoin remains resilient against attacks and maintains its trustless nature. Nodes play a crucial role in upholding the integrity of the ledger, contributing to the Bitcoin's decentralization ethos.

##### 3. Users: Empowered Participants

Users — the lifeblood of the Bitcoin network — are individuals who engage in transactions. You can think of users as regular people who just have empowered themselves by integrating Bitcoin into their lives. For example, some users save their money in bitcoin while others use it as money to buy groceries and receive their salary.

Bitcoin empowers users by eliminating the need for intermediaries like banks and governments, allowing for direct peer-to-peer transactions. This also means that users have full control over their money and transactions.

##### 4. Developers and Projects: Architects of Innovation

The monetary system of the future won't build itself, nor will it be globally adopted in an ethically correct way without eﬀort. That’s where Bitcoin developers and projects come into play. Developers wield their technical expertise to enhance and innovate on the Bitcoin protocol. These individuals contribute code, propose improvements, and address vulnerabilities, ensuring the network evolves in response to all types of challenges. Bitcoin's open-source nature invites collaboration, allowing developers worldwide to contribute to its growth.

The beauty of this decentralized development prevents a single entity from monopolizing control over the protocol. This happens through a consensus-driven process. Developers propose ideas and changes, and only those with the best ideas who are aligned with the broader vision for a better world receive support from the community, empowering Bitcoin's transparent and democratic evolution as it scales to 8 billion people.

Bitcoin projects involve diverse groups, from mission-driven nonprofits and corporations to groups and individuals who create valuable content. These people work together on a specific goal or focus within the bigger Bitcoin mission toward collective freedom. Bitcoin projects play a crucial role in shaping and promoting the adoption of Bitcoin, working toward a future that prioritizes the empowerment and freedom of the human race.


---


#### The Symphony

Bitcoin's decentralization can be thought of as a synergetic orchestra, a balancing act where all the different musicians make the most beautiful music together. There is no boss in the Bitcoin network: miners, nodes, users, developers, and projects perform their roles with autonomy and collaboration.

The decentralized ledger, maintained by nodes, guarantees transparency, while the proof-of-work mechanism provides security and deters centralization in mining; users experience financial sovereignty and empowerment, free from the control of the fiat system; developers, guided by consensus, ensure the protocol adapts to meet the evolving needs of humanity; Bitcoin projects, in their own unique ways, contribute to the broader mission of collective freedom.

Each participant in this decentralized orchestra plays a vital role in shaping Bitcoin's adoption and empowering humanity, contributing to the resilience and longevity of Bitcoin and creating a trust-free, borderless and empowering ecosystem.


> **Callout – Summary**
>
> The symphony of decentralization in Bitcoin resonates as a testament to Satoshi Nakamoto's vision and the immense passion of a global community seeking freedom and empowerment.


![Networks](https://cdn.sanity.io/images/vje9ehw2/staging/a9129cf63654e10793f6767f8617e820a3a09f19-344x235.svg)


---


#### Activity: Consensus

https://qr.myfirstbitcoin.org/consensus.pdf

This is a class exercise where participants learn firsthand how difficult synchronizing actions is in a group without a defined leader. The intent is for participants to understand how agreement (consensus) is achieved in Bitcoin.

###### Key Points

1. **Consensus = agreement**
1. One big difference between a group with centralized control and one without is the question of trust. Decentralized groups like peer-to-peer networks do not have a leader and participants do not trust each other. They require a different way to coordinate.
1. For developers of peer-to-peer networks, this is known as the Byzantine Generals Problem. Bitcoin solves this challenge with math and proof-of-work mining.
1. Bitcoin being decentralized is critical to its value. Historically, human leaders always succumb to the temptation to debase money over the long term.
1. The Nakamoto Consensus is named after the creator of Bitcoin, Satoshi Nakamoto. This consensus mechanism is how thousands of strangers who do not trust each other have maintained the Bitcoin ledger since 2009.
