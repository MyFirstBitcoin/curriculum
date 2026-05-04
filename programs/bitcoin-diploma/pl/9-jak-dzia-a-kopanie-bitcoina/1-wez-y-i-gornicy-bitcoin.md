# 9.1 Węzły i górnicy Bitcoin

Węzły Bitcoin mogą brzmieć technicznie, ale to po prostu oprogramowanie, które przechowuje kopię łańcucha bloków Bitcoin na komputerze. Łańcuch bloków to wspólny rejestr wszystkich transakcji Bitcoin.

Gdy uruchamiasz własny węzeł, samodzielnie weryfikujesz transakcje Bitcoin, zamiast polegać na kimś innym. Daje Ci to większą niezależność i pomaga utrzymać zdecentralizowaną sieć Bitcoin.

Możesz myśleć o węźle Bitcoin jak o cyfrowym policjancie ruchu drogowego z kilkoma ważnymi zadaniami.

1. Przechowuje kopię łańcucha bloków, czyli historię wszystkich transakcji Bitcoin.
1. Węzły łączą się z innymi węzłami na całym świecie i wymieniają się informacjami. Przykładem jest lista nowych transakcji oczekujących na potwierdzenie, zwana mempoolem.
1. Węzły sprawdzają, czy każda transakcja spełnia zasady Bitcoin. Jeśli transakcja jest nieprawidłowa, węzeł ją odrzuca.

Węzły pomagają także nowym węzłom dołączyć do sieci, udostępniając im łańcuch bloków. Jednak każdy nowy węzeł i tak samodzielnie sprawdza wszystkie zasady.

Każdy może uruchomić węzeł, instalując oprogramowanie takie jak Bitcoin Core i pobierając łańcuch bloków. Po skonfigurowaniu węzeł otrzymuje nowe bloki mniej więcej co 10 minut i weryfikuje je, zanim doda je do swojej kopii łańcucha bloków.

Uruchomienie węzła pomaga zwiększyć bezpieczeństwo i decentralizację sieci Bitcoin, ponieważ więcej osób niezależnie weryfikuje system.

#### Czym jest węzeł Bitcoin?

> Celem kopania nie jest tworzenie nowych bitcoinów; to jest system motywacyjny. Kopanie to mechanizm, dzięki któremu bezpieczeństwo Bitcoin jest zdecentralizowane.  
_Andreas M. Antonopoulos_


> **Callout**
>
> Górnicy zbierają niepotwierdzone transakcje, tworzą blok i zużywają energię, aby znaleźć klucz, który doda i zabezpieczy blok.


Górnicy rywalizują o dodanie kolejnego bloku transakcji do łańcucha bloków. Aby to zrobić, muszą znaleźć specjalną liczbę, która tworzy prawidłowy skrót bloku. Możesz to sobie wyobrazić jak szukanie właściwego klucza wśród miliardów możliwości. Pierwszy górnik, który znajdzie poprawny skrót, wygrywa wyścig i zdobywa prawo do dodania swojego bloku do łańcucha bloków.

Gdy górnik znajdzie prawidłowy skrót, udostępnia swój blok sieci. Inni górnicy szybko weryfikują, czy rozwiązanie jest poprawne. Jeśli tak, blok zostaje dodany do łańcucha bloków, pomagając zabezpieczyć publiczny rejestr Bitcoin.

Górnicy zarabiają bitcoiny na dwa sposoby:

* **Nagrody za blok:** Nowe bitcoiny są tworzone i przekazywane górnikowi, który pomyślnie doda blok do łańcucha bloków.
* **Opłaty transakcyjne:** Gdy ludzie wysyłają bitcoiny, dołączają niewielką opłatę. Górnik, który doda blok, otrzymuje opłaty z transakcji zawartych w tym bloku.

#### Halvingi Bitcoina


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12,5 BTC | 6,25 BTC | 3,125 BTC |



> **Callout**
>
> Nagrody dla górników za ukończenie jednego bloku zmniejszają się o połowę co 210 000 bloków, czyli mniej więcej co cztery lata.


Bitcoin ma stałą maksymalną podaż wynoszącą 21 000 000 bitcoinów, ale nie wszystkie zostały stworzone na początku istnienia Bitcoin. Zamiast tego nowe bitcoiny są stopniowo wprowadzane do obiegu poprzez **kopanie**.

Gdy górnicy pomyślnie dodadzą nowy blok transakcji do sieci Bitcoin, otrzymują **nagrodę za blok** w bitcoinach. W początkowych latach Bitcoin nagroda ta wynosiła 50 bitcoinów za blok. Ta nagroda zachęcała ludzi do używania mocy obliczeniowej i energii elektrycznej, aby pomóc zabezpieczyć sieć.

Mniej więcej co 210 000 bloków (czyli co około 4 lata) nagroda za blok jest zmniejszana o połowę. To wydarzenie nazywa się **halvingiem**. Halving spowalnia tworzenie nowych bitcoinów i pomaga zapewnić, że całkowita podaż nigdy nie przekroczy 21 milionów. Z czasem sprawia to, że bitcoin staje się coraz bardziej rzadki.


> **Definition – Podaż w obiegu**
>
> **Podaż w obiegu** odnosi się do całkowitej dostępnej ilości danej waluty. W przypadku Bitcoina całkowita podaż w obiegu to liczba monet, które zostały wykopane i znajdują się w obiegu w danym momencie.


![ Bitcoin Supply Schedule](https://cdn.sanity.io/images/vje9ehw2/staging/1d323c57922fdd96fb9ac2f46c505218afe7f342-292x200.svg)


> **Definition – Harmonogram podaży Bitcoina**
>
> **Harmonogram podaży Bitcoina** to z góry ustalony i publiczny plan wprowadzania nowych bitcoinów do obiegu, zaprojektowany tak, aby utrzymać rzadkość Bitcoina w czasie.


Po każdym halvingu nagroda w bitcoinach, którą górnicy otrzymują za dodanie bloku, jest zmniejszana o połowę. To zmniejsza tempo tworzenia nowych bitcoinów.

Górnicy nadal zarabiają opłaty transakcyjne z transakcji zawartych w wydobytym przez nich bloku. Z czasem oczekuje się, że opłaty te staną się większą częścią dochodów górników.

Halvingi są wbudowane w protokół Bitcoina i odbywają się automatycznie mniej więcej co cztery lata. Dzięki temu harmonogram podaży Bitcoina jest przewidywalny i przejrzysty.

Tabela przedstawia nadchodzące halvingi, w tym przybliżoną datę, numer bloku, w którym nastąpią, nową nagrodę za blok oraz procent całkowitej podaży bitcoinów, który zostanie już wydobyty.


| Wydarzenie | Data | Blok | Nagroda | Wydobyto |
| --- | --- | --- | --- | --- |
| 5. Halving | 2028 | 1 050 000 | 1,5625 BTC | 98,44 % |
| 6. Halving | 2032 | 1 260 000 | 0,78125 BTC | 99,22 % |
| 7. Halving | 2036 | 1 470 000 | 0,390625 BTC | 99,61 % |


W miarę wydobywania kolejnych bitcoinów, ilość bitcoinów w obiegu stale rośnie, aż do osiągnięcia maksymalnej podaży 21 000 000 bitcoinów, co przewiduje się na około rok 2140. Ponieważ z czasem powstaje coraz mniej nowych bitcoinów, jeśli popyt wzrośnie, cena Bitcoina może wzrosnąć. To również zachęca górników do dalszego zabezpieczania sieci poprzez udostępnianie swojej mocy obliczeniowej.

#### Czym jest prawidłowy hash bloku w Bitcoinie?

W sieci Bitcoin górnicy rywalizują, aby znaleźć specjalny kod zwany **hashem bloku**. Ten kod identyfikuje blok transakcji i pozwala na jego dodanie do łańcucha bloków.

Każdy blok zawiera informacje o ostatnich transakcjach oraz hash poprzedniego bloku. Łączy to wszystkie bloki ze sobą, tworząc łańcuch od pierwszego bloku (Genesis Block) aż do najnowszego.

Hash działa jak **cyfrowy odcisk palca** dla danych w bloku. Jeśli jakakolwiek informacja w bloku zostałaby zmieniona, odcisk palca również by się zmienił. Dzięki temu każdy może łatwo zweryfikować, że historia transakcji w blockchainie nie została zmieniona, co pomaga utrzymać bezpieczeństwo sieci.


> **Callout**
>
> Satoshi Nakamoto, twórca Bitcoina, wydobył Genesis Block, który odblokował łącznie 50 bitcoinów.


#### Wyścig o wydobycie bloku

Górnicy rywalizują, aby znaleźć prawidłowy hash bloku. Pierwszy górnik, który go znajdzie, może dodać nowy blok do blockchaina i otrzymać nagrodę w bitcoinach.

Aby hash bloku był prawidłowy, musi być niższy od liczby ustalonej przez sieć, zwanej celem trudności. Ponieważ hashe są losowe, górnicy muszą próbować różnych danych wejściowych, aż znajdą odpowiedni wynik.

Jeśli zbyt wielu górników rywalizuje, bloki byłyby znajdowane zbyt szybko. Jeśli zbyt mało górników uczestniczy, znalezienie bloków trwałoby zbyt długo. Aby system działał płynnie, Bitcoin automatycznie dostosowuje poziom trudności co 2 016 bloków (czyli mniej więcej co dwa tygodnie).

To dostosowanie zapewnia, że średnio nowy blok jest dodawany do blockchaina co około 10 minut.


> **Definition – Definicja poziomu trudności**
>
> Poziom **trudności** w kopaniu Bitcoina mierzy, jak trudno jest znaleźć prawidłowy hash bloku. Sieć dostosowuje ten poziom trudności co 2 016 bloków (czyli mniej więcej co dwa tygodnie), aby nowe bloki były dodawane do blockchaina co około 10 minut. Im wyższy poziom trudności, tym trudniej górnikom znaleźć prawidłowy blok.


Znajdując prawidłowy hash bloku, górnik udowadnia, że wykonał pracę wymaganą do dodania nowego bloku do blockchaina. Ten proces nazywa się **Proof of Work** (PoW). To mechanizm bezpieczeństwa, który pozwala Bitcoinowi potwierdzać transakcje i dodawać nowe bloki do blockchaina. Górnik, który jako pierwszy znajdzie prawidłowy hash, otrzymuje nagrodę w bitcoinach, która obejmuje nagrodę za blok oraz opłaty transakcyjne z transakcji zawartych w tym bloku.

Proof of Work (PoW) pomaga utrzymać bezpieczeństwo Bitcoina, ponieważ sprawia, że próba oszukania lub przejęcia kontroli nad siecią jest niezwykle kosztowna. Zamiast tego znacznie bardziej opłaca się przestrzegać zasad.

Górnicy pełnią cztery główne role:

1. **Zbierają transakcje**: Górnicy wybierają transakcje przesłane do sieci i umieszczają je w kandydackim bloku.
1. **Wykonują Proof of Work**: Górnicy rywalizują, aby rozwiązać trudną zagadkę matematyczną, znajdując prawidłowy hash bloku.
1. **Rozgłoś blok**: Pierwszy górnik, który znajdzie poprawne rozwiązanie, udostępnia nowy blok w sieci.
1. **Zarabiaj nagrody**: Jeśli blok jest poprawny, zostaje dodany do łańcucha bloków, a górnik otrzymuje nowo utworzone bitcoiny oraz opłaty transakcyjne.

Wielu górników na całym świecie próbuje jednocześnie stworzyć kolejny blok. Gdy jeden z nich znajdzie poprawne rozwiązanie, sieć sprawdza blok. Jeśli wszystko się zgadza, blok zostaje dodany do łańcucha bloków. Inne konkurencyjne bloki są odrzucane. Ten proces utrzymuje zgodność sieci i zapobiega podwójnemu wydawaniu.

* Górnicy to komputery, które pomagają utrzymywać i aktualizować księgę Bitcoin.
* Zbierają transakcje i grupują je w blok. Następnie przepuszczają dane bloku przez algorytm haszujący, aby stworzyć unikalny kod zwany hashem.
* Górnicy powtarzają ten proces wiele razy, szukając hasha, który spełnia zasady Bitcoin. Pierwszy górnik, który znajdzie poprawny hash, otrzymuje nowo utworzone bitcoiny jako nagrodę, a jego blok zostaje dodany do łańcucha bloków.
* Hash każdego bloku łączy go także z poprzednim blokiem. Gdyby ktoś próbował zmienić wcześniejszą transakcję, hashe przestałyby się zgadzać i sieć odrzuciłaby zmieniony łańcuch. To właśnie zapewnia bezpieczeństwo księgi Bitcoin.
