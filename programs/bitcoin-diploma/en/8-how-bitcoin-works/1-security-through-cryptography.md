# 8.1 Security through Cryptography

> What Bitcoin gives us is a hard promise: the program will execute exactly as specified.  
_Andreas M. Antonopoulos_



#### Public/Private Key Cryptography


> **Definition – Definition of Cryptography**
>
> **Cryptography** is the practice of turning information into a secret that only the right people can read.


* **Encryption** is the process of turning information into a coded form so that only someone with the correct key can read it.
* **Decryption** is the process of turning that coded information back into something readable.

In traditional cryptography, two people who want to communicate privately must first share the same secret key, similar to a shared password. One person uses this key to encrypt the message before sending it, and the other person uses the same key to decrypt and read it.

The problem with this system is that both people must already share the secret key. If someone else gets access to that key, they can read any intercepted messages.

Bitcoin solves this problem using a different approach called public-key cryptography, where users do not need to share secret keys in advance.

Public/private key cryptography solves the problem of sharing secrets. Instead of sharing a password, each person has two keys: a public key and a private key.

* The **public key** can be shared with anyone.
* The **private key** must always be kept secret.

If John wants to send something to Arel, he can use Arel’s public key. Only Arel can unlock it using his private key. Even if someone intercepts the message, they cannot read or use it without the private key.

In Bitcoin, this system is used to create digital signatures. A digital signature proves that the owner of a private key approved a transaction, similar to signing your name on a document. This is what allows Bitcoin transactions to be secure and verifiable without trusting a third party.


> **Info**
>
> Each user has two keys: a **private key**, which is **kept secret**, and a **public key** that can be **shared with others**.
>
> The **private key** serves as a form of identification and proof of ownership, confirming: “This address belongs to me and I have control over it.”
>
> **Digital signatures** are created to identify unique transactions.


Bitcoin transactions involve transferring the ownership of a certain amount of bitcoin from one address to another.

Encryption is used to ensure that only the real holder of the bitcoin has the authority to send their money to someone else. It ensures their property is guarded against malicious actors.

As an additional measure of protection, each Bitcoin transaction automatically gets a UNIQUE digital signature. This unique digital signature is powered by tamper-proof technology that helps the network verify that the real owner of the bitcoin, and not someone else, has sent them.

###### How a Bitcoin Transaction Works

1. **Creating the Transaction**: A user initiates a Bitcoin transaction by specifying details such as the recipient's address and the amount of bitcoin to be sent.
1. **Digital Signature Generation**: The sender generates a unique **digital signature** using their **private key**. This signature is a unique cryptographic code that verifies the transaction's authenticity.
1. **Broadcasting the Transaction**: The signed transaction is broadcast to the Bitcoin network, indicating the intent to transfer ownership of bitcoin from the sender to the recipient.
1. **Verification on the Network**: Nodes on the Bitcoin network receive the transaction and use the recipient's **public key** to verify the authenticity of the signature. of the transaction. Simultaneously, they use the sender's **public key** to verify the **digital signature**.
1. **Confirmation on the Bitcoin network**: If the verification is successful, the transaction will be added to the ledger, which serves as a secure, transparent record of all transactions. Once confirmed, the ownership of the bitcoin is oﬃcially transferred from the sender to the recipient.


> **Callout – Summary**
>
> The **digital signature**, created with the sender’s **private key**, proves that the transaction was authorized by the owner of the bitcoin.
>
> The Bitcoin network can then verify this proof and record the transaction.


#### Hashing Explanation

Please don’t be intimidated by the technical terms and mathematical concepts ahead. We understand that not everyone is crazy about math, but you might surprise yourself and see that even the most complex ideas can be grasped with a little bit of effort.


> **Definition – Definition of a function**
>
> A **function** is like a machine that takes some information and turns it into something new. The information you give the function is called the **input**. The new information the function creates is called the **output**. Functions help computers do tasks and solve problems.


##### What is a function?

A function is a set of instructions that takes an input and produces an output. You can think of it like a recipe: you follow the steps with certain ingredients, and you always end up with a predictable result.

In Bitcoin, functions are used to process and verify transactions. When someone sends bitcoin, cryptographic functions help check that the transaction is valid, confirm that the sender has enough funds, and update the balances on the Bitcoin ledger. Once verified and added to a block, the transaction becomes part of the permanent record on the blockchain.

##### What is a one-way function?

A one-way function is a special type of function that is easy to compute in one direction but extremely difficult to reverse.

For example, blending ingredients into a smoothie is easy, but you cannot separate the smoothie back into the original ingredients.

Bitcoin security relies on one-way functions. They are used in public and private key cryptography, allowing people to share a public key while keeping their private key secret. Even though the public key is visible, it is nearly impossible to derive the private key from it. This is what makes Bitcoin transactions secure.

##### What is a hash function?


> **Definition – Definition of a hash function**
>
> A **hash function** is like a secret code machine.
>
> It takes in a **message** and turns it into a code.


###### How Hashing Works in Bitcoin Transactions

In Bitcoin, every transaction is turned into a hash before it is added to the blockchain. A hash is a unique digital fingerprint of the transaction. If anyone tries to change even a small part of the transaction, the hash will change completely. This makes it easy for the network to detect tampering.

###### The Role of Hashing in Bitcoin Security

Hashing helps protect the Bitcoin network by making transactions easy to verify and impossible to quietly modify. Because each transaction has its own unique hash, the network can quickly detect if something has been altered.

A hash function takes data and converts it into a fixed string of numbers and letters called a hash. The same input will always produce the same hash, but even a tiny change in the input will create a completely different result. This property allows computers to check that data has not been changed.


> **Definition – Definition of Hashing**
>
> **Hashing** is like creating a fingerprint for digital data. It is the process of taking a digital message and turning it into a fixed length code, which serves as a unique identifier. Just like a fingerprint can identify a person, a hash can identify a digital message. Hashes are used in many applications, including Bitcoin transactions.


The **output**, or hash, is always the same length, no matter how long the original information was. Bitcoin uses a few specific types of hash function called **SHA-256** and **RIPEMD160**.

A few examples are below:

* SHA256 hash of the string **hello world**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* SHA256 hash of the string **hello world.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Notice that a small change in the input changes the output completely when compared to the first one
* SHA256 hash of the downloadable iso file **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * This input is a huge file yet the output is still the same fixed length

You can also think of hashing as a musical score that captures the essence of a piece of music. Just as a musical score is a unique representation of a tune, a hash value is a unique representation of a piece of data.

By comparing the score of a piece of music with the actual performance, a musician can determine if the performance is accurate. Similarly, by comparing the hash value of received data with the original hash value, one can determine if the data has been altered during transmission.

Just as a slight deviation in a musical performance can cause it to sound different, even the slightest change to the original data will result in a different hash value. This makes hashing a powerful tool for ensuring the integrity and authenticity of a Bitcoin transaction.

The process of encoding the **public key** through hashing is used to improve the security of information by converting it into a fixed-length, unreadable format. Bitcoin uses the SHA-256 and RIPEMD160 algorithms to produce public addresses. The resulting output serves as a unique identifier for the **public key** and helps to ensure the integrity and security of transactions stored in the ledger. By encrypting the information in this way, it becomes more diﬃcult for unauthorized individuals to access and manipulate the data.

##### Properties of a hashing function

* **Deterministic**: The same ingredients always produce the same smoothie. In the same way, the same data will always produce the same hash.
* **Pre-image resistance**: If you only have the smoothie, you cannot figure out the exact fruits that were used. Similarly, if you only have a hash, you cannot determine the original data.
* **Avalanche effect**: Changing even a tiny part of the ingredients creates a completely different smoothie. In hashing, a very small change in the data produces a completely different hash.
* **Collision resistance**: It is extremely difficult to find two different sets of ingredients that produce the exact same smoothie. In the same way, it is extremely unlikely that two different pieces of data will produce the same hash.
* **Fast to verify**: Making the smoothie is quick, and it is easy to check that the result is a smoothie. Hash functions are fast to compute and easy for anyone to verify.

#### Activity: Generate SHA 256 Hash

https://tools.keycdn.com/sha256-online-generator

Curious about how hashing works?

Scan the QR code to instantly generate a SHA256 hash from any word, sentence, or input you choose.

Hash functions are like digital fingerprints: they're one-way, meaning once something is hashed, it can't be reversed.

Try it out and see for yourself!
