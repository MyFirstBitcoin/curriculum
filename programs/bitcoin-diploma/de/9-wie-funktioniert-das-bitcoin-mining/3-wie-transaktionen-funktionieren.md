# 9.3 Wie Transaktionen funktionieren

Jetzt, da Sie öffentliche und private Schlüssel sowie die Rollen von Nodes und Minern verstanden haben, erfahren Sie hier, wie eine Bitcoin-Transaktion von Anfang bis Ende abläuft.

1. Adam möchte Bitcoin an Gerardo senden. Er erstellt eine Transaktion mit Gerardos Adresse, dem zu sendenden Betrag und einer Gebühr.
1. Adam signiert die Transaktion mit seinem privaten Schlüssel, um den Besitz nachzuweisen.
1. Er sendet die Transaktion an das Bitcoin-Netzwerk.
1. Nodes empfangen sie und prüfen, ob sie den Regeln entspricht, einschließlich der Überprüfung der Signatur und ob Adam genügend Bitcoin besitzt.
1. Wenn sie gültig ist, wird die Transaktion im gesamten Netzwerk geteilt und in den Mempool aufgenommen, wo ausstehende Transaktionen warten.
1. Miner wählen Transaktionen aus dem Mempool aus und fügen sie in einen Block ein, den sie zu minen versuchen.
1. Wenn ein Miner erfolgreich einen Block mined, wird dieser mit dem Netzwerk geteilt und von anderen Nodes überprüft.
1. Ist der Block gültig, wird er zur Blockchain hinzugefügt. Gerardo erhält die Bitcoin.
1. Mit jedem weiteren Block, der hinzugefügt wird, erhält die Transaktion weitere Bestätigungen und wird dadurch sicherer.

Sobald die Transaktion in einen Block aufgenommen wurde, ist sie bestätigt. Adam kann diese Bitcoin nicht erneut ausgeben und Gerardo kann das, was er erhalten hat, in einer neuen Transaktion ausgeben.


> **Note**
>
> Transaktion & Gebühr ausgewählt → Vom Wallet signiert und gesendet → Von Nodes verteilt → Miner fügt Transaktion zur Blockvorlage hinzu → Miner gewinnt Proof-of-Work-Wettbewerb → Neuer Block wird validiert → Neuer Block wird von Nodes verteilt


###### Ressourcen


[▶ YouTube](https://www.youtube.com/watch?v=xc_TxlByxeY)
