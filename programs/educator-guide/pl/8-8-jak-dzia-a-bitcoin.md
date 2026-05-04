# 8 - Jak działa Bitcoin

Czas trwania: 90 minut

Główna idea: Bezpieczeństwo Bitcoina opiera się na prostych, ale potężnych rozwiązaniach technicznych, takich jak klucze, podpisy, haszowanie i UTXO, które umożliwiają własność i weryfikację bez centralnej instytucji.

#### Cele nauczania

Po zakończeniu tej lekcji uczniowie powinni być w stanie:

* Wyjaśnić, w jaki sposób klucze publiczne i prywatne pomagają zabezpieczyć własność i transakcje Bitcoina.
* Opisać, czym jest podpis cyfrowy i jak dowodzi, że transakcja została autoryzowana przez prawowitego właściciela.
* Wyjaśnić prostym językiem, co oznaczają kryptografia, szyfrowanie i deszyfrowanie w kontekście Bitcoina.
* Zdefiniować haszowanie i opisać, dlaczego funkcje skrótu są ważne dla bezpieczeństwa i integralności danych Bitcoina.
* Wskazać podstawowe cechy funkcji skrótu, takie jak stała długość wyjścia, jednokierunkowość i wrażliwość na drobne zmiany wejścia.
* Wyjaśnić model UTXO oraz jak bitcoin jest wydawany, otrzymywany i zwracany jako reszta poprzez wyjścia transakcji.
* Opisać, jak węzły pomagają zapobiegać podwójnemu wydawaniu poprzez sprawdzanie, czy dane wyjście zostało już wydane.

#### Narzędzia i zasoby

##### Pomoc wizualna

* Rozdział 8 – Jak działa Bitcoin

##### Biblioteka wsparcia

* Karta słownictwa — Rozdział 8 — Terminy: kryptografia, hash, UTXO, podpis cyfrowy, klucz prywatny/publiczny, drzewo Merkle’a, blockchain
* Biblioteka błędnych przekonań — Rozdział 8 — Tematy: „zgubioną frazę seed można odzyskać”, „klucz prywatny = hasło”, „blockchain jest anonimowy”
* Techniczne wyjaśnienia i pogłębienia — Funkcje skrótu, klucze publiczne/prywatne, model UTXO, bezpieczeństwo Proof of Work

#### Aktywności

* Transakcje w praktyce
* Odkrywanie mempoola

#### Nauczanie online

* Użyj cyfrowej tablicy i rysuj każdy koncept na żywo, zamiast polegać wyłącznie na wyjaśnieniach ustnych.
* Ucz jedną techniczną ideę na raz i często rób przerwy na pytania sprawdzające.
* Używaj wizualizacji dla kluczy, podpisów, hashy i UTXO, aby uczniowie mogli śledzić strukturę.
* Skup się na zrozumieniu koncepcji i unikaj zbyt głębokiego wchodzenia w matematykę lub żargon.

#### Przygotowanie

* Przygotuj i zalaminuj diagramy: pary kluczy publiczny/prywatny, podpisy cyfrowe, model UTXO, haszowanie (funkcja jednokierunkowa).
* Dodaj do zakładek eksplorator blockchain i kalkulator hash SHA-256; wybierz 2-3 prawdziwe transakcje Bitcoina do przejścia krok po kroku.
* Przygotuj notatki na tablicę do wyjaśnienia wejść, wyjść i jak transakcje są potwierdzane w blockchainie.

#### Procedura

Ta lekcja daje uczniom pierwsze spojrzenie na techniczną stronę Bitcoina bez zakładania wcześniejszej wiedzy technicznej. Przewodnik teraz podąża za tą samą skróconą strukturą co Dyplom, z kryptografią pod jednym nagłówkiem i UTXO pod drugim.

##### 8.0 Wprowadzenie, 8 minut

Na początek ustal oczekiwania:

* Co sprawia, że Bitcoin jest bezpieczny, skoro nie kontroluje go żaden bank centralny?
* Jak sieć może wiedzieć, czy dana osoba naprawdę posiada bitcoiny, które próbuje wysłać?
* Co tak naprawdę dzieje się „za kulisami”, gdy ktoś wykonuje transakcję Bitcoin?

Wyjaśnij, że ten rozdział skupia się na podstawowych technicznych fundamentach Bitcoina, szczególnie kluczach, podpisach, haszowaniu i UTXO. Uspokój też uczniów, że nie muszą zostać inżynierami, aby zrozumieć podstawową logikę. Sam rozdział jasno to podkreśla, porównując Bitcoina do internetu – wielu ludzi korzysta z niego codziennie, nie rozumiejąc wszystkich warstw pod spodem.

##### 8.1 Bezpieczeństwo dzięki kryptografii, 57 minut

**Bitcoin jako księga przechowywana na wielu komputerach**

Zacznij od prostego ujęcia sieci Bitcoin z rozdziału:

* Bitcoin to zapis transakcji
* ten zapis jest przechowywany na wielu komputerach zwanych węzłami
* księga jest publiczna i pseudonimowa
* pokazuje adresy i historię transakcji, a nie dane osobowe

Ta sekcja pomaga uczniom nawiązać do tego, co już wiedzą z wcześniejszych rozdziałów. Bitcoin nie opiera się na ukrytych kontach w banku. Opiera się na wspólnej księdze, którą wielu uczestników może zweryfikować. jest tu szczególnie pomocny, bo pokazuje użytkowników, portfele i szerszą sieć Bitcoina połączoną z publiczną księgą.

**Klucze publiczne i prywatne**

Teraz przejdź do kryptografii.

Wyjaśnij, że każdy użytkownik Bitcoina ma:

* klucz prywatny, który musi pozostać tajny
* klucz publiczny, który można udostępniać

Wyjaśnij ich cel prostymi słowami:

* klucz prywatny potwierdza kontrolę i upoważnia do wydania środków
* klucz publiczny pomaga innym zweryfikować, że transakcja została prawidłowo autoryzowana

Silnym punktem dydaktycznym tego rozdziału jest to, że Bitcoin używa kryptografii klucza publicznego/prywatnego, a nie starszego modelu, w którym dwie osoby muszą najpierw podzielić się tym samym tajnym kluczem. To ważne, ponieważ pozwala na bezpieczną weryfikację bez konieczności ujawniania sekretu chroniącego środki użytkownika.

Możesz to wyjaśnić w ten sposób:

* klucz prywatny to jak tajny dowód, że bitcoin należy do ciebie
* klucz publiczny to część tego, co pozwala sieci zweryfikować twoje upoważnienie
* kto kontroluje klucz prywatny, ten ma możliwość wydania bitcoina

Uważaj, aby nie komplikować zbytnio języka szyfrowania. Najważniejszy punkt dla uczniów to własność i upoważnienie.

**Podpisy cyfrowe i autoryzacja transakcji**

Teraz wyjaśnij, co się dzieje, gdy ktoś wysyła bitcoina.

Użyj kolejności z rozdziału:

* użytkownik tworzy transakcję
* nadawca generuje podpis cyfrowy za pomocą swojego klucza prywatnego
* transakcja jest rozgłaszana w sieci
* węzły weryfikują, czy podpis jest ważny
* po weryfikacji i potwierdzeniu własność jest przenoszona w rejestrze

Wyjaśnij wyraźnie, że podpis cyfrowy to nie to samo, co wpisanie swojego imienia. To kryptograficzny dowód, że prawdziwy właściciel autoryzował transakcję. To jeden z kluczowych mechanizmów, które pozwalają Bitcoinowi działać bez centralnej instytucji zatwierdzającej transakcje ręcznie. Diagram jest przydatny, bo wizualnie pokazuje podpisywanie i weryfikację, a także ścieżkę transakcji od nadawcy do walidacji w sieci.

Dobre zdanie na lekcję to:

Transakcje bitcoin nie są zatwierdzane dlatego, że bank tak mówi. Są akceptowane, ponieważ sieć może zweryfikować ważny kryptograficzny dowód.

**Haszowanie i funkcje jednokierunkowe**

Następnie wyjaśnij haszowanie.

Zacznij prosto:

* funkcja przyjmuje dane wejściowe i generuje wynik
* funkcja jednokierunkowa jest łatwa do wykonania w jedną stronę, ale praktycznie niemożliwa do odwrócenia
* funkcja skrótu (hashująca) przyjmuje dane dowolnej wielkości i zamienia je na wynik o stałej długości zwany haszem

Użyj jednej z analogii z rozdziału, tej, która będzie najjaśniejsza dla twojej grupy:

* analogia smoothie dla funkcji jednokierunkowych
* analogia odcisku palca dla haszy
* analogia partytury muzycznej do sprawdzania, czy coś się zmieniło

Analogia odcisku palca jest prawdopodobnie najjaśniejsza dla większości klas:

* hasz to jak cyfrowy odcisk palca dla danych
* jeśli dane wejściowe zmienią się choćby minimalnie, hasz zmienia się całkowicie
* to pomaga komputerom sprawdzać integralność i wykrywać manipulacje

Następnie wyjaśnij, dlaczego haszowanie jest ważne w Bitcoinie:

* transakcje są haszowane
* sieć używa haszy do weryfikacji integralności
* jeśli transakcja zostanie zmieniona, hasz się zmienia
* to pomaga chronić rejestr przed niezauważoną manipulacją

Ilustracje na stronach 7–10 są tutaj bardzo przydatne. Rozdział pokazuje zarówno ideę wyniku o stałej długości, jak i zasadę „mała zmiana, zupełnie inny wynik”, co jest jednym z najważniejszych pojęć do zrozumienia przez uczniów.

**Podstawowe właściwości funkcji skrótu**

Krótko omów właściwości podkreślone w rozdziale, nie czyniąc ich zbyt akademickimi:

* Deterministyczność: te same dane wejściowe zawsze dają ten sam wynik
* Jednokierunkowość / odporność na pre-image: nie da się realistycznie odwrócić procesu
* Wrażliwość na zmiany: nawet mała zmiana wejścia daje zupełnie inny wynik
* Odporność na kolizje: niezwykle trudno znaleźć dwa różne wejścia o tym samym wyniku
* Szybkość weryfikacji: funkcja działa i sprawdza się wydajnie

Nie musisz wymagać od uczniów zapamiętania wszystkich terminów, ale powinni rozumieć ogólną ideę: haszowanie daje Bitcoinowi niezawodny sposób identyfikacji danych i wykrywania zmian.

##### 8.2 Model UTXO, 25 minut

**Model UTXO**

Teraz przejdź do drugiej głównej części rozdziału: UTXO, czyli niewydane wyjścia transakcji.

Wyjaśnij to prostymi słowami, używając analogii z gotówką z tego rozdziału:

* bitcoin nie jest śledzony jak saldo na koncie bankowym
* zamiast tego składa się z wydawalnych części zwanych UTXO
* kiedy wydajesz bitcoina, używasz jednego lub kilku istniejących UTXO jako wejść
* następnie tworzone są nowe UTXO jako wyjścia

Użyj przykładu z rozdziału:

* jeśli masz UTXO o wartości 10 BTC
* i wysyłasz 6 BTC
* nowe UTXO o wartości 6 BTC trafia do odbiorcy
* nowe UTXO reszty wraca do Ciebie
* niewielka część jest płacona jako opłata dla górnika

To pomaga uczniom zobaczyć, że Bitcoin działa bardziej jak wydawanie gotówki i otrzymywanie reszty niż odejmowanie liczb z prostego salda konta. Diagramy są tutaj szczególnie pomocne, ponieważ wizualnie pokazują, jak jedno UTXO jest dzielone na wyjście do odbiorcy, wyjście reszty i opłatę.

Wyraźnie zaznacz dwa kluczowe punkty:

* saldo Twojego portfela to suma Twoich UTXO
* kiedy wydajesz, stare UTXO są zużywane, a nowe tworzone

**Zapobieganie podwójnemu wydawaniu**

Zakończ treść, wyjaśniając jedno z najważniejszych następstw modelu UTXO.

Jeśli ktoś spróbuje wydać to samo wyjście dwa razy, węzły odrzucą drugą próbę, ponieważ utrzymują księgę i mogą zweryfikować, czy dane UTXO zostało już wydane. Tak właśnie Bitcoin zapobiega podwójnemu wydawaniu bez potrzeby istnienia centralnej firmy płatniczej zarządzającej zapisami. Przykład jest tutaj bardzo przydatny, ponieważ pokazuje krok po kroku, jak Alicja łączy UTXO, wysyła środki do Bartka, otrzymuje resztę i jak potwierdzona transakcja aktualizuje księgę na wszystkich węzłach.

Jasny sposób, by powiedzieć to na lekcji, to:

Bitcoin zapobiega podwójnemu wydawaniu, ponieważ sieć śledzi, które wyjścia pozostają niewydane, a które już zostały użyte.

###### Podsumowanie i sprawdzenie zrozumienia

Zakończ kilkoma szybkimi pytaniami:

* Jaka jest różnica między kluczem publicznym a prywatnym?
* Co udowadnia podpis cyfrowy?
* Dlaczego haszowanie jest przydatne w Bitcoinie?
* Co się stanie, jeśli transakcja zostanie zmieniona po jej zhashowaniu?
* Czym jest UTXO w prostych słowach?
* Jak sieć powstrzymuje kogoś przed wydaniem tego samego bitcoina dwa razy?

#### Notatki dla edukatora

Ten rozdział zawiera więcej technicznego języka niż wcześniejsze, więc priorytetem powinny być jasność, analogie i powtórzenia.

Celem nie jest uczynienie z uczniów programistów. Celem jest pomóc im zrozumieć, dlaczego bezpieczeństwo Bitcoina działa.

Najważniejsze punkty, na których należy się skupić, jeśli brakuje czasu, to:

* klucz prywatny vs klucz publiczny
* podpisy cyfrowe
* do czego służy haszowanie
* UTXO jako wydawalne części bitcoina
* jak zapobiega się podwójnemu wydawaniu

Najbardziej przydatne wizualizacje w tym rozdziale to:

* diagram użytkownik-portfel-sieć
* wizualizacja podpisu cyfrowego
* przykłady haszowania i diagramy stałej długości wyjścia na stronach 7–10
* diagramy UTXO na stronach 10–12

##### Jak wygląda dobra odpowiedź

* Ważne jest, aby traktować kryptografię jako fundament, a nie tajemnicę, używać wielu wizualizacji, unikać głębokiej matematyki, nawiązywać do wcześniejszych rozdziałów i sprawdzać zrozumienie poprzez zastosowania, np. „Co się stanie, jeśli ktoś zmieni jedną transakcję?”
* Nauczyciele powinni być cierpliwi wobec uczniów, którzy mają trudności, myśleć wizualnie i wszystko rysować, być szczerzy co do tego, czego uczniowie nie muszą rozumieć, być gotowi powiedzieć „Nie wiem, ale oto jak byśmy to sprawdzili” i przez cały czas zachęcać.
* Uczniowie rozumieją, dlaczego Bitcoin nie może zostać zhakowany, ponieważ chroni go matematyka, doceniają elegancki projekt systemu, czują się swobodnie złożonością wiedząc, że nie muszą znać każdego szczegółu, zyskują pewność w zadawaniu pytań bez oceniania i rozpoznają, że osiągnęli wyższy poziom zrozumienia czegoś, czego większość ludzi nie rozumie.
* Efekty uczenia się powinny zostać osiągnięte, jeśli uczniowie potrafią wyjaśnić podstawy kryptografii, takie jak funkcje jednokierunkowe i podpisy cyfrowe bez głębokiej matematyki, rozumieją model UTXO pokazujący, że posiadają monety, a nie konta, rozpoznają haszowanie jako fundament bezpieczeństwa Bitcoina, rozumieją anatomię transakcji, w tym podpisy i potwierdzenia, wyjaśniają, dlaczego Bitcoin jest niezmienny, oraz zadają krytyczne pytania o potencjalne ataki lub podatności.

##### Zarządzanie czasem

Jeśli brakuje czasu, priorytetowo potraktuj:

* Klucz prywatny vs klucz publiczny
* Podpisy cyfrowe
* Do czego służy haszowanie
* UTXO jako wydzielone, możliwe do wydania części bitcoina
* Jak zapobiega się podwójnemu wydawaniu

Jeśli masz zapas czasu, poświęć uwagę:

* Schemat użytkownik-portfel-sieć i wizualny model bezpieczeństwa
* Wizualizacja podpisu cyfrowego: szczegółowy proces kryptograficzny
* Drzewa Merkle’a i bezpieczeństwo łańcucha
* Zaawansowane wektory ataku i dlaczego zawodzą

##### Jeśli uczniowie mają trudności

* Kryptografia wydaje się groźna → „Używasz jej na co dzień; My First Bitcoin korzysta z niej w ten sam sposób.”
* Haszowanie jako pojęcie → Analogia do odcisku palca; unikalny, nie da się zmienić bez zmiany hasza.
* Podpisy cyfrowe → „Dowód autoryzacji bez ujawniania hasła.”
