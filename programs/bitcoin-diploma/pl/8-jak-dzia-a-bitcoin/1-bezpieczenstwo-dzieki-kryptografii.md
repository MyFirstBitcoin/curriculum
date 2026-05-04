# 8.1 Bezpieczeństwo dzięki kryptografii

> To, co daje nam Bitcoin, to twarda obietnica: program zostanie wykonany dokładnie tak, jak określono.  
_Andreas M. Antonopoulos_

#### Kryptografia klucza publicznego/prywatnego


> **Definition – Definicja kryptografii**
>
> **Kryptografia** to praktyka zamieniania informacji w tajemnicę, którą mogą odczytać tylko odpowiednie osoby.


* **Szyfrowanie** to proces zamieniania informacji na zakodowaną formę, tak aby tylko ktoś z odpowiednim kluczem mógł ją odczytać.
* **Deszyfrowanie** to proces zamieniania tej zakodowanej informacji z powrotem na coś czytelnego.

W tradycyjnej kryptografii dwie osoby, które chcą komunikować się prywatnie, muszą najpierw podzielić się tym samym tajnym kluczem, podobnie jak wspólnym hasłem. Jedna osoba używa tego klucza do zaszyfrowania wiadomości przed jej wysłaniem, a druga osoba używa tego samego klucza do odszyfrowania i odczytania jej.

Problemem tego systemu jest to, że obie osoby muszą już wcześniej znać tajny klucz. Jeśli ktoś inny uzyska dostęp do tego klucza, może odczytać każdą przechwyconą wiadomość.

Bitcoin rozwiązuje ten problem, stosując inne podejście zwane kryptografią klucza publicznego, gdzie użytkownicy nie muszą dzielić się tajnymi kluczami z wyprzedzeniem.

Kryptografia klucza publicznego/prywatnego rozwiązuje problem dzielenia się tajemnicami. Zamiast udostępniać hasło, każda osoba ma dwa klucze: klucz publiczny i klucz prywatny.

* **klucz publiczny** można udostępniać każdemu.
* **klucz prywatny** musi być zawsze utrzymywany w tajemnicy.

Jeśli Jan chce wysłać coś do Arka, może użyć klucza publicznego Arka. Tylko Arek może to odblokować za pomocą swojego klucza prywatnego. Nawet jeśli ktoś przechwyci wiadomość, nie może jej odczytać ani użyć bez klucza prywatnego.

W Bitcoinie ten system jest używany do tworzenia podpisów cyfrowych. Podpis cyfrowy udowadnia, że właściciel klucza prywatnego zatwierdził transakcję, podobnie jak podpisanie się na dokumencie. To właśnie pozwala na to, by transakcje Bitcoin były bezpieczne i weryfikowalne bez konieczności zaufania stronie trzeciej.

Transakcje Bitcoin polegają na przenoszeniu własności bitcoinów z jednego adresu na inny.

Szyfrowanie jest używane, aby upewnić się, że tylko prawdziwy właściciel bitcoinów ma prawo wysłać swoje pieniądze do kogoś innego. Zapewnia to ochronę ich własności przed złośliwymi osobami.

Jako dodatkowy środek ochrony każda transakcja Bitcoin automatycznie otrzymuje UNIKALNY podpis cyfrowy. Ten unikalny podpis cyfrowy jest oparty na technologii odpornej na manipulacje, która pomaga sieci zweryfikować, że to prawdziwy właściciel bitcoinów, a nie ktoś inny, je wysłał.


> **Info**
>
> Każdy użytkownik ma dwa klucze: **klucz prywatny**, który jest **utrzymywany w tajemnicy**, oraz **klucz publiczny** który może być **udostępniany innym**. **Klucz prywatny** służy jako forma identyfikacji i dowód własności, potwierdzając: „Ten adres należy do mnie i mam nad nim kontrolę.”


###### Jak działa transakcja Bitcoin

1. **Tworzenie transakcji**: Użytkownik inicjuje transakcję Bitcoin, określając szczegóły takie jak adres odbiorcy i ilość bitcoinów do wysłania.
1. **Generowanie podpisu cyfrowego**: Nadawca generuje unikalny **podpis cyfrowy** używając swojego **klucza prywatnego**. Ten podpis to unikalny kod, który potwierdza autentyczność transakcji.
1. **Rozgłaszanie transakcji**: Podpisana transakcja jest rozgłaszana w sieci Bitcoin, wskazując zamiar przeniesienia własności bitcoinów od nadawcy do odbiorcy.
1. **Weryfikacja w sieci**: Węzły w sieci Bitcoin otrzymują transakcję i używają **klucza publicznego** aby zweryfikować autentyczność podpisu transakcji. Jednocześnie używają klucza publicznego nadawcy,**klucz publiczny** aby zweryfikować **podpis cyfrowy**.
1. **Potwierdzenie w sieci Bitcoin**: Jeśli weryfikacja się powiedzie, transakcja zostanie dodana do księgi, która służy jako bezpieczny, przejrzysty rejestr wszystkich transakcji. Po potwierdzeniu własność bitcoina zostaje oficjalnie przeniesiona od nadawcy do odbiorcy.


> **Callout – Podsumowanie**
>
> **podpis cyfrowy**, utworzony za pomocą **klucza prywatnego** nadawcy, potwierdza, że transakcja została autoryzowana przez właściciela bitcoina. Sieć Bitcoin może następnie zweryfikować ten dowód i zapisać transakcję.


#### Wyjaśnienie haszowania

Nie zrażaj się technicznymi terminami i pojęciami matematycznymi, które pojawią się dalej. Rozumiemy, że nie każdy przepada za matematyką, ale możesz się zaskoczyć i zobaczyć, że nawet najbardziej złożone idee można pojąć przy odrobinie wysiłku.


> **Definition – Definicja funkcji**
>
> **funkcja** jest jak maszyna, która przyjmuje pewne informacje i zamienia je w coś nowego. Informacje, które przekazujesz funkcji, to **wejście**. Nowe informacje, które tworzy funkcja, to **wyjście**. Funkcje pomagają komputerom wykonywać zadania i rozwiązywać problemy.


##### Czym jest funkcja?

Funkcja to zestaw instrukcji, który przyjmuje dane wejściowe i generuje dane wyjściowe. Możesz o niej myśleć jak o przepisie: postępujesz według kroków z określonymi składnikami i zawsze otrzymujesz przewidywalny rezultat.

W Bitcoinie funkcje są używane do przetwarzania i weryfikacji transakcji. Gdy ktoś wysyła bitcoina, funkcje kryptograficzne pomagają sprawdzić, czy transakcja jest ważna, potwierdzić, że nadawca ma wystarczające środki, i zaktualizować salda w księdze Bitcoin. Po zweryfikowaniu i dodaniu do bloku, transakcja staje się częścią trwałego zapisu w blockchainie.

##### Czym jest funkcja jednokierunkowa?

Funkcja jednokierunkowa to szczególny rodzaj funkcji, którą łatwo obliczyć w jednym kierunku, ale niezwykle trudno odwrócić. Na przykład, zmiksowanie składników na smoothie jest łatwe, ale nie da się już oddzielić smoothie na oryginalne składniki.

Bezpieczeństwo Bitcoina opiera się na funkcjach jednokierunkowych. Są one wykorzystywane w kryptografii klucza publicznego i prywatnego, pozwalając ludziom udostępniać klucz publiczny przy jednoczesnym zachowaniu tajności klucza prywatnego. Nawet jeśli klucz publiczny jest widoczny, nie da się z niego wywnioskować klucza prywatnego. To właśnie sprawia, że transakcje Bitcoin są bezpieczne.

##### Czym jest funkcja skrótu (hashująca)?

**funkcja skrótu** jest jak maszyna do tajnych kodów. Przyjmuje wiadomość i zamienia ją w kod.

###### Jak działa haszowanie w transakcjach Bitcoin

W Bitcoinie każda transakcja jest zamieniana na hash, zanim zostanie dodana do blockchaina. Hash to unikalny cyfrowy odcisk palca transakcji. Jeśli ktoś spróbuje zmienić choćby najmniejszą część transakcji, hash zmieni się całkowicie. Dzięki temu sieć łatwo wykrywa próby manipulacji.

###### Rola haszowania w bezpieczeństwie Bitcoina

Haszowanie pomaga chronić sieć Bitcoin, sprawiając, że transakcje są łatwe do zweryfikowania i niemożliwe do cichej modyfikacji. Ponieważ każda transakcja ma swój unikalny hash, sieć może szybko wykryć, czy coś zostało zmienione.

Funkcja skrótu przyjmuje dane i zamienia je w ciąg o stałej długości, składający się z cyfr i liter, zwany hashem. Te same dane wejściowe zawsze dadzą ten sam hash, ale nawet najmniejsza zmiana w danych wejściowych spowoduje zupełnie inny wynik. Ta właściwość pozwala komputerom sprawdzić, czy dane nie zostały zmienione.


> **Definition – Definicja haszowania**
>
> **Haszowanie** jest jak tworzenie odcisku palca dla danych cyfrowych. To proces polegający na przekształceniu cyfrowej wiadomości w kod o stałej długości, który służy jako unikalny identyfikator. Tak jak odcisk palca może zidentyfikować osobę, tak hash może zidentyfikować cyfrową wiadomość.


**wyjście**, czyli hash, zawsze ma tę samą długość, niezależnie od długości oryginalnych danych. Bitcoin używa kilku konkretnych rodzajów funkcji skrótu, takich jak **SHA-256** oraz **RIPEMD160**.

Kilka przykładów poniżej:

* Hash SHA256 dla ciągu znaków **witaj świecie**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* Skrót SHA256 ciągu znaków **witaj świecie.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Zauważ, że drobna zmiana w danych wejściowych całkowicie zmienia wynik w porównaniu do pierwszego przykładu
* Skrót SHA256 pobieranego pliku iso **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * To wejście to ogromny plik, a mimo to wynik nadal ma tę samą, stałą długość

Możesz także pomyśleć o haszowaniu jak o zapisie nutowym, który oddaje istotę utworu muzycznego. Tak jak zapis nutowy jest unikalną reprezentacją melodii, tak wartość skrótu jest unikalną reprezentacją danych.

Porównując zapis nutowy utworu z rzeczywistym wykonaniem, muzyk może ocenić, czy wykonanie jest poprawne. Podobnie, porównując wartość skrótu otrzymanych danych z oryginalną wartością skrótu, można sprawdzić, czy dane zostały zmienione podczas przesyłania.

Tak jak nawet niewielkie odstępstwo w wykonaniu muzycznym może sprawić, że zabrzmi ono inaczej, tak najmniejsza zmiana w oryginalnych danych spowoduje powstanie innej wartości skrótu. Dzięki temu haszowanie jest potężnym narzędziem zapewniającym integralność i autentyczność transakcji Bitcoin.

Proces kodowania **klucza publicznego** poprzez haszowanie służy zwiększeniu bezpieczeństwa informacji poprzez przekształcenie jej w nieczytelny ciąg o stałej długości. Bitcoin wykorzystuje algorytmy SHA-256 i RIPEMD160 do generowania adresów publicznych. Otrzymany wynik służy jako unikalny identyfikator dla **klucza publicznego** i pomaga zapewnić integralność oraz bezpieczeństwo transakcji zapisanych w księdze. Szyfrując informacje w ten sposób, znacznie trudniej jest nieupoważnionym osobom uzyskać dostęp do danych i je modyfikować.

##### Właściwości funkcji skrótu

* **Deterministyczność**: Te same składniki zawsze dają ten sam koktajl. Tak samo te same dane zawsze dadzą ten sam skrót.
* **Odporność na preimage**: Mając tylko koktajl, nie jesteś w stanie odgadnąć dokładnie, jakie owoce zostały użyte. Podobnie, mając tylko skrót, nie można ustalić oryginalnych danych.
* **Efekt lawiny**: Nawet niewielka zmiana składników powoduje powstanie zupełnie innego koktajlu. W haszowaniu bardzo mała zmiana danych daje zupełnie inny skrót.
* **Odporność na kolizje**: Niezwykle trudno jest znaleźć dwa różne zestawy składników, które dadzą dokładnie ten sam koktajl. Tak samo jest bardzo mało prawdopodobne, by dwa różne zestawy danych dały ten sam skrót.
* **Szybka weryfikacja**: Przygotowanie koktajlu jest szybkie i łatwo sprawdzić, czy to faktycznie koktajl. Funkcje skrótu są szybkie do obliczenia i łatwe do zweryfikowania przez każdego.

#### Ćwiczenie: Wygeneruj skrót SHA 256

https://tools.keycdn.com/sha256-online-generator

Ciekawi Cię, jak działa haszowanie? Zeskanuj kod QR, aby natychmiast wygenerować skrót SHA256 z dowolnego słowa, zdania lub wybranego przez Ciebie tekstu. Funkcje skrótu są jak cyfrowe odciski palców: są jednokierunkowe, co oznacza, że po zahaszowaniu czegoś nie da się tego odwrócić. Wypróbuj i przekonaj się sam!
