# 6 - Hoe Bitcoin te gebruiken

Duur: 90 minuten

Kernidee: Door Bitcoin on-chain te gebruiken leren studenten in de praktijk hoe eigenaarschap, zelfbewaring en verificatie werken, waardoor theorie wordt omgezet in directe financiële handeling.

#### Leerdoelen

Aan het einde van deze les moeten studenten in staat zijn om:

* Veelvoorkomende manieren identificeren om bitcoin te verkrijgen en te verhandelen, waaronder peer-to-peer en gecentraliseerde beurzen.
* Het verschil uitleggen tussen zelfbewaarde en bewaarde wallets, en waarom zelfbewaring belangrijk is bij Bitcoin.
* Het doel beschrijven van privésleutels, publieke adressen, seed phrases en wallet-interfaces.
* Verschillende wallettypes vergelijken en hun afwegingen beoordelen op basis van veiligheid, gemak, privacy en controle.
* Een mobiele Bitcoin-wallet instellen en het basisproces voor herstel uitleggen.
* Demonstreren hoe je een on-chain bitcointransactie ontvangt en verstuurt.

Het principe "Vertrouw niet, verifieer" toepassen op walletkeuze, transacties en breder Bitcoin-gebruik.

#### Tools & Bronnen

##### Visuele hulpmiddelen

* Hoofdstuk 6 - Hoe gebruik je Bitcoin

##### Ondersteuningsbibliotheek

* Woordenkaart — Hoofdstuk 6 — Termen: wallet, privésleutel, publiek adres, seed phrase, bewaard, zelfbewaard, UTXO, transactiekosten
* Vergelijkingskaarten & Referentiebladen — Vergelijking van wallettypes (bewaard, mobiel, hardware, papier)
* Technische uitleg & Verdiepingen — Publieke/privésleutels, UTXO-model, transactiebevestiging
* Verdieping privésleutelbeveiliging — Seed phrases, sleutelafleiding, back-upmethoden, aanvalsvectoren
* Transactie-anatomiegids — Stapsgewijs voorbeeld van hoe een Bitcointransactie werkt
* Checklist beste beveiligingspraktijken — Voor je begint, wallet aanmaken, ontvangen, versturen, phishingpreventie

#### Activiteiten

* Transacties in actie
* Lightning Estafette
* De Mempool verkennen

#### Online lesgeven

* Maak vanaf het begin duidelijk of studenten een demonstratie bekijken of zelf een wallet instellen.
* Gebruik grote, goed leesbare screenshots voor elke stap van het walletinstellen.
* Pauzeer na elke stap en vraag studenten om in de chat te bevestigen dat ze het begrijpen voordat je doorgaat.
* Geef een directe waarschuwing vóór het gedeelte over de seed phrase en herinner studenten eraan nooit gevoelige informatie online te delen.

#### Voorbereiding

* Download en test een mobiele wallet-app (Blue Wallet of Muun); bereid screenshots voor van de belangrijkste instelstappen.
* Bereid een handleiding voor walletinstelling voor (download → aanmaken → seed back-up → ontvangen) als naslag.
* Zorg dat het netwerk/WiFi werkt; heb een demo-adres en QR-code klaar om te tonen.

#### Procedure

Deze les gaat van theorie naar directe praktijk. Het sluit nu direct aan bij de structuur van het Diploma, zodat verwerving, wallets, installatie, transacties en verificatie onder dezelfde hoofdonderdelen vallen als in de studentengids. Extra onderwijsondersteuning blijft binnen die secties genest.

##### 6.0 Introductie, 8 minuten

Begin met het verbinden van dit hoofdstuk aan het vorige:

* Als Bitcoin geld is, hoe krijgen en gebruiken mensen het dan eigenlijk?
* Wat betekent het om echt controle te hebben over je bitcoin?
* Waarom is het gebruik van Bitcoin anders dan het gebruik van een bankapp?

Maak duidelijk dat dit hoofdstuk over praktisch gebruik gaat. Studenten leren niet langer alleen wat Bitcoin is, maar ook hoe ze er direct mee kunnen omgaan.

##### 6.1 Bitcoin verkrijgen en uitwisselen, 12 minuten

Leg uit dat mensen op verschillende manieren bitcoin kunnen verkrijgen, waaronder:

* uitbetaald worden in bitcoin
* bitcoin minen
* fiat omwisselen voor bitcoin in persoon
* fiat omwisselen voor bitcoin online

Richt je daarna op de twee belangrijkste manieren van verkrijgen die in het hoofdstuk worden behandeld:

* peer-to-peer, in persoon
* peer-to-peer, online
* gecentraliseerde beurzen

Maak de afwegingen duidelijk.

Benadruk bij P2P-transacties in persoon de directe uitwisseling zonder bank of tussenpersoon, maar noem ook de praktische risico’s van het afspreken met mensen voor contante transacties.

Leg bij P2P online escrow uit in eenvoudige bewoordingen, als een manier om het tegenpartijrisico te verkleinen terwijl directe uitwisseling tussen personen mogelijk blijft.

Maak bij gecentraliseerde beurzen duidelijk dat ze handig zijn, maar dat gebruikers een bedrijf moeten vertrouwen, vaak persoonlijke informatie moeten delen en hun geld onder controle van een derde partij laten tot het wordt opgenomen. Dit is een goed moment om te benadrukken dat gemak vaak gepaard gaat met concessies op het gebied van privacy en autonomie.

##### 6.2 Een introductie tot Bitcoin-wallets, 35 minuten

**Wat een Bitcoin-wallet eigenlijk is**

Maak direct een veelvoorkomend misverstand duidelijk: bitcoin wordt niet opgeslagen in de wallet-app zoals fysiek geld in een tas.  
De bitcoin bestaat op het grootboek dat door het netwerk wordt bijgehouden. Wat de gebruiker beheert, is de mogelijkheid om het uit te geven via privésleutels.

Leg vervolgens de twee dingen uit die mensen vaak bedoelen met "wallet":

* het privésleutelsysteem, waaruit adressen worden gegenereerd
* de app of interface die wordt gebruikt om met het netwerk te communiceren

Gebruik indien nuttig de e-mailanalogie uit het hoofdstuk:

* publiek adres = als een e-mailadres dat je kunt delen
* privésleutel = als een wachtwoord dat je moet beschermen

Wees hier heel duidelijk: wie de privésleutels beheert, beheert de bitcoin. Dat is het kernconcept dat studenten moeten begrijpen.

**Zelfbeheer versus bewaarportemonnees**

Dit is een van de belangrijkste onderdelen van het hoofdstuk.

Leg het onderscheid duidelijk uit:

* Zelfbeheer-wallet: de gebruiker beheert de privésleutels
* Bewaarwallet: een derde partij beheert de privésleutels namens de gebruiker

Loop vervolgens de afwegingen door:

Zelfbeheer

* volledige controle over de fondsen
* geen goedkeuringsproces
* bescherming tegen willekeurige inbeslagname
* meer verantwoordelijkheid
* geen eenvoudige herstelmogelijkheid als de seed phrase verloren gaat

Bewaarwallet

* eenvoudiger herstel en ondersteuning
* makkelijker voor beginners
* meer blootgesteld aan bevriezing van accounts, hacks en controle door derden
* de gebruiker bezit de bitcoin niet echt

Dit is het juiste moment om de volgende uitdrukking te benadrukken:

"Niet jouw sleutels, niet jouw munten."

Studenten moeten dit onderdeel verlaten met niet alleen begrip van de slogan, maar ook wat deze in de praktijk betekent.

**Verschillende soorten wallets en hoe je er een kiest**

Introduceer de wallettypes die in het hoofdstuk worden behandeld:

* online wallet
* mobiele wallet
* desktop wallet
* hardware wallet
* papieren wallet

Behandel er niet één als perfect. Leg in plaats daarvan uit dat elk type afwegingen kent tussen:

* beveiliging
* privacy
* gemak
* compatibiliteit
* kosten
* controle
* reputatie

Maak ook duidelijk dat wij aanraden om aandacht te besteden aan of walletsoftware open-source is, omdat open-source tools door de gemeenschap kunnen worden bekeken, gecontroleerd en voortgezet. Dit sluit direct aan bij het principe van verificatie in Bitcoin.

##### 6.3 Een mobiele Bitcoin-wallet instellen, 10 minuten

Loop met de studenten door het basisproces zoals beschreven in het hoofdstuk:

* download de wallet
* maak een nieuwe wallet aan
* genereer en schrijf de herstelzin op
* bevestig de herstelzin
* voeg extra beveiliging toe indien beschikbaar
* open de wallet en zoek de ontvangfunctie

Maak de waarschuwing over de seed phrase heel duidelijk:

* als de seed phrase verloren gaat, kan de toegang tot de fondsen verloren gaan
* als iemand anders de seed phrase krijgt, kan diegene de fondsen nemen

Als studenten dit praktisch uitvoeren, moet de docent bij elke stap pauzeren en controleren of iedereen begrijpt wat ze doen. Als de les meer conceptueel is, kan dit gedeelte als een walkthrough worden uitgelegd in plaats van live uitgevoerd. De hersteloptie die in het hoofdstuk wordt getoond, is ook nuttig om uit te leggen dat wallets kunnen worden hersteld als de seed phrase correct is geback-upt.

##### 6.4 Ontvangen en Verzenden van Transacties, 17 minuten

**Ontvangen en Verzenden van On-chain Transacties**

Leg nu uit hoe on-chain transacties werken.

Voor het ontvangen van bitcoin:

* open de wallet
* tik op ontvangen of storten
* kopieer het adres, deel de link of toon de QR-code

Voor het verzenden van bitcoin:

* open de wallet
* plak of scan het adres van de ontvanger
* voer het bedrag in
* controleer alle gegevens dubbel
* zend de transactie uit
* wacht op bevestiging

Maak deze kernpunten duidelijk:

* de transactie draagt eigendom over, niet fysieke munten
* transacties zijn onomkeerbaar
* nodes controleren de geldigheid
* miners nemen transacties op in blokken
* transactiekosten beïnvloeden de prioriteit van bevestiging
* on-chain transacties zijn over het algemeen veilig, maar trager en vaak duurder dan Lightning-transacties

Het transactiestroomschema in het hoofdstuk is hier vooral nuttig, omdat het studenten helpt het traject van walletverzoek tot netwerkbevestiging te visualiseren.

**Transacties in de Praktijk en Oefenen met Rollen**

Gebruik de coöperatieve oefenstructuur uit het hoofdstuk om het begrip te versterken. Leg de vier betrokken rollen uit:

* verzender
* ontvanger
* miner
* node-operator

Een eenvoudige aanpak in de klas is om rollen toe te wijzen en één transactie stap voor stap door te nemen. Dit helpt studenten inzien dat een Bitcoin-transactie geen magie is, maar een gecoördineerd proces van goedkeuring, verificatie, opname in een blok en bijwerken van het grootboek.

Het doel hier is niet technische diepgang. Het is om studenten te helpen begrijpen wie wat doet in een transactie en waarom verificatie belangrijk is.

##### 6.5 Vertrouw niet, verifieer, 8 minuten

Leg uit dat dit van toepassing is op:

* wallets
* beurzen
* apps
* transactiedetails
* claims over "gemakkelijk winst maken"
* projecten die doen alsof ze op Bitcoin lijken

Maak duidelijk dat Bitcoin gebruikers vraagt kritisch na te denken, te verifiëren wat ze gebruiken en blind vertrouwen te vermijden. Leg ook uit waarom open-source tools in deze context belangrijk zijn: ze maken onafhankelijke verificatie mogelijk.

###### Afronding en Begripscontrole

Sluit af met een paar snelle vragen:

* Wat is het verschil tussen een custodial en een zelfbewaarde wallet?
* Waarom is de seed phrase zo belangrijk?
* Wat gebeurt er als je een on-chain transactie verstuurt?
* Waarom zijn on-chain transacties trager dan sommige andere Bitcoin-betalingen?
* Wat betekent "Don't Trust, Verify" in de praktijk?

#### Aantekeningen voor de docent

Dit hoofdstuk is zeer praktisch, dus geef prioriteit aan duidelijkheid, veiligheid en herhaling.

Leerlingen hoeven niet elk type wallet in één les te beheersen. De belangrijkste doelen zijn:

* begrijpen van de basis van wallets
* begrijpen van zelfbewaring
* leren van de basisstappen van een transactie
* aannemen van een verantwoordelijke verificatiehouding

Wees extra voorzichtig bij het bespreken van seed phrases en het instellen van wallets. Leerlingen moeten begrijpen dat dit geen kleine details zijn, maar de basis vormen van Bitcoin-bezit.

De meest bruikbare visuals en activiteiten in dit hoofdstuk zijn:

* de vergelijking tussen zelfbewaarde en custodial wallets
* de tabel met afwegingen tussen wallettypes
* de stapsgewijze oefening voor het instellen van een wallet
* het diagram van het transactieproces
* de transactie-activiteit op basis van rollen

##### Hoe Goed eruitziet

* Het is belangrijk dat leerlingen daadwerkelijk een wallet instellen of een zorgvuldige demonstratie bekijken, de seed phrase centraal stellen met "Deze 12 woorden ZIJN je Bitcoin", scenario's testen zoals "Wat gebeurt er als je je telefoon kwijtraakt?", en oefenen met het herkennen van phishing.
* Docenten moeten praktische begeleiders zijn die dit eerder hebben gedaan, veiligheid centraal stellen zonder paranoia, en eerlijk zijn over de leercurve en de benodigde inspanning.
* Leerlingen hebben het gevoel dat ze een echte vaardigheid hebben geleerd die ze kunnen gebruiken, begrijpen dat de seed phrase echt en belangrijk is in plaats van abstract, voelen zich in staat hun eigen Bitcoin te beheren, en begrijpen dat decentralisatie persoonlijke verantwoordelijkheid vereist.
* Leerdoelen zijn behaald als leerlingen een wallet kunnen instellen en het verschil tussen publieke en private sleutels begrijpen, de afwegingen tussen custodial en zelfbewaarde wallets kunnen uitleggen, weten hoe een transactie werkt inclusief inputs, outputs en fees, veiligheidsbewustzijn tonen zoals bescherming van de seed phrase, en kritische vragen stellen over eigendom en controle.

##### Tijdsplanning

Als de tijd beperkt is, geef prioriteit aan:

* Begrijpen van de basis van wallets
* Begrijpen van zelfbewaring
* Leren van de basisstappen van een transactie
* Aannemen van een verantwoordelijke verificatiehouding

Als er tijd over is, besteed extra aandacht aan:

* Vergelijkingstabel zelfbewaarde vs custodial wallets
* Tabel met afwegingen tussen wallettypes
* Stapsgewijze wallet setup-oefening met live demo
* Diagram van het transactieproces met fee-berekeningen
* Geavanceerde beveiligingspraktijken en hardware wallet-overwegingen

##### Als leerlingen moeite hebben

* Seed phrases als "echt" → "Deze phrase IS je bitcoin; geen klantenservice."
* Publieke vs. private sleutels → E-mail-analogie (adres vs. wachtwoord).
* Waarom het moeilijk is → "Jij beheert het; jij bent verantwoordelijk." Erken het compromis.
