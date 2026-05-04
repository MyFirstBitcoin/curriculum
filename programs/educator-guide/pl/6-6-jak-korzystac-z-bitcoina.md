# 6 - Jak korzystać z Bitcoina

Czas trwania: 90 minut

Główna idea: Korzystanie z Bitcoina na łańcuchu bloków uczy uczniów, jak w praktyce działa własność, samodzielna kontrola i weryfikacja, zamieniając teorię w bezpośrednie działanie finansowe.

#### Cele nauczania

Po zakończeniu tej lekcji uczniowie powinni być w stanie:

* Wskazać popularne sposoby zdobywania i wymiany bitcoina, w tym metody peer-to-peer oraz scentralizowane giełdy.
* Wyjaśnić różnicę między portfelami samodzielnymi a powierniczymi oraz dlaczego samodzielna kontrola jest ważna w Bitcoinie.
* Opisać cel kluczy prywatnych, publicznych adresów, fraz seed oraz interfejsów portfeli.
* Porównać różne typy portfeli i ocenić ich zalety i wady pod względem bezpieczeństwa, wygody, prywatności i kontroli.
* Skonfigurować mobilny portfel Bitcoin i wyjaśnić podstawowy proces odzyskiwania.
* Zademonstrować, jak otrzymać i wysłać transakcję bitcoin na łańcuchu bloków.

Zastosować zasadę „Nie ufaj, weryfikuj” przy wyborze portfela, transakcjach i szerszym korzystaniu z Bitcoina.

#### Narzędzia i zasoby

##### Pomoc wizualna

* Rozdział 6 – Jak korzystać z Bitcoina

##### Biblioteka wsparcia

* Karta słownictwa — Rozdział 6 — Terminy: portfel, klucz prywatny, adres publiczny, fraza seed, powierniczy, samodzielny, UTXO, opłata transakcyjna
* Tabele porównawcze i karty referencyjne — Porównanie typów portfeli (powierniczy, mobilny, sprzętowy, papierowy)
* Techniczne wyjaśnienia i pogłębienia — Klucze publiczne/prywatne, model UTXO, potwierdzanie transakcji
* Pogłębienie bezpieczeństwa klucza prywatnego — Frazy seed, pochodzenie kluczy, metody kopii zapasowych, wektory ataku
* Przewodnik po anatomii transakcji — Przykład krok po kroku, jak działa transakcja Bitcoin
* Lista najlepszych praktyk bezpieczeństwa — Przed rozpoczęciem, tworzenie portfela, odbieranie, wysyłanie, zapobieganie phishingowi

#### Aktywności

* Transakcje w praktyce
* Wyścig sztafetowy Lightning
* Odkrywanie mempoola

#### Nauczanie online

* Od początku jasno określ, czy uczniowie oglądają demonstrację, czy samodzielnie konfigurują portfel.
* Używaj dużych, czytelnych zrzutów ekranu dla każdego kroku konfiguracji portfela.
* Zatrzymuj się po każdym kroku i poproś uczniów o potwierdzenie zrozumienia na czacie przed kontynuacją.
* Daj bezpośrednie ostrzeżenie przed sekcją dotyczącą frazy seed i przypomnij uczniom, aby nigdy nie udostępniali wrażliwych informacji online.

#### Przygotowanie

* Pobierz i przetestuj aplikację mobilnego portfela (Blue Wallet lub Muun); przygotuj zrzuty ekranu kluczowych etapów konfiguracji.
* Przygotuj przewodnik konfiguracji portfela (pobierz → utwórz → kopia zapasowa seed → odbierz) do wykorzystania jako odniesienie.
* Upewnij się, że sieć/WiFi działa; przygotuj adres demonstracyjny i kod QR do pokazania.

#### Procedura

Ta lekcja przechodzi od teorii do bezpośredniej praktyki. Teraz odpowiada bezpośrednio strukturze Dyplomu, tak aby zdobywanie, portfele, konfiguracja, transakcje i weryfikacja pojawiały się pod tymi samymi głównymi nagłówkami co przewodnik ucznia. Dodatkowe wsparcie dydaktyczne pozostaje zagnieżdżone w tych sekcjach.

##### 6.0 Wprowadzenie, 8 minut

Rozpocznij, łącząc ten rozdział z poprzednim:

* Jeśli Bitcoin to pieniądz, to jak ludzie faktycznie go zdobywają i używają?
* Co to znaczy naprawdę kontrolować swojego bitcoina?
* Dlaczego korzystanie z Bitcoina różni się od korzystania z aplikacji bankowej?

Wyjaśnij, że ten rozdział dotyczy praktycznego użycia. Uczniowie nie uczą się już tylko, czym jest Bitcoin, ale jak bezpośrednio z nim się kontaktować.

##### 6.1 Zdobywanie i wymiana Bitcoina, 12 minut

Wyjaśnij, że ludzie mogą zdobywać bitcoina na różne sposoby, w tym:

* otrzymywanie wynagrodzenia w bitcoinie
* kopanie bitcoina
* wymiana waluty fiducjarnej na bitcoina osobiście
* wymiana waluty fiducjarnej na bitcoina online

Następnie skup się na dwóch głównych sposobach zdobywania opisanych w rozdziale:

* peer-to-peer, osobiście
* peer-to-peer, online
* scentralizowane giełdy

Wyjaśnij jasno kompromisy.

W przypadku P2P osobiście podkreśl bezpośrednią wymianę bez udziału banku lub pośrednika, ale wspomnij także o praktycznych zagrożeniach związanych ze spotkaniami w celu wymiany gotówki.

Dla P2P online wyjaśnij pojęcie escrow prostymi słowami, jako sposób na zmniejszenie ryzyka drugiej strony przy jednoczesnym umożliwieniu bezpośredniej wymiany między osobami.

W przypadku scentralizowanych giełd wyjaśnij, że są wygodne, ale wymagają zaufania do firmy, często udostępnienia danych osobowych oraz pozostawienia środków pod kontrolą strony trzeciej do momentu wypłaty. To dobry moment, aby podkreślić, że wygoda często wiąże się z kompromisami w zakresie prywatności i suwerenności.

##### 6.2 Wprowadzenie do portfeli Bitcoin, 35 minut

**Czym naprawdę jest portfel Bitcoin**

Od razu wyjaśnij powszechne nieporozumienie: bitcoin nie jest przechowywany w aplikacji portfela jak gotówka w torbie.  
Bitcoin istnieje w księdze prowadzonej przez sieć. Użytkownik kontroluje możliwość wydania go za pomocą kluczy prywatnych.

Następnie wyjaśnij dwie rzeczy, które ludzie często mają na myśli, mówiąc "portfel":

* system kluczy prywatnych, z którego generowane są adresy
* aplikacja lub interfejs używany do interakcji z siecią

Użyj analogii z e-mailem z tego rozdziału, jeśli to pomocne:

* adres publiczny = jak adres e-mail, który możesz udostępnić
* klucz prywatny = jak hasło, które musisz chronić

Bądź tutaj bardzo jasny: ten, kto kontroluje klucze prywatne, kontroluje bitcoiny. To jest kluczowa koncepcja, którą uczniowie muszą zrozumieć.

**Portfele samodzielne a powiernicze**

To jedna z najważniejszych części rozdziału.

Wyjaśnij wyraźnie różnicę:

* Portfel samodzielny: użytkownik kontroluje klucze prywatne
* Portfel powierniczy: strona trzecia kontroluje klucze prywatne w imieniu użytkownika

Następnie omów kompromisy:

Samodzielny

* pełna kontrola nad środkami
* brak procesu zatwierdzania
* ochrona przed arbitralną konfiskatą
* większa odpowiedzialność
* brak łatwego odzyskania w przypadku utraty frazy seed

Powierniczy

* łatwiejsze odzyskiwanie i wsparcie
* prostszy dla początkujących
* większa podatność na zamrożenie konta, ataki hakerskie i kontrolę przez stronę trzecią
* użytkownik nie posiada naprawdę bitcoinów

To właściwy moment, aby podkreślić frazę:

"Nie twoje klucze, nie twoje monety."

Uczniowie powinni po tej części rozumieć nie tylko hasło, ale także, co ono oznacza w praktyce.

**Różne typy portfeli i jak wybrać odpowiedni**

Przedstaw typy portfeli omawiane w rozdziale:

* portfel online
* portfel mobilny
* portfel na komputer
* portfel sprzętowy
* portfel papierowy

Nie traktuj żadnego jako idealnego. Zamiast tego wyjaśnij, że każdy z nich wiąże się z kompromisami pomiędzy:

* bezpieczeństwem
* prywatnością
* wygodą
* kompatybilnością
* opłatami
* kontrolą
* reputacja

Wyjaśnij również, że zalecamy zwracanie uwagi na to, czy oprogramowanie portfela jest open-source, ponieważ narzędzia open-source mogą być przeglądane, audytowane i rozwijane przez społeczność. To bezpośrednio łączy się z zasadą weryfikacji w Bitcoinie.

##### 6.3 Konfigurowanie mobilnego portfela Bitcoin, 10 minut

Przeprowadź uczniów przez podstawowy proces pokazany w rozdziale:

* pobierz portfel
* utwórz nowy portfel
* wygeneruj i zapisz frazę odzyskiwania
* potwierdź frazę odzyskiwania
* dodaj dodatkowe zabezpieczenia, jeśli są dostępne
* otwórz portfel i znajdź funkcję odbioru

Wyraźnie podkreśl ostrzeżenie dotyczące frazy seed:

* jeśli fraza seed zostanie zgubiona, dostęp do środków może zostać utracony
* jeśli ktoś inny zdobędzie frazę seed, może przejąć środki

Jeśli uczniowie wykonują to ćwiczenie praktycznie, nauczyciel powinien zatrzymać się na każdym kroku i sprawdzić, czy wszyscy rozumieją, co robią. Jeśli zajęcia mają bardziej koncepcyjny charakter, tę sekcję można wyjaśnić jako omówienie krok po kroku, a nie wykonywać na żywo. Opcja odzyskiwania pokazana w rozdziale jest również przydatna do wyjaśnienia, że portfele można przywrócić, jeśli fraza seed została poprawnie zarchiwizowana.

##### 6.4 Odbieranie i wysyłanie transakcji, 17 minut

**Odbieranie i wysyłanie transakcji on-chain**

Teraz wyjaśnij, jak działają transakcje on-chain.

Aby otrzymać bitcoiny:

* otwórz portfel
* naciśnij odbierz lub wpłać
* skopiuj adres, udostępnij link lub pokaż kod QR

Aby wysłać bitcoiny:

* otwórz portfel
* wklej lub zeskanuj adres odbiorcy
* wpisz kwotę
* sprawdź wszystkie szczegóły
* wyślij transakcję
* poczekaj na potwierdzenie

Wyjaśnij te kluczowe kwestie:

* transakcja przenosi własność, a nie fizyczne monety
* transakcje są nieodwracalne
* węzły weryfikują poprawność
* górnicy dołączają transakcje do bloków
* opłaty wpływają na priorytet potwierdzenia
* transakcje on-chain są zazwyczaj bezpieczne, ale wolniejsze i często droższe niż transakcje Lightning

Diagram przepływu transakcji w rozdziale jest tutaj szczególnie przydatny, ponieważ pomaga uczniom zobaczyć ścieżkę od żądania w portfelu do potwierdzenia w sieci.

**Transakcje w praktyce i ćwiczenia z podziałem na role**

Użyj struktury ćwiczenia kooperacyjnego z rozdziału, aby utrwalić zrozumienie. Wyjaśnij cztery zaangażowane role:

* nadawca
* odbiorca
* górnik
* operator węzła

Prostym podejściem w klasie jest przydzielenie ról i przejście przez jedną transakcję krok po kroku. Pomaga to uczniom zrozumieć, że transakcja Bitcoin to nie magia, lecz skoordynowany proces obejmujący zatwierdzenie, weryfikację, dołączenie do bloku i aktualizację księgi.

Celem tutaj nie jest głęboka techniczna wiedza. Chodzi o to, by uczniowie zrozumieli, kto co robi w transakcji i dlaczego weryfikacja jest ważna.

##### 6.5 Nie ufaj, weryfikuj, 8 minut

Wyjaśnij, że dotyczy to:

* portfeli
* giełd
* aplikacji
* szczegółów transakcji
* twierdzenia o „łatwych zyskach”
* projekty udające, że są jak Bitcoin

Wyjaśnij jasno, że Bitcoin wymaga od użytkowników krytycznego myślenia, weryfikowania tego, czego używają, i unikania ślepego zaufania. Wytłumacz także, dlaczego narzędzia open-source są w tym kontekście ważne: umożliwiają niezależną weryfikację.

###### Podsumowanie i sprawdzenie zrozumienia

Zakończ kilkoma szybkimi pytaniami:

* Jaka jest różnica między portfelem powierniczym a samodzielnym (self-custodial)?
* Dlaczego fraza seed jest tak ważna?
* Co się dzieje, gdy wysyłasz transakcję on-chain?
* Dlaczego transakcje on-chain są wolniejsze niż niektóre inne płatności Bitcoin?
* Co oznacza w praktyce „Nie ufaj, weryfikuj”?

#### Notatki dla edukatora

Ten rozdział jest bardzo praktyczny, więc priorytetem powinny być jasność, bezpieczeństwo i powtarzanie.

Uczniowie nie muszą opanować każdego typu portfela na jednej lekcji. Główne cele to:

* zrozumienie podstaw portfela
* zrozumienie samodzielnej kontroli nad środkami
* poznanie podstawowego przebiegu transakcji
* przyjęcie odpowiedzialnej postawy weryfikacyjnej

Bądź szczególnie ostrożny, omawiając frazy seed i konfigurację portfela. Uczniowie powinni wyjść z lekcji ze zrozumieniem, że to nie są drobne szczegóły, lecz podstawa posiadania Bitcoin.

Najbardziej przydatne materiały wizualne i aktywności w tym rozdziale to:

* porównanie portfela samodzielnego i powierniczego
* tabela kompromisów typów portfeli
* ćwiczenie krok po kroku z konfiguracją portfela
* schemat przebiegu transakcji
* aktywność transakcyjna z podziałem na role

##### Jak wygląda dobra praktyka

* Ważne jest, aby uczniowie faktycznie skonfigurowali portfel lub obejrzeli uważną demonstrację, uczynili frazę seed centralnym punktem z „Te 12 słów TO twój Bitcoin”, przetestowali scenariusze typu „Co się stanie, jeśli zgubisz telefon?” oraz ćwiczyli rozpoznawanie phishingu.
* Edukatorzy powinni być praktycznymi przewodnikami, którzy mają już to doświadczenie, być świadomi kwestii bezpieczeństwa (bez paranoi) i szczerze mówić o krzywej trudności oraz wymaganej nauce.
* Uczniowie czują, że nauczyli się praktycznej umiejętności, rozumieją, że fraza seed jest realna i ważna, a nie abstrakcyjna, czują się zdolni do samodzielnego przechowywania Bitcoin i rozumieją, że decentralizacja wymaga osobistej odpowiedzialności.
* Efekty nauczania zostaną osiągnięte, jeśli uczniowie potrafią skonfigurować portfel i rozumieją różnicę między kluczami publicznymi a prywatnymi, znają kompromisy między portfelami powierniczymi a samodzielnymi, potrafią wyjaśnić, jak działa transakcja (w tym wejścia, wyjścia i opłaty), wykazują świadomość bezpieczeństwa (w tym ochronę frazy seed) oraz zadają krytyczne pytania dotyczące własności i kontroli.

##### Zarządzanie czasem

Jeśli czasu jest mało, priorytetowo potraktuj:

* Zrozumienie podstaw portfela
* Zrozumienie samodzielnej kontroli nad środkami
* Poznanie podstawowego przebiegu transakcji
* Przyjęcie odpowiedzialnej postawy weryfikacyjnej

Jeśli masz więcej czasu, poświęć go na:

* Tabelę porównawczą portfeli samodzielnych i powierniczych
* Tabelę kompromisów typów portfeli
* Ćwiczenie krok po kroku z konfiguracją portfela na żywo
* Schemat przebiegu transakcji z obliczaniem opłat
* Zaawansowane praktyki bezpieczeństwa i rozważania dotyczące portfeli sprzętowych

##### Jeśli uczniowie mają trudności

* Frazy seed jako „realne” → „Ta fraza TO twój bitcoin; nie ma obsługi klienta.”
* Klucze publiczne vs. prywatne → analogia do e-maila (adres vs. hasło).
* Dlaczego to trudne → „Ty kontrolujesz, więc jesteś odpowiedzialny.” Podkreśl kompromis.
