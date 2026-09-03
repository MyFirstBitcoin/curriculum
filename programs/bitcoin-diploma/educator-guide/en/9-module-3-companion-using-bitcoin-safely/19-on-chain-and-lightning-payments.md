# 9.19 On-chain and Lightning payments

Use a comparison that separates payment path from custody.


| Question | On-chain | Lightning |
| --- | --- | --- |
| Where is settlement recorded? | Directly in Bitcoin's blockchain | Payment updates occur through a network built above Bitcoin; channels ultimately depend on Bitcoin |
| Common beginner receiving information | On-chain address | Invoice, supported Lightning address, or another approved request type |
| Typical use | Base-layer settlement, often larger or less frequent transfers | Often small or frequent payments where local tools and liquidity support them |
| Timing | First confirmation depends on block inclusion | Often rapid, but payments can fail |
| Fees and capacity | Depend on transaction data and block-space demand | Depend on wallet, route, liquidity, service, and payment conditions |
| Custody | Can be custodial or self-custodial | Can be custodial or self-custodial |
| Main beginner check | Correct address, network, amount, fee, and confirmation | Correct invoice or destination, amount, expiry, fee, and payment result |


Lightning is not a separate coin. A successful Lightning payment does not prove the wallet is safe for a larger balance. Channel operation, routing infrastructure, and liquidity management belong outside Core unless selected as Advanced learning.
