# Fee & Speed Comparison Tool

# Fee & Speed Comparison Tool

Choosing the right payment method for different scenarios.


---

## **Quick Reference: Payment Methods Compared**

| Payment Method | Speed | Cost | Best For | Worst For |
|----------------|-------|------|----------|-----------|
| **Bank Wire**  | 2-5 days | $15-50 | Large transfers; official | Speed; micropayments |
| **Credit Card** | Instant | 2-3% | Shopping online | Privacy; international |
| **PayPal/Stripe** | 1-3 days | 2.9% + $0.30 | Online sales | Cross-border; speed |
| **Bitcoin On-Chain** | \~10 min | $2-20 | Large amounts; settling | Micropayments; time-sensitive |
| **Lightning Network** | Seconds | <$0.01 | Daily spending; remittances | Large one-time transfers |


---

## **Scenario-Based Comparison**

### **Sending $100 Coffee Payment**

| Method | Speed | Cost | Notes |
|--------|-------|------|-------|
| **Credit card** | Instant | $3   | Store gets $97 |
| **Bitcoin On-Chain** | 10 min | $2   | Overkill; too slow |
| **Lightning** | <1 sec | <$0.01 | **BEST OPTION** |

**Winner:** Lightning Network


---

### **Sending $5,000 to Business Partner**

| Method | Speed | Cost | Notes |
|--------|-------|------|-------|
| **Bank wire** | 2-3 days | $30  | Standard but slow |
| **Bitcoin On-Chain** | 10 min | $5   | **BEST OPTION** |
| **Lightning** | <1 sec | <$0.01 | Channel capacity might not fit $5k |
| **PayPal** | Instant | $150+ | High fee; can be reversed |

**Winner:** Bitcoin On-Chain (or Lightning if channels support it)


---

### **Monthly Remittance: $500 to Philippines**

| Method | Speed | Cost | Notes |
|--------|-------|------|-------|
| **Bank wire** | 3-5 days | $40-50 | Expensive; slow |
| **Money service** | 1-2 days | $25-40 | Still expensive |
| **Bitcoin On-Chain** | 10 min | $3   | Recipient must convert to peso |
| **Lightning** | <1 sec | <$0.01 | **BEST OPTION** if recipient has Lightning |
| **Stablecoin (USDT)** | 1-2 min | <$0.50 | Good alternative (less volatile) |

**Winner:** Lightning Network (or stablecoin)\n**Savings:** $35-50 per month per transaction


---

## **Fee Structure Explained**

### **Bitcoin On-Chain**

```
Your transaction size: 250 bytes
Network fee rate: 50 satoshis/byte (high congestion)
Your fee: 250 × 50 = 12,500 satoshis = $2.50

During low congestion:
Network fee rate: 10 satoshis/byte
Your fee: 250 × 10 = 2,500 satoshis = $0.50
```

### **Lightning Network**

```
Routing fee (optional):
Base fee: 1 satoshi
Proportional fee: 0.001% of amount

Sending 100,000 satoshis:
Routing: 1 + (100,000 × 0.001%) = 1 + 1 = 2 satoshis = < $0.0001
Your fee: < $0.01
```

### **Credit Card**

```
Purchase: $100
Store pays: 2.9% + $0.30 = $3.20 fee
Store gets: $96.80

Customer pays: $100
Issuing bank gets interest if payment delayed
```


---

## **Cost Example: $10,000 Transfer**

### **Scenario: Freelancer sending to international client**

**Bank Wire (Traditional)**

* Time: 2-3 days
* Cost: $30-40
* Recipient gets: $9,960-9,970

**Bitcoin On-Chain**

* Time: \~10 minutes
* Cost: $5
* Recipient gets: $9,995

**Lightning Network**

* Time: <1 second
* Cost: <$0.01
* Recipient gets: $9,999.99+

**Monthly saving with Lightning:** $30-40 × 12 = $360-480/year!


---

## **Speed Breakdown: What's Happening**

### **On-Chain Bitcoin**

```
0 sec: You hit send
1-30 sec: Transaction broadcast to network
1-10 min: First Bitcoin node includes in block
~10 min: 1st confirmation (safe for most)
~60 min: 6 confirmations (very safe)
```

### **Lightning Network**

```
0 sec: You hit send
<100 ms: Routes through network
<500 ms: Payment channels update
<1 sec: Recipient notified of payment
(Settlement to blockchain happens later, if channel closes)
```

### **Traditional Bank Wire**

```
Day 1: You initiate wire
Day 1-2: Your bank processes
Day 2-3: Intermediary bank processes
Day 3-5: Recipient bank receives
Day 5: Recipient sees money

Reality: Often takes 5-7 days internationally
```


---

## **When You Need What**

### **Choose Bitcoin On-Chain When:**

* Sending large amounts ($1,000+)
* Need strong settlement finality
* Closing Lightning channels
* Can wait 10 minutes

### **Choose Lightning When:**

* Daily spending
* Micropayments
* Remittances
* Need instant confirmation

### **Choose Traditional Banking When:**

* Business entities require it
* Court orders demand it
* No other option available
* Regulatory compliance needed


---

## **Future Cost Trends**

**Bitcoin On-Chain:**

* Fees will stay similar (\~$2-20) due to block space scarcity
* Suitable for large transactions

**Lightning:**

* Fees will remain tiny (<$0.01) indefinitely
* Designed for scale

**Traditional Banking:**

* Fees unlikely to drop significantly
* Will remain expensive long-term


---

*Choose the right tool for the job. On-chain Bitcoin ≠ Lightning. Both are Bitcoin, different use cases.*