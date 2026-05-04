# 2.7 Bitcoin is niet echt gedecentraliseerd

> De complexiteit van crypto ontstaat door pogingen tot decentralisatie—door macht en bestuur in het systeem te verspreiden, is er theoretisch geen behoefte aan vertrouwde tussenpersonen zoals financiële instellingen. Dat was het uitgangspunt van het oorspronkelijke Bitcoin-whitepaper, dat een cryptografische oplossing bood waarmee betalingen konden worden verzonden zonder tussenkomst van een financiële instelling of andere vertrouwde tussenpersoon. Bitcoin werd echter al snel gecentraliseerd en is nu afhankelijk van een kleine groep softwareontwikkelaars en miningpools om te functioneren  
_Internationaal Monetair Fonds_

Zoals het bovenstaande citaat uit een vrij recent bericht van het Internationaal Monetair Fonds laat zien, blijft de reguliere financiële sector beweren dat Bitcoin niet gedecentraliseerd is, en verwart men Bitcoin bovendien met andere crypto-activa.

##### Inleiding

![Trilemma](https://cdn.sanity.io/images/vje9ehw2/staging/5f43c065cf35646438433c15e39e290a48d1eb7c-161x167.svg)

Decentralisatie is een cruciaal aspect van Bitcoin. Het vermogen om de regels van het protocol, zoals schaarste en distributie, te handhaven zonder centrale autoriteit zorgt ervoor dat het kan functioneren als permissieloos geld voor een mondiale samenleving.

Zoals Satoshi opmerkte in zijn online correspondentie, hielden gedecentraliseerde diensten zoals BitTorrent ‘stand’ tegen overheidsmaatregelen, in vergelijking met diensten met geïdentificeerde eigenaar(s) en gecentraliseerde servers. Hij maakte zich duidelijk zorgen over het potentiële risico dat overheden of andere belangen Bitcoin zouden kunnen uitschakelen of anderszins nadelig beïnvloeden.

In deze context zijn we geïnteresseerd in de decentralisatie van:

* De ontwikkeling en het beheer van de code die het protocol uitvoert; wie mag de regels veranderen?
* De miningfunctie die nieuwe blokken creëert volgens de regels en controleert op dubbele uitgaven
* De nodes die transacties op geldigheid controleren en een kopie van de blockchain bijhouden

##### Ontwikkelaars

Bitcoin is een open-sourceprotocol dat iedereen vrij kan bekijken, downloaden, kopiëren of voorstellen om te wijzigen. Het is beschikbaar in een GitHub-bibliotheek, waarbij de broncode oorspronkelijk in 2009 werd gelanceerd door Satoshi Nakamoto. Iedereen kan de code downloaden en een node draaien, waarvan de meerderheid de originele Bitcoin Core-software draait, die in de loop der tijd is bijgewerkt.

![How Does an idea Make Its Way Into Bitcoin Core?](https://cdn.sanity.io/images/vje9ehw2/staging/49f70d059c9dbe19a6e4500e9abd8db66ca97bff-1300x1439.png)

_Bron: https://river.com/learn/what-is-bitcoin-core/_

De ontwikkeling van Bitcoin Core volgt de best practices van open source-ontwikkeling. Op elk moment kunnen er meerdere ontwikkelaars zijn die code schrijven of wijzigingen beoordelen. Zij moeten luisteren naar de zorgen van de node-operators en miners, evenals de gebruikersbasis, voordat ze een kritieke wijziging in de code aanbrengen, die zal worden beoordeeld en goedgekeurd zoals weergegeven in het bovenstaande stroomschema voordat deze in de code wordt opgenomen.

De regels van Bitcoin zijn vervolgens gecodeerd in deze Bitcoin Core-software, die op elke node draait. Iedereen kan een wijziging in de regels voorstellen – de regels zijn code, maar ze zijn niet_alleen_code, ze zijn_overeengekomen_code. Als ze eenzijdig worden gewijzigd, maakt de nieuwe code geen deel meer uit van het consensusmechanisme en dus niet meer van Bitcoin. Iets veranderen aan Bitcoin en toch binnen de consensus blijven is lastig. Voorgestelde wijzigingen aan de code vallen in een van drie categorieën:

* Binnen de bestaande regels: Kleine upgrades zoals spelfouten, een mooiere gebruikersinterface of gegevensbeheer kunnen hieronder vallen en zijn relatief eenvoudig goed te keuren.
* Het toevoegen van een nieuwe regel die beperkingen toevoegt aan de bestaande regels – zoals het verkleinen van de blokgrootte. Dit wordt een ‘soft fork’ genoemd. Nodes die ervoor kiezen de codewijziging niet te implementeren en op de oude versie blijven, kunnen nog steeds deelnemen aan het netwerk.
* Het toevoegen van een nieuwe regel die de huidige regels breekt, bijvoorbeeld een verhoging van de blokgrootte. Nodes die niet upgraden naar de nieuwe code zullen een blok dat in het grotere formaat is aangemaakt als ongeldig beschouwen. Dit wordt een ‘hard fork’ genoemd en zal een splitsing veroorzaken tussen de nodes die de originele en de nieuwe code draaien, en creëert een nieuwe munt. Dit is eerder gebeurd, maar heeft niet geleid tot langdurig succes voor de nieuwe munt, omdat de meerderheid van de nodes ervoor koos de originele code te behouden.

Daarom kan een enkele partij of groep mensen de Bitcoin-code niet eenzijdig wijzigen zonder consensus te bereiken, anders riskeren ze een splitsing van de keten en het ontstaan van een nieuwe munt met een ander stel regels.

##### Mining

De miningfunctie valideert de transacties net als elke andere node op het netwerk, maar zal vervolgens de energie verbruiken die nodig is om een nieuw blok te creëren dat voldoet aan de consensusregels in de code. Succes stelt de miner in staat om de beloningen te ontvangen in de vorm van transactiekosten en Bitcoin-beloningen (op het moment van schrijven 3,125 munten per blok).

Mining wordt normaal gesproken uitgevoerd door miningpools, waarbij mensen hun rekenkracht of hash rate bundelen om de kans op het succesvol minen van een blok te vergroten en de beloningen te delen. Er bestaat een gevaar dat een of meer van deze miningpools kunnen samenwerken om een dominantie van 51% in mining te bereiken en in wezen het validatieprotocol van het netwerk in hun voordeel kunnen overrulen om munten dubbel uit te geven. Dit zou een enorme hoeveelheid middelen vereisen tegen hoge kosten, en individuele miners kunnen op elk moment eenvoudig overstappen naar een andere miningpool. Zo'n aanval zou waarschijnlijk ook de waarde van bitcoin doen instorten, omdat het duidelijk zou zijn dat de integriteit van het netwerk is aangetast. Een aanvaller zou daarom snel eventuele verkregen bitcoin moeten omzetten in fiat voordat de waarde daalt. Dit maakt het nog moeilijker om een aanval langdurig vol te houden, en daarom is het voor een miner of pooloperator winstgevender om zich aan de regels te houden en te proberen geldige blokken te minen.

De geografische spreiding van de miningfunctie is ook belangrijk om te voorkomen dat bijvoorbeeld overheden de miningcapaciteit overnemen of uitschakelen. Een recent verbod op mining door China toonde bijvoorbeeld het aanpassingsvermogen van Bitcoin aan en het vermogen om dergelijke overheidsinterventie te overleven, waarbij het netwerk zich snel aanpaste en herstelde van het verlies aan rekenkracht.

##### Nodes

In tegenstelling tot mining, waarvoor een aanzienlijke financiële investering nodig is om effectief te kunnen concurreren in de race om nieuwe blokken te minen, of codeontwikkeling waarvoor programmeerkennis vereist is, is het draaien van een node iets wat iedereen die wil bijdragen aan de decentralisatie van Bitcoin kan doen.

Nodes draaien de Bitcoin Core-software en handhaven de regels die in de code zijn opgenomen om ervoor te zorgen dat miners niet vals spelen, bijvoorbeeld door zichzelf een hogere blokbeloning toe te kennen dan is toegestaan. Ze handhaven ook het maximum van 21 miljoen munten, wat cruciaal is om de schaarste van Bitcoin te behouden. Om Bitcoin te stoppen, zou een overheid of kwaadwillende elke kopie van de blockchain moeten vernietigen, die momenteel op duizenden nodes wereldwijd draait—een vrijwel onmogelijke opgave.

##### Mensen

Een ander aspect van mogelijke centralisatie zijn mensen. Elke andere ‘alt-coin’ heeft een boegbeeld—iemand die mogelijk onder druk gezet kan worden om veranderingen te bepleiten die niet in het belang van Bitcoin zijn. Satoshi Nakamoto bleef lang genoeg om ervoor te zorgen dat Bitcoin op weg was naar succes, voordat hij voorgoed verdween en het in handen liet van anderen om de software te verbeteren en aan te passen.

Hoe zit het met houders van grote hoeveelheden Bitcoin? Vroege investeerders die hun munten hebben behouden en niet zijn kwijtgeraakt, zullen nu extreem rijk zijn. Het is belangrijk op te merken dat dit inderdaad het geval kan zijn, maar dat geeft hen niet meer invloed op het systeem dan wie dan ook, in tegenstelling tot ‘proof of stake’-munten waarbij de vroege gebruikers die al rijk zijn in die munt voordelen krijgen bij het nemen van beslissingen en de distributie van toekomstige munten. Dit heeft of zal onvermijdelijk leiden tot centralisatie op termijn.

##### Conclusie

Wat zijn de potentiële bedreigingen die decentralisatie kan proberen te beperken?

* Overheid die Bitcoin uitschakelt of verbiedt
* Ongewenste wijzigingen in de code die één groep belangen binnen Bitcoin bevoordelen, bijvoorbeeld het verhogen van de blokbeloning
* Dwang op het protocol door overheid of kwaadwillenden om de richting van het protocol te beïnvloeden
* De mogelijkheid voor een groep miners om het netwerk over te nemen en Bitcoin dubbel uit te geven – een 51%-aanval

Zoals we kunnen zien, zorgt de combinatie van nodes, codeontwikkelaars en miners, evenals het gebruik van het ‘proof of work’-mechanisme, ervoor dat Bitcoin voldoende gedecentraliseerd is zodat deze potentiële bedreigingen niet als groot risico worden beschouwd. De gemeenschap zal de situatie moeten blijven monitoren om ervoor te zorgen dat dit zo blijft.
