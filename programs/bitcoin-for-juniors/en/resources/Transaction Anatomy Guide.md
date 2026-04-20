# Transaction Anatomy Guide

# Transaction Anatomy Guide

Understanding what happens inside a Bitcoin transaction.


---

## **Basic Transaction Structure**

```
TRANSACTION
├── Inputs (What you're spending)
│   ├── Input 1: UTXO #1 from previous transaction
│   ├── Input 2: UTXO #2 from previous transaction
│   └── Input Signature: Proof you own these UTXOs
├── Outputs (Where it goes)
│   ├── Output 1: 0.5 BTC to recipient address
│   └── Output 2: 0.45 BTC to your change address (leftover)
├── Metadata
│   ├── Amount: Total input - total output = fee
│   ├── Fee: 0.05 BTC (goes to miner)
│   └── Timestamp: When transaction was created
```


---

## **Step-by-Step Example**

### **You want to send 0.5 BTC to a friend**

### **Step 1: Wallet shows your balance**

```
You own:
- UTXO A: 0.7 BTC (received last week)
- UTXO B: 0.3 BTC (received yesterday)
Total available: 1.0 BTC
```

### **Step 2: You initiate send**

```
Recipient: Alice's address (bc1qxy2kgdyhjm7h24j...)
Amount: 0.5 BTC
Fee: 0.0005 BTC (chosen by wallet based on network congestion)
```

### **Step 3: Wallet creates transaction**

```
Inputs:
- Spend UTXO A (0.7 BTC) — because it's enough to cover 0.5 + 0.0005 fee

Outputs:
- 0.5 BTC → Alice's address
- 0.1995 BTC → Your change address (0.7 - 0.5 - 0.0005 = 0.1995)

UTXO B (0.3 BTC) remains unspent
```

### **Step 4: Wallet signs with your private key**

```
Digital signature proves you authorized this spending
- Proves you own UTXO A
- Proves you haven't changed the transaction
- Does not reveal private key
```

### **Step 5: Transaction broadcast to network**

```
"Hey network, here's a transaction:
- Spend 0.7 BTC that I own (UTXO A)
- Send 0.5 to Alice
- Send 0.1995 to my change address
- Here's my proof (digital signature)
```

### **Step 6: Nodes validate**

```
Nodes check:
✓ UTXO A hasn't been spent before
✓ Signature is valid
✓ You have authority (private key holder)
✓ Amounts add up correctly
✓ Not a double-spend

Verdict: VALID
Transaction enters mempool (waiting room)
```

### **Step 7: Miners include in block**

```
Miners see transaction in mempool
Compare fee rate: 0.0005 BTC for ~250 bytes = ~2000 satoshis/byte
(High fee = high priority)

Miners include it in next block
(Miners prioritize higher fees first)
```

### **Step 8: Block is mined**

```
Miner solves Proof of Work puzzle
Block is broadcast to network
Your transaction is now "1 confirmation"
```

### **Step 9: More blocks confirm**

```
After 6 blocks (~60 minutes):
- Network strongly agrees transaction is valid
- Extremely difficult to reverse
- Alice considers 0.5 BTC received
```


---

## **Fee Mechanics**

### **Fee Calculation**

```
Fee = Total Input - Total Output
Fee = 0.7 - (0.5 + 0.1995) = 0.0005 BTC

Fee Rate = Fee / Transaction Size
Fee Rate = 0.0005 BTC / 250 bytes = 0.000002 BTC/byte = 20 satoshis/byte
```

### **Fee Priority**

```
Network Congestion Status: 50,000 unconfirmed transactions in mempool

Miners choose:
- High fee (100 sat/byte) → included in next block (~10 min)
- Medium fee (20 sat/byte) → included in next few blocks (~30-60 min)
- Low fee (5 sat/byte) → might take hours or days

During high congestion: high fee necessary
During low congestion: low fee acceptable
```


---

## **Confirmation Timeline**

| Time | Status | Security |
|------|--------|----------|
| 0 min | Broadcast to network | Not yet confirmed |
| \~2-10 min | Included in mempool | Visible but unconfirmed |
| \~10 min | 1 confirmation | 1 block deep |
| \~20 min | 2 confirmations | Unlikely to reverse |
| \~60 min | 6 confirmations | Very hard to reverse |
| \~24 hours | \~144 confirmations | Essentially irreversible |


---

## **Common Questions**

### **Q: What if I set fee too low?**

A: Transaction stays in mempool. Miners skip it for higher-fee transactions. Eventually, it might be confirmed (when network is empty) or expire after \~2 weeks (then rebroadcast).

### **Q: Can I cancel a transaction?**

A: No. Once broadcast, you cannot cancel. You can only send a new transaction with higher fee (RBF - Replace By Fee).

### **Q: Why do I need a change address?**

A: Bitcoin doesn't do "partial spending." You spend entire UTXO. Change address receives the leftover.

### **Q: Is my transaction private?**

A: No. All transactions are public on blockchain. Addresses are pseudonymous (linked to identity only if you share it).

### **Q: Can a transaction be reversed?**

A: Only by miner coordination (unlikely after 6 confirmations). Bitcoin transactions are irreversible; unlike credit cards.


---

*Transactions are atomic: either fully confirmed or not at all. No partial confirmations.*