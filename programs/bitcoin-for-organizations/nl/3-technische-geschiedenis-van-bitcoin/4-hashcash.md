# 3.4 Hashcash

Hashcash werd gecreëerd door Adam Back, een andere van de vroege vernieuwers in dit domein. Adam had een sterke interesse in vrije markten en privacy op het internet, en kwam terecht op de Cypherpunks-mailinglijst, waar hij zich bij aansloot en een actief deelnemer werd.

Hij was erg geïnteresseerd in digitaal geld en deed enkele suggesties over hoe de groep mogelijk nauwer zou kunnen samenwerken aan DigiCash met Chaum, maar daar kwam niets van terecht. Vervolgens richtte hij zijn aandacht op een ander opkomend probleem – e-mailspam. Hij en de rest van de Cypherpunks wilden een oplossing vinden voor het probleem van spam, waarbij het voor spammers triviaal was om duizenden e-mails te maken en te versturen die netwerken verstoppen. Zijn innovatieve oplossing was gebaseerd op hashing – de mogelijkheid binnen cryptografie om elk gegeven om te zetten in een unieke en willekeurige tekenreeks van een specifieke lengte, om zo het equivalent van een digitale ‘postzegel’ te creëren die aan de e-mail moest worden toegevoegd om deze als geldig te beschouwen en over het netwerk te verzenden. Een triviale kost voor een echte e-mail, maar onbetaalbaar voor een spammer.

De belangrijkste innovatie die Hashcash bracht, was het koppelen van echte middelen – rekenkracht – aan een digitaal netwerk. Terwijl digitale middelen tot dan toe onbeperkt konden worden gerepliceerd, werd het aantal gecreëerde ‘hashcash’ beperkt door hoeveel energie mensen bereid waren erin te steken.

Hoewel de oplossing aan enkele van de criteria voldeed waarvan Adam dacht dat ze nodig waren in een digitaal geldsysteem; het was anoniem, veerkrachtig en trustless, was elke hashcash niet herbruikbaar en niet echt schaars. Hij stelde andere manieren voor waarop deze problemen konden worden aangepakt met behulp van externe derde partijen.

##### BitGold

Nick Szabo bouwde voort op het concept van Hashcash en proof of work om een alternatieve oplossing voor te stellen, die hij beschreef op een mailinglijst een jaar nadat Hashcash werd gepubliceerd, in 1998.

Hoewel dit voorstel dichter bij een oplossing kwam, waren er nog steeds verschillende uitdagingen.

* Wie zou het register van hash-eigendom beheren en hoe kan men hen vertrouwen?
* Hashing zou over het algemeen goedkoper worden na verloop van tijd, wat ook een uitdaging was voor HashCash.

Omdat de gekoppelde hashes van een tijdstempel zouden worden voorzien, stelde hij een vorm van historische tracking voor van de moeilijkheidsgraad van hashing op dat moment; een eerdere hash zou meer verwerkingskosten vereisen dan een latere, omdat de kosten zijn gedaald. Helaas betekende dit dat hashes niet ‘fungibel’ zouden zijn, d.w.z. van gelijke waarde, wat als een belangrijk kenmerk van digitaal geld wordt beschouwd. Om dit op te lossen stelde Nick een vorm van ‘vrij bankieren’ voor bovenop BitGold, waarmee verschillende groepen hashes konden worden samengevoegd die dan als gelijkwaardig zouden worden gewaardeerd.

##### B-Money

Kort na het Bit Gold-voorstel kwam Wei Dai met een vergelijkbare oplossing. Hij had al verschillende andere tools voor de Cypherpunks ontwikkeld en had zijn eigen ideeën over digitaal geld.

Zijn voorstel leek op Bit Gold doordat het digitale handtekeningen gebruikte om geld over te dragen, en de transactieregisters zouden worden opgeslagen op een grootboek, met daarin openbare sleutels en het aantal valuta-eenheden dat aan elk werd toegeschreven. Net als bij Bit-Gold werden vertrouwde derde partijen als beveiligingslekken beschouwd, en men geloofde dat een elektronisch geldsysteem niet afhankelijk mocht zijn van één enkele entiteit om saldi, transacties of het voorkomen van dubbele uitgaven bij te houden.

Wei Dai stelde verschillende oplossingen voor deze problemen voor, waarvan één was dat in plaats van een centrale entiteit(en) die het grootboek bijhoudt, ALLE nodes een kopie zouden bijhouden. Als alle gebruikers hun eigen grootboek en de geldigheid van elke transactie controleerden, zouden de grootboeken gesynchroniseerd moeten blijven over het netwerk zolang alle nodes up-to-date blijven. Dit sterk gedistribueerde systeem zou moeilijk te corrumperen zijn.

Wei Dai erkende dat dit het Byzantijnse generaalsprobleem (1) niet oploste, omdat nodes gemakkelijk synchronisatie konden verliezen of simpelweg konden liegen. Hij stelde alternatieve methoden voor, zoals het hebben van een subset van ‘vertrouwde’ servers die het grootboek bijhouden, en het creëren van financiële prikkels om deze servers eerlijk te houden.

Voor het monetair beleid stelde hij voor de koopkracht van B-Money te koppelen aan een externe consumentenprijsindex. Hij wilde dat dezelfde hoeveelheid B-Money een gelijk aandeel in de index zou kunnen kopen in de loop van de tijd, om zo enige prijsstabiliteit te bieden. Iedereen zou nieuwe valuta-eenheden kunnen genereren door een geldige hash te leveren, maar de moeilijkheidsgraad van het genereren van een hash zou in de loop van de tijd kunnen veranderen op basis van CPU-kosten en de prijsindex, zodat elke eenheid ‘onveranderlijk’ zou zijn.
