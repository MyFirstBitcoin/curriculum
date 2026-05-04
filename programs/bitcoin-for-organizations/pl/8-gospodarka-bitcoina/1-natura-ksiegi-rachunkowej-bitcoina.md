# 8.1 Natura księgi rachunkowej Bitcoina

Rejestr transakcji Bitcoina (nazywany również timechain lub blockchain) to publicznie dostępny, opatrzony znacznikiem czasu zapis każdej ważnej transakcji, która kiedykolwiek miała miejsce w sieci. W tradycyjnym systemie finansowym transakcje wewnętrzne są widoczne tylko dla upoważnionych uczestników, takich jak banki, regulatorzy czy operatorzy danych, tacy jak SWIFT, BACS lub SEPA. Dostęp do danych płatniczych w tradycyjnych systemach może być bardzo ograniczony i kosztowny.

Natomiast w sieci Bitcoin każdy z dostępem do internetu może zobaczyć każdą transakcję – od największych kwot aż po pojedynczego Satoshiego. Uczestnicy mogą śledzić całkowitą podaż bitcoinów w czasie rzeczywistym, monitorować aktywność adresów i portfeli oraz przeglądać nagrody dla górników i zachowania dotyczące opłat. Choć widoczna aktywność w rejestrze jest powiązana z publicznymi adresami kluczy, a nie z tożsamościami osób, możliwe jest agregowanie dużych zbiorów danych dotyczących zachowań wydatkowych, co pozwala każdemu analizować i badać aktywność gospodarczą na bieżąco. W miarę jak sieć rośnie i jest coraz szerzej akceptowana jako źródło prawdy ekonomicznej, możemy obserwować mniejsze uzależnienie od instytucji rządowych i zewnętrznych dostawców w zakresie tworzenia analiz statystycznych i raportów dotyczących zachowań konsumenckich.



#### 8.1.1 Węzły i eksploratory bloków

Każdy, kto chce niezależnie zweryfikować rejestr Bitcoina i uzyskać dostęp do jego danych, powinien uruchomić pełny węzeł. Pełny węzeł jest często opisywany jako najbardziej podstawowy sposób uczestnictwa i weryfikacji gospodarki Bitcoina. Jest dostępny na całym świecie jako oprogramowanie open-source, które po uruchomieniu pobiera i weryfikuje cały rejestr Bitcoina od „Bloku Genesis”, opublikowanego w styczniu 2009 roku, aż do dnia dzisiejszego. Wspiera również bezpieczeństwo sieci Bitcoin, pomagając weryfikować nowe transakcje dodawane do rejestru. Uzyskując dostęp do rejestru Bitcoina w ten sposób, pełny węzeł służy jako źródło prawdy dla badaczy i audytorów sieci. Dla użytkowników Bitcoina pełny węzeł działa jako „samodzielna” brama do informacji transakcyjnych gospodarki Bitcoina, ponieważ zwiększa prywatność i bezpieczeństwo poprzez eliminację zależności od usług stron trzecich.

Podczas gdy pełne węzły pobierają surowe dane, eksploratory bloków, takie jak mempool.space czy blockstream.info, oferują wizualny interfejs do wyszukiwania i interpretowania aktywności w rejestrze. Eksplorator bloków pozwala śledzić poszczególne transakcje oraz przeglądać salda i historię portfeli. Pokazuje także wskaźniki aktywności górników, takie jak nagrody za bloki i dane dotyczące opłat transakcyjnych.

Razem pełne węzły i eksploratory bloków to narzędzia, które sprawiają, że przejrzystość sieci Bitcoin jest użyteczna.



#### 8.1.2 Ćwiczenie: Odkrywanie rejestru Bitcoina

1. Otwórz [mempool.space](https://mempool.space) i przejrzyj stronę główną.
  * Jaka jest wysokość najnowszego bloku?
  * Jaka jest obecna opłata transakcyjna (niski, średni i wysoki priorytet)?
  * Ile transakcji czeka w mempoolu na kolejny blok?
1. Otwórz najnowszy blok w rejestrze.
  * Ile transakcji zostało uwzględnionych?
  * Podaj nazwę górnika tego bloku.
  * Jaka była nagroda za blok?
1. Otwórz jedną z transakcji w bloku.
  * Ile wejść i wyjść ma ta transakcja?
  * Jaka jest wartość transakcji w BTC i PLN?

Omów różnice między sposobem, w jaki pieniądze przemieszczają się w tradycyjnym systemie, a tym, jak firma lub rząd może wykorzystać taką przejrzystość.
