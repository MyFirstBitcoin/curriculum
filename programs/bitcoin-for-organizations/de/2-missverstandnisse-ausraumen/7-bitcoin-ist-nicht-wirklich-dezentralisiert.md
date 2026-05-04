# 2.7 Bitcoin ist nicht wirklich dezentralisiert.

> Die Komplexität von Krypto entsteht durch den Versuch der Dezentralisierung – indem Macht und Verwaltung im System verteilt werden, besteht theoretisch keine Notwendigkeit für vertrauenswürdige Vermittler wie Finanzinstitute. Das war die Prämisse des ursprünglichen Bitcoin-Whitepapers, das eine kryptografische Lösung bot, um Zahlungen ohne die Beteiligung eines Finanzinstituts oder eines anderen vertrauenswürdigen Vermittlers zu ermöglichen. Allerdings wurde Bitcoin sehr schnell zentralisiert und ist heute auf eine kleine Gruppe von Softwareentwicklern und Mining-Pools angewiesen, um zu funktionieren.  
_Internationaler Währungsfonds_

Wie das obige Zitat aus einem relativ aktuellen Beitrag des Internationalen Währungsfonds zeigt, behauptet die Mainstream-Finanzindustrie weiterhin, dass Bitcoin nicht dezentralisiert sei, und verwechselt Bitcoin zudem mit anderen Krypto-Assets.

##### Einleitung

![Trilemma](https://cdn.sanity.io/images/vje9ehw2/staging/5337a11afce96171214ca02dcbb743cccbff5fa4-161x167.svg)

Dezentralisierung ist ein entscheidender Aspekt von Bitcoin. Die Fähigkeit, die Regeln des Protokolls wie Knappheit und Verteilung ohne zentrale Autorität aufrechtzuerhalten, stellt sicher, dass es als erlaubnisfreies Geld für eine globale Gesellschaft dienen kann.

Wie Satoshi in seiner Online-Korrespondenz feststellte, konnten sich dezentralisierte Dienste wie BitTorrent gegen staatliche Eingriffe behaupten, im Vergleich zu Diensten mit identifizierten Eigentümern und zentralisierten Servern. Er war offensichtlich besorgt über das potenzielle Risiko, dass Regierungen oder andere Interessen Bitcoin abschalten oder anderweitig negativ beeinflussen könnten.

In diesem Zusammenhang interessieren wir uns für die Dezentralisierung von:

* Die Entwicklung und Verwaltung des Codes, der das Protokoll ausführt; wer darf die Regeln ändern?
* Die Mining-Funktion, die neue Blöcke gemäß den Regeln erstellt und gegen Double-Spending validiert
* Die Nodes, die Transaktionen auf Gültigkeit prüfen und eine Kopie der Blockchain speichern

##### Entwickler

Bitcoin ist ein Open-Source-Protokoll, das jeder einsehen, herunterladen, kopieren oder Änderungsvorschläge machen kann. Es ist in einer GitHub-Bibliothek verfügbar, der Quellcode wurde ursprünglich 2009 von Satoshi Nakamoto veröffentlicht. Jeder kann den Code herunterladen und einen Node betreiben, wobei die Mehrheit die originale Bitcoin-Core-Software verwendet, die im Laufe der Zeit aktualisiert wurde.

![How Does an idea Make Its Way Into Bitcoin Core?](https://cdn.sanity.io/images/vje9ehw2/staging/49f70d059c9dbe19a6e4500e9abd8db66ca97bff-1300x1439.png)

_Quelle: https://river.com/learn/what-is-bitcoin-core/_

Die Entwicklung von Bitcoin Core folgt den Best Practices der Open-Source-Entwicklung. Zu jeder Zeit kann es eine beliebige Anzahl von Entwicklern geben, die Codeänderungen schreiben oder überprüfen. Sie müssen auf die Anliegen der Node-Betreiber und Miner sowie der Nutzerbasis hören, bevor sie eine kritische Änderung am Code vornehmen, die wie im obigen Flussdiagramm überprüft und vereinbart wird, bevor sie in den Code aufgenommen wird.

Die Regeln von Bitcoin sind dann in dieser Bitcoin-Core-Software kodiert, die auf jedem Node läuft. Jeder kann eine Änderung der Regeln vorschlagen – die Regeln sind Code, aber sie sind nicht _nur_ Code, sie sind _vereinbarter_ Code. Wenn sie einseitig geändert werden, ist der neue Code nicht mehr Teil des Konsenses und gehört nicht mehr zu Bitcoin. Etwas an Bitcoin zu ändern und im Konsens zu bleiben, ist schwierig. Vorgeschlagene Änderungen am Code fallen in eine von drei Kategorien:

* Innerhalb der bestehenden Regeln: Kleine Verbesserungen wie Rechtschreibfehler, eine schönere Benutzeroberfläche oder Datenverwaltung können in diese Kategorie fallen und sind relativ einfach zu genehmigen.
* Hinzufügen einer neuen Regel, die die bestehenden Regeln einschränkt – zum Beispiel die Verringerung der Blockgröße. Dies wird als 'Soft Fork' bezeichnet. Nodes, die die Codeänderung nicht implementieren und bei der alten Version bleiben, können weiterhin am Netzwerk teilnehmen.
* Hinzufügen einer neuen Regel, die die aktuellen Regeln bricht, z. B. eine Erhöhung der Blockgröße. Nodes, die nicht auf den neuen Code aktualisieren, werden einen Block mit größerer Größe als ungültig ablehnen. Dies wird als 'Hard Fork' bezeichnet und führt zu einer Aufspaltung der Kette zwischen den Nodes, die den ursprünglichen und den neuen Code ausführen, und erschafft eine neue Coin. Dies ist bereits vorgekommen, hat aber langfristig keinen Erfolg für die neue Coin gebracht, da die Mehrheit der Nodes beim ursprünglichen Code geblieben ist.

Daher kann eine einzelne Partei oder Gruppe von Personen den Bitcoin-Code nicht einseitig ändern, ohne einen Konsens zu erzielen, andernfalls riskieren sie eine Kettenspaltung und die Entstehung einer neuen Coin mit einem anderen Regelwerk.

##### Mining

Die Mining-Funktion validiert die Transaktionen wie jeder andere Node im Netzwerk, verbraucht dann aber die Energie, die erforderlich ist, um einen neuen Block zu erstellen, der den Konsensregeln im Code entspricht. Der Erfolg ermöglicht es dem Miner, die Belohnungen in Form von Transaktionsgebühren und Bitcoin-Belohnungen zu erhalten (zum Zeitpunkt des Schreibens 3,125 Coins pro Block).

Mining wird normalerweise von Mining-Pools durchgeführt, bei denen Menschen ihre Rechenleistung oder Hashrate bündeln, um die Chancen auf das erfolgreiche Minen eines Blocks zu erhöhen und die Belohnungen zu teilen. Es besteht die Gefahr, dass einer oder mehrere dieser Mining-Pools zusammenarbeiten könnten, um eine 51%-Dominanz im Mining zu erreichen und im Wesentlichen das Netzwerkvalidierungsprotokoll zu ihren Gunsten außer Kraft zu setzen, um Coins doppelt auszugeben. Dies würde jedoch enorme Ressourcen erfordern und wäre mit hohen Kosten verbunden, und einzelne Miner können jederzeit sehr einfach zu einem anderen Mining-Pool wechseln. Ein solcher Angriff würde wahrscheinlich auch den Wert von Bitcoin zum Einsturz bringen, da offensichtlich wäre, dass die Integrität des Netzwerks kompromittiert wurde. Ein Angreifer müsste daher jegliche erlangten Bitcoins schnell in Fiat umtauschen, bevor der Wert verfällt. Das würde es noch schwieriger machen, einen Angriff über einen längeren Zeitraum aufrechtzuerhalten, und macht es daher für einen Miner oder Pool-Betreiber profitabler, sich an die Regeln zu halten und zu versuchen, gültige Blöcke zu minen.

Auch die geografische Verteilung der Mining-Funktion ist wichtig, um beispielsweise zu verhindern, dass Regierungen die Mining-Kapazität übernehmen oder abschalten. Ein aktuelles Beispiel ist das Mining-Verbot in China, das gezeigt hat, dass Bitcoin in der Lage ist, sich an solche staatlichen Eingriffe anzupassen und sich schnell von dem daraus resultierenden Verlust an Hashrate zu erholen.

##### Nodes

Im Gegensatz zum Mining, das eine erhebliche finanzielle Investition erfordert, um im Rennen um neue Blöcke effektiv konkurrieren zu können, oder der Code-Entwicklung, die Programmierkenntnisse voraussetzt, ist das Betreiben eines Nodes etwas, das jeder, der zur Dezentralisierung von Bitcoin beitragen möchte, tun kann.

Nodes führen die Bitcoin-Core-Software aus und setzen die Regeln durch, die im Code enthalten sind, um sicherzustellen, dass die Miner nicht betrügen, zum Beispiel indem sie sich selbst eine höhere Blockbelohnung zuweisen, als erlaubt ist. Sie setzen auch das 21-Millionen-Limit durch, das entscheidend ist, um die Knappheit von Bitcoin zu erhalten. Um Bitcoin zu stoppen, müsste eine Regierung oder ein böswilliger Akteur jede einzelne Kopie der Blockchain zerstören, die derzeit auf Tausenden von weltweit verteilten Nodes läuft – eine nahezu unmögliche Aufgabe.

##### Menschen

Ein weiterer Aspekt potenzieller Zentralisierung sind Menschen. Jede andere 'Altcoin' hat eine Leitfigur – jemanden, der möglicherweise dazu gezwungen werden könnte, Änderungen zu befürworten, die nicht im besten Interesse von Bitcoin sind. Satoshi Nakamoto blieb lange genug, um sicherzustellen, dass Bitcoin auf Erfolgskurs war, bevor er endgültig verschwand und es anderen überließ, die Software weiterzuentwickeln und anzupassen.

Was ist mit Inhabern großer Mengen an Bitcoin? Frühe Investoren, die ihre Coins gehalten und nicht verloren haben, sind inzwischen extrem wohlhabend. Es ist wichtig zu beachten, dass dies durchaus der Fall sein kann, ihnen aber nicht mehr Einfluss auf das System gibt als jedem anderen – im Gegensatz zu 'Proof-of-Stake'-Coins, bei denen die frühen Anwender, die bereits wohlhabend in dieser Coin sind, Vorteile bei der Entscheidungsfindung und der Verteilung zukünftiger Coins erhalten. Dies hat oder wird zwangsläufig im Laufe der Zeit zur Zentralisierung führen.

##### Fazit

Welche potenziellen Bedrohungen kann die Dezentralisierung zu mindern versuchen?

* Regierungen, die Bitcoin abschalten oder verbieten
* Unerwünschte Änderungen am Code, die eine bestimmte Interessengruppe in Bitcoin bevorzugen, z. B. eine Erhöhung der Blockbelohnung
* Beeinflussung des Protokolls durch Regierungen oder böswillige Akteure, um die Richtung des Protokolls zu steuern
* Die Möglichkeit, dass ein Mining-Pool das Netzwerk übernimmt und Bitcoin 'doppelt ausgibt' – ein 51%-Angriff

Wie wir sehen können, dezentralisiert die Kombination aus Nodes, Code-Entwicklern und Minern sowie die Verwendung des 'Proof-of-Work'-Mechanismus Bitcoin auf ein ausreichendes Maß, sodass diese potenziellen Bedrohungen nicht als besonders besorgniserregend gelten. Die Community muss die Situation weiterhin beobachten, um sicherzustellen, dass dies so bleibt.
