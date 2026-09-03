# 8.10 Users, nodes, miners, developers, and services

Use these exact beginner boundaries:


| Role | Main beginner function | Does not mean |
| --- | --- | --- |
| User | Chooses to receive, hold, send, verify, and accept bitcoin, directly or through services | Automatically runs every part of the network |
| Node | Independently checks transactions and blocks against its rules and relays valid data | Creates new blocks or dictates rules to everyone |
| Miner | Builds candidate blocks and performs proof of work to propose their order | Can make invalid issuance or transactions valid to honest nodes |
| Developer | Reviews, writes, and proposes software | Can force participants to adopt a rule change |
| Bitcoin service | Provides a wallet, exchange, explorer, payment, or other interface | Is the Bitcoin protocol itself |


#### Activity: invalid block

Give one learner acting as a miner a candidate block that creates more subsidy than the node rule card allows. Learners acting as nodes check it and reject it.

Debrief:

* The miner did real work but still did not gain permission to break the rules.
* Nodes independently apply rules, but the real network is software and communication, not a classroom vote.
* A developer can write other rules, but adoption is voluntary and incompatible rules may create a separate network.

Ask:

> Why does a node verify transactions? Name at least one rule it checks.
