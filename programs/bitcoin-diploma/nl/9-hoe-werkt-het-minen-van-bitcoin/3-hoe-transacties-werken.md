# 9.3 Hoe transacties werken

Nu je begrijpt wat publieke en private sleutels zijn, en ook de rollen van nodes en miners, volgt hier hoe een Bitcoin-transactie van begin tot eind werkt.

1. Adam wil bitcoin naar Gerardo sturen. Hij maakt een transactie aan met Gerardo’s adres, het te versturen bedrag en een vergoeding.
1. Adam ondertekent de transactie met zijn privésleutel om eigenaarschap te bewijzen.
1. Hij zendt de transactie uit naar het Bitcoin-netwerk.
1. Nodes ontvangen de transactie en controleren of deze aan de regels voldoet, waaronder het verifiëren van de handtekening en of Adam genoeg bitcoin heeft.
1. Als de transactie geldig is, wordt deze gedeeld over het netwerk en toegevoegd aan de mempool, waar wachtende transacties staan.
1. Miners kiezen transacties uit de mempool en nemen ze op in een blok dat ze proberen te minen.
1. Wanneer een miner succesvol een blok mined, wordt het gedeeld met het netwerk en gecontroleerd door andere nodes.
1. Als het blok geldig is, wordt het toegevoegd aan de blockchain. Gerardo ontvangt de bitcoin.
1. Naarmate er meer blokken worden toegevoegd, krijgt de transactie meer bevestigingen, waardoor deze veiliger wordt.

Zodra de transactie in een blok is opgenomen, is deze bevestigd. Adam kan die bitcoin niet opnieuw uitgeven, en Gerardo kan het ontvangen bedrag in een nieuwe transactie uitgeven.


> **Note**
>
> Transactie & vergoeding geselecteerd → Ondertekend door wallet en verzonden → Verspreid door nodes → Miner voegt transactie toe aan bloktemplate → Miner wint Proof-of-Work-wedstrijd → Nieuw blok wordt gevalideerd → Nieuw blok wordt verspreid door nodes


###### Bronnen


[▶ YouTube](https://www.youtube.com/watch?v=xc_TxlByxeY)
