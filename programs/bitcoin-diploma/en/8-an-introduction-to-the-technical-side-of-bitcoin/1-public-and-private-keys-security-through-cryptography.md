# 8.1 Public and Private Keys: Security through Cryptography

> What Bitcoin gives us is a hard promise: the program will execute exactly as specified.  
_Andreas M. Antonopoulos_



#### 8.1.1 Public/Private Key Cryptography


> **Info**
>
> Cryptography is a way of keeping information secret by disguising it in code.


* Encryption is the process of taking information and transforming it in a special code, making it unreadable to anyone who does not have the correct decryption method. This is similar
* Decryption, on the other hand, is the process of taking the encrypted information and making it readable again, like unlocking the safe and being able to read the information inside.

For instance, let’s say John wants to send Arel a secret message that isn’t meant for anyone else to read. They agree to use the Pigpen Cipher encryption method to disguise the message before sending it. Only those with the cipher can decrypt the message, making it unreadable to anyone else. Though this method is not considered secure today, it does illustrate the principle of private-key cryptography to send messages.

##### So, how does cryptography work in Bitcoin?

In traditional private-key cryptography, John and Arel would have to first share a secret key, like a password or the Pigpen Cipher. John would then use this key to encrypt his message before sending it to Arel. Arel, who also knows the secret key, would then use the same key to decrypt and read the message.

However, if someone else is in possession of the key and intercepts the message, they could decrypt it and read it.

![ ]

Public/private key cryptography, the type used in Bitcoin, has solved this problem. With public key cryptography, John and Arel don’t need to share a password or encryption method with each other. Instead, they each have two diﬀerent keys: a **public key** (which is safe to share with anyone) and a **private key** (which should be kept private).

In this case, when John wants to send a message to Arel, he can use Arel’s **public key** to encrypt his own message before sending it to Arel. When Arel receives the message, only he is able to decrypt it with his **private key**. No one else, even if they intercept the message, will be able to read the message. The chances to steal the key are also much lower, because not even John and Arel need to share their private keys with each other.

![Digital Signatures]

So, the main advantage of public/private key cryptography over private is that it allows for secure communication without the need for the sender and receiver to first share a secret key (or another encryption method like Pigpen Cipher), which could be intercepted by a third party.

In Bitcoin, public/private key cryptography is not used to send encrypted messages. Instead, it is used to create unique digital signatures that make Bitcoin transactions immutable. A digital signature is a way to prove the authenticity of a Bitcoin transaction, similar to when you write your signature on a document.




> **Callout – Public/Private Key Cryptography**
>
> Each user has two keys: a **private key**, which is **kept secret**, and a **public key** that can be **shared with others**.
>
> The **private key** serves as a form of identification and proof of ownership, confirming: “This address belongs to me and I have control over it.”
>
> **Digital signatures** are created to identify unique transactions.




![ ]

* Bitcoin transactions involve transferring the ownership of a certain amount of bitcoin from one address to another.
* Encryption is used to ensure that only the real holder of the bitcoin has the authority to send their money to someone else. It ensures their property is guarded against malicious actors.
* As an additional measure of protection, each Bitcoin transaction automatically gets a UNIQUE digital signature. This unique digital signature is powered by tamper-proof technology that helps the network verify that the real owner of the bitcoin, and not someone else, has sent them.

**How this works in a real Bitcoin transaction, in simple terms:**

1. **Creating the Transaction**: A user initiates a Bitcoin transaction by specifying details such as the recipient's address and the amount of bitcoin to be sent.
1. **Digital Signature Generation**: The sender generates a unique **digital signature** using their **private key**. This signature is a unique cryptographic code that verifies the transaction's authenticity.
1. **Broadcasting the Transaction**: The signed transaction is broadcast to the Bitcoin network, indicating the intent to transfer ownership of bitcoin from the sender to the recipient.
1. **Verification on the Network**: Nodes on the Bitcoin network receive the transaction and use the recipient's **public key** to verify the authenticity of the signature. of the transaction. Simultaneously, they use the sender's **public key** to verify the **digital signature**.
1. **Confirmation on the Bitcoin network**: If the verification is successful, the transaction will be added to the ledger, which serves as a secure, transparent record of all transactions. Once confirmed, the ownership of the bitcoin is oﬃcially transferred from the sender to the recipient.


> **Info**
>
> In summary, the digital signature, created with the sender's private key, serves as cryptographic proof of authenticity and ownership, allowing Bitcoin’s decentralized network to validate and record the transaction on the ledger.


#### 8.1.2 Hashing Explanation

Please don’t be intimidated by the technical terms and mathematical concepts ahead. We understand that not everyone is crazy about math, but you might surprise yourself and see that even the most complex ideas can be grasped with a little bit of effort.



##### What is a function?


> **Callout**
>
> _A function_ is like a machine that takes some information and turns it into something new.
>
> The information you give the function is called the **input**. The new information the function creates is called the **output**. Functions help computers do tasks and solve problems.


![Function Machine]

Think of it like a recipe for making a salad. The recipe (or function) tells you what ingredients to use and how to mix them together to make the salad. You can put different ingredients in, but the recipe will always give you the salad as the output. Functions can be used to help make things easier and more efficient.

This recipe is a function that takes the ingredients as the input and generates the tossed salad as the output. In Bitcoin, functions are utilized to execute transactions. We already know that Bitcoin transactions are essentially transfers of value (money) from one address to another. To perform a transaction, a number of cryptographic functions are used to validate the transaction and update the state of the Bitcoin ledger.

The functions used in a Bitcoin transaction include verifying the authenticity of the transaction inputs, checking that the sender has suﬃcient funds, and updating the balances of the relevant addresses. Once a transaction is verified and added to a block in the ledger, it becomes part of the permanent record of all transactions on the blockchain.

##### What is a one-way function?

![Smoothies]

A one-way function uses a set of instructions to process information and turns it into something new — like a smoothie recipe turns ingredients into a new drink. But, just as you can’t un-blend a smoothie to get the original ingredients back, you can’t reverse the one-way function to get the original information back.

Public/private key cryptography, of which the public key is a part, relies on the use of one-way functions, which make it diﬃcult to determine the private key from the public key. In theory, it is not exactly “impossible” to find the private key from the public key, but it would take an inordinate amount of time and computational power to do so. Finding a private key from a public key in Bitcoin is like trying to find a needle in a haystack as large as a football field. The needle represents the private key and the haystack represents all the possible private keys. One-way functions are designed to realistically be irreversible and cannot be decrypted.



##### What is a hash function?


> **Callout**
>
> _Hashing_ is like creating a fingerprint for digital data. It is the process of taking a digital message and turning it into a fixed length code, which serves as a unique identifier. Just like a fingerprint can identify a person, a hash can identify a digital message. Hashes are used in many applications, including Bitcoin transactions.


![ ]

**How Hashing Is Used in Bitcoin Transactions**

In Bitcoin, every transaction is hashed before it is added to a block in the ledger. The hash acts as a signature for the transaction, verifying that the transaction is valid and has not been tampered with. If someone tries to change even a single letter in the transaction, the hash will be completely diﬀerent, alerting others to the change.

**The Role of Hashing in Providing Security**

Hashing is essential to the security of the Bitcoin network. By using hashes to identify transactions, the network can detect any attempt to change or manipulate a transaction. This helps to prevent fraud and ensure that all transactions are recorded accurately on the ledger.

A hash function is a type of one-way function that takes an input (referred to as the “message” or “data”) and converts it into a numerical representation referred to as a “hash.” The **output** hash is unique to the input data, so even a small change in the **input** data results in a completely different hash.


> **Callout**
>
> _A hash function_ is like a secret code machine. It takes in a **message** and turns it into a code.


The output always looks the same for the same message. If you change the message even a little, the code will be completely different. This helps computers remember things and check if anything has been changed.


---


#### Activity: Generate SHA 256 Hash

Curious about how hashing works? Scan the QR code to instantly generate a SHA256 hash from any word, sentence, or input you choose. Hash functions are like digital fingerprints: they're one-way, meaning once something is hashed, it can't be reversed. Try it out and see for yourself!

![ ]

The **output**, or hash, is always the same length, no matter how long the original information was. Bitcoin uses a few specific types of hash function called **SHA-256** and **RIPEMD160**.

A few examples are below:

* SHA256 hash of the string **hello world**
  * b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9
* SHA256 hash of the string **hello world.**
  * 7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87
  * Notice that a small change in the input changes the output completely when compared to the first one
* SHA256 hash of the downloadable iso file **Ubuntu 18.10**
  * 7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765
  * This input is a huge file yet the output is still the same fixed length as the other two

You can also think of hashing as a musical score that captures the essence of a piece of music. Just as a musical score is a unique representation of a tune, a hash value is a unique representation of a piece of data.

By comparing the score of a piece of music with the actual performance, a musician can determine if the performance is accurate. Similarly, by comparing the hash value of received data with the original hash value, one can determine if the data has been altered during transmission.

Just as a slight deviation in a musical performance can cause it to sound diﬀerent, even the slightest change to the original data will result in a different hash value. This makes hashing a powerful tool for ensuring the integrity and authenticity of a Bitcoin transaction.

The process of encoding the **public key** through hashing is used to improve the security of information by converting it into a fixed-length, unreadable format. Bitcoin uses the SHA-256 and RIPEMD160 algorithms to produce public addresses. The resulting output serves as a unique identifier for the **public key** and helps to ensure the integrity and security of transactions stored in the ledger. By encrypting the information in this way, it becomes more diﬃcult for unauthorized individuals to access and manipulate the data.

##### Properties of a hashing function

![ ]

* **Deterministic**: The same ingredients always yield the same smoothie.
* **Pre-Image Resistance**: You can’t reassemble a strawberry from a smoothie.
* **Correlation Resistance**: Changing the ingredients a little results in a completely different smoothie.
* **Collision Resistance**: It’s hard to find different ingredients for a smoothie that result in the exact same one.
* **Speed & Verifiablility**: Throw fruit into the mixer. It’s fast and what comes out for sure is a smoothie.
