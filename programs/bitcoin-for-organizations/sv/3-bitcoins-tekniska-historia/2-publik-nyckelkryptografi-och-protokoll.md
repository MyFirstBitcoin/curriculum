# 3.2 Publik nyckelkryptografi och protokoll

Internet idag, och de flesta moderna datasystem, är beroende av kryptografi, en metod för att dölja information så att endast mottagaren kan avkoda den. Grunderna för den kryptografi som används för att säkra Bitcoin kan spåras tillbaka till 70-talet.

Det första problemet att lösa är – hur man skickar en gemensam hemlighet över ett osäkert medium.

Detta undersöktes först av Whitfield Diffie och Martin Hellman.

Problemet: de två parterna – vanligtvis kallade Alice och Bob – vill dela hemlig information över ett nätverk där andra kan lyssna. För att uppnå detta skapade de Diffie-Hellman-nyckelutbytesprocessen.

Denna gemensamma hemlighet kan sedan användas som startvärde för att skapa många symmetriska nycklar för att kryptera och dekryptera meddelanden som skickas mellan varandra utan att själva nyckeln delas öppet.

Eftersom den privata nyckeln aldrig behöver delas, och olika nycklar används i varje ände för att kryptera och dekryptera, kallas detta en asymmetrisk krypteringsalgoritm.

Användningsområden:

* Alice signerar ett meddelande med Bobs publika nyckel – han är den enda som kan dekryptera det med sin privata nyckel
* Alice signerar ett meddelande med sin privata nyckel – genom att dekryptera med hennes publika nyckel kan vem som helst verifiera att meddelandet skickades av Alice, utan att känna till hennes privata nyckel
* Genom att kombinera dessa två metoder med två lager av kryptering kan ett meddelande skickas krypterat så att endast Bob kan dekryptera det, och han kan sedan verifiera att avsändaren verkligen var Alice

Även om han inte krediterades på artikeln, var Ralph Merkle avgörande för att lösa det som fram till dess ansågs vara ett olösligt problem – hur man etablerar eller återupprättar privat kommunikation över ett öppet och potentiellt fientligt nätverk.

Denna metod är i sig sårbar för en brute force-attack, där en angripare kan ta de delade siffrorna och så småningom återskapa en gemensam nyckel om de har tillräckligt med tid och resurser, så det är inte hela lösningen i sig.

##### Protokoll för publika nyckelkryptosystem

Förutom att bidra till Diffie-Hellman-systemet som beskrivs ovan, **Ralph Merkle** fortsatte att bidra inom detta område i många år, och var avgörande för utvecklingen av några nyckelkomponenter som används av Bitcoin.

En kryptografisk hashfunktion är en matematisk algoritm som tar indata av vilken storlek som helst och utför komplexa beräkningar för att returnera ett hashvärde i bitar, vilket vanligtvis representeras av en alfanumerisk utdata med fast längd i hexadecimal format.

* Indata kan vara av vilken storlek som helst
* Utdatan är alltid av fast längd och deterministisk (samma indata ger samma hash varje gång)
* Det är lätt att verifiera men extremt svårt att omvända processen för att bestämma indata
* En liten ändring av datan förändrar helt utdatan

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/fcfb250d64f20a2c54e1b205bdbccc25127cf680-515x331.svg)

Hashning är en integrerad del av Bitcoin-protokollet. SHA-256, som används i Bitcoin, skapades av NSA och är ett exempel på en kryptografisk hashalgoritm.

* Varje block i kedjan hash:as så att data inte kan ändras – vilket säkerställer integriteten i den distribuerade huvudboken
* Den genererade hashen måste uppfylla 'Proof of work'-kriterierna för att anses vara ett giltigt block
* Merkleträd – genom att använda förgreningar och hash av hash, kan hashträd möjliggöra verifiering av stora datamängder med minimalt lagringsutrymme
* Hashbaserade signaturer och nycklar kan användas för plånböcker, adresser och auktorisation av transaktioner

Distribuerad verifiering av blockkedjans tillstånd och tilläggs-bara huvudboksmodeller som är motståndskraftiga mot ändringar möjliggörs av envägs-hashning. Hashfunktioner ger det pålitliga, deterministiska sättet att verifiera händelser på publika huvudböcker som Bitcoin utan en centraliserad förtroendemodell.

Dessa nya möjligheter inom kryptografiområdet förväntades av dess skapare leda till en ny våg av innovation.

##### Elliptisk kurvkryptografi

En av dessa senare innovationer kom i form av elliptisk kurvkryptografi.

Elliptisk kurvkryptografi introducerades 1985 av två forskare, N. Koblitz och V. Miller. De föreslog idén att använda punkter definierade av elliptiska kurvor istället för ändliga primfält så att antagandet om det diskreta logaritmproblemet gäller, vilket ofta används i det vanliga Diffie-Hellman-nyckelutbytesprotokollet. Detaljerna om hur detta fungerar ligger utanför denna sektion, men på en hög nivå är en elliptisk kurva mängden av punkter som uppfyller en specifik matematisk ekvation.

Ekvationen för en elliptisk kurva ser ut ungefär så här:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

Detta har några användbara egenskaper:

* Horisontell symmetri. Varje punkt på kurvan kan speglas över x-axeln och förblir på samma kurva.
* alla icke-vertikala linjer kommer att skära kurvan på högst tre ställen.
* Kompakta nyckelstorlekar är avgörande för effektiv lagring och överföring av publika nycklar i blockkedjan.

Dessa egenskaper kan användas för att skapa nyckelpar på ett liknande sätt som Diffie-Hellman-algoritmen. Bitcoin använder ECDSA, vilket står för Elliptic Curve Digital Signature Algorithm. Det är en process som använder en elliptisk kurva och ett ändligt fält för att "signera" data på ett sådant sätt att tredje part kan verifiera signaturens äkthet medan undertecknaren behåller den exklusiva förmågan att skapa signaturen. Med bitcoin är datan som signeras transaktionen som överför äganderätten.

Den 'ändliga' delen är liknande 'mod'-metoden med Diffie-Hellman, där ekvationens utdata delas och resten används för att säkerställa att det passar inom ett visst talintervall.
