# 7.4 Senden und Empfangen von Lightning-Transaktionen

Mit einer Lightning-Wallet ist die Nutzung von Bitcoin schnell, günstig und privat, wodurch Transaktionen zwischen zwei Personen einfach werden. Du kannst blitzschnell Bitcoin für alltägliche Dinge wie den Kauf eines Kaffees senden und empfangen.

Schauen wir uns ein paar Beispiele an, wie das Lightning-Netzwerk in der Praxis funktioniert.

###### Beispiel 1

Sowohl Marcia als auch Eva haben 5 Einheiten der Währung. Marcia möchte Eva 2 Einheiten senden. Die Zahlung läuft über Jens, der hilft, die Zahlung durch das Lightning-Netzwerk weiterzuleiten. Nach Abschluss der Zahlung hat Eva 7 Einheiten und Marcia 3.

Jens hilft, die Zahlung zu routen, aber er kann die Gelder nicht stehlen. Das Lightning-Netzwerk verwendet Kryptografie, um sicherzustellen, dass nur der vorgesehene Empfänger die Zahlung erhalten kann. Jens hilft lediglich, die Zahlung durch das Netzwerk zu leiten.

Das zeigt einen entscheidenden Vorteil des Lightning-Netzwerks: Menschen können Zahlungen schnell senden, ohne Mittelsmänner wie Banken vertrauen zu müssen.

Node-Betreiber wie Jens können auch kleine Gebühren verdienen, wenn sie helfen, Zahlungen zu routen. Dadurch tragen sie dazu bei, dass das Netzwerk dezentralisiert und effizient bleibt.

Im Vergleich zu regulären Bitcoin-Transaktionen:

* **On-Chain-Transaktionen** finden direkt auf der Bitcoin-Blockchain statt. Sie sind sehr sicher, können aber langsamer und teurer sein.
* **Lightning-Transaktionen** finden außerhalb der Blockchain (off-chain) statt und ermöglichen es, Zahlungen viel schneller und zu deutlich geringeren Kosten zu senden.

Deshalb eignet sich Lightning besonders für kleine, alltägliche Zahlungen, während On-Chain-Transaktionen oft für größere Überweisungen oder langfristige Aufbewahrung genutzt werden.

###### Beispiel 2

Mina geht gerne essen und besucht oft ihr Lieblingscafé um die Ecke. Bei so vielen verschiedenen Zahlungsmöglichkeiten ist sie sich nicht sicher, welche die beste Wahl ist. Zum Glück hat sie schon ein wenig über Bitcoin und das Lightning-Netzwerk gelernt. Nach dem Abwägen ihrer Optionen erkennt Mina, dass eine Lightning-Zahlung die beste Möglichkeit ist.

Mina möchte einen Kaffee kaufen, aber das Bezahlen mit einer regulären Bitcoin-Transaktion kann manchmal dauern und höhere Gebühren erfordern. Deshalb entscheidet sie sich, das Lightning-Netzwerk zu nutzen.

Das Lightning-Netzwerk ermöglicht es Menschen, Bitcoin sofort und mit sehr niedrigen Gebühren zu senden. Das macht es ideal für kleine, alltägliche Einkäufe wie Kaffee.

Um Lightning zu nutzen, lädt Mina eine Lightning-Wallet auf ihr Handy herunter. Dann sendet sie etwas Bitcoin von ihrer regulären Bitcoin-Wallet an ihre Lightning-Wallet. Dieser Schritt nutzt eine normale Bitcoin-Transaktion auf der Blockchain. Sobald die Gelder in ihrer Lightning-Wallet sind, können sie im Lightning-Netzwerk verwendet werden.

Jetzt kann Mina das Café sofort mit Lightning bezahlen. Die Zahlung findet außerhalb der Haupt-Bitcoin-Blockchain statt, weshalb sie viel schneller und günstiger ist als eine reguläre On-Chain-Transaktion.


| Vorteile | Lightning-Netzwerk | Traditionelles Bankensystem |
| --- | --- | --- |
| Geschwindigkeit | Schnell | Langsam |
| Transparenz | Transparent | Intransparent |
| Sicherheit | Sicher | Verwundbar |
| Transaktionsgebühren | Niedrig | Hoch |
| Finanzielle Inklusion | Hoch | Begrenzt |
| Skalierbarkeit | Hoch | Niedrig |
| Privatsphäre | Hoch | Mittel |
| Interoperabilität | Hoch | Niedrig |
| Rechtliche Konformität | Mittel | Hoch |
| Kosteneffizienz | Hoch | Mittel |


On-Chain-Transaktionen finden direkt auf der Bitcoin-Blockchain statt und können mehr Zeit und Gebühren erfordern. Lightning-Transaktionen erfolgen außerhalb der Blockchain und ermöglichen schnelle und kostengünstige Zahlungen, während weiterhin bitcoin verwendet wird.


| Visa, Inc. | Bitcoin On-Chain | Lightning-Netzwerk |
| --- | --- | --- |
| Kapazität von 65.000 Transaktionen pro Sekunde. | Kapazität von 7 Transaktionen pro Sekunde. | Kapazität von Millionen Transaktionen pro Sekunde. |


![Lightning Network Map](https://cdn.sanity.io/images/vje9ehw2/staging/5a760247cf4c32074c62f40aea8dc21095882740-504x245.svg)


https://mempool.space/graphs/lightning/nodes-channels-map

_Mempool.space Nodes Channels Map_


Dies ist eine Karte des gesamten Lightning-Netzwerks. Dank tausender Lightning-Node-Betreiber kannst du Sats an jeden Nutzer mit einer Bitcoin-Lightning-Wallet senden, egal wo auf der Welt er sich befindet. Die Zahlung kommt in wenigen Sekunden an und kostet nur ein paar Cent.**Probier es selbst aus!**

#### Aktivität: Lightning-Staffellauf


https://qr.myfirstbitcoin.org/lightning.pdf

_Activity: Lightning_


**Dies ist eine praktische Übung, bei der die Teilnehmenden echte Sats über das Lightning-Netzwerk senden und empfangen.**

###### Wichtige Punkte

1. Die Nutzung einer Lightning-Wallet stärkt dein Vertrauen darin, echte Sats zu empfangen und zu senden.
1. Achte auf die Einheiten. Manche Wallets erlauben es, entweder bitcoin ODER Sats (1/100.000.000 eines bitcoin) zu senden.
1. Lightning-Zahlungen können manchmal beim Routing hängen bleiben, besonders bei größeren Beträgen. Obwohl das möglich ist, wird diese Art von Nutzererfahrung seltener, je weiter das Netzwerk reift.

###### Tipp für Teilnehmende

Frag deine Lehrkraft, ob und wie die aktuellen On-Chain-Bitcoin-Transaktionsgebühren die von dir verwendete Lightning-Wallet beeinflussen.
