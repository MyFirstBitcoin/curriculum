# 7.4 Senden und Empfangen von Lightning-Transaktionen

Mit einer Lightning-Wallet ist die Nutzung von Bitcoin schnell, günstig und privat, wodurch Transaktionen zwischen zwei Personen einfach werden. Du kannst Bitcoin schnell senden und empfangen – zum Beispiel für alltägliche Dinge wie den Kauf eines Kaffees.

Schauen wir uns einige Beispiele an, wie das Lightning-Netzwerk in der Praxis funktioniert.

###### Beispiel 1

Sowohl Marcia als auch Eve besitzen 5 Einheiten der Währung. Marcia möchte 2 Einheiten an Eve senden. Die Zahlung läuft über Jeff, der hilft, die Zahlung durch das Lightning-Netzwerk weiterzuleiten. Nach Abschluss der Zahlung hat Eve 7 Einheiten und Marcia 3.

Jeff hilft dabei, die Zahlung zu routen, aber er kann die Gelder nicht stehlen. Das Lightning-Netzwerk verwendet Kryptografie, um sicherzustellen, dass nur der vorgesehene Empfänger die Zahlung erhalten kann. Jeff hilft lediglich, die Zahlung durch das Netzwerk zu leiten.

Dies zeigt einen entscheidenden Vorteil des Lightning-Netzwerks: Menschen können Zahlungen schnell senden, ohne Mittelsleuten wie Banken vertrauen zu müssen.

Knotenbetreiber wie Jeff können auch kleine Gebühren dafür verdienen, dass sie Zahlungen weiterleiten. Dadurch helfen sie, das Netzwerk dezentral und effizient zu halten.

Im Vergleich zu regulären Bitcoin-Transaktionen:

* **On-Chain-Transaktionen** finden direkt auf der Bitcoin-Blockchain statt. Sie sind sehr sicher, können aber langsamer und teurer sein.
* **Lightning-Transaktionen** finden außerhalb der Blockchain (off-chain) statt und ermöglichen es, Zahlungen viel schneller und zu deutlich geringeren Kosten abzuwickeln.

Deshalb eignet sich Lightning besonders für kleine, alltägliche Zahlungen, während On-Chain-Transaktionen oft für größere Überweisungen oder langfristige Aufbewahrung genutzt werden.

###### Beispiel 2

Mina geht gerne essen und besucht oft ihr Lieblingscafé. Bei so vielen verschiedenen Zahlungsmöglichkeiten ist sie sich nicht sicher, welche die beste Wahl ist. Zum Glück hat sie schon etwas über Bitcoin und das Lightning-Netzwerk gelernt. Nach dem Abwägen ihrer Optionen erkennt Mina, dass eine Lightning-Zahlung die beste Möglichkeit ist.

Mina möchte einen Kaffee kaufen, aber das Bezahlen mit einer regulären Bitcoin-Transaktion kann manchmal dauern und höhere Gebühren erfordern. Deshalb entscheidet sie sich, das Lightning-Netzwerk zu nutzen.

Das Lightning-Netzwerk ermöglicht es, Bitcoin sofort und mit sehr niedrigen Gebühren zu senden. Das macht es ideal für kleine, alltägliche Einkäufe wie Kaffee.

Um Lightning zu nutzen, lädt Mina eine Lightning-Wallet auf ihr Handy. Dann sendet sie etwas Bitcoin von ihrer regulären Bitcoin-Wallet an ihre Lightning-Wallet. Dieser Schritt erfolgt über eine normale Bitcoin-Transaktion auf der Blockchain. Sobald die Gelder in ihrer Lightning-Wallet sind, kann sie sie im Lightning-Netzwerk verwenden.

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


On-Chain-Transaktionen finden direkt auf der Bitcoin-Blockchain statt und können mehr Zeit und Gebühren in Anspruch nehmen. Lightning-Transaktionen erfolgen Off-Chain und ermöglichen schnelle und kostengünstige Zahlungen, während weiterhin Bitcoin verwendet wird.


| Visa, Inc. | Bitcoin On-Chain | Lightning-Netzwerk |
| --- | --- | --- |
| Kapazität von 65.000 Transaktionen pro Sekunde. | Kapazität von 7 Transaktionen pro Sekunde. | Kapazität von Millionen Transaktionen pro Sekunde. |


![Lightning Network Map](https://cdn.sanity.io/images/vje9ehw2/staging/5a760247cf4c32074c62f40aea8dc21095882740-504x245.svg)

https://mempool.space/graphs/lightning/nodes-channels-map

Dies ist eine Karte des gesamten Lightning-Netzwerks. Dank Tausender Lightning-Node-Betreiber kannst du Sats an jeden Nutzer mit einer Bitcoin-Lightning-Wallet senden, egal wo auf der Welt er sich befindet. Die Zahlung kommt in wenigen Sekunden an und kostet nur ein paar Cent.**Probier es selbst aus!**

#### Aktivität: Lightning-Staffellauf

https://qr.myfirstbitcoin.org/lightning.pdf

**Dies ist eine praktische Übung, bei der die Schüler echte Sats über das Lightning-Netzwerk senden und empfangen.**

###### Wichtige Punkte

1. Die Nutzung einer Lightning-Wallet stärkt dein Selbstvertrauen beim Empfangen und Senden echter Sats.
1. Achte auf die Einheiten. Manche Wallets erlauben es, entweder Bitcoin ODER Sats (1/100.000.000 eines Bitcoins) zu senden.
1. Lightning-Zahlungen können manchmal beim Routing hängen bleiben, besonders bei größeren Beträgen. Obwohl dies möglich ist, wird diese Art von Nutzererfahrung immer seltener, da das Netzwerk reift.

###### Tipp für Schüler

Frage deinen Lehrer, ob und wie aktuelle On-Chain-Bitcoin-Transaktionsgebühren die von dir verwendete Lightning-Wallet beeinflussen.
