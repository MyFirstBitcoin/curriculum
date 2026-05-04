# 3.7 Bitcoin

Nach vielen Jahren und gescheiterten Versuchen hatten die Cypherpunks größtenteils das Interesse an der Idee einer digitalen, erlaubnisfreien Währung verloren, als Adam Back eine E-Mail mit einem Link zu einem Entwurf eines Whitepapers namens „electronic cash without a third party“ von einer anonymen Person erhielt, die sich Satoshi Nakamoto nannte.

Um an diesem Punkt zusammenzufassen, haben wir zumindest die folgenden Ideen:

* Kryptografische Signaturen, die ein gewisses Maß an Privatsphäre und Anonymität bieten könnten
* Konzept einer nicht gedeckten Währung (B-Money)
* Vorschläge (aber keine Mittel) zur Begrenzung der Ausgabe neuer Währung
* Digitale Münzen, deren Eigentum durch öffentliche Schlüssel zugeordnet wurde (B-Money) und die durch Signieren übertragen und basierend auf der Empfängeradresse neu zugewiesen werden konnten (RPOW und Hashcash)
* Alle Knoten halten eine Kopie eines vollständig verteilten Ledgers (B-Money) (damals als unpraktisch abgetan)
* Zeitstempelprotokoll – Verwendung von Merkle-Baum-Hashing, um eine mathematisch nachweisbare Chronologie von Ereignissen zu liefern, die schwer zu fälschen ist, wenn alle Nutzer die gleichen Aufzeichnungen führen
* Proof of Work, um realen Aufwand mit dem System zu verknüpfen (aber der Hash selbst wurde als Währung verwendet)
* Vollständig dezentralisierte Netzwerke, in denen alle Peers gleichberechtigt sind und das Netzwerk jederzeit betreten oder verlassen können (BitTorrent)
* Konzept, neue Hashes mit vorherigen Hashes zu verknüpfen (Bit Gold und Zeitstempel)

Was zu diesem Zeitpunkt fehlte, war unter anderem:

* Eine praktikable Lösung für das ‚Byzantinische Generäle‘-Problem
* Eine Methode, um die Geldmenge trotz kontinuierlicher Hardware-Verbesserungen zu begrenzen
* Anreizsystem, damit Menschen teilnehmen (Henne-Ei-Problem)

Der andere große Unterschied zwischen den jüngsten Versuchen und Bitcoin war, dass Satoshi bereits seit einiger Zeit am Code arbeitete – ganz im ursprünglichen Ethos „Cypherpunks schreiben Code“ – bevor er ihn auf den Mailinglisten ankündigte, im Gegensatz zu Bit Gold und B-Money, die eher konzeptionell waren.

Was war die Innovation, die Bitcoin von früheren Versuchen mit elektronischem Geld unterschied?

Proof of Work sollte als Konsensmechanismus und als Mittel zur Bereitstellung von Sicherheit und Unveränderlichkeit dienen: Anstatt den Hash als Geldform zu verwenden, sollte er durch einen neuen konzeptionellen Prozess namens Mining genutzt werden, bei dem ein Knoten eine Reihe von Transaktionen bündelt, eine Zufallszahl hinzufügt und dann das Hashing auf den „Block“ von Daten anwendet. Ein gültiger Block, der die Hash-Anforderung erfüllt, würde dann im Netzwerk bekannt gemacht. Diese Blöcke würden miteinander verbunden, indem jeweils der Hash des vorherigen Blocks verwendet wird, und die längste Blockchain würde im Falle eines Gleichstands verwendet, wenn verschiedene Knoten gleichzeitig unterschiedliche Blöcke validieren und bekannt machen, was zu Kettenaufspaltungen führt. Proof of Work wurde zum verteilten Entscheidungsmechanismus, um das Problem der byzantinischen Generäle zu lösen.

Diese Miner erhielten außerdem einen Anreiz, die für den Proof of Work erforderliche Rechenleistung bereitzustellen, indem ihnen für jeden Block neue Bitcoin zugeteilt wurden. Die Menge an Bitcoin, die sie erhalten, ist ebenfalls so programmiert, dass sie etwa alle 4 Jahre sinkt, bis alle Bitcoin erschaffen wurden, wodurch ein festes Limit für die Gesamtmenge an Bitcoin, die jemals im Umlauf sein wird, von 21 Millionen entsteht.

Die originellste Idee war die Art und Weise, wie er das Problem löste, wie viel Geld geschaffen wird, wenn sich die Hardware verbessert und mehr Rechenleistung auf das Netzwerk angewendet werden kann. Die Zeitstempel einer bestimmten Anzahl von Blöcken (2016) würden gemittelt, und wenn sie zu schnell erzeugt werden, würde der für einen neuen Block erforderliche Hash schwieriger gemacht, wenn zu langsam, würde er erleichtert. Dies war im dezentralen Protokoll eingebaut, das alle Knoten ausführen, sodass jeder Miner, der dies ignoriert, Energie aufwenden würde, um einen Block ohne Nutzen zu minen, da dieser vom Rest des Netzwerks abgelehnt würde. Diese Anpassung stellt sicher, dass die Erzeugung neuer Blöcke im geplanten Ausgabeschema bleibt und schafft Anreize für Miner, sich an die Regeln zu halten.

####   
Zusammenfassung

Viele der Puzzleteile, die nötig sind, um ein dezentrales Peer-to-Peer-E-Cash-System auf Basis solider Geldprinzipien zu bauen, waren bereits vorhanden, bevor Satoshi sein Whitepaper veröffentlichte und kurz darauf den ersten Code freigab.

> Die Natur von Bitcoin ist so beschaffen, dass mit der Veröffentlichung von Version 0.1 das Kerndesign für den Rest seiner Lebensdauer in Stein gemeißelt war  
_Satoshi Nakamoto_

Obwohl viele Ideen für Verbesserungen (BIPs) vorgeschlagen und übernommen wurden, arbeitet Bitcoin seit 2009 im Hintergrund nach dem im ursprünglichen Release festgelegten Protokoll und mit kaum nennenswerten Unterbrechungen. Alle Verbesserungen wurden so vorgenommen, dass die Rückwärtskompatibilität mit allen vorherigen Versionen erhalten blieb.



##### Anmerkungen

1. Für eine Erklärung des Problems der byzantinischen Generäle siehe [https://de.wikipedia.org/wiki/Byzantinischer_Fehler](https://en.wikipedia.org/wiki/Byzantine_fault)
