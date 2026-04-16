# 8.2 Le modèle UTXO

##### Que sont les UTXO ?

Ne soyez pas intimidé par ce nom étrange. Vous pouvez considérer les UTXO comme des morceaux de bitcoin, similaires aux billets et pièces dans votre portefeuille. Par exemple, si vous payez un article à 6 $ avec un billet de 10 $, vous recevez 4 $ de monnaie. Le bitcoin fonctionne de manière similaire.

Tous les bitcoins que vous possédez sont constitués de différents UTXO. Lorsque vous envoyez des bitcoins, votre portefeuille utilise un ou plusieurs de ces morceaux pour effectuer le paiement.

Si le morceau que vous dépensez est plus grand que le montant que vous envoyez, la valeur restante vous revient comme monnaie sous la forme d’un nouvel UTXO. En même temps, le destinataire reçoit un nouvel UTXO représentant les bitcoins que vous avez envoyés.

Le solde de votre portefeuille est simplement la valeur totale de tous les UTXO que vous contrôlez.


> **Callout – Confidentialité**
>
> Il est important de noter que vous ne devez pas révéler vos UTXO aux autres, car si quelqu’un les connaît, il peut suivre vos transactions et finira par savoir combien d’argent vous possédez.


###### Exemple

1. Alice souhaite envoyer 5 BTC à Bob.
1. Son portefeuille utilise deux de ses UTXO qui valent ensemble 6 BTC.
1. La transaction envoie **5 BTC à Bob**, créant un nouvel UTXO dans le portefeuille de Bob.
1. Le reste, soit **0,99 BTC revient à Alice comme monnaie**, après avoir payé des **frais de transaction de 0,01 BTC**.
1. Une fois la transaction confirmée, elle est ajoutée au registre de Bitcoin et les UTXO utilisés par Alice sont marqués comme dépensés, ils ne peuvent donc plus être utilisés.

###### Ressources


[▶ YouTube](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
