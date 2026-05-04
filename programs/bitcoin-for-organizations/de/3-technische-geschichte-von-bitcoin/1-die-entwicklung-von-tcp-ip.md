# 3.1 Die Entwicklung von TCP/IP

Die meisten von uns kennen die heute verwendeten TCP/IP-Protokolle als Grundlage des Internets. Ihre Ursprünge reichen bis in die späten 70er Jahre zurück, als Wissenschaftler alternative Entwürfe zum Arpanet erforschten – einem noch früheren Netzwerk, das vom US-Verteidigungsministerium entwickelt wurde, um die gemeinsame Nutzung von Ressourcen zwischen entfernten Computern zu ermöglichen. TCP/IP wurde 1983 zum Protokollstandard für das Arpanet, was dazu führte, dass es bis Ende der 1990er Jahre das dominierende Netzwerkmodell wurde und die Grundlage für das Internet bildet, auf dem Bitcoin heute läuft.


| OSI-Modell | TCP/IP |
| --- | --- |
| Anwendung | Anwendung |
| Darstellung | Anwendung |
| Sitzung | Anwendung |
| Transport | Transport |
| Netzwerk | Netzwerk |
| Sicherung | Sicherung |
| Physikalisch | Physikalisch |


Zur gleichen Zeit, als das TCP/IP-Modell entwickelt wurde, wurde von der Internationalen Standardisierungsorganisation (ISO) und der Telekommunikationsindustrie (CCITT) ein ähnliches, aber umfassenderes Rahmenwerk entwickelt. Der Prozess zur Entwicklung neuer Protokolle oder zur Vorschlag von Änderungen war im Vergleich zum dezentraleren Ansatz bei TCP/IP langsam und schwerfällig, was zur heutigen Dominanz dieses Ansatzes führte.

##### Antrag auf Änderung

Jede vorgeschlagene Weiterentwicklung bestehender Protokolle oder Ideen für neue kann im TCP/IP-Modell durch einen **Antrag auf Änderung**-Prozess vorgeschlagen werden. Diese durchlaufen einen Genehmigungsprozess, der von der Internet Engineering Task Force (IETF) verwaltet wird, und werden nach der Genehmigung als Open Source veröffentlicht, damit jeder sie implementieren und übernehmen kann. Einige bemerkenswerte Beispiele:

* 1969 RFC 1 Dokumentierte, wie Pakete im Arpanet gesendet werden sollten
* 1981 RFC791 definierte das Internetprotokoll V4 – noch heute weit verbreitet
* 1982 RFC 821 Simple Mail Transfer Protocol
* 1987 Domain Name System – wie Domainnamen in IP-Adressen aufgelöst werden
* 1999 RFC 2616 Hypertext Transfer Protocol – unerlässlich für das Surfen im Web


> **Callout**
>
> Der **Bitcoin Improvement Proposal** (BIP) folgt einem ähnlichen Ansatz wie RFC, konzentriert sich jedoch ausschließlich auf Verbesserungen an Bitcoin selbst und nicht auf die Entwicklung neuer oder alternativer Protokolle. Bitcoin übernimmt auch dieses Schichtenmodell, und Sie werden zusätzliche Protokolle als Layer zwei oder drei beschrieben sehen.


In ähnlicher Weise wie sich die Basisschichten des TCP/IP-Modells in den letzten Jahrzehnten nur wenig verändert haben und die Innovationen in höheren Schichten stattfinden, wird auch erwartet, dass sich die Basisschicht von Bitcoin nun nur noch sehr langsam verändert, während Skalierungslösungen wie Lightning und Liquid darüber angesiedelt sind.

Ein gutes Beispiel dafür, wie sich Protokolle auf der Basisschicht im Laufe der Zeit nur schwer ändern lassen, ist IPv6. Die erwartete Erschöpfung des Adressraums in IPv4 schuf die Nachfrage nach einem neuen Protokoll. Der erste Entwurf wurde 1998 erstellt, aber erst 2017 als Internetstandard ratifiziert. Obwohl es viele Probleme von IPv4 löste und wesentlich zukunftssicherer ist, wird es in der Branche bis heute nur sehr langsam übernommen. In dieser Zeit wurden viele neue Protokolle auf den oberen Schichten definiert, um Multimedia, E-Mail usw. zu ermöglichen.

##### Die Bausteine, die von Bitcoin verwendet werden

Diese Trennung der Probleme der Interkonnektivität ermöglicht es, Protokolle unabhängig von den darüber- und darunterliegenden Schichten zu entwickeln. Anstatt für jede Schicht eigene Lösungen neu zu erfinden, kann das Bitcoin-Netzwerk auf die zugrundeliegenden Fähigkeiten des Netzwerks auf der physischen und Sicherungsschicht zurückgreifen.


| Schicht | TCP/IP Original |
| --- | --- |
| Anwendung | Verwendet das Domain Name System (DNS), um benachbarte Knoten zu identifizieren. Port 8333 signalisiert das Bitcoin-Protokoll. |
| Transport | UDP für FIBRE-Kommunikation zwischen Minern für geringe Latenz. TCP für P2P-Kommunikation zwischen Knoten. |
| Transport | TOR-Routing: Ermöglicht Anonymität und Privatsphäre. Broadcast-Protokoll: Leitet den Datenverkehr über das Netzwerk. |
| Sicherung | Funktioniert über jedes Medium (z. B. Ethernet, WLAN usw.) |
| Physikalisch | Physikalische Übertragung über Funk, Ethernet oder andere Hardware-Schnittstellen. |


##### Bitcoin ist ein neutrales Protokoll zum Übertragen von Werten, so wie HTTPS ein Protokoll zum Übertragen von Informationen ist.

* **HTTPS**: Sichere Webseiten
* **SMTP**: E-Mails senden
* **FTP**: Dateien übertragen
* **DNS**: Domainnamen verwalten
* **BTC**: Wert speichern und übertragen

Bitcoin ermöglicht es, Wert zuverlässig und ohne Dritte zwischen Personen oder Geräten über das Internet zu übertragen. Dies wird voraussichtlich enormen Mehrwert schaffen.
