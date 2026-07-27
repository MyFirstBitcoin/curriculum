# 9.3 Jak działają transakcje

Teraz, gdy rozumiesz klucze publiczne i prywatne, a także role węzłów i górników, oto jak przebiega transakcja Bitcoin od początku do końca.

1. Adam chce wysłać bitcoiny do Adama. Tworzy transakcję z adresem Adama, kwotą do wysłania oraz opłatą.
1. Adam podpisuje transakcję swoim kluczem prywatnym, aby udowodnić własność.
1. Następnie rozgłasza transakcję w sieci Bitcoin.
1. Węzły ją odbierają i sprawdzają, czy spełnia zasady, w tym weryfikują podpis oraz czy Adam ma wystarczającą ilość bitcoinów.
1. Jeśli jest poprawna, transakcja jest udostępniana w całej sieci i trafia do mempoola, gdzie oczekują niepotwierdzone transakcje.
1. Górnicy wybierają transakcje z mempoola i umieszczają je w bloku, który próbują wydobyć.
1. Gdy górnik pomyślnie wydobędzie blok, jest on udostępniany w sieci i sprawdzany przez inne węzły.
1. Jeśli blok jest poprawny, zostaje dodany do łańcucha bloków. Adam otrzymuje bitcoiny.
1. Wraz z dodawaniem kolejnych bloków, transakcja zyskuje potwierdzenia, co czyni ją bardziej bezpieczną.

Po włączeniu do bloku transakcja jest potwierdzona. Adam nie może ponownie wydać tych bitcoinów, a Adam może wydać to, co otrzymał, w nowej transakcji.


> **Light**
>
> Wybrano transakcję i opłatę → Podpisana przez portfel i wysłana → Rozpowszechniona przez węzły → Górnik dodaje transakcję do szablonu bloku → Górnik wygrywa konkurs Proof-of-Work → Nowy blok jest weryfikowany → Nowy blok jest rozpowszechniany przez węzły


###### Materiały


[▶ Obejrzyj ten film o węzłach Bitcoina](https://www.youtube.com/watch?v=xc_TxlByxeY)
