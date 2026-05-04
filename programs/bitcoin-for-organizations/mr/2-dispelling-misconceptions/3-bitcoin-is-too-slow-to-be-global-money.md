# 2.3 Bitcoin is too slow to be global money

> Visionaries see a future of telecommuting workers, interactive libraries and multimedia classrooms. They speak of electronic town meetings and virtual communities…..The truth is no online database will replace your daily newspaper, no CD-ROM can take the place of a competent teacher and no computer network will change the way government works.  
_Clifford Stroll_

17 years later, Newsweek ceased print publication and became exclusively available online. Imagine being alive in 1974 when the Transmission Control Protocol (TCP) was first created.

No one foresaw the smartphone, with all its apps, sitting in your hand. No one saw the SatNav system in your car.

The internet did not emerge as a one and done, but rather gradually as an evolution of protocols and layers. These evolutions have built on, but mainly not changed TCP.

> So as I look at transitioning to the communication platforms of the future, I see that the beauty of Internet protocols is you get the separation of the layers between service and technology.  
_Michael K Powell_



##### Compare Bitcoin’s evolution with that of the internet

TCP was necessary but not sufficient for the emergence of everything else on the internet. Bitcoin’s evolution seems to be following a similar path. Open systems seem to be more resilient and successful when developed in layers, although there can be a lot of elapsed time between the laying of the initial building blocks and widespread adoption. All in one solutions do not seem to be as effective in open systems as those built in layers on protocols . Just as no one has needed to rebuild the internet because films couldn’t be streamed using TCP, so it is likely to be with Bitcoin.

There are already a number of layer 2 protocols sitting on top of Bitcoin, and there are many applications sitting on top of these layer 2 protocols (see section 201.4 for more details on these).

Rather than focusing on what bitcoin and the Bitcoin network can’t do today, think about what can already be done today, and compare that with what it could do 10 years ago. Do this exercise with the internet from 1985 to 1995, and then look at how much faster the internet got over the subsequent 30 years and the applications that became possible. Use that insight to roll Bitcoin forward and imagine what it may look like in just another 10 years, or 30 if your imagination can stretch that far.



##### Compare Bitcoin with the existing global money system

The central claim that Bitcoin is too slow to be global money is arguably true if we are to be restricted to the base layer of Bitcoin. It is also true that the base layer of our existing money systems are too slow to be global money, if a similar restriction meant that there were no payments infrastructure built on top of it by private banks and payments services such as Visa and Mastercard. Our existing system is built in layers, so we might expect the future to look similar. Some design trade-offs such as between trust, speed and cost may translate between systems delivering the same solutions albeit they are built to move different tokens of value.

Some of the existing layer 2s on Bitcoin directly address the speed issue, for example Liquid and the Lightning Network (See section 201.4 for more details). Liquid is faster and cheaper than the Bitcoin blockchain, and the Lightning Network is even faster and cheaper than Liquid. A proliferation of layer 2s, each with different trade-offs is to be expected and is healthy.

There will likely be more layer 2s and 3s and an explosion of applications making use of these, just as happened with the evolution of the internet.



##### Motivation

When this criticism is raised, it is worth considering whether the critic has other motivations. For instance, do they have a new or different blockchain project? This may be analogous to trying to sell a better Transmission Control Protocol.

The Scalability, or Blockchain, Trilemma, was first raised by Vitalik Buterin in 2017. It says that there is always a trade-off in blockchain design between the properties of Decentralisation, Security and Scalability. Anyone raising the criticism that Bitcoin is too slow and that they have a quicker solution in a layer 1 blockchain will be sacrificing some security or decentralisation in order to achieve it. Whilst such a trade-off for a blockchain designed for other uses may make sense, the order of priority for a global money must be:


> **Note**
>
> * **Decentralisation**
>   * Makes it possible to remove trusted parties
> * **Security**
>   * Inhibits bad actors from tampering with transactions or the ledger
> * **Scalability**
>   * Allows the system to scale economically in users and speed


The first two features create the environment for issuance without makers, payments without mediators and custody without managers.

Bitcoin makes the right trade off of the three blockchain design features given that its targeted use case is as global money, and it mitigates the scalability and speed trade offs using layers.

> Satoshi discovered how to protect the integrity of digital money without trusted parties - no makers, mediators or managers needed.  
_Resistance Money, 2024, Bailey, Retter, Warmke_
