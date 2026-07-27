# 8.2 Das UTXO-Modell

##### Was sind UTXOs?

Lass dich nicht von dem seltsamen Namen einschüchtern. Du kannst UTXOs als Stücke von Bitcoin betrachten, ähnlich wie die Scheine und Münzen in deinem Portemonnaie. Wenn du zum Beispiel einen Artikel für 6 € mit einem 10-€-Schein bezahlst, erhältst du 4 € Wechselgeld. Bitcoin funktioniert auf ähnliche Weise.

Alle Bitcoin, die du besitzt, bestehen aus verschiedenen UTXOs. Wenn du Bitcoin versendest, verwendet deine Wallet eines oder mehrere dieser Stücke, um die Zahlung zu tätigen.

Wenn das Stück, das du ausgibst, größer ist als der Betrag, den du sendest, erhältst du den verbleibenden Wert als Wechselgeld in Form eines neuen UTXO zurück. Gleichzeitig erhält der Empfänger ein neues UTXO, das die von dir gesendeten Bitcoin repräsentiert.

Dein Wallet-Guthaben ist einfach der Gesamtwert aller UTXOs, die du kontrollierst.


> **Callout – Privatsphäre**
>
> Du solltest anderen deine UTXOs nicht bekannt machen, denn wenn jemand sie kennt, kann er deine Transaktionen nachverfolgen und letztlich wissen, wie viel Geld du besitzt.


###### Beispiel

1. Anna möchte Bernd 5 BTC senden.
1. Ihre Wallet verwendet zwei ihrer UTXOs, die zusammen 6 BTC wert sind.
1. Die Transaktion sendet **5 BTC an Bernd**, wodurch ein neues UTXO in Bernds Wallet entsteht.
1. Der verbleibende **0,99 BTC geht als Wechselgeld an Anna zurück**, nachdem eine **Transaktionsgebühr von 0,01 BTC** bezahlt wurde.
1. Sobald die Transaktion bestätigt ist, wird sie in das Bitcoin-Hauptbuch aufgenommen und die von Anna verwendeten UTXOs werden als ausgegeben markiert, sodass sie nicht erneut verwendet werden können.

###### Ressourcen


[▶ Sieh dir „How Bitcoin Works under the Hood“ an](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
