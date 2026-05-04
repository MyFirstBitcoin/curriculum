# 8.2 Metriken zur Analyse des Hauptbuchs

Da die Transparenz von Bitcoin im Gegensatz zu traditionellen Finanzsystemen steht – in denen ein Großteil der Geldflüsse hinter verschlossenen institutionellen Türen stattfindet – entsteht ein reiches Feld der On-Chain-Analytik, bei dem Netzwerkdaten als Linse dienen, um das Nutzerverhalten, Geldflüsse und langfristige Trends zu verstehen. Diese Kennzahlen können helfen, spezifische Fragen zu beantworten, etwa wie aktiv das Netzwerk genutzt wird, ob Coins akkumuliert oder verkauft werden und ob das Netzwerk sicherer wird.

Das Verständnis dieser Kennzahlen ist nicht nur für Bitcoin-Nutzer hilfreich, sondern auch für Forscher oder politische Entscheidungsträger, die Einblicke in dieses einzigartig transparente Finanzsystem gewinnen möchten.

Dieser Abschnitt enthält einige häufig verwendete Kennzahlen zur Analyse der Bitcoin-Aktivität, gruppiert in Unterkategorien. Es handelt sich nicht um eine vollständige Liste. Besuchen Sie [www.bitcoinmagazinepro.com/charts](https://www.bitcoinmagazinepro.com/charts) für eine umfassendere Liste und Beschreibungen.



#### 8.2.1 Adress-Kennzahlen

Adress-Kennzahlen sind nützlich, um sie im Zeitverlauf zu beobachten, da sie das Aktivitätsniveau im Bitcoin-Netzwerk anzeigen. Beispielsweise steigt mit zunehmender Akzeptanz von Bitcoin die Anzahl der aktiven Adressen. Wir können dies weiter untersuchen, indem wir die Anzahl der Adressen betrachten, die eine bestimmte Mindestmenge an Bitcoin halten, zum Beispiel 0,1 BTC, innerhalb eines bestimmten Zeitraums, etwa ein Jahr. Während dies einen Einblick in die Bitcoin-Adoption im Zeitverlauf bietet, ist es nicht perfekt, da eine Person mehrere Bitcoin-Adressen besitzen kann. Umgekehrt können Börsen oder ETFs als einzelne Einheiten erscheinen, obwohl sie Gelder für eine große Anzahl von Personen halten.

![Bitcoin: Addresses Hodling > X BTC by Year](https://cdn.sanity.io/images/vje9ehw2/staging/b88a9239820e45ed50ce00812170e2bb4d02b5d2-1407x766.png)

_Adressen, die Bitcoin > X BTC nach Jahr halten. Quelle: Bitcoin Magazine Pro._

Durch den Vergleich von Adressen mit dem aktuellen Marktpreis von BTC ist es möglich, den Prozentsatz aller Bitcoin-Adressen im Gewinn zu sehen. Dies ermöglicht es uns, die Marktstimmung zu verfolgen, da wir sehen können, welcher Anteil des Marktes BTC mit Gewinn oder Verlust hält.

Zum Beispiel zeigt das **Prozentualer nicht realisierter Gewinn**-Diagramm unten den Anteil aller Ledger-Adressen mit einem nicht realisierten Gewinn, gemessen in US-Dollar. Beachten Sie, dass, da das untenstehende Diagramm nahe am Allzeithoch von Bitcoin aufgenommen wurde, der Prozentsatz der Adressen mit nicht realisiertem Gewinn nahe bei einhundert Prozent liegt. Wir sehen auch, dass längere Zeiträume mit einem Prozentualen nicht realisierten Gewinn unter einer Standardabweichung vom Mittelwert ungewöhnlich sind. Ein Unterschreiten dieser Linie kann daher einen guten Einstiegszeitpunkt für Käufer anzeigen.

![Percent Unrealised Profit](https://cdn.sanity.io/images/vje9ehw2/staging/f306f03f31ce4faada8bf34137dd76f9d550697a-1041x491.png)

_Prozentualer nicht realisierter Gewinn. Quelle: checkonchain.com_



#### 8.2.2 On-Chain-Indikatoren

On-Chain-Indikatoren sind nützlich, weil sie Einblicke in das Netzwerkverhalten bieten, die über das hinausgehen, was Preis- und Adress-Kennzahlen allein zeigen können. Sie helfen Analysten, die Handlungen und die Stimmung verschiedener Teilnehmergruppen zu verstehen, etwa von Langzeitinhabern im Vergleich zu kurzfristigen Händlern, indem sie verfolgen, wie Coins gehalten, bewegt oder im Zeitverlauf bewertet werden. Diese Indikatoren nutzen die transparente Natur des Ledgers, um verborgene Marktdynamiken wie Akkumulation, Distribution oder sogar die Überzeugung von Investoren sichtbar zu machen. Das macht sie besonders nützlich, um strukturelle Trends zu erkennen, zu beurteilen, ob der Markt überhitzt oder unterbewertet ist, und Wendepunkte in einem Marktzyklus vorherzusehen.

Zum Beispiel können wir durch die Betrachtung des Werts der BTC-Bestände seit ihrer letzten Transaktion ableiten, ob sich der Markt in einer Stresssituation befindet (wie es bei einem großen Zyklustief der Fall sein könnte). Diese Kennzahl ist bekannt als **Realisierter Preis** und gibt uns eine „durchschnittliche Kostenbasis“ aller im Umlauf befindlichen BTC. Fällt der Marktpreis unter den Realisierten Preis, zeigt dies, dass die Mehrheit der Adressen im Durchschnitt einen Buchverlust hält.

Durch die weitere Gruppierung der Ledger-Daten in Altersbänder können wir zeigen, wie sich die Menge an BTC im Zeitverlauf zwischen Adressen bewegt, was wellenartige Muster in einem Diagramm erzeugt, die als **HODL-Wellen** bezeichnet werden.

![Bitcoin HODL Waves](https://cdn.sanity.io/images/vje9ehw2/staging/ce108e45a1a7217e081101e4a276ee2d9e95a22e-1129x577.png)

_Bitcoin HODL-Wellen. Quelle: Bitcoin Magazine Pro._

Die HODL-Wellen zeigen, was Langzeit-, Mittelzeit- und Kurzzeithalter mit ihren BTC machen. Im obigen Diagramm sind Kurzzeithalter in Rot und Orange dargestellt, und wir sehen Aktivitätsspitzen, wenn diese Gruppe in der Nähe von Markthochs eilig kauft. Am anderen Ende sehen wir, dass sehr langfristige Halter (in Lila und Blau) ihren Anteil am Netzwerk stetig erhöhen, was auf eine hohe Überzeugung in diesen Gruppen hinweist. Das Diagramm ist nicht perfekt, da einige Coins von alten zu neuen Adressen unter Kontrolle desselben Nutzers verschoben werden können. Dennoch bietet es einen interessanten Einblick in die Überzeugung von Langzeithaltern.

Eine weitere Möglichkeit, das „Smart Money“ der Langzeithalter zu betrachten, ist die Analyse der **Zerstörten Coin-Tage** (Coin Days Destroyed, CDD). Das Konzept der „Coin Days“ ist das Produkt aus der Anzahl der BTC und der Tage, seit die Coins zuletzt bewegt wurden. Zum Beispiel haben 5 BTC, die 100 Tage lang nicht bewegt wurden, 500 Coin Days angesammelt, und 10 BTC, die 10 Tage lang nicht bewegt wurden, haben 100 Coin Days angesammelt. Auf diese Weise gewichten wir Coins, die länger gehalten werden, stärker. Wenn diese Coins bewegt werden, werden diese Coin Days „zerstört“. Dieser Indikator zeigt Anstiege bei CDD zu Zeiten signifikanter Preisbewegungen, was Analysten eine Möglichkeit bietet, routinemäßige Marktaktivität von bedeutenden Veränderungen in der Stimmung der Langzeithalter zu unterscheiden.

Eine weitere Kennzahl, die helfen kann zu erkennen, ob der Markt BTC unter- oder überbewertet, ist das Verhältnis von Marktwert zu realisiertem Wert oder **MVRV**. Es wird einfach als das Verhältnis von Marktwert (Anzahl der ausgegebenen BTC multipliziert mit dem Marktpreis) geteilt durch den realisierten Wert (die Summe aller BTC seit ihrer letzten Bewegung) berechnet. Ein hoher MVRV deutet darauf hin, dass mehr Coins im Gewinn sind (oft in der Nähe von Markthochs zu sehen), und ein niedriger MVRV zeigt, dass viele Coins mit Verlust gehalten werden (zu beobachten bei Markttiefs).



#### 8.2.3 Mining-Kennzahlen

Mining-Kennzahlen sind nützlich, um die Sicherheit, die wirtschaftlichen Anreize und die allgemeine Gesundheit des Bitcoin-Netzwerks zu verstehen. Kennzahlen wie Hashrate, Miner-Einnahmen, Schwierigkeitsgrad und Gebührenverhältnisse zeigen, wie viel Rechenleistung die Blockchain sichert und wie gut Miner für ihre Aktivitäten entlohnt werden.

Die **Hashrate** des Bitcoin-Netzwerks ist vielleicht der am häufigsten zitierte Indikator für die Netzwerkgesundheit und die Stärke der Sicherheit. Da der Mining-Prozess das Netzwerk sichert und bestätigt, dass Transaktionen im Ledger gültig sind, gilt: Je mehr Rechen- (bzw. Hash-)Leistung vorhanden ist, desto schwieriger wäre es für einen böswilligen Akteur, das Netzwerk zu überwältigen und anzugreifen.

![Bitcoin Hashrate](https://cdn.sanity.io/images/vje9ehw2/staging/fcb4a24c431a37580d3d6c4ec62b664e7e41c362-1134x584.png)

_Bitcoin Hashrate. Quelle: Bitcoin Magazine Pro._

Das obige Diagramm zeigt, dass im Mai 2025 die gesamte Rechenleistung des Netzwerks bei etwa 900 TeraHash/s liegt (900 Billionen kryptografische „Hash“-Berechnungen pro Sekunde). Wenn die Hashrate steigt, zeigt dies, dass das Netzwerk sicherer wird, was für Nutzer beruhigend ist.

Das Puell Multiple (entwickelt von David Puell) betrachtet den Marktzyklus aus der Perspektive der Miner und ihrer Einnahmen. Die Kennzahl wird berechnet, indem die tägliche Ausgabe von BTC (in USD) durch den gleitenden 365-Tage-Durchschnitt des täglichen Ausgabewerts geteilt wird. Die Kennzahl hilft, Perioden von Stress oder Entlastung für Miner zu identifizieren. Historisch gesehen ging einem Multiple über 3 ein Rückgang des Marktwerts von BTC voraus, da dies auf eine hohe Rentabilität der Miner hinweist. Ein Wert unter 0,5 zeigt Stress an und hat historisch Markttiefs für den Wert von BTC signalisiert.
