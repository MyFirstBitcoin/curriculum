# 9.1 Bitcoin-noder och gruvarbetare

Bitcoin-noder kan låta tekniskt, men de är helt enkelt programvara som håller en kopia av Bitcoin-blockkedjan på en dator. Blockkedjan är en gemensam redovisning av alla Bitcoin-transaktioner.

När du kör din egen nod verifierar du Bitcoin-transaktioner själv istället för att lita på någon annan. Det ger dig mer självständighet och hjälper till att hålla Bitcoin-nätverket decentraliserat.

Du kan tänka på en Bitcoin-nod som en digital trafikpolis med några viktiga uppgifter.

1. Den håller en kopia av blockkedjan, vilket är historiken över alla Bitcoin-transaktioner.
1. Noder kopplar upp sig mot andra noder runt om i världen och delar information. Ett exempel är listan över nya transaktioner som väntar på att bekräftas, vilket kallas mempoolen.
1. Noder kontrollerar att varje transaktion följer Bitcoins regler. Om en transaktion är ogiltig, avvisar noden den.

Noder hjälper också nya noder att ansluta till nätverket genom att dela blockkedjan med dem. Men varje ny nod kontrollerar ändå alla regler självständigt.

Vem som helst kan köra en nod genom att installera programvara som Bitcoin Core och ladda ner blockkedjan. När den är igång fortsätter noden att ta emot nya block ungefär var tionde minut och verifierar dem innan de läggs till i dess kopia av blockkedjan.

Att köra en nod hjälper till att göra Bitcoin-nätverket säkrare och mer decentraliserat, eftersom fler personer självständigt verifierar systemet.

#### Vad är en Bitcoin-nod?

> Syftet med mining är inte att skapa nya bitcoin; det är incitamentssystemet. Mining är mekanismen som gör Bitcoins säkerhet decentraliserad.  
_Andreas M. Antonopoulos_


> **Callout**
>
> Miners samlar in obekräftade transaktioner, bildar ett block och använder energi för att hitta en nyckel som lägger till och säkrar blocket.


Miners tävlar om att lägga till nästa block av transaktioner till blockkedjan. För att göra detta måste de hitta ett speciellt nummer som skapar en giltig blockhash. Du kan föreställa dig det som att leta efter rätt nyckel bland miljarder möjligheter. Den första minern som hittar rätt hash vinner loppet och får rätten att lägga till sitt block i blockkedjan.

När en miner hittar en giltig hash delar de sitt block med nätverket. Andra miners verifierar snabbt att lösningen är korrekt. Om den är det läggs blocket till i blockkedjan, vilket hjälper till att hålla Bitcoins offentliga huvudbok säker.

Miners tjänar bitcoin på två sätt:

* **Blockbelöningar:** Nya bitcoin skapas och ges till den miner som lyckas lägga till ett block i blockkedjan.
* **Transaktionsavgifter:** När folk skickar bitcoin inkluderar de en liten avgift. Den miner som lägger till blocket får avgifterna från transaktionerna som ingår i det blocket.

#### Bitcoin-halveringar


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12,5 BTC | 6,25 BTC | 3,125 BTC |



> **Callout**
>
> Miners belöningar för att slutföra ett block halveras var 210 000:e block, ungefär vart fjärde år.


Bitcoin har ett fast maximalt utbud på 21 000 000 bitcoin, men alla skapades inte när Bitcoin startade. Istället introduceras nya bitcoin gradvis i omlopp genom **mining**.

När miners framgångsrikt lägger till ett nytt block av transaktioner till Bitcoin-nätverket får de en **blockbelöning** i bitcoin. I Bitcoins tidiga dagar var denna belöning 50 bitcoin per block. Denna belöning uppmuntrade folk att använda datorkraft och elektricitet för att hjälpa till att säkra nätverket.

Ungefär var 210 000:e block (ungefär vart fjärde år) halveras blockbelöningen. Denna händelse kallas **halvering**. Halveringen saktar ner skapandet av nya bitcoin och hjälper till att säkerställa att det totala utbudet aldrig överstiger 21 miljoner. Med tiden gör detta bitcoin allt mer sällsynt.


> **Definition – Cirkulerande utbud**
>
> **Cirkulerande utbud** avser den totala tillgängliga mängden av en valuta. För Bitcoin är det totala cirkulerande utbudet det antal mynt som har minerats och är i omlopp vid en given tidpunkt.


![ Bitcoin Supply Schedule](https://cdn.sanity.io/images/vje9ehw2/staging/d89296555e713b656f79e420fcca06f08a1fc5c0-292x200.svg)


> **Definition – Bitcoins utbudsschema**
>
> **Bitcoins utbudsschema** är den förutbestämda och offentliga planen för hur nya bitcoin släpps ut i omlopp, utformad för att bevara Bitcoins knapphet över tid.


Efter varje halvering halveras den bitcoin-belöning som miners får för att lägga till ett block. Detta minskar takten på skapandet av nya bitcoin.

Miners tjänar fortfarande transaktionsavgifter från de transaktioner som ingår i blocket de miner. Med tiden förväntas dessa avgifter bli en större del av miners inkomster.

Halveringar är inbyggda i Bitcoin-protokollet och sker automatiskt ungefär vart fjärde år. Tack vare detta är Bitcoins utgivningsschema förutsägbart och transparent.

Tabellen visar kommande halveringar, inklusive ungefärligt datum, blocknummer när de sker, den nya blockbelöningen och procentandelen av den totala bitcoinmängden som har blivit utvunnen.


| Händelse | Datum | Block | Belöning | Utvunnet |
| --- | --- | --- | --- | --- |
| 5:e halveringen | 2028 | 1 050 000 | 1,5625 BTC | 98,44 % |
| 6:e halveringen | 2032 | 1 260 000 | 0,78125 BTC | 99,22 % |
| 7:e halveringen | 2036 | 1 470 000 | 0,390625 BTC | 99,61 % |


När fler bitcoin utvinns ökar den cirkulerande mängden tills det maximala antalet på 21 000 000 bitcoin har nåtts, vilket förväntas ske runt år 2140. Eftersom färre nya bitcoin skapas över tid, kan priset på Bitcoin stiga om efterfrågan ökar. Detta uppmuntrar också gruvarbetare att fortsätta säkra nätverket genom att bidra med sin datorkraft.

#### Vad är en giltig blockhash i Bitcoin?

I Bitcoin tävlar gruvarbetare om att hitta en speciell kod som kallas en **blockhash**. Denna kod identifierar ett block med transaktioner och gör det möjligt att lägga till det i blockkedjan.

Varje block innehåller information om senaste transaktionerna och inkluderar även hashvärdet från föregående block. Detta länkar samman varje block och bildar en kedja från det allra första blocket (Genesis Block) till det senaste.

En hash fungerar som ett **digitalt fingeravtryck** för datan i blocket. Om någon information i blocket skulle ändras, skulle fingeravtrycket också ändras. Detta gör det enkelt för vem som helst att verifiera att blockkedjans transaktionshistorik inte har manipulerats och hjälper till att hålla nätverket säkert.


> **Callout**
>
> Satoshi Nakamoto, skaparen av Bitcoin, utvann Genesis Block, vilket låste upp totalt 50 bitcoin.


#### Kapplöpningen om att utvinna ett block

Gruvarbetare tävlar om att hitta en giltig blockhash. Den första gruvarbetaren som hittar en får lägga till det nya blocket i blockkedjan och ta emot en bitcoinbelöning.

För att vara giltig måste blockets hash vara lägre än ett tal som nätverket bestämmer, kallat svårighetsgränsen. Eftersom hashvärden är slumpmässiga måste gruvarbetarna fortsätta att prova olika indata tills de hittar en som fungerar.

Om för många gruvarbetare tävlar skulle block hittas för snabbt. Om för få deltar skulle det ta för lång tid att hitta block. För att hålla systemet igång smidigt justerar Bitcoin automatiskt svårighetsgraden var 2 016:e block (ungefär varannan vecka).

Denna justering säkerställer att det i genomsnitt läggs till ett nytt block i blockkedjan ungefär var tionde minut.


> **Definition – Definition av svårighetsgrad**
>
> Svårighetsgraden**svårighetsgrad** i Bitcoin-mining mäter hur svårt det är att hitta en giltig blockhash. Nätverket justerar denna svårighetsgrad var 2 016:e block (ungefär varannan vecka) så att nya block läggs till i blockkedjan ungefär var tionde minut. Ju högre svårighetsgrad, desto svårare är det för gruvarbetare att hitta en giltig block.


Genom att hitta en giltig blockhash bevisar en gruvarbetare att de har utfört det arbete som krävs för att lägga till ett nytt block i blockkedjan. Denna process kallas **Proof of Work** (PoW). Det är säkerhetsmekanismen som gör det möjligt för Bitcoin att bekräfta transaktioner och lägga till nya block i blockkedjan. Den gruvarbetare som först hittar den giltiga hashen får en belöning i bitcoin, vilket inkluderar blockbelöningen och transaktionsavgifterna från de transaktioner som ingår i blocket.

Proof of Work (PoW) hjälper till att hålla Bitcoin säkert genom att göra det extremt dyrt för någon att försöka fuska eller ta kontroll över nätverket. Istället är det mycket mer lönsamt att följa reglerna.

Gruvarbetare har fyra huvudroller:

1. **Samla in transaktioner**: Gruvarbetare väljer transaktioner som har skickats till nätverket och placerar dem i ett kandidatblock.
1. **Utföra Proof of Work**: Gruvarbetare tävlar om att lösa ett svårt matematiskt problem genom att hitta en giltig blockhash.
1. **Sänd ut blocket**: Den första minern som hittar en giltig lösning delar det nya blocket med nätverket.
1. **Tjäna belöningar**: Om blocket är giltigt läggs det till i blockkedjan och minern får nyskapade bitcoin samt transaktionsavgifter.

Många miners runt om i världen försöker skapa nästa block samtidigt. När en miner hittar en giltig lösning kontrollerar nätverket blocket. Om allt är korrekt läggs det till i blockkedjan. Andra konkurrerande block kasseras. Denna process håller nätverket överens och förhindrar dubbelspendering.

* Miners är datorer som hjälper till att underhålla och uppdatera Bitcoins huvudbok.
* De samlar in transaktioner och grupperar dem i ett block. Sedan kör de blockets data genom en hash-algoritm för att skapa en unik kod som kallas en hash.
* Miners upprepar denna process många gånger och letar efter en hash som uppfyller Bitcoins regler. Den första minern som hittar en giltig hash får nyskapade bitcoin som belöning, och deras block läggs till i blockkedjan.
* Varje blocks hash kopplar också ihop det med föregående block. Om någon försökte ändra en tidigare transaktion skulle hasharna inte längre stämma, och nätverket skulle avvisa den ändrade kedjan. Det är detta som håller Bitcoins huvudbok säker.
