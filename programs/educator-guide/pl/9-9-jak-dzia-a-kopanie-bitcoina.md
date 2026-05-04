# 9 - Jak działa kopanie Bitcoina

Czas trwania: 90 minut

Główna idea: Kopanie Bitcoinów i walidacja przez węzły współpracują, aby zabezpieczyć sieć, potwierdzać transakcje i egzekwować zasady systemu poprzez Proof of Work.

#### Cele nauczania

Po zakończeniu tej lekcji uczniowie powinni być w stanie:

* Wyjaśnić różnicę między rolą węzłów Bitcoin a rolą górników Bitcoin.
* Opisać, jak węzły weryfikują transakcje, udostępniają informacje i pomagają egzekwować zasady Bitcoin.
* Wyjaśnić, czym zajmują się górnicy, w tym wybieranie transakcji, budowanie kandydatów na bloki i rywalizowanie o znalezienie poprawnego hasha bloku.
* Zdefiniować mempool i wyjaśnić, dlaczego działa jak poczekalnia dla niepotwierdzonych transakcji.
* Opisać, jak opłaty transakcyjne wpływają na wybór przez górników i szybkość potwierdzenia.
* Wyjaśnić Proof of Work jako mechanizm, który zabezpiecza Bitcoin, czyniąc ataki kosztownymi.
* Opisać, jak dostosowanie trudności pomaga utrzymać średni czas bloku na poziomie około 10 minut.
* Przeprowadzić przez cały cykl życia transakcji Bitcoin, od utworzenia i podpisania do potwierdzenia w bloku.

#### Narzędzia i zasoby

##### Pomoc wizualna

* Rozdział 9 – Jak działa kopanie Bitcoin?

##### Biblioteka wsparcia

* Karta słownictwa — Rozdział 9 — Terminy: kopanie, Proof of Work, łamigłówka hash, dostosowanie trudności, nagroda za blok, mempool, atak 51%
* Biblioteka błędnych przekonań — Rozdział 9 — Wyjaśnij: „górnicy tworzą Bitcoiny z niczego”, „górnicy kontrolują Bitcoin”, „więcej kopania = mniej bezpieczeństwa”
* Tabele porównawcze i karty referencyjne — Ekonomia kopania: przychody, koszty, zgodność motywacji; dostosowanie trudności
* Techniczne wyjaśnienia i pogłębienia — Bezpieczeństwo Proof of Work; dlaczego atakowanie jest kosztowne; próg 51%

#### Aktywności

* Odkrywanie mempool
* Transakcje w praktyce

#### Nauczanie online

* Użyj jednego przejrzystego diagramu przepływu transakcji od podpisania w portfelu do potwierdzenia.
* Przez całą lekcję utrzymuj wizualne rozdzielenie węzłów i górników na ekranie.
* Użyj mempool.space lub zrzutu ekranu z niego, aby pokazać niepotwierdzone transakcje i presję opłat.
* Zatrzymaj się po każdym etapie procesu kopania i zadaj jedno krótkie pytanie sprawdzające zrozumienie.

#### Przygotowanie

* Przygotuj diagram procesu kopania (mempool → wybór transakcji → tworzenie bloku → dostosowanie trudności) do wyświetlenia.
* Dodaj do zakładek mempool.space lub stronę kopania na blockchain.com; przygotuj zrzuty ekranu z aktualnymi statystykami kopania i dostosowaniami trudności.
* Stwórz wizualne wyjaśnienie Proof of Work jako mechanizmu bezpieczeństwa; pokaż dostosowanie trudności z ostatnich 3–6 miesięcy.

#### Procedura

Ta lekcja przygląda się bliżej temu, jak transakcje Bitcoin przemieszczają się przez sieć i stają się częścią łańcucha bloków. Teraz bezpośrednio podąża za strukturą Dyplomu, więc główne sekcje są zgodne z przewodnikiem dla ucznia, jednocześnie zachowując pełniejsze wyjaśnienia dla nauczyciela w każdej sekcji.

##### 9.0 Wprowadzenie, 8 minut

Rozpocznij od powiązania tego rozdziału z poprzednim:

* Jeśli użytkownik podpisze transakcję kluczem prywatnym, co dzieje się dalej?
* Kto sprawdza, czy ta transakcja jest ważna?
* Jak zostaje dodana do łańcucha bloków?
* Dlaczego Bitcoin potrzebuje zarówno węzłów, jak i górników?

Wyjaśnij, że ten rozdział opisuje, jak sieć przetwarza transakcje w praktyce i jak kopanie zabezpiecza system bez centralnej władzy.

##### 9.1 Węzły i górnicy Bitcoin, 47 minut

**Węzły i górnicy, różne role**

Zacznij od wyraźnego rozdzielenia tych dwóch ról.

Węzły Bitcoin:

* przechowują kopię łańcucha bloków
* weryfikują, czy transakcje są zgodne z zasadami
* udostępniają informacje innym węzłom
* pomagają portfelom i innemu oprogramowaniu uzyskać dostęp do danych z łańcucha bloków
* mogą odrzucać nieprawidłowe transakcje lub nieprawidłowe bloki

Rozdział opisuje węzły jako strażników walidacji i rozwija to poprzez analogię do „cyfrowego policjanta ruchu drogowego”. To pomocne, ponieważ pokazuje węzły jako kontrolerów i koordynatorów, a nie władców. Diagram również podkreśla, że wiele węzłów przechowuje kopie księgi na całym świecie.

Górnicy Bitcoina:

* zbierają prawidłowe transakcje
* tworzą kandydackie bloki
* rywalizują o znalezienie prawidłowego hasha bloku
* rozsyłają prawidłowe bloki, gdy wygrają
* otrzymują nagrody za blok i opłaty transakcyjne

Kluczowym punktem dydaktycznym z rozdziału jest to, że celem kopania nie jest po prostu tworzenie nowych bitcoinów, ale decentralizacja bezpieczeństwa Bitcoina. Nowe bitcoiny są zachętą, natomiast sam proces kopania jest mechanizmem bezpieczeństwa.

**Co faktycznie robią węzły**

Rozwiń sekcję o węzłach, korzystając z listy funkcji węzłów z rozdziału:

* Strażnicy walidacji: sprawdzają, czy transakcje i bloki są zgodne z zasadami
* Centrum komunikacji: łączą się ze sobą i udostępniają dane o transakcjach
* Kontroler jakości: odrzucają nieprawidłowe informacje
* Informator blockchain: dostarczają dane innemu oprogramowaniu, np. portfelom
* Witający nowe węzły: pomagają nowym węzłom uzyskać blockchain, przy czym każdy nowy węzeł i tak samodzielnie weryfikuje dane

To dobry moment, by podkreślić, że uruchomienie własnego węzła daje użytkownikowi większą niezależność. Zamiast całkowicie polegać na zewnętrznych usługach informujących o stanie sieci, mogą to zweryfikować samodzielnie. wyraźnie to podkreśla, w tym wspomina o Bitcoin Core jako jednej z implementacji, którą użytkownicy mogą uruchomić.

**Co faktycznie robią górnicy**

Teraz wyjaśnij kopanie dokładniej.

Górnicy:

* zbierają zweryfikowane, ale niepotwierdzone transakcje
* grupują je w kandydacki blok
* wielokrotnie haszują dane bloku, szukając prawidłowego hasha bloku
* rozsyłają zwycięski blok do sieci
* otrzymują nagrody, jeśli blok zostanie zaakceptowany

Użyj analogii z rozdziału o „ogromnym stogu kluczy”, jeśli to pomaga. Daje ona uczniom konkretne wyobrażenie o wyścigu górników. Główną ideą nie jest to, że górnicy rozwiązują użyteczny problem matematyczny w zwykłym sensie, lecz że udowadniają, iż zużyli rzeczywistą energię i moc obliczeniową, by zabezpieczyć system.

To także odpowiedni moment, by wyjaśnić nagrody dla górników:

* nagroda za blok: nowo wydane bitcoiny
* opłaty transakcyjne: opłaty dołączone do transakcji, które użytkownicy chcą potwierdzić

Wyjaśnij, że górnicy zazwyczaj priorytetowo traktują transakcje z wyższymi opłatami, ponieważ zwiększają one ich nagrodę. Rozdział wyjaśnia tu także halvingi, więc możesz krótko wspomnieć, że nagroda za blok zmniejsza się co 210 000 bloków, czyli mniej więcej co cztery lata, zgodnie z publicznym harmonogramem podaży Bitcoina. Strony 5 i 6 zawierają harmonogram podaży i tabelę nadchodzących halvingów, co może pomóc wzmocnić przewidywalność emisji Bitcoina.

**Prawidłowy hash bloku, Proof of Work i dostosowanie trudności**

Ta sekcja jest sednem rozdziału.

Wyjaśnij, że górnicy szukają prawidłowego hasha bloku, czyli takiego, który spełnia cel sieci. Rozdział tłumaczy to jako znalezienie liczby niższej niż cel ustalony przez sieć.

Następnie jasno wyjaśnij Proof of Work:

* górnicy muszą wykonywać powtarzalną pracę obliczeniową
* ten, kto pierwszy znajdzie prawidłowy hash, udowadnia, że wykonał tę pracę
* to sprawia, że przepisywanie lub atakowanie księgi jest kosztowne
* węzły następnie weryfikują blok przed jego akceptacją

Mocne zdanie do nauczania to:

Proof of Work zabezpiecza Bitcoina, czyniąc nieuczciwość kosztowną, a weryfikację łatwą.

Wyjaśnij także dostosowanie trudności:

* sieć dostosowuje trudność kopania co 2 016 bloków
* dzieje się to mniej więcej co dwa tygodnie
* celem jest utrzymanie średniego czasu bloku blisko 10 minut
* jeśli do sieci dołącza więcej mocy obliczeniowej, trudność rośnie
* jeśli mocy obliczeniowej jest mniej, trudność spada

Strony 7 i 8 wyjaśniają ten proces i pokazują, jak trudniejsze cele wymagają więcej pracy. Pomaga to uczniom zrozumieć, że czas Bitcoina nie jest kontrolowany przez centralny organ, lecz przez zasady protokołu, które automatycznie reagują na warunki sieciowe.

##### 9.2 Czym jest mempool?, 15 minut

Przejdź teraz do mempoola.

Wyjaśnij, że mempool to poczekalnia dla prawidłowych, niepotwierdzonych transakcji. Gdy użytkownik rozsyła transakcję, węzły najpierw ją weryfikują. Jeśli jest prawidłowa, dodają ją do swojego mempoola i udostępniają innym węzłom. Następnie górnicy mogą wybierać spośród tych oczekujących transakcji podczas budowania bloku. Strony 10 i 11 wyjaśniają ten proces bezpośrednio.

Ważne punkty do podkreślenia:

* mempool to nie blockchain
* transakcje tam są nadal niepotwierdzone
* każdy węzeł utrzymuje własny mempool
* nie istnieje jeden uniwersalny mempool
* transakcje z wyższą opłatą mają większą szansę na szybsze wybranie

Rozdział wyjaśnia także typowe powody, dla których transakcja może pozostać długo niepotwierdzona:

* niska opłata
* zator w sieci
* próba podwójnego wydania
* nieprawidłowe lub niekompletne dane
* niepoprawnie sformułowana transakcja

Jeśli to pomocne, wspomnij o ćwiczeniu z mempool.space jako praktycznym sposobie wizualizacji niepotwierdzonych transakcji i stawek opłat. Wyjaśnij też, że mempool.space to tylko jeden z eksploratorów, a nie sam mempool.

##### 9.3 Jak działają transakcje Bitcoin, 20 minut

Teraz połącz wszystko, korzystając z sekwencji krok po kroku z rozdziału.

Jasna wersja do klasy to:



1. Nadawca wybiera UTXO i tworzy transakcję
1. Nadawca dodaje adres odbiorcy i opłatę
1. Nadawca podpisuje transakcję swoim kluczem prywatnym
1. Transakcja jest rozgłaszana do sieci
1. Węzły ją weryfikują i dodają do swoich mempooli
1. Górnicy wybierają ją do kandydującego bloku
1. Górnicy rywalizują poprzez Proof of Work
1. Jeden z górników znajduje poprawny hash bloku i rozgłasza blok
1. Węzły weryfikują blok i dodają go do blockchaina
1. Transakcja otrzymuje potwierdzenia wraz z dodawaniem kolejnych bloków
1. Wyraźnie zaznacz na końcu:
1. gdy transakcja zostanie uwzględniona w poprawnym bloku, jest potwierdzona
1. wydane wejścia nie mogą być już użyte ponownie
1. odbiorca kontroluje teraz nowe UTXO utworzone przez tę transakcję

Diagram podsumowujący jest tutaj szczególnie przydatny, ponieważ wizualnie łączy cały proces od podpisania w portfelu, przez włączenie przez górnika, po weryfikację przez węzeł i dystrybucję bloku.

###### Podsumowanie i sprawdzenie zrozumienia

Zakończ kilkoma szybkimi pytaniami:

* Jaka jest różnica między węzłem a górnikiem?
* Czym jest mempool?
* Dlaczego niektóre transakcje są potwierdzane szybciej niż inne?
* Co udowadnia Proof of Work?
* Dlaczego Bitcoin dostosowuje trudność wydobycia?
* Jakie są główne kroki od wysłania transakcji do otrzymania potwierdzenia?

#### Notatki dla edukatora

Zachowaj jasny główny wątek nauczania: węzły weryfikują, górnicy rywalizują, Proof of Work zabezpiecza, a mempool przechowuje ważne transakcje do czasu ich potwierdzenia.

Ten rozdział może wydawać się techniczny, więc często używaj analogii i diagramów.

Unikaj przedstawiania wydobycia jako „tworzenia bitcoinów z niczego”. Wyjaśnij precyzyjnie, że nagroda to zachęta, a sam proces wydobycia zabezpiecza sieć.

Najważniejsze punkty, na których warto się skupić, jeśli brakuje czasu, to:



1. Różnice między rolami węzła i górnika
1. Mempool jako poczekalnia
1. Proof of Work
1. Dostosowanie trudności
1. Przepływ transakcji od podpisania do potwierdzenia

##### Jak wygląda dobra odpowiedź

* Ważne jest, aby od razu wyjaśnić, że Górnicy ≠ Węzły, pokazać wydobycie jako działalność gospodarczą z realnymi kosztami sprzętu i energii, wykorzystać dostosowanie trudności i Proof of Work do wyjaśnienia mechanizmu bezpieczeństwa oraz sprawdzić zrozumienie na przykładach zmian w sieci.
* Nauczyciele powinni używać rzeczywistych liczb, aby ugruntować dyskusje, być absolutnie jasnymi i powtarzalnymi w kwestii różnicy między górnikami a węzłami, realistycznie podchodzić do obaw związanych z centralizacją w pulach wydobywczych oraz szanować autentyczną złożoność tego zagadnienia.
* Uczniowie rozumieją, że kopanie to inteligentni ludzie wykonujący skomplikowaną pracę, ponieważ zarabiają Bitcoiny, dostrzegają, że motywacje napędzają uczciwe zachowania, bo zyski górników zależą od sukcesu Bitcoina, widzą samoregulację systemu poprzez automatyczną regulację trudności, rozumieją, że kopanie to prawdziwy biznes, a nie działalność charytatywna, i doceniają, że bezpieczeństwo Bitcoina kosztuje prawdziwą energię elektryczną i pieniądze.
* Efekty nauczania zostaną osiągnięte, jeśli uczniowie potrafią odróżnić górników, którzy tworzą bloki, od węzłów, które je weryfikują, rozumieją Proof of Work jako mechanizm bezpieczeństwa, który sprawia, że ataki są wykładniczo droższe, rozpoznają, że regulacja trudności utrzymuje czas bloku na poziomie około 10 minut, rozumieją motywacje górników związane z nagrodami za blok i opłatami, potrafią wyjaśnić, dlaczego atak 51% nie działa, oraz widzą kopanie jako działalność gospodarczą z realnymi kosztami i korzyściami.

##### Zarządzanie czasem

Jeśli czasu jest mało, priorytetowo potraktuj:

* Role węzła i górnika (kluczowa różnica)
* Mempool jako poczekalnia
* Mechanizm Proof of Work
* Regulacja trudności (samoregulujący się system)
* Przepływ transakcji od podpisania do potwierdzenia

Jeśli jesteś do przodu, poświęć czas na:

* Ekonomia kopania i szczegóły sprzętowe
* Dynamika pul wydobywczych i obawy o centralizację
* Scenariusze ataku 51% i dlaczego matematycznie się nie udają
* Długoterminowe bezpieczeństwo dzięki zbieżności motywacji

##### Jeśli uczniowie mają trudności

* Górnicy vs. węzły (zamieszanie) → "Węzły weryfikują, górnicy proponują; sędziowie vs. gracze."
* Proof of Work marnotrawstwo → "Drogi system bezpieczeństwa zapobiega atakom; czyni je bezsensownymi."
* Regulacja trudności → "Więcej górników = szybsze bloki = trudność rośnie; system oddycha."
