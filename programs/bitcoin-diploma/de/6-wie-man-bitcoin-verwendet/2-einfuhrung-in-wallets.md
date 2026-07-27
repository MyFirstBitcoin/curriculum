# 6.2 Einführung in Wallets

Im Gegensatz zu physischem Geld werden Bitcoin nicht tatsächlich in einer Bitcoin-Wallet aufbewahrt. Stattdessen existieren sie auf dem dezentralen Kassenbuch, das vom Bitcoin-Netzwerk ständig überprüft und gesichert wird. Wie kann man also Bitcoin besitzen?

Du besitzt deine Bitcoin nur, wenn du die privaten Schlüssel kontrollierst, die es dir ermöglichen, Transaktionen zu signieren und das Eigentum an deinen Bitcoin an jemand anderen zu übertragen. Das ist der Vorgang des Sendens von Bitcoin.

Schauen wir uns zwei Konzepte an, auf die wir uns beziehen, wenn wir den Begriff **Wallet**:

* Ein Master-Privatschlüssel, ähnlich wie ein Passwort, aus dem deine öffentlichen Schlüssel, vergleichbar mit E-Mail-Adressen, generiert werden. Du kannst deine öffentliche Adresse mit anderen teilen, um Bitcoin zu empfangen und zu senden, aber du darfst niemals deinen privaten Schlüssel weitergeben!
* Die mobile oder Desktop-Oberfläche, mit der du mit dem Bitcoin-Netzwerk interagierst, deinen Bitcoin-Bestand prüfst, Transaktionen sendest und empfängst und diese im Netzwerk veröffentlichst. Verschiedene Arten von Wallets sowie deren Vorteile und Kompromisse werden in den nächsten Abschnitten beschrieben.

#### Selbstverwahrte vs. Verwahrte Wallets

Bevor wir die verschiedenen Arten von Bitcoin-Wallets und deren Eigenschaften im Detail betrachten, wollen wir einen wichtigen Unterschied zwischen selbstverwahrten und verwahrten Wallets machen. Jede Art hat ihre eigenen Vorteile, Risiken und Kontrollmöglichkeiten über die Bitcoin. Selbstverwahrung bedeutet, dass der Nutzer die privaten Schlüssel hält und somit die volle Kontrolle über seine Bitcoin hat; bei verwahrten Wallets hält ein Dritter die Bitcoin für den Nutzer.


| Typ | Kontrolle | Vorteile | Risiken |
| --- | --- | --- | --- |
| Selbstverwahrt | Der Nutzer | Volle Kontrolle über Guthaben und Transaktionen, kein Genehmigungsprozess oder Kontosperrung, keine Kontrolle durch Unternehmen oder Regierung, Schutz vor Beschlagnahmung. | Keine Wiederherstellung möglich, wenn die Wiederherstellungsphrase verloren geht, volle Verantwortung liegt beim Nutzer. |
| Verwahrt | Der Drittanbieter | Einfache Wiederherstellung bei Verlust des Zugangs, einfacherer Kundensupport. | Guthaben ist mit dem Internet verbunden, dadurch anfälliger für Hackerangriffe. Der Verwahrer kann Konten einfrieren. |


In einer selbstverwahrten Wallet (auch Non-Custodial Wallet genannt) bist nur du im Besitz der Schlüssel zur Wallet und hast die volle Kontrolle darüber, was hinein- und hinausgeht. In einer verwahrten Wallet hingegen hält jemand anderes den privaten Schlüssel und hat somit vollen Zugriff auf alle Bitcoin, die dieser Anbieter in deinem Namen verwaltet.

* Selbstverwahrung ist wie deine eigene Bank zu sein. Transaktionen unterliegen nicht der Kontrolle und Überwachung
* Selbstverwahrung stellt sicher, dass Dritte deine Bitcoin nicht beschlagnahmen können.
* Selbstverwahrung gibt in unsicheren Zeiten ein beruhigendes Gefühl, weil du weißt, dass deine Bitcoin sicher sind.

Es ist wichtig, die richtige Wallet-Art für die eigenen Bedürfnisse zu wählen. Manchmal fällt es Menschen schwer zu erkennen, ob sie eine selbstverwahrte oder eine verwahrte Wallet installieren. Diese Tabelle zeigt die Unterschiede im Installationsprozess.


| Typ | Schritt 1: Wählen | Schritt 2: Installieren | Schritt 3: Erstellen | Schritt 4: Sichern |
| --- | --- | --- | --- | --- |
| Selbstverwahrt | Wähle eine selbstverwahrte Wallet | Folge den Wallet-Anweisungen | Erzeuge eine Wiederherstellungsphrase | Bewahre die Wiederherstellungsphrase an einem sicheren Ort auf |
| Verwahrt | Wähle eine verwahrte Wallet | Folge den Wallet-Anweisungen | Erstelle ein Konto | N/A |


„**Nicht deine Schlüssel, nicht deine Coins**“ ist ein beliebtes Sprichwort unter Bitcoin-Besitzern. Es bedeutet, dass du keine wirkliche Kontrolle über deine Coins hast, wenn du nicht direkten Zugriff auf die privaten Schlüssel deiner Bitcoin-Wallet hast.

Wer immer Zugriff auf deine privaten Schlüssel hat, besitzt auch deine Bitcoin. Deshalb ist es von größter Wichtigkeit, sie zu schützen und vor neugierigen Blicken zu bewahren! Später im Buch werden wir einige Möglichkeiten kennenlernen, wie du das tun kannst.

Im Folgenden sprechen wir nur über selbstverwahrte Wallets, bei denen der Nutzer seine Schlüssel besitzt und die volle Kontrolle über seine Bitcoin hat.

Mach dir keine Sorgen, wenn es kompliziert erscheint oder du nicht alles verstehst – das ist eine Reise, und je mehr du Bitcoin benutzt, desto besser wirst du es verstehen!

#### Verschiedene Arten von Bitcoin-Wallets

Wo dein privater Schlüssel erstellt und gespeichert wird, bestimmt, wie wir Bitcoin-Wallets beschreiben. Wenn die Schlüssel auf deinem Smartphone sind, ist es eine **Mobile Wallet**. Wenn sie sicher auf einem speziellen Gerät gespeichert werden, handelt es sich um eine **Hardware-Wallet**.


| Typ | Beschreibung | Vorteile | Nachteile | Beispiel-Nutzer |
| --- | --- | --- | --- | --- |
| Online-Wallet | Über einen Webbrowser zugänglich | Von jedem Gerät mit Internetverbindung aus zugänglich | Weniger sicher, da sie gehackt oder kompromittiert werden kann | Muss häufig auf seine Wallet zugreifen und hat nicht viele Mittel zu speichern |
| Mobile Wallet | Auf einem mobilen Gerät installiert | Einfach zu bedienen | Kann verloren gehen, wenn das Gerät gestohlen oder gehackt wird | Muss unterwegs Transaktionen durchführen und hat nicht viele Mittel zu speichern |
| Desktop-Wallet | Auf einem Desktop-Computer installiert | Praktisch und von überall aus zugänglich | Kann gehackt werden, wenn der Computer mit Malware infiziert ist | Möchte eine große Menge Bitcoin speichern und fühlt sich im Umgang mit einem Desktop-Computer wohl |
| Hardware-Wallet | Ein physisches Gerät, das Bitcoin offline speichert | Sicherer als Online-Wallets und kann offline verwendet werden | Mittel könnten unwiederbringlich verloren gehen | Möchte eine große Menge Bitcoin speichern und ist bereit, für zusätzliche Sicherheit zu bezahlen |


Da Schlüssel von einem Gerät auf ein anderes übertragen werden können, ist der „Status“ deiner Bitcoin-Wallet nicht festgelegt. Wenn ich zum Beispiel meine Wallet-Schlüssel auf einem Computer erstelle und sie später auf mein Handy übertrage, wird die „Desktop-Wallet“ zu einer „Mobile Wallet“.

Beim Aufbewahren deiner Bitcoin geht es nicht nur darum, wer die Kontrolle über die Schlüssel hat – es gibt viele weitere Risiken zu berücksichtigen. Deshalb ist es wichtig, eine Aufbewahrungslösung zu finden, die sowohl sicher als auch bequem ist. Wenn du die Vor- und Nachteile der verschiedenen Wallet-Typen analysierst, wirst du feststellen, dass es keine ideale Wallet gibt, die alle Bedürfnisse erfüllt.

##### Was du bei der Auswahl einer Wallet beachten solltest

* **Sicherheit**: Stelle sicher, dass die Wallet über starke Sicherheitsmaßnahmen verfügt.
* **Privatsphäre**: Überlege, ob die Wallet persönliche Informationen verlangt.
* **Benutzerfreundlichkeit**: Wähle eine Wallet, die einfach zu bedienen und zu navigieren ist.
* **Kompatibilität**: Stelle sicher, dass die Wallet mit deinem Gerät kompatibel ist.
* **Gebühren**: Vergleiche die von verschiedenen Wallets erhobenen Gebühren.
* **Ruf**: Überprüfe den Ruf der Entwickler, um sicherzustellen, dass sie vertrauenswürdig sind.
* **Kontrolle**: Manche Wallets geben dir mehr Kontrolle über deine privaten Schlüssel.

##### Open Source vs. Closed Source

Ein weiterer wichtiger Faktor bei der Auswahl einer Bitcoin-Wallet ist, ob die Anwendung oder Software Open Source ist. Das ist wichtig, weil Open-Source-Projekte es der Community ermöglichen, den Code zu überprüfen und das Projekt fortzuführen, falls das Team die Arbeit einstellt. Genau wie der Code von Bitcoin für alle offen zur Überprüfung, Nutzung und Modifikation ist, sollte auch der Code der Wallet, mit der du deine Bitcoin verwaltest, offen sein.

#### Aktivität: Diskussion und Bewertung von Bitcoin-Wallets


https://bitcoin.org/en/choose-your-wallet

_QR Code: Choose your wallet_


Gehe auf folgende Webseite: [https://bitcoin.org/en/choose-your-wallet](https://bitcoin.org/en/choose-your-wallet)

Nutze dein neues Wissen über Bitcoin-Wallets, um diejenige auszuwählen, die am besten zu deinen Bedürfnissen passt – basierend auf den Kriterien, die wir heute besprochen haben.
