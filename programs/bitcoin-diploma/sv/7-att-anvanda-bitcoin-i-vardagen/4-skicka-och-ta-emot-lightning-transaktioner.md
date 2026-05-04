# 7.4 Skicka och ta emot Lightning-transaktioner

Med en Lightning-plånbok är det snabbt, billigt och privat att använda Bitcoin, vilket gör transaktioner mellan två personer enkla. Du kan snabbt skicka och ta emot bitcoin för vardagliga saker som att köpa kaffe.

Låt oss titta på några exempel på hur Lightning-nätverket fungerar i praktiken.

###### Exempel 1

Både Marcia och Eva har 5 enheter av valuta. Marcia vill skicka 2 enheter till Eva. Betalningen går via Johan, som hjälper till att vidarebefordra betalningen genom Lightning-nätverket. Efter att betalningen är genomförd har Eva 7 enheter och Marcia har 3.

Johan hjälper till att dirigera betalningen, men han kan inte stjäla pengarna. Lightning-nätverket använder kryptografi för att säkerställa att endast den avsedda mottagaren kan ta emot betalningen. Johan hjälper helt enkelt betalningen att röra sig genom nätverket.

Detta visar en viktig fördel med Lightning-nätverket: människor kan skicka betalningar snabbt utan att behöva lita på mellanhänder som banker.

Nodoperatörer som Johan kan också tjäna små avgifter för att hjälpa till att dirigera betalningar. Genom att göra detta hjälper de nätverket att förbli decentraliserat och effektivt.

Jämfört med vanliga Bitcoin-transaktioner:

* **Transaktioner på kedjan** sker direkt på Bitcoin-blockkedjan. De är mycket säkra men kan vara långsammare och dyrare.
* **Lightning-transaktioner** sker utanför kedjan och gör det möjligt för betalningar att gå mycket snabbare och till en mycket lägre kostnad.

På grund av detta är Lightning användbart för små, vardagliga betalningar, medan transaktioner på kedjan ofta används för större överföringar eller långtidsförvaring.

###### Exempel 2

Mina älskar att äta ute och stannar ofta till på sitt favoritkafé. Med så många olika betalningsalternativ tillgängliga är hon osäker på vilket som är det bästa valet. Som tur är har hon lärt sig lite om Bitcoin och Lightning-nätverket. Efter att ha gått igenom sina alternativ inser Mina att det bästa är att använda en Lightning-betalningsmetod.

Mina vill köpa en kaffe, men att betala med en vanlig Bitcoin-transaktion kan ibland ta tid och kräva högre avgifter. Istället bestämmer hon sig för att använda Lightning-nätverket.

Lightning-nätverket gör det möjligt för människor att skicka bitcoin direkt och med mycket låga avgifter. Detta gör det perfekt för små, vardagliga köp som kaffe.

För att börja använda Lightning laddar Mina ner en Lightning-plånbok på sin telefon. Hon skickar sedan lite bitcoin från sin vanliga Bitcoin-plånbok till sin Lightning-plånbok. Detta steg använder en vanlig Bitcoin-transaktion på blockkedjan. När pengarna finns i hennes Lightning-plånbok kan de användas på Lightning-nätverket.

Nu kan Mina betala kaféet direkt med Lightning. Betalningen sker utanför den vanliga Bitcoin-blockkedjan, vilket är anledningen till att det går mycket snabbare och är billigare än en vanlig transaktion på kedjan.


| Fördelar | Lightning-nätverket | Traditionellt banksystem |
| --- | --- | --- |
| Hastighet | Snabb | Långsam |
| Transparens | Transparent | Ogenomskinlig |
| Säkerhet | Säker | Sårbar |
| Transaktionsavgifter | Låga | Höga |
| Finansiell inkludering | Hög | Begränsad |
| Skalbarhet | Hög | Låg |
| Integritet | Hög | Måttlig |
| Interoperabilitet | Hög | Låg |
| Rättslig efterlevnad | Måttlig | Hög |
| Kostnadseffektivitet | Hög | Måttlig |


On-chain-transaktioner sker direkt på Bitcoin-blockkedjan och kan ta mer tid och ha högre avgifter. Lightning-transaktioner sker utanför kedjan, vilket möjliggör snabba och billiga betalningar samtidigt som du fortfarande använder bitcoin.


| Visa, Inc. | Bitcoin On-chain | Lightning-nätverket |
| --- | --- | --- |
| Kapacitet på 65 000 transaktioner per sekund. | Kapacitet på 7 transaktioner per sekund. | Kapacitet på miljontals transaktioner per sekund. |


![Lightning Network Map](https://cdn.sanity.io/images/vje9ehw2/staging/5a760247cf4c32074c62f40aea8dc21095882740-504x245.svg)

https://mempool.space/graphs/lightning/nodes-channels-map

Det här är en karta över hela Lightning-nätverket. Tack vare tusentals Lightning-nodoperatörer kan du skicka sats till vilken användare som helst med en Bitcoin Lightning-plånbok, var de än befinner sig i världen. Betalningen kommer fram på några sekunder och kostar bara några öre.**Prova själv!**

#### Aktivitet: Lightning-stafett

https://qr.myfirstbitcoin.org/lightning.pdf

**Detta är en praktisk övning där elever skickar och tar emot riktiga sats med hjälp av Lightning-nätverket.**

###### Viktiga punkter

1. Genom att använda en Lightning-plånbok bygger du upp självförtroende att ta emot och skicka riktiga sats.
1. Var uppmärksam på enheterna. Vissa plånböcker låter användare skicka bitcoin ELLER sats (1/100 000 000 av en bitcoin).
1. Lightning-betalningar kan ibland fastna i routingen, särskilt vid större betalningar. Även om det är möjligt, blir denna typ av användarupplevelse allt ovanligare i takt med att nätverket mognar.

###### Tips till elever

Kontrollera med din instruktör om/hur aktuella on-chain Bitcoin-transaktionsavgifter påverkar den specifika Lightning-plånbok du använder.
