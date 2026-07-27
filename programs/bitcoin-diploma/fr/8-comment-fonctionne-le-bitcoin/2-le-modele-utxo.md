# 8.2 Le modèle UTXO

##### Que sont les UTXO ?

Ne vous laissez pas intimider par ce nom un peu bizarre. Vous pouvez considérer les UTXO comme des « morceaux » de bitcoin, un peu comme les billets et les pièces que vous avez dans votre portefeuille. Par exemple, si vous payez un article à 6 $ avec un billet de 10 $, vous recevez 4 $ de monnaie. Le bitcoin fonctionne de la même manière.

Tous les bitcoins que vous possédez sont constitués de différents UTXO. Lorsque vous envoyez des bitcoins, votre portefeuille utilise un ou plusieurs de ces éléments pour effectuer le paiement.

Si le montant que vous dépensez est supérieur à celui que vous envoyez, la valeur restante vous est restituée sous forme de monnaie, via un nouvel UTXO. Dans le même temps, le destinataire reçoit un nouvel UTXO correspondant au bitcoin que vous lui avez envoyé.

Le solde de votre portefeuille correspond tout simplement à la valeur totale de tous les UTXO que vous contrôlez.


> **Callout – Confidentialité**
>
> Vous ne devez pas divulguer vos UTXO à des tiers, car si quelqu'un en prend connaissance, il pourra suivre vos transactions et finira par connaître le montant de vos avoirs.


###### Exemple

1. Alice souhaite envoyer 5 BTC à Bob.
1. Son portefeuille utilise deux de ses UTXO qui, ensemble, représentent une valeur de 6 BTC.
1. La transaction envoie **5 BTC à Bob**, ce qui crée un nouvel UTXO dans le portefeuille de Bob.
1. Les autres **0,99 BTC est rendu à Alice à titre de monnaie**, après avoir payé un **0,01 BTC de frais de transaction**.
1. Une fois la transaction confirmée, elle est ajoutée au registre Bitcoin et les UTXO utilisés par Alice sont marqués comme dépensés, ce qui les rend inutilisables.

###### Ressources


[▶ Regardez « Comment fonctionne le Bitcoin en coulisses »](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
