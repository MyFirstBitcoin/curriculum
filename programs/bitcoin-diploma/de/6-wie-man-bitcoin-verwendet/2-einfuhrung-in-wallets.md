# 6.2 Einführung in Wallets

Im Gegensatz zu physischem Geld werden Bitcoin nicht tatsächlich in einer Bitcoin-Wallet aufbewahrt. Stattdessen existieren sie auf dem dezentralen Hauptbuch, das das Bitcoin-Netzwerk ständig überprüft und absichert. Wie kann man also Bitcoin besitzen?

Du besitzt deine Bitcoin nur, wenn du die privaten Schlüssel kontrollierst, die es dir ermöglichen, Transaktionen zu signieren und das Eigentum an deinen Bitcoin an jemand anderen zu übertragen. Das ist der Vorgang des Sendens von Bitcoin.

Schauen wir uns zwei Konzepte an, auf die wir uns beziehen, wenn wir den Begriff **Wallet**:

* Ein Master-Privatschlüssel (wie ein Passwort), aus dem deine öffentlichen Schlüssel (wie E-Mail-Adressen) generiert werden [Gedankenstrich] – du kannst deine öffentliche Adresse mit anderen teilen, um Bitcoin zu empfangen und zu senden, aber du darfst niemals deinen privaten Schlüssel weitergeben!
* Die mobile oder Desktop-Oberfläche, über die du mit dem Bitcoin-Netzwerk interagieren kannst, um deinen Bitcoin-Bestand abzurufen, Transaktionen zu senden und zu empfangen und sie im Netzwerk zu veröffentlichen. Verschiedene Arten von Wallets sowie deren Vorteile und Kompromisse werden in den nächsten Abschnitten beschrieben.

#### Selbstverwahrte vs. Verwahrte Wallets

Bevor wir die verschiedenen Arten von Bitcoin-Wallets und ihre Eigenschaften im Detail betrachten, wollen wir einen wichtigen Unterschied zwischen selbstverwahrten und verwahrten Wallets machen. Jede Art hat ihre eigenen Vorteile, Risiken und Kontrollmöglichkeiten über die Bitcoin. Selbstverwahrung bedeutet, dass der Nutzer die privaten Schlüssel hält und seine Bitcoin wirklich kontrolliert; bei verwahrten Wallets hält ein Dritter die Bitcoin für den Nutzer.


| Wallet-Typ | Wer kontrolliert? | Vorteile | Risiken |
| --- | --- | --- | --- |
| Selbstverwahrt | Der Nutzer | Vollständige Kontrolle über Guthaben und Transaktionen, kein Genehmigungsprozess oder Kontosperre, keine Kontrolle durch Unternehmen oder Regierung, Schutz vor Beschlagnahmung. | Keine Wiederherstellung möglich, wenn die Wiederherstellungsphrase verloren geht, die volle Verantwortung liegt beim Nutzer. |
| Verwahrt | Der Drittanbieter | Einfache Wiederherstellung bei Verlust des Zugangs, einfacherer Kundensupport. | Guthaben ist mit dem Internet verbunden, dadurch anfälliger für Hackerangriffe. Der Verwahrer kann Konten einfrieren. |


In einer selbstverwahrten Wallet (auch Non-Custodial Wallet genannt) bist nur du im Besitz der Schlüssel zur Wallet und hast die volle Kontrolle darüber, was hinein- und hinausgeht. In einer verwahrten Wallet hingegen hält jemand anderes den privaten Schlüssel und hat damit vollen Zugriff auf alle Bitcoin, die dieser Anbieter in deinem Namen verwaltet.

* Selbstverwahrung ist wie deine eigene Bank zu sein. Transaktionen unterliegen nicht der Kontrolle und Überwachung
* Selbstverwahrung stellt sicher, dass Dritte deine Bitcoin nicht beschlagnahmen können.
* Selbstverwahrung gibt in unsicheren Zeiten ein beruhigendes Gefühl, weil du weißt, dass deine Bitcoin sicher sind.

Es ist wichtig, den richtigen Wallet-Typ für die eigenen Bedürfnisse zu wählen. Manchmal fällt es Menschen schwer zu erkennen, ob sie eine selbstverwahrte oder eine verwahrte Wallet installieren. Diese Tabelle zeigt die Unterschiede im Installationsprozess.


| Wallet-Typ | Schritt 1: Wählen | Schritt 2: Installieren | Schritt 3: Erstellen | Schritt 4: Sichern |
| --- | --- | --- | --- | --- |
| Selbstverwahrt | Wähle eine selbstverwahrte Wallet | Folge den Wallet-Anweisungen | Erzeuge eine Wiederherstellungsphrase | Bewahre die Wiederherstellungsphrase an einem sicheren Ort auf |
| Verwahrt | Wähle eine verwahrte Wallet | Folge den Wallet-Anweisungen | Erstelle ein Konto | N/A |


„**Nicht deine Schlüssel, nicht deine Coins**“ ist ein beliebtes Sprichwort unter Bitcoin-Besitzern. Es bezieht sich auf die Idee, dass du keine wirkliche Kontrolle über deine Coins hast, wenn du nicht direkten Zugriff auf die privaten Schlüssel deiner Bitcoin-Wallet hast.

Wer auch immer Zugriff auf deine privaten Schlüssel hat, besitzt deine Bitcoin. Deshalb ist es von größter Wichtigkeit, sie zu schützen und vor neugierigen Blicken fernzuhalten! Später im Buch werden wir einige Möglichkeiten sehen, wie du das tun kannst.

Im Folgenden sprechen wir nur über selbstverwahrte Wallets, bei denen der Nutzer seine Schlüssel besitzt und die volle Kontrolle über seine Bitcoin hat.

Mach dir keine Sorgen, wenn es kompliziert erscheint oder du nicht alles verstehst – das ist eine Reise, und je mehr du Bitcoin benutzt, desto besser wirst du es verstehen!


---


#### Verschiedene Arten von Bitcoin-Wallets

Wo dein privater Schlüssel erstellt und gespeichert wird, bestimmt, wie wir Bitcoin-Wallets beschreiben. Wenn die Schlüssel auf deinem Smartphone sind, ist es eine **Mobile Wallet**. Wenn sie sicher auf einem speziellen Gerät gespeichert werden, handelt es sich um ein **Hardware-Wallet**.


| Wallet-Typ | Beschreibung | Vorteile | Nachteile | Beispielnutzer |
| --- | --- | --- | --- | --- |
| Online-Wallet | Über einen Webbrowser zugänglich | Von jedem Gerät mit Internetverbindung aus zugänglich | Weniger sicher, da es gehackt oder kompromittiert werden kann | Muss häufig auf sein Wallet zugreifen und hat nicht viele Mittel zu speichern |
| Mobile Wallet | Auf einem mobilen Gerät installiert | Einfach zu bedienen | Kann verloren gehen, wenn das Gerät gestohlen oder gehackt wird | Muss unterwegs Transaktionen durchführen und hat nicht viele Mittel zu speichern |
| Desktop-Wallet | Auf einem Desktop-Computer installiert | Bequem und von überall aus zugänglich | Kann gehackt werden, wenn der Computer mit Malware infiziert ist | Möchte eine große Menge Bitcoin speichern und ist mit der Nutzung eines Desktop-Computers vertraut |
| Hardware-Wallet | Ein physisches Gerät, das Bitcoin offline speichert | Sicherer als Online-Wallets und kann offline verwendet werden | Mittel könnten unwiederbringlich verloren gehen | Möchte eine große Menge Bitcoin speichern und ist bereit, für zusätzliche Sicherheit zu bezahlen |


Da Schlüssel von einem Gerät auf ein anderes übertragen werden können, ist der „Status“ Ihres Bitcoin-Wallets nicht festgelegt. Wenn ich zum Beispiel meine Wallet-Schlüssel auf einem Computer erstelle und sie später auf mein Handy übertrage, wird das „Desktop-Wallet“ zu einem „Mobile Wallet“.

Beim Speichern Ihrer Bitcoins geht es nicht nur darum, wer die Kontrolle über die Schlüssel hat – es gibt viele weitere Risiken zu beachten. Deshalb ist es wichtig, eine Speicherlösung zu finden, die sowohl sicher als auch bequem ist. Wenn Sie die Vor- und Nachteile der verschiedenen Wallet-Typen analysieren, werden Sie feststellen, dass es kein ideales Wallet gibt, das alle Bedürfnisse erfüllt.

##### Was Sie bei der Auswahl eines Wallets beachten sollten

* **Sicherheit**: Stellen Sie sicher, dass das Wallet über starke Sicherheitsmaßnahmen verfügt.
* **Privatsphäre**: Überlegen Sie, ob das Wallet persönliche Informationen erfordert.
* **Benutzerfreundlichkeit**: Wählen Sie ein Wallet, das einfach zu bedienen und zu navigieren ist.
* **Kompatibilität**: Stellen Sie sicher, dass das Wallet mit Ihrem Gerät kompatibel ist.
* **Gebühren**: Vergleichen Sie die von verschiedenen Wallets erhobenen Gebühren.
* **Ruf**: Überprüfen Sie den Ruf der Entwickler, um sicherzustellen, dass sie vertrauenswürdig sind.
* **Kontrolle**: Einige Wallets geben Ihnen mehr Kontrolle über Ihre privaten Schlüssel.

##### Open Source vs. Closed Source

Ein weiterer wichtiger Faktor bei der Auswahl eines Bitcoin-Wallets ist zu wissen, ob die Anwendung oder Software Open Source ist. Das ist wichtig, weil Open-Source-Projekte es der Community ermöglichen, den Code zu überprüfen und das Projekt fortzuführen, falls das Team die Arbeit einstellt. Genau wie der Code von Bitcoin für alle offen zur Überprüfung, Nutzung und Modifikation ist, sollte auch der Code des Wallets, das Sie zur Verwaltung Ihrer Bitcoins verwenden, offen sein.

#### Aktivität: Diskussion und Bewertung von Bitcoin-Wallets

https://bitcoin.org/en/choose-your-wallet

Gehen Sie auf folgende Webseite: [https://bitcoin.org/en/choose-your-wallet](https://bitcoin.org/en/choose-your-wallet)

Nutzen Sie Ihr neues Wissen über Bitcoin-Wallets, um dasjenige auszuwählen, das am besten zu Ihren Bedürfnissen passt, basierend auf den Kriterien, die wir heute besprochen haben.
