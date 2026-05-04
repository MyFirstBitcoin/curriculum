# 8.2 Model UTXO

##### Czym są UTXO?

Nie zrażaj się dziwną nazwą. Możesz myśleć o UTXO jak o kawałkach bitcoina, podobnych do banknotów i monet w Twoim portfelu. Na przykład, jeśli płacisz za przedmiot o wartości 24 zł banknotem 40-złotowym, otrzymujesz 16 zł reszty. Bitcoin działa w podobny sposób.

Wszystkie bitcoiny, które posiadasz, składają się z różnych UTXO. Gdy wysyłasz bitcoina, Twój portfel używa jednego lub kilku z tych kawałków, aby zrealizować płatność.

Jeśli kawałek, który wydajesz, jest większy niż kwota, którą wysyłasz, pozostała wartość wraca do Ciebie jako reszta w postaci nowego UTXO. Jednocześnie odbiorca otrzymuje nowe UTXO, które reprezentuje przesłanego przez Ciebie bitcoina.

Saldo Twojego portfela to po prostu łączna wartość wszystkich UTXO, które kontrolujesz.


> **Callout – Prywatność**
>
> Nie powinieneś ujawniać innym swoich UTXO, ponieważ jeśli ktoś je zna, może śledzić Twoje transakcje i ostatecznie dowiedzieć się, ile masz pieniędzy.


###### Przykład

1. Alicja chce wysłać Bartkowi 5 BTC.
1. Jej portfel używa dwóch jej UTXO, które razem są warte 6 BTC.
1. Transakcja wysyła **5 BTC do Bartka**, tworząc nowe UTXO w portfelu Bartka.
1. Pozostałe **0,99 BTC wraca do Alicji jako reszta**, po opłaceniu **0,01 BTC opłaty transakcyjnej**.
1. Po potwierdzeniu transakcji zostaje ona dodana do księgi Bitcoina, a UTXO użyte przez Alicję są oznaczone jako wydane, więc nie mogą być użyte ponownie.

###### Materiały


[▶ YouTube](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
