# 6.2 Wprowadzenie do portfeli

W przeciwieństwie do fizycznych pieniędzy, bitcoiny nie są faktycznie przechowywane w portfelu Bitcoin. Zamiast tego istnieją w rozproszonej księdze, którą sieć Bitcoin nieustannie weryfikuje i zabezpiecza. Jak więc możesz posiadać bitcoiny?

Jesteś właścicielem swoich bitcoinów tylko wtedy, gdy kontrolujesz klucze prywatne pozwalające Ci podpisywać transakcje i przekazywać własność swoich bitcoinów komuś innemu. To właśnie jest wysyłanie bitcoinów.

Przyjrzyjmy się dwóm pojęciom, do których odnosimy się, używając terminu **portfel**:

* Główny klucz prywatny, podobny do hasła, z którego generowane są Twoje klucze publiczne, podobne do adresów e-mail. Możesz udostępniać swój publiczny adres innym, aby otrzymywać i wysyłać bitcoiny, ale nigdy nie wolno udostępniać klucza prywatnego!
* Mobilny lub komputerowy interfejs służący do interakcji z siecią Bitcoin, sprawdzania salda bitcoinów, wysyłania i odbierania transakcji oraz ich rozgłaszania w sieci. Różne typy portfeli, wraz z ich zaletami i kompromisami, zostaną opisane w kolejnych sekcjach.

#### Portfele samodzielne a powiernicze

Zanim szczegółowo omówimy różne typy portfeli Bitcoin i ich cechy, dokonajmy ważnego rozróżnienia między portfelami samodzielnymi a powierniczymi. Każdy typ ma swoje zalety, ryzyka i poziom kontroli nad bitcoinami. Portfel samodzielny oznacza, że użytkownik posiada klucze prywatne i naprawdę kontroluje swoje bitcoiny; w portfelu powierniczym to strona trzecia przechowuje bitcoiny dla użytkownika.


| Typ | Kontrola | Zalety | Ryzyka |
| --- | --- | --- | --- |
| Samodzielny | Użytkownik | Pełna kontrola nad środkami i transakcjami, brak procesu zatwierdzania lub blokady konta, brak kontroli korporacyjnej lub rządowej, ochrona przed konfiskatą. | Brak możliwości odzyskania w przypadku utraty frazy odzyskiwania, pełna odpowiedzialność spoczywa na użytkowniku. |
| Powierniczy | Dostawca zewnętrzny | Łatwe odzyskanie dostępu w przypadku utraty, łatwiejsza obsługa klienta. | Środki są połączone z Internetem, bardziej podatne na ataki hakerskie. Powiernik może zamrozić konta. |


W portfelu samodzielnym (nazywanym też portfelem niepowierniczym) tylko Ty masz klucze do portfela i pełną kontrolę nad tym, co do niego trafia i z niego wychodzi. Z kolei w portfelu powierniczym ktoś inny posiada klucz prywatny, co daje tej osobie pełny dostęp do przesuwania bitcoinów, które ten dostawca kontroluje w Twoim imieniu.

* Samodzielne przechowywanie to jak bycie własnym bankiem. Transakcje nie podlegają kontroli ani nadzorowi
* Samodzielne przechowywanie zapewnia, że osoby trzecie nie mogą skonfiskować Twoich bitcoinów.
* Samodzielne przechowywanie daje spokój w czasach niepewności, ponieważ wiesz, że Twoje bitcoiny są bezpieczne.

Ważne jest, aby wybrać odpowiedni typ portfela do indywidualnych potrzeb. Czasami ludzie mają trudność z rozróżnieniem, czy instalują portfel samodzielny, czy powierniczy. Ta tabela pokazuje różnice w procesie instalacji.


| Typ | Krok 1: Wybierz | Krok 2: Zainstaluj | Krok 3: Utwórz | Krok 4: Zabezpiecz |
| --- | --- | --- | --- | --- |
| Samodzielny | Wybierz portfel samodzielny | Postępuj zgodnie z instrukcjami portfela | Wygeneruj frazę odzyskiwania | Przechowuj frazę odzyskiwania w bezpiecznym miejscu |
| Powierniczy | Wybierz portfel powierniczy | Postępuj zgodnie z instrukcjami portfela | Utwórz konto | N/D |


„**Nie twoje klucze, nie twoje monety**” to popularne powiedzenie wśród posiadaczy bitcoinów. Odnosi się do przekonania, że jeśli nie masz bezpośredniej kontroli nad kluczami prywatnymi powiązanymi z twoim portfelem Bitcoin, nie jesteś prawdziwym właścicielem monet.

Każdy, kto uzyska dostęp do twoich kluczy prywatnych, staje się właścicielem twoich bitcoinów. Dlatego tak ważne jest, aby je chronić i trzymać z dala od ciekawskich oczu! W dalszej części książki pokażemy kilka sposobów, jak to zrobić.

W dalszej części będziemy mówić wyłącznie o portfelach samodzielnych, w których użytkownik posiada swoje klucze i ma pełną kontrolę nad swoimi bitcoinami.

Nie martw się, jeśli wydaje się to skomplikowane lub nie rozumiesz wszystkiego — to podróż i z czasem, korzystając z Bitcoin, zrozumiesz coraz więcej!

#### Różne typy portfeli Bitcoin

To, gdzie twój klucz prywatny jest tworzony i przechowywany, decyduje o tym, jak opisujemy portfele Bitcoin. Jeśli klucze są na twoim smartfonie, to jest to **portfel mobilny**. Jeśli są przechowywane bezpiecznie na dedykowanym urządzeniu, to jest to **portfel sprzętowy**.


| Typ | Opis | Zalety | Wady | Przykładowy użytkownik |
| --- | --- | --- | --- | --- |
| Portfel online | Dostępny przez przeglądarkę internetową | Dostępny z każdego urządzenia z połączeniem internetowym | Mniej bezpieczny, ponieważ może zostać zhakowany lub przejęty | Potrzebuje często korzystać ze swojego portfela i nie ma dużo środków do przechowania |
| Portfel mobilny | Zainstalowany na urządzeniu mobilnym | Łatwy w użyciu | Można go utracić, jeśli urządzenie zostanie skradzione lub zhakowane | Potrzebuje wykonywać transakcje w podróży i nie ma dużo środków do przechowania |
| Portfel na komputer | Zainstalowany na komputerze stacjonarnym | Wygodny i można z niego korzystać z dowolnego miejsca | Może zostać zhakowany, jeśli komputer jest zainfekowany złośliwym oprogramowaniem | Chce przechowywać dużą ilość bitcoinów i czuje się swobodnie korzystając z komputera stacjonarnego |
| Portfel sprzętowy | Fizyczne urządzenie, które przechowuje bitcoiny offline | Bardziej bezpieczny niż portfele online i może być używany offline | Środki mogą być nie do odzyskania | Chce przechowywać dużą ilość bitcoinów i jest gotowy zapłacić za dodatkowe bezpieczeństwo |


Ponieważ klucze można przenosić z jednego urządzenia na drugie, „status” Twojego portfela Bitcoin nie jest stały. Na przykład, jeśli utworzę klucze portfela na komputerze, a później przeniosę je na telefon, „portfel na komputer” staje się „portfelem mobilnym”.

Jeśli chodzi o przechowywanie swoich bitcoinów, nie chodzi tylko o to, kto ma kontrolę nad kluczami — istnieje wiele innych zagrożeń, które należy wziąć pod uwagę. Dlatego ważne jest, aby znaleźć rozwiązanie do przechowywania, które jest zarówno bezpieczne, jak i wygodne. Analizując kompromisy różnych typów portfeli, dowiesz się, że nie ma idealnego portfela, który spełni wszystkie potrzeby.

##### Na co zwrócić uwagę przy wyborze portfela

* **Bezpieczeństwo**: Upewnij się, że portfel posiada silne zabezpieczenia.
* **Prywatność**: Zastanów się, czy portfel wymaga podania danych osobowych.
* **Łatwość obsługi**: Wybierz portfel, który jest prosty w obsłudze i nawigacji.
* **Kompatybilność**: Upewnij się, że portfel jest kompatybilny z Twoim urządzeniem.
* **Opłaty**: Porównaj opłaty pobierane przez różne portfele.
* **Reputacja**: Sprawdź reputację twórców, aby upewnić się, że są godni zaufania.
* **Kontrola**: Niektóre portfele dają Ci większą kontrolę nad Twoimi kluczami prywatnymi.

##### Open Source vs Closed Source

Kolejnym ważnym czynnikiem, o którym warto pamiętać przy wyborze portfela Bitcoin, jest to, czy aplikacja lub oprogramowanie jest open-source. To ważne, ponieważ projekty open-source pozwalają społeczności przeglądać kod i kontynuować projekt, jeśli zespół przestanie nad nim pracować. Tak jak kod Bitcoina jest całkowicie otwarty do przeglądania, używania i modyfikowania przez każdego, tak samo powinien być kod portfela, którego używasz do zarządzania swoimi bitcoinami.

#### Aktywność: Dyskusja i ocena portfeli Bitcoin

https://bitcoin.org/en/choose-your-wallet

Przejdź na następującą stronę internetową: [https://bitcoin.org/en/choose-your-wallet](https://bitcoin.org/en/choose-your-wallet)

Wykorzystaj swoją nową wiedzę o portfelach Bitcoin, aby wybrać ten, który najlepiej odpowiada Twoim potrzebom, na podstawie kryteriów, które dziś omówiliśmy.
