# 2.4 Es gibt keine Innovation bei Bitcoin.

> Die Entstehung von tausend Wäldern liegt in einer einzigen Eichel.   
_Ralph Waldo Emerson_

Kritiker versuchen oft zu behaupten, dass Bitcoin eine 'alte' oder 'tote' Technologie sei, weil das Basisprotokoll nicht so häufig geändert wird wie bei konkurrierenden Blockchains. Diese Behauptung ignoriert sowohl die Gründe, warum Änderungen an Bitcoin nur langsam übernommen werden, als auch die Menge an Innovationen, die zur Skalierung des Netzwerks auf höheren Ebenen wie dem Lightning Network stattfinden. Sie ignoriert auch, dass viele unserer flexibelsten und langlebigsten Technologien ebenfalls nicht schnell auf der Basisschicht skalieren.

Zum Beispiel gibt es auch keine Innovationen im Transmission Control Protocol (TCP), das dem Internet zugrunde liegt. TCP wurde erstmals 1974 entwickelt. Das letzte Mal wurde TCP 1982 aktualisiert. Es tut, was es tun soll. Es ist nicht perfekt, und es gibt Debatten darüber, ob wir IPv4 aufrüsten müssen, um zukünftige Entwicklungen des Internets zu unterstützen. Zu behaupten, dass es seit 1982 keine Innovationen im Internet gegeben habe, wäre jedoch eine bemerkenswerte Aussage. All diese Innovationen fanden 'auf' TCP statt, nicht 'in' TCP.

Die überwiegende Mehrheit der Innovationen findet nicht 'in' Bitcoin, sondern 'auf' Bitcoin statt. Eines Tages wird es wahrscheinlich keine Innovationen mehr 'in' Bitcoin geben, und das sollte ein Ziel und keine Kritik sein, da es widerspiegelt, wie grundlegend Bitcoin für die Unterstützung der Weltwirtschaft geworden ist, indem es die Grundlage für globales, neutrales und erlaubnisfreies, solides Geld bietet. Geld, das sowohl im wirtschaftlichen Sinne solide ist, da es ein festes Angebot und ein unveränderliches Hauptbuch gibt, als auch im technologischen Sinne, da es sich nicht verändert und das, was läuft, jahrelang ununterbrochene Betriebszeit hatte. Bitcoin hat in den letzten 10 Jahren bereits 100 % Betriebszeit erreicht.

Es wäre jedoch bedenklich, wenn keine Innovationen 'auf' Bitcoin stattfinden würden. Werfen wir einen Blick darauf in den letzten 10 Jahren:



#### 'In' Bitcoin

Segregated Witness (SegWit) wurde 2017 implementiert, um Transaktionsmanipulationen zu verhindern und die Blockkapazität zu erhöhen. SegWit war auch eine notwendige Voraussetzung dafür, dass Lightning und einige Sidechains effizient funktionieren können.

Taproot wurde 2021 implementiert, um das Bündeln und Validieren mehrerer Signaturen durch die Integration von Schnorr-Signaturen zu ermöglichen, eine Skriptsprache einzuführen, die komplexere Funktionalitäten erlaubt, und die Privatsphäre sowie die Zensurresistenz von Transaktionen zu erhöhen.



#### 'Auf' Bitcoin

##### Liquid Sidechain

Die Liquid Sidechain wurde 2018 implementiert. Liquid ist wie andere Sidechains ein separates Blockchain-Hauptbuch, das nach einem vordefinierten Satz von Regeln mit der Haupt-Bitcoin-Blockchain verbunden ist. Diese Regeln sind flexibel genug, um es der Liquid-Chain zu ermöglichen, sich weiterzuentwickeln und im Laufe der Zeit Design- und Skalierbarkeitsverbesserungen zu integrieren. Die Verbindung zur Bitcoin-Blockchain stellt jedoch sicher, dass das Gesamtangebot von 21 Millionen Bitcoin auf beiden Chains konsistent bleibt.

Der Vermögenswert in Liquid, L-BTC, ist mit Bitcoin auf der Hauptkette in beide Richtungen gekoppelt. Es gibt Kosten-, Geschwindigkeits-, Datenschutz- und Sicherheitskompromisse, die L-BTC für bestimmte Anwendungen ideal machen. Kosten, Geschwindigkeit und Privatsphäre werden mit L-BTC verbessert, allerdings auf Kosten eines gewissen Vertrauens in die Organisationen, die die Liquid Federation bilden, welche gemeinsam einen 11-von-15-Multisig-Prozess kontrollieren, um L-BTC in Bitcoin und umgekehrt ein- und auszubuchen.

##### Lightning Network

Das Lightning Network wurde 2018 implementiert. Lightning ist als Peer-to-Peer-Zahlungsnetzwerk in Form eines Graphen von Knoten konzipiert, die über Kanäle verbunden sind; es ist keine Blockchain. Bitcoin wird von einem Node-Betreiber auf der Haupt-Blockchain gesperrt, um ihn für die Nutzung im Lightning Network verfügbar zu machen. Dies stellt sicher, dass nur 'echte' Bitcoin verwendet werden. Knoten können dann über Multisig-Smart-Contracts Liquiditätskanäle miteinander eröffnen. Zahlungen finden ihren Weg durch das Netzwerk vom Ursprung bis zum Ziel, wobei die Kosten gegen die Anforderung optimiert werden, dass zwischen jedem Knoten im Pfad ausreichend Liquidität in die richtige Richtung vorhanden ist. Das Lightning Network verbessert Kosten, Geschwindigkeit und Privatsphäre erheblich, im Gegenzug für einen Verlust an Sicherheit (bzw. erhöhtes erforderliches Vertrauen) und eine Zunahme an Komplexität. Es ist jedoch für hochvolumige, niedrigwertige Alltagszahlungen gedacht, sodass dieser Kompromiss für seine Millionen täglichen Transaktionen (Quelle: River, 2023) als sehr angemessen gilt.

##### Chaumian eCash Mints

Fedimints können als gemeinschaftsgebundenes Lightning-Netzwerk betrachtet werden. Sie sind darauf ausgelegt, das inhärente Vertrauen, das innerhalb bestimmter Gemeinschaften (z. B. Familien, Dörfer, Freundesgruppen) besteht, zu nutzen, um im Gegenzug die Komplexität für die Nutzer zu vereinfachen und die Privatsphäre zu erhöhen. Sie sind modulare, quelloffene Protokolle zur Verwahrung und Transaktion von Bitcoin im Gemeinschaftskontext. Sie sind mit dem Lightning Network selbst interoperabel.

**Cashu** ist ein Inhabertoken, der auf einem Gerät wie einem Mobiltelefon gespeichert werden kann; das Design zielt darauf ab, die Vorteile von physischem Bargeld in digitaler Form nachzubilden. Cashu ist ein Beispiel für Chaumian eCash, das auf Bitcoin aufbaut, und erhöht die Privatsphäre und Zensurresistenz sowie reduziert die Komplexität im Gegenzug für das Vertrauen in die verwendete eCash-Mint. Cashu-Mints geben eCash-Token aus, die Bitcoin repräsentieren und von Nutzern ausgegeben werden können, ohne deren Identität preiszugeben. Cashu ist mit dem Lightning Network interoperabel.

Es werden in Zukunft wahrscheinlich noch viele weitere Layer-2-Anwendungen entwickelt werden, auf denen wiederum viele Layer-3-Anwendungen aufgebaut werden.

Als Beispiel für die unglaubliche Anzahl von Anwendungen, die auf Lightning aufgebaut werden, hier ein Auszug aus einem Lightning Network Research Report von River.

![The Lightning Network Industry Market Map 2023](https://cdn.sanity.io/images/vje9ehw2/staging/a5d3bdf5b343b7ae7e44663cf6e56a76a4bdec2d-501x706.svg)
