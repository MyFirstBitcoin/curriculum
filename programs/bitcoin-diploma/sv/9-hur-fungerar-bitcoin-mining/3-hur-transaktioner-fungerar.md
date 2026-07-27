# 9.3 Hur transaktioner fungerar

Nu när du förstår publika och privata nycklar, samt rollerna för noder och miners, så här fungerar en Bitcoin-transaktion från början till slut.

1. Adam vill skicka bitcoin till Gustav. Han skapar en transaktion med Gustavs adress, beloppet som ska skickas och en avgift.
1. Adam signerar transaktionen med sin privata nyckel för att bevisa ägarskap.
1. Han sänder ut transaktionen till Bitcoin-nätverket.
1. Noder tar emot den och kontrollerar att den följer reglerna, inklusive att verifiera signaturen och att Adam har tillräckligt med bitcoin.
1. Om den är giltig delas transaktionen över nätverket och läggs till i mempoolen, där väntande transaktioner ligger.
1. Miners väljer transaktioner från mempoolen och inkluderar dem i ett block de försöker mina.
1. När en miner lyckas mina ett block delas det med nätverket och kontrolleras av andra noder.
1. Om det är giltigt läggs blocket till i blockkedjan. Gustav tar emot bitcoinen.
1. När fler block läggs till får transaktionen fler bekräftelser, vilket gör den säkrare.

När transaktionen har inkluderats i ett block är den bekräftad. Adam kan inte spendera den bitcoinen igen, och Gustav kan använda det han fått i en ny transaktion.


> **Light**
>
> Transaktion & avgift väljs → Signeras av plånboken och skickas → Distribueras av noder → Miner lägger till transaktionen i blockmallen → Miner vinner Proof-of-Work-tävlingen → Nytt block valideras → Nytt block distribueras av noder


###### Resurser


[▶ Titta på den här videon om Bitcoin-noder](https://www.youtube.com/watch?v=xc_TxlByxeY)
