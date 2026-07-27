# 6.4 Odbieranie i wysyłanie transakcji

Transakcja Bitcoin to przekazanie własności bitcoinów nowemu właścicielowi. Zwróć uwagę, że nie są przekazywane same monety, lecz prawo do ich wydania, czyli własność: innymi słowy, prawo do ich wydania. Za każdym razem, gdy transakcja zostaje zaakceptowana do bloku, wszystkie węzły w sieci aktualizują swoją lokalną kopię publicznego rejestru, aby odzwierciedlić zmianę własności. Pod tym względem transakcja Bitcoin jest bardziej podobna do transakcji nieruchomości (lub innego majątku) niż do transakcji gotówkowej.

Aby „wysłać” bitcoiny, nadawca podpisuje wiadomość swoim kluczem prywatnym, sygnalizując sieci, że prawowity właściciel bitcoinów przekazał ich własność odbiorcy.

Bitcoiny będą teraz powiązane z adresem odbiorcy, dając mu prawo własności do bitcoinów, tak że tylko nowy właściciel może je wydać, używając swojego klucza prywatnego.

Nowe transakcje Bitcoin są inicjowane z portfeli na całym świecie, ale nie ma centralnego operatora płatności. Zamiast tego górnicy konkurują o zapisanie transakcji w rejestrze.

Załóżmy, że Jakub jest winien Elżbiecie 0,5 BTC i jest gotów jej oddać. Oboje mają portfele cyfrowe.

1. Elżbieta udostępnia swój adres Jakubowi.
1. Jakub używa swojego oprogramowania portfela, aby utworzyć transakcję, która zawiera adres Elżbiety, kwotę do przelania (0,5 BTC) oraz opłatę dla górnika. Wyższe opłaty zwiększają szansę, że górnik uwzględni transakcję w następnym bloku.
1. Po podpisaniu transakcji jest ona rozgłaszana do sieci, gdzie jest weryfikowana przez węzły. Sprawdzają one, czy Jakub ma wystarczające środki i czy jest prawowitym właścicielem monet, które chce wydać. Jeśli nie, natychmiast odrzucają transakcję.
1. Po zweryfikowaniu transakcji górnicy decydują, czy dodać ją do następnego bloku, zazwyczaj na podstawie wybranej opłaty. Gdy transakcja znajdzie się w bloku, zostaje dodana do łańcucha bloków, a środki są przekazywane na adres Elżbiety.
1. Własność została przekazana Elżbiecie. Teraz może użyć swojego klucza prywatnego, aby wydać środki.

_Ważne jest, aby pamiętać, że po zakończeniu transakcji nie można jej cofnąć._


> **Light – Jak działa transakcja Bitcoin**
>
> 1. Ktoś zleca transakcję
> 1. Transakcja jest rozgłaszana do komputerów P2P (węzłów)
> 1. Górnicy weryfikują transakcję
> 1. Transakcje są łączone w blok danych
> 1. Nowy blok zostaje dodany do istniejącego łańcucha bloków
> 1. Transakcja została zakończona



> **Light – Odbieranie transakcji Bitcoin**
>
> Aby otrzymać bitcoiny, musisz podać nadawcy publiczny adres Bitcoin. Jest to unikalny ciąg liter i cyfr, który reprezentuje Twój portfel i służy do jego identyfikacji w sieci Bitcoin.
>
> Możesz znaleźć swój publiczny adres, otwierając swój portfel Bitcoin i szukając opcji „Odbierz” lub „Wpłać” bitcoiny.
>
> Następnie możesz udostępnić swój adres Bitcoin na kilka sposobów:
>
> 1. **Skopiuj i wklej adres**: Możesz skopiować adres, zaznaczając go i naciskając „Kopiuj”, a następnie wkleić go do e-maila lub wiadomości.
> 1. **Udostępnij link do swojego portfela Bitcoin**: Niektóre portfele Bitcoin pozwalają utworzyć link do Twojego portfela, który możesz udostępnić nadawcy. Może on wtedy kliknąć link, aby uzyskać dostęp do Twojego portfela i wysłać bitcoiny.
> 1. **Udostępnij kod QR**: Jeśli nadawca ma smartfon z zainstalowaną aplikacją portfela Bitcoin, może zeskanować kod QR, aby uzyskać Twój adres Bitcoin.


Gdy nadawca ma Twój adres, może wysłać Ci bitcoiny, wpisując Twój adres i kwotę, którą chce przesłać. Bitcoiny są wtedy przesyłane z jego portfela do Twojego portfela.

Transakcja jest potwierdzana przez sieć Bitcoin i zwykle trwa to około 10 minut. Dla większego bezpieczeństwa zaleca się poczekać na dwa potwierdzenia, co zajmuje około 20 minut.


> **Light – Wysyłanie transakcji Bitcoin**
>
> Aby wysłać bitcoiny, będziesz potrzebować kilku rzeczy: portfela Bitcoin, publicznego adresu odbiorcy oraz kwoty bitcoinów, którą chcesz wysłać.
>
> 1. Otwórz swój portfel Bitcoin.
> 1. Przejdź do przycisku „Wyślij” i wklej adres odbiorcy w polu „Do”. Alternatywnie możesz zeskanować kod QR, jeśli odbiorca go udostępnił.
> 1. Wpisz ilość bitcoinów, którą chcesz wysłać, w polu „Kwota”.
> 1. Sprawdź dokładnie adres odbiorcy i kwotę do wysłania. Pamiętaj, że transakcje są nieodwracalne!
> 1. Przed kliknięciem „Potwierdź i wyślij” zalecamy jeszcze raz sprawdzić szczegóły transakcji, aby upewnić się, że wysyłasz właściwą ilość bitcoinów na właściwy adres.
> 1. Wyślij transakcję do sieci i poczekaj na jej potwierdzenie przez sieć.
>
> Teraz wiesz, jak ocenić, wybrać i skonfigurować portfel Bitcoin, w którym samodzielnie przechowujesz środki. Wysyłanie i odbieranie bitcoinów w sieci Bitcoin nazywane jest transakcjami „on-chain”. Dzieje się tak, ponieważ transakcje odbywają się w głównej sieci Bitcoin i są zapisywane w blockchainie.
>
> Transakcje on-chain są najbezpieczniejszym sposobem dokonywania transakcji bitcoinami dzięki zdecentralizowanej weryfikacji zapewnianej przez sieć.
>
> Jednak transakcje on-chain są wolniejsze i mogą być znacznie droższe niż inne opcje (które omówimy w module 7) ze względu na opłatę dla górnika.


#### Ćwiczenie: Transakcje w praktyce


https://qr.myfirstbitcoin.org/transactions.pdf

_Activity: Transactions_


**To ćwiczenie kooperacyjne upraszcza podstawowe role osób zaangażowanych w transakcję Bitcoin.**

###### Kluczowe punkty

1. W każdej transakcji bitcoin biorą udział cztery typy uczestników: nadawca, odbiorca, górnicy i operatorzy węzłów.
1. Nadawca musi zatwierdzić (podpisać kryptograficznie) **ilość bitcoinów** do wysłania ORAZ **konkretny adres** na który wysyła środki.
1. Odbiorca musi podać **prawidłowy adres** nadawcy ORAZ zweryfikować, że transakcja została pomyślnie potwierdzona w blockchainie.
1. Górnicy upewniają się, że wszystkie kryteria są spełnione, zanim dodadzą transakcje do przyszłych bloków.
1. Operatorzy węzłów weryfikują, czy wydobyte bloki są prawidłowe, zanim zaktualizują swoją wersję blockchaina (księgi rachunkowej).

###### Wskazówka dla ucznia

Zamieniajcie się wszystkimi czterema rolami, aby doświadczyć, co robi każdy uczestnik.
