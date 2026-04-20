# Network Participants Role Guide

# Network Participants Role Guide

Who participates in Bitcoin and what each role does.


---

## **Users / Hodlers**

**What they do:** Send, receive, hold Bitcoin\n**Incentive:** Store wealth, make payments, participate in network\n**Example:** Anyone with a wallet\n**Power:** Choose which software to run; vote with their adoption


---

## **Miners**

**What they do:** Solve math puzzles; create new blocks; validate transactions\n**Incentive:** Earn block reward (6.25 BTC) + transaction fees\n**Equipment:** Specialized hardware (ASICs); electricity\n**Power:** Can order transactions in a block; cannot reverse past transactions or break consensus rules


---

## **Node Operators**

**What they do:** Run Bitcoin software; keep full copy of blockchain; validate all transactions and blocks\n**Incentive:** Participate in network security; maintain Bitcoin rules without permission\n**Equipment:** Computer running Bitcoin Core (or other implementation)\n**Power:** Reject invalid blocks/transactions; enforce consensus rules; cannot mine but can validate


---

## **Developers**

**What they do:** Write and maintain Bitcoin code; propose protocol improvements (BIPs)\n**Incentive:** Technical contribution; Bitcoin philosophy alignment; community respect\n**Examples:** Bitcoin Core maintainers, protocol researchers\n**Power:** Can propose changes, but cannot force adoption; community consensus required


---

## **Exchanges & Custodians**

**What they do:** Buy/sell Bitcoin; hold Bitcoin for users (custodial wallets)\n**Incentive:** Transaction fees; trading spreads; margin interest\n**Examples:** Coinbase, Kraken, Binance\n**Criticism:** Custodial model contradicts Bitcoin's self-custody principle; single point of failure


---

## **Merchants & Businesses**

**What they do:** Accept Bitcoin as payment; use Bitcoin payment processors (BTCPay, Bitpay)\n**Incentive:** Lower fees than credit cards; attract Bitcoin-savvy customers; store-of-value hedge\n**Examples:** Online retailers, coffee shops, services\n**Advantage:** No chargebacks; irreversible transactions; transparent fees


---

## **Miners (Mining Pools)**

**What they do:** Coordinate many small miners; combine hash power; distribute rewards\n**Why pools exist:** Solo mining has low probability of winning blocks; pools increase consistency\n**Drawback:** Increases centralization (pool operators could censor); still more distributed than central banks


---

## **Ecosystem Developers**

**What they do:** Build wallets, exchanges, Layer 2 solutions, analytics tools\n**Incentive:** Business opportunity; Bitcoin adoption\n**Examples:** Wallet developers (Blue Wallet, Muun), Lightning developers, analytics sites\n**Dependency:** Depend on Bitcoin protocol but independent from core developers


---

## **How They Interact**

```
User wants to send Bitcoin:
1. User creates transaction in wallet (software by ecosystem developer)
2. Transaction broadcast to network
3. Nodes validate transaction is legitimate
4. Miners include transaction in new block (competing for block reward)
5. Miners solve Proof of Work puzzle
6. New block broadcast to network
7. Nodes validate block
8. Transaction confirmed; Bitcoin moved
9. If Merchant: uses processor to convert to fiat (exchange/custodian) or hold as Bitcoin
```


---

## **Why Decentralization Matters**

**If Bitcoin had only ONE of each:**

* 1 miner → controls what transactions happen
* 1 node → controls what blockchain is valid
* 1 developer → controls code changes
* 1 exchange → controls who can buy/sell

**With many of each:**

* No single entity can control Bitcoin
* If one fails, network continues
* Competition improves security and innovation


---

## **Discussion Prompts**

* "If you were a miner, why would you follow the rules instead of stealing Bitcoin?"
* "What happens if miners and nodes disagree on which blocks are valid?"
* "Why do we need both miners AND nodes?"
* "Is a large mining pool a threat to Bitcoin?"


---

*Every role matters. Bitcoin's strength is in redundancy and diversity.*