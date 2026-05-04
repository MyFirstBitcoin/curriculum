# 3.2 Public Key Cryptography and Protocols

The Internet today, and most modern computer systems, rely on cryptography, a method of obscuring information so that only the recipient of the information can decode it. The foundations for the cryptography used to secure Bitcoin can be traced back to the 70’s.

The first issue to resolve is – how to send a shared secret over an unsecured medium.

This was first looked at by Whitfield Diffie and Martin Hellman.

The problem: the two parties – usually referred to as Alice and Bob – want to share secret information across a network where others may be listening in. To achieve this, they created the Diffie-Hellman key exchange process.

This shared secret can then be used as the seed value to create numerous symmetric keys to encrypt and decrypt messages to send to each other without sharing the key itself in the open.

As the private key never has to be shared, and different keys are used at each end to encrypt and decrypt, this is referred to as an asymmetric encryption algorithm.

Use cases:

* Alice signs a message with Bob’s public key – who is the only person who can decrypt it using his private key
* Alice signs a message with her private key – by decrypting with her public key anyone can verify that the message was sent by Alice, without knowing her private key
* Combining these two approaches with two layers of encryption, a message can be sent encrypted so that only Bob can decrypt it, and he can then verify the sender was indeed Alice

Although not credited on the paper, Ralph Merkle was instrumental in helping to solve what was considered up until then this unsolvable puzzle – how to establish or reestablish private communication across an open and potentially hostile network.

This approach on its own is susceptible to a brute force attack, where an attacker can take the shared numbers and recreate a shared key eventually given enough time and resources, so it’s not the complete answer on its own.

##### Protocols for Public Key Cryptosystems

As well as contributing to the Diffie-Hellman public-key system described above, **Ralph Merkle** continued to contribute to this space for many years, and was instrumental in the development of some key components used by Bitcoin.

A cryptographic hash function is a mathematical algorithm that takes inputs of any size and processes complex calculations to return a hash value in bits, which is usually represented by a fixed-length alphanumeric output using hexadecimal format.

* Inputs can be any size
* The output is always of a fixed length and deterministic (same input creates the same hash each time)
* It is easy to verify but exceedingly difficult to reverse the process to determine the input
* A minor modification of the data completely alters the outputs

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/7c8a3db12ec6210a440a241e0bec1af419d89d7b-515x331.svg)

Hashing is an integral part of the Bitcoin protocol. SHA-256, used in Bitcoin, was created by the NSA and is an example of a cryptographic hashing algorithm.

* Each block in the chain is hashed so that data can’t be changed – ensuring integrity of the distributed ledger
* The hash generated needs to meet the ‘Proof of work’ criteria to be considered a valid block
* Merkle trees – by employing branching and hashes of hashes, hash trees can enable the verification of large datasets with minimal storage
* Hash based Signatures and Keys can be used for wallets, addresses and authorisation of transactions

Distributed verification of blockchain states and append-only ledger models resistant to revision is made possible by one-way hashing. Hash functions provide the dependable, deterministic approach to verify events on public ledgers such as Bitcoin in the absence of a centralised trust model.

These new capabilities in the cryptography space were expected by its creators to usher in a new wave of innovation in this space.

##### Elliptic curve cryptography

One of these later innovations came in the form of elliptic curve cryptography.

Elliptic curve cryptography was introduced in 1985 by two scientists, N. Koblitz and V. Miller. They proposed the idea of using points defined by elliptic curves instead of the finite prime fields such that the Discrete Logarithm problem assumption holds, as commonly used in the standard Diffie-Hellman key exchange protocol. The details of how this works is beyond the scope of this section, but at a high level, an elliptic curve is the set of points that satisfy a specific mathematical equation.

The equation for an elliptic curve looks something like:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

This has some useful properties:

* Horizontal symmetry. Any point on the curve can be reflected over the x axis and remain the same curve.
* any non-vertical line will intersect the curve in at most three places.
* Compact key sizes are essential for efficient storage and transmission of public keys in the blockchain.

These properties can be used to create key pairs in a similar way to the Diffie-Hellman algorithm. Bitcoin uses ECDSA, which is short for Elliptic Curve Digital Signature Algorithm. It’s a process that uses an elliptic curve and a finite field to “sign” data in such a way that third parties can verify the authenticity of the signature while the signer retains the exclusive ability to create the signature. With bitcoin, the data that is signed is the transaction that transfers ownership.

The ‘finite’ part is similar to the ‘mod’ approach with Diffie-Hellman, where the output of the equation is divided and the remainder is used to ensure that it fits within a range of numbers.
