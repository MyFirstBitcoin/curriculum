# 3.6 Reusable proof of work

Hal Finney is another famous member of the Cypherpunk movement, who was very interested in the development of electronic cash and active on the mailing list.

He decided to have another go at the development of a proof-of-work based electronic cash system. Up until this point, the hash output had been unique to each transaction, but his idea was to create ‘reusable proofs of work’.

The drawback to this approach is the centralised server, which needs to be trusted not to double spend, or be shutdown. To get round this, Hal proposed using Free and open source software which could be hosted on a secure hardware component and independently validated.

The solution still faced some of the same problems as the other proposals:

* The ‘chicken and egg’ problem of getting adoption, where an incentive is missing for users to want to request tokens, and sellers don’t want to connect to the system unless users want to pay with these tokens.
* POW is also likely to get cheaper over time as computing performance improves, suggesting that the market would eventually be flooded with RPOW currency units

> If Moore’s law continues to hold true, the cost of creating a (POW) token will drop at a steady, exponential rate. Keep in mind that this is not money and is not intended to be a store of value, but rather an easy-to-exchange representation of computer effort.  
 _Hal Finney_

These attributes limited the appeal and hence adoption of the project, and despite his best efforts the project ended up as another failed attempt at creating electronic cash.
