# 7.4 Wysyłanie i odbieranie transakcji Lightning

Dzięki portfelowi Lightning korzystanie z Bitcoina jest szybkie, tanie i prywatne, co sprawia, że transakcje między dwiema osobami są łatwe. Możesz szybko wysyłać i odbierać bitcoiny na codzienne wydatki, takie jak kupowanie kawy.

Przyjrzyjmy się kilku przykładom działania sieci Lightning w praktyce.

###### Przykład 1

Zarówno Marcia, jak i Ewa mają po 5 jednostek waluty. Marcia chce wysłać 2 jednostki do Ewy. Płatność przechodzi przez Jacka, który pomaga przekazać płatność przez sieć Lightning. Po zakończeniu transakcji Ewa ma 7 jednostek, a Marcia 3.

Jacek pomaga przekierować płatność, ale nie może ukraść środków. Sieć Lightning wykorzystuje kryptografię, aby zapewnić, że tylko zamierzony odbiorca może otrzymać płatność. Jacek po prostu pomaga płatności przejść przez sieć.

To pokazuje kluczową zaletę sieci Lightning: ludzie mogą wysyłać płatności szybko, bez konieczności zaufania pośrednikom takim jak banki.

Operatorzy węzłów, tacy jak Jacek, mogą również zarabiać niewielkie opłaty za pomoc w przekierowywaniu płatności. Dzięki temu pomagają sieci pozostać zdecentralizowaną i wydajną.

W porównaniu do zwykłych transakcji Bitcoin:

* **Transakcje on-chain** odbywają się bezpośrednio na łańcuchu bloków Bitcoina. Są bardzo bezpieczne, ale mogą być wolniejsze i droższe.
* **Transakcje Lightning** odbywają się poza łańcuchem i pozwalają na znacznie szybsze oraz tańsze przesyłanie płatności.

Dzięki temu Lightning jest przydatny do małych, codziennych płatności, podczas gdy transakcje on-chain są często używane do większych przelewów lub długoterminowego przechowywania.

###### Przykład 2

Mina uwielbia jeść na mieście i często odwiedza swoją ulubioną lokalną kawiarnię. Przy tylu różnych opcjach płatności nie jest pewna, która jest najlepsza. Na szczęście nauczyła się trochę o Bitcoinie i sieci Lightning. Po przeanalizowaniu opcji Mina dochodzi do wniosku, że korzystanie z płatności Lightning jest najlepszym wyborem.

Mina chce kupić kawę, ale płacenie zwykłą transakcją Bitcoin może czasem zająć trochę czasu i wymagać wyższych opłat. Zamiast tego decyduje się użyć sieci Lightning.

Sieć Lightning pozwala ludziom wysyłać bitcoiny natychmiastowo i przy bardzo niskich opłatach. Dzięki temu idealnie nadaje się do małych, codziennych zakupów, takich jak kawa.

Aby zacząć korzystać z Lightning, Mina pobiera portfel Lightning na swój telefon. Następnie przesyła trochę bitcoinów ze swojego zwykłego portfela Bitcoin do portfela Lightning. Ten krok wykorzystuje normalną transakcję Bitcoin na blockchainie. Gdy środki znajdą się w jej portfelu Lightning, mogą być używane w sieci Lightning.

Teraz Mina może zapłacić w kawiarni natychmiastowo, korzystając z Lightning. Płatność odbywa się poza głównym łańcuchem bloków Bitcoina, dlatego jest znacznie szybsza i tańsza niż zwykła transakcja on-chain.


| Korzyści | Sieć Lightning | Tradycyjny system bankowy |
| --- | --- | --- |
| Szybkość | Szybka | Wolna |
| Przejrzystość | Przejrzysta | Nieprzejrzysta |
| Bezpieczeństwo | Bezpieczna | Podatna na zagrożenia |
| Opłaty transakcyjne | Niskie | Wysokie |
| Włączenie finansowe | Wysokie | Ograniczone |
| Skalowalność | Wysoka | Niska |
| Prywatność | Wysoka | Umiarkowana |
| Interoperacyjność | Wysoka | Niska |
| Zgodność z prawem | Umiarkowana | Wysoka |
| Efektywność kosztowa | Wysoki | Umiarkowany |


Transakcje on-chain odbywają się bezpośrednio na blockchainie Bitcoina i mogą wymagać więcej czasu oraz wyższych opłat. Transakcje Lightning odbywają się poza łańcuchem, umożliwiając szybkie i tanie płatności, nadal z użyciem bitcoina.


| Visa, Inc. | Bitcoin On-chain | Lightning Network |
| --- | --- | --- |
| Wydajność: 65 000 transakcji na sekundę. | Wydajność: 7 transakcji na sekundę. | Wydajność: miliony transakcji na sekundę. |


![Lightning Network Map](https://cdn.sanity.io/images/vje9ehw2/staging/5a760247cf4c32074c62f40aea8dc21095882740-504x245.svg)

https://mempool.space/graphs/lightning/nodes-channels-map

To jest mapa całej sieci Lightning Network. Dzięki tysiącom operatorów węzłów Lightning możesz wysyłać saty do każdego użytkownika z portfelem Bitcoin Lightning, gdziekolwiek się znajduje na świecie. Płatność dotrze w kilka sekund i będzie kosztować tylko kilka groszy.**Sprawdź to samodzielnie!**

#### Aktywność: Sztafeta Lightning

https://qr.myfirstbitcoin.org/lightning.pdf

**To ćwiczenie praktyczne, w którym uczniowie wysyłają i odbierają prawdziwe saty za pomocą Lightning Network.**

###### Kluczowe punkty

1. Korzystanie z portfela Lightning zwiększy Twoją pewność w odbieraniu i wysyłaniu prawdziwych satów.
1. Zwróć uwagę na jednostki. Niektóre portfele pozwalają użytkownikom wysyłać bitcoiny LUB saty (1/100 000 000 bitcoina).
1. Płatności Lightning mogą czasem utknąć podczas routingu, zwłaszcza przy większych kwotach. Chociaż jest to możliwe, takie doświadczenia użytkownika stają się coraz rzadsze wraz z rozwojem sieci.

###### Wskazówka dla ucznia

Zweryfikuj z instruktorem, czy i jak aktualne opłaty za transakcje on-chain Bitcoin wpłyną na konkretny portfel Lightning, którego używasz.
