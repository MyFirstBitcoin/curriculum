# 3.0 Inleiding

> **Dark – De samenvatting van het Bitcoin White Paper**
>
> **Een puur peer-to-peer versie van elektronisch geld** zou het mogelijk maken om online betalingen rechtstreeks van de ene partij naar de andere te sturen zonder tussenkomst van een financiële instelling. **Digitale handtekeningen bieden een deel van de oplossing**, maar de belangrijkste voordelen gaan verloren als er een **vertrouwde derde partij** nog steeds nodig is om dubbel uitgeven te voorkomen. Wij stellen een oplossing voor het probleem van dubbel uitgeven voor met behulp van een **peer-to-peer netwerk**. Het **netwerk voorziet transacties van een tijdstempel** door ze te hashen in een voortdurende keten van **hash-gebaseerd proof-of-work,** waarmee een registratie wordt gevormd die niet kan worden gewijzigd zonder het **proof-of-work** opnieuw uit te voeren. De langste keten dient niet alleen als bewijs van de volgorde van gebeurtenissen, maar ook als bewijs dat deze afkomstig is van de grootste pool van rekenkracht (CPU power). Zolang de meerderheid van de rekenkracht wordt gecontroleerd door nodes die niet samenwerken om het netwerk aan te vallen, zullen zij de langste keten genereren en aanvallers voorblijven. **Het netwerk zelf vereist minimale structuur. Berichten worden op basis van best effort uitgezonden, en nodes kunnen het netwerk naar wens verlaten en opnieuw toetreden**, waarbij ze de langste proof-of-work keten accepteren als bewijs van wat er is gebeurd terwijl ze weg waren.


Bitcoin is niet uit het niets ontstaan, maar is gebouwd op het werk van velen in de voorgaande decennia. In deze module verkennen we de fundamenten van het internet waarop Bitcoin voortbouwt, evenals het onderzoek en de ontwikkeling die in het whitepaper worden erkend.

In de jaren 70 keek een groep individuen naar hoe de Amerikaanse overheid in het bijzonder probeerde de toegang tot cryptografie te beperken, en zij zetten zich ervoor in om ervoor te zorgen dat deze technologie voor iedereen beschikbaar zou zijn om hun privacy online te beschermen. Sommige van deze vroege pioniers richtten zich ook op de potentiële voordelen van een digitaal ‘sound money’ systeem dat gebruikt kon worden om waarde op te slaan en uit te wisselen via het opkomende internet. Friedrich Hayek – een toonaangevende bijdrager aan de Oostenrijkse economie – voorzag al ruim voor het internettijdperk hoe een ideale valuta gebaseerd op vrije marktwerking eruit zou zien, maar vond het technisch en politiek onhaalbaar. Naast digitale privacy probeerde deze groep, die later de Cypherpunks werd, Hayeks visie voor digitaal geld te realiseren, maar deze pogingen mislukten tot Satoshi zijn ideeën op de mailinglijst publiceerde.

* TCP/IP-protocol (1976)
* Protocollen voor Public Key Cryptosystemen - Ralph Merkle (1980)
* Digicash - David Chaum (1989)
* Digitale tijdstempeling (jaren 90)
* Hashcash - Adam Back (1997)
* BitTorrent - Bram Cohen (2001)
* Herbruikbare POW - Hal Finney (2004)
* Bitcoin Whitepaper - Satoshi Nakamoto (2008)

Een belangrijke invloed op de ontwikkeling van Bitcoin was de opkomst van de Cypherpunk-beweging in de jaren 90. Zij ontwikkelden verschillende cryptografische technologieën, waaronder public-key cryptografie, waarmee gebruikers veilig en privé konden communiceren en informatie delen. Veel van de hier beschreven ontwikkelingen en betrokken personen maakten deel uit van deze groep.

De behoefte aan digitaal geld werd ook onderkend en er werden verschillende pogingen gedaan om het te creëren, maar deze hadden beperkingen waardoor ze niet succesvol waren. Het genie van Satoshi Nakamoto was om deze mogelijkheden samen te brengen en, met enkele eigen innovaties, hierop voort te bouwen om het Bitcoin-protocol te creëren dat vandaag de dag wordt gebruikt. In de volgende secties zullen we enkele van deze ontwikkelingen verkennen en uitleggen hoe ze hebben bijgedragen aan het ontwerp van Bitcoin. We bespreken ook welke ontbrekende puzzelstukken Satoshi wist op te lossen.
