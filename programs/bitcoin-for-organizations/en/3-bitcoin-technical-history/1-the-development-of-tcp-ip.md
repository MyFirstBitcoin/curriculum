# 3.1 The development of TCP/IP

Most of us are familiar with the TCP/IP protocols in use today as the foundation for the internet. Their origins date back to the late 70’s when scientists were exploring alternative designs to Arpanet – an even earlier network conceived by the U.S Department of Defense to enable resource sharing between remote computers. TCP/IP became the protocol standard for Arpanet in 1983, which led to it becoming the dominant networking model by the end of the 1990’s and the foundation for the internet that Bitcoin runs on today.


| OSI Model | TCP/IP |
| --- | --- |
| Application | Application |
| Presentation | Application |
| Session | Application |
| Transport | Transport |
| Network | Network |
| Data Link | Data Link |
| Physical | Physical |


At the same time as the TCP/IP model was being developed, a similar but more comprehensive framework was being developed by the International Standards Organisation (ISO) and the Telecoms industry (CCITT). The process to develop new protocols or suggest changes was slow and unwieldy in comparison to the more decentralised approach used to develop TCP/IP, leading to the dominance of this approach today.

##### Request for Change

Any suggested developments to existing protocols or ideas for new ones can be proposed in the TCP/IP model through a **Request for Change** process. These go through an approval process, managed by the Internet Engineering Task Force (IETF), and become open source once approved to allow anyone to implement and adopt them. Some examples of note:

* 1969 RFC 1 Documented how packets would be sent in the Arpanet
* 1981 RFC791 defined the Internet protocol V4 – still widely adopted today
* 1982 RFC 821 Simple mail Transfer protocol
* 1987 Domain Name System – how domain names are resolved to IP addresses
* 1999 RDC 2616 Hypertext Transfer protocol – essential for browsing the web


> **Callout**
>
> The **Bitcoin Improvement Proposal** (BIP) follows a similar approach to RFC, but focusing purely on improvements to Bitcoin itself rather than the development of new or alternate protocols. Bitcoin also borrows from this layered model, and you will see additional protocols described as layer two or three.


In the same way that the base layers of the TCP/IP model have changed relatively little in the last few decades, with the innovation happening at higher layers, the base Bitcoin layer is expected to change very slowly at this point, with scaling solutions such as Lightning and Liquid happening above.

A good example of how base layer protocols become difficult to change over time is IPv6. The expected exhaustion of address space in IPv4 created a demand for a new protocol. The first draft standard was created in 1998, but not ratified as an internet standard until 2017. While it solved many problems with IPv4 and is far more future-proof, it has still seen very slow adoption in the industry today. During this time, many new protocols have been defined at the upper layers to enable multimedia, email etc.

##### The Building blocks used by Bitcoin

This separation of the problems of interconnectivity allows protocols to be developed independently from the layers above and below it. Rather than having to reinvent solutions for each layer, Bitcoin the network can rely on the underlying capabilities of the network delivered at the physical and data link layers.


| Layer | TCP/IP Original |
| --- | --- |
| Application | Uses Domain Name System (DNS) to identify neighbouring nodes. Port 8333 signals Bitcoin protocol. |
| Transport | UDP for FIBRE comms between miners for low latency. TCP for P2P communications between nodes. |
| Transport | TOR Routing: Enables anonymity and privacy. Broadcast Protocol: Routes trafic across the network. |
| Link | Operates over any medium (e.g., Ethernet, Wi-Fi, etc.) |
| Physical | Physical transmission via wireless, Ethernet, or other hardware interfaces. |


##### Bitcoin is a neutral protocol to transfer value like HTTPS is a protocol to transfer information

* **HTTPS**: Secure Websites
* **SMTP**: Send Emails
* **FTP**: Transfer files
* **DNS**: Manage domain names
* **BTC**: Store and transfer value

Bitcoin enables value to be transported reliably and without requiring a third party between people or devices across the Internet. This is expected to unlock tremendous value.
