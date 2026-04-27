# 9.1 Bitcoin-Knoten und Miner

Bitcoin-Nodes mögen technisch klingen, aber sie sind einfach Software, die eine Kopie der Bitcoin-Blockchain auf einem Computer speichert. Die Blockchain ist ein gemeinsames Register aller Bitcoin-Transaktionen.

Wenn du deinen eigenen Node betreibst, überprüfst du Bitcoin-Transaktionen selbst, anstatt jemand anderem zu vertrauen. Das gibt dir mehr Unabhängigkeit und hilft, das Bitcoin-Netzwerk dezentral zu halten.

Du kannst dir einen Bitcoin-Node wie einen digitalen Verkehrspolizisten vorstellen, der einige wichtige Aufgaben hat.

1. Er bewahrt eine Kopie der Blockchain auf, also die Historie aller Bitcoin-Transaktionen.
1. Nodes verbinden sich mit anderen Nodes auf der ganzen Welt und tauschen Informationen aus. Ein Beispiel ist die Liste neuer Transaktionen, die auf Bestätigung warten, der sogenannte Mempool.
1. Nodes prüfen, ob jede Transaktion den Bitcoin-Regeln entspricht. Ist eine Transaktion ungültig, lehnt der Node sie ab.

Nodes helfen auch neuen Nodes, dem Netzwerk beizutreten, indem sie ihnen die Blockchain zur Verfügung stellen. Dennoch prüft jeder neue Node alle Regeln unabhängig.

Jeder kann einen Node betreiben, indem er Software wie Bitcoin Core installiert und die Blockchain herunterlädt. Sobald alles eingerichtet ist, empfängt der Node etwa alle 10 Minuten neue Blöcke und überprüft sie, bevor er sie seiner Kopie der Blockchain hinzufügt.

Das Betreiben eines Nodes macht das Bitcoin-Netzwerk sicherer und dezentraler, weil mehr Menschen das System unabhängig überprüfen.

#### Was ist ein Bitcoin-Node?

> Der Zweck des Minings ist nicht die Erschaffung neuer Bitcoin; das ist das Anreizsystem. Mining ist der Mechanismus, durch den die Sicherheit von Bitcoin dezentralisiert wird.  
_Andreas M. Antonopoulos_


> **Callout**
>
> Miner sammeln unbestätigte Transaktionen, bilden daraus einen Block und nutzen Energie, um einen Schlüssel zu finden, der den Block hinzufügt und sichert.


Miner konkurrieren darum, den nächsten Block mit Transaktionen zur Blockchain hinzuzufügen. Dafür müssen sie eine spezielle Zahl finden, die einen gültigen Block-Hash erzeugt. Du kannst es dir vorstellen wie die Suche nach dem richtigen Schlüssel unter Milliarden von Möglichkeiten. Der erste Miner, der den korrekten Hash findet, gewinnt das Rennen und erhält das Recht, seinen Block zur Blockchain hinzuzufügen.

Wenn ein Miner einen gültigen Hash findet, teilt er seinen Block dem Netzwerk mit. Andere Miner überprüfen schnell, ob die Lösung korrekt ist. Ist das der Fall, wird der Block zur Blockchain hinzugefügt und trägt zur Sicherheit des öffentlichen Bitcoin-Kontos bei.

Miner verdienen Bitcoin auf zwei Arten:

* **Blockbelohnungen:** Neue Bitcoin werden erschaffen und dem Miner gegeben, der erfolgreich einen Block zur Blockchain hinzufügt.
* **Transaktionsgebühren:** Wenn Menschen Bitcoin versenden, fügen sie eine kleine Gebühr hinzu. Der Miner, der den Block hinzufügt, erhält die Gebühren der in diesem Block enthaltenen Transaktionen.

#### Bitcoin-Halvings


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12,5 BTC | 6,25 BTC | 3,125 BTC |



> **Callout**
>
> Die Belohnung der Miner für das Abschließen eines Blocks halbiert sich alle 210.000 Blöcke, also etwa alle vier Jahre.


Bitcoin hat eine feste maximale Menge von 21.000.000 Bitcoin, aber sie wurden nicht alle erschaffen, als Bitcoin gestartet ist. Stattdessen werden neue Bitcoin nach und nach durch **Mining** in Umlauf gebracht.

Wenn Miner erfolgreich einen neuen Block mit Transaktionen zum Bitcoin-Netzwerk hinzufügen, erhalten sie eine **Blockbelohnung** in Bitcoin. In den Anfangstagen von Bitcoin betrug diese Belohnung 50 Bitcoin pro Block. Diese Belohnung motivierte Menschen, Rechenleistung und Strom zu nutzen, um das Netzwerk zu sichern.

Etwa alle 210.000 Blöcke (ungefähr alle 4 Jahre) wird die Blockbelohnung halbiert. Dieses Ereignis nennt man das **Halving**. Das Halving verlangsamt die Erzeugung neuer Bitcoin und sorgt dafür, dass die Gesamtmenge nie 21 Millionen überschreitet. Mit der Zeit macht das Bitcoin immer knapper.


> **Definition – Umlaufmenge**
>
> **Umlaufmenge** bezeichnet die insgesamt verfügbare Menge einer Währung. Bei Bitcoin ist die gesamte Umlaufmenge die Anzahl der Münzen, die bereits gemined wurden und sich zu einem bestimmten Zeitpunkt im Umlauf befinden.


![ Bitcoin Supply Schedule](https://cdn.sanity.io/images/vje9ehw2/staging/86534a1a581b46dfb9493f9a293874bfd6071cdb-292x200.svg)


> **Definition – Bitcoin-Ausgabeplan**
>
> Der **Bitcoin-Ausgabeplan** ist der vorab festgelegte und öffentliche Plan für die Freigabe neuer Bitcoin in den Umlauf, der darauf ausgelegt ist, die Knappheit von Bitcoin im Laufe der Zeit zu erhalten.


Nach jedem Halving-Ereignis wird die Bitcoin-Belohnung, die Miner für das Hinzufügen eines Blocks erhalten, halbiert. Dadurch verringert sich die Geschwindigkeit, mit der neue Bitcoin erschaffen werden.

Miner verdienen weiterhin Transaktionsgebühren aus den Transaktionen, die im von ihnen geminten Block enthalten sind. Mit der Zeit wird erwartet, dass diese Gebühren einen größeren Teil des Einkommens der Miner ausmachen.

Halvings sind im Bitcoin-Protokoll fest verankert und erfolgen automatisch etwa alle vier Jahre. Dadurch ist der Ausgabefahrplan von Bitcoin vorhersehbar und transparent.

Die Tabelle zeigt die kommenden Halvings, einschließlich des ungefähren Datums, der Blocknummer, zu der sie stattfinden, der neuen Blockbelohnung und des Prozentsatzes der insgesamt bereits geminten Bitcoin.


| Ereignis | Datum | Block | Belohnung | Gemint |
| --- | --- | --- | --- | --- |
| 5. Halving | 2028 | 1.050.000 | 1,5625 BTC | 98,44 % |
| 6. Halving | 2032 | 1.260.000 | 0,78125 BTC | 99,22 % |
| 7. Halving | 2036 | 1.470.000 | 0,390625 BTC | 99,61 % |


Je mehr Bitcoin gemint werden, desto mehr steigt der Umlaufbestand, bis das maximale Angebot von 21.000.000 Bitcoin erreicht ist, was voraussichtlich um das Jahr 2140 geschieht. Da im Laufe der Zeit immer weniger neue Bitcoin geschaffen werden, kann der Preis von Bitcoin steigen, wenn die Nachfrage zunimmt. Das motiviert auch die Miner, das Netzwerk weiterhin durch ihre Rechenleistung zu sichern.

#### Was ist ein gültiger Block-Hash bei Bitcoin?

Bei Bitcoin konkurrieren Miner darum, einen speziellen Code zu finden, der **Block-Hash** genannt wird. Dieser Code identifiziert einen Block mit Transaktionen und ermöglicht es, ihn zur Blockchain hinzuzufügen.

Jeder Block enthält Informationen über aktuelle Transaktionen und auch den Hash des vorherigen Blocks. Dadurch werden alle Blöcke miteinander verbunden und bilden eine Kette vom allerersten Block (dem Genesis Block) bis zum neuesten.

Ein Hash funktioniert wie ein **digitaler Fingerabdruck** für die Daten im Block. Wenn sich irgendwelche Informationen im Block ändern würden, würde sich auch der Fingerabdruck ändern. So kann jeder leicht überprüfen, dass die Transaktionshistorie der Blockchain nicht verändert wurde, und das Netzwerk bleibt sicher.


> **Callout**
>
> Satoshi Nakamoto, der Erfinder von Bitcoin, hat den Genesis Block gemint, wodurch insgesamt 50 Bitcoin freigeschaltet wurden.


#### Das Rennen um das Mining eines Blocks

Miner konkurrieren darum, einen gültigen Block-Hash zu finden. Der erste Miner, dem das gelingt, darf den neuen Block zur Blockchain hinzufügen und erhält eine Bitcoin-Belohnung.

Um gültig zu sein, muss der Hash des Blocks niedriger sein als eine vom Netzwerk festgelegte Zahl, die als Schwierigkeitsziel bezeichnet wird. Da Hashes zufällig sind, müssen Miner immer wieder verschiedene Eingaben ausprobieren, bis sie eine passende finden.

Wenn zu viele Miner konkurrieren, würden Blöcke zu schnell gefunden werden. Wenn zu wenige teilnehmen, würde es zu lange dauern, einen Block zu finden. Um das System stabil zu halten, passt Bitcoin die Schwierigkeit automatisch alle 2.016 Blöcke (etwa alle zwei Wochen) an.

Diese Anpassung stellt sicher, dass im Durchschnitt etwa alle 10 Minuten ein neuer Block zur Blockchain hinzugefügt wird.


> **Definition – Definition des Schwierigkeitsgrads**
>
> Der **Schwierigkeitsgrad** beim Bitcoin-Mining misst, wie schwer es ist, einen gültigen Block-Hash zu finden. Das Netzwerk passt diese Schwierigkeit alle 2.016 Blöcke (etwa alle zwei Wochen) an, sodass neue Blöcke etwa alle 10 Minuten zur Blockchain hinzugefügt werden. Je höher die Schwierigkeit, desto schwerer ist es für Miner, einen gültigen Block zu finden.


Indem ein Miner einen gültigen Block-Hash findet, beweist er, dass er die nötige Arbeit geleistet hat, um einen neuen Block zur Blockchain hinzuzufügen. Dieser Prozess wird **Proof of Work** (PoW) genannt. Es ist der Sicherheitsmechanismus, der es Bitcoin ermöglicht, Transaktionen zu bestätigen und neue Blöcke zur Blockchain hinzuzufügen. Der Miner, der den gültigen Hash zuerst findet, erhält eine Belohnung in Bitcoin, die sowohl die Blockbelohnung als auch die Transaktionsgebühren der im Block enthaltenen Transaktionen umfasst.

Proof of Work (PoW) trägt dazu bei, Bitcoin sicher zu halten, indem es extrem teuer wird, das Netzwerk zu betrügen oder zu übernehmen. Es ist stattdessen viel profitabler, sich an die Regeln zu halten.

Miner übernehmen vier Hauptaufgaben:

1. **Transaktionen sammeln**: Miner wählen Transaktionen aus, die an das Netzwerk gesendet wurden, und fügen sie in einen Kandidatenblock ein.
1. **Proof of Work durchführen**: Miner konkurrieren darum, ein schwieriges mathematisches Rätsel zu lösen, indem sie einen gültigen Block-Hash finden.
1. **Den Block übertragen**: Der erste Miner, der eine gültige Lösung findet, teilt den neuen Block mit dem Netzwerk.
1. **Belohnungen verdienen**: Wenn der Block gültig ist, wird er zur Blockchain hinzugefügt und der Miner erhält neu erzeugte Bitcoin sowie Transaktionsgebühren.

Viele Miner auf der ganzen Welt versuchen gleichzeitig, den nächsten Block zu erstellen. Wenn ein Miner eine gültige Lösung findet, überprüft das Netzwerk den Block. Wenn alles korrekt ist, wird er zur Blockchain hinzugefügt. Andere konkurrierende Blöcke werden verworfen. Dieser Prozess hält das Netzwerk im Konsens und verhindert doppelte Ausgaben.

* Miner sind Computer, die helfen, das Kassenbuch von Bitcoin zu pflegen und zu aktualisieren.
* Sie sammeln Transaktionen und fassen sie zu einem Block zusammen. Dann lassen sie die Blockdaten durch einen Hash-Algorithmus laufen, um einen einzigartigen Code zu erzeugen, der Hash genannt wird.
* Miner wiederholen diesen Vorgang viele Male und suchen nach einem Hash, der den Regeln von Bitcoin entspricht. Der erste Miner, der einen gültigen Hash findet, erhält neu erzeugte Bitcoin als Belohnung und sein Block wird zur Blockchain hinzugefügt.
* Der Hash jedes Blocks verbindet ihn außerdem mit dem vorherigen Block. Wenn jemand versuchen würde, eine vergangene Transaktion zu ändern, würden die Hashes nicht mehr übereinstimmen und das Netzwerk würde die veränderte Kette ablehnen. Das ist es, was das Kassenbuch von Bitcoin sicher macht.
