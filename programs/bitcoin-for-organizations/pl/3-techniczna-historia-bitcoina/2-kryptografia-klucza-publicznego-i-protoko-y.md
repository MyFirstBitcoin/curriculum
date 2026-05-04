# 3.2 Kryptografia klucza publicznego i protokoły

Współczesny Internet i większość nowoczesnych systemów komputerowych opiera się na kryptografii, czyli metodzie ukrywania informacji w taki sposób, aby tylko odbiorca mógł ją odszyfrować. Podstawy kryptografii wykorzystywanej do zabezpieczania Bitcoina sięgają lat 70.

Pierwszym problemem do rozwiązania jest – jak przesłać wspólny sekret przez niezabezpieczone medium.

Jako pierwsi zajęli się tym Whitfield Diffie i Martin Hellman.

Problem: dwie strony – zwykle nazywane Alicją i Bartkiem – chcą wymienić się tajną informacją przez sieć, w której inni mogą podsłuchiwać. Aby to osiągnąć, stworzyli proces wymiany klucza Diffiego-Hellmana.

Ten wspólny sekret może następnie posłużyć jako wartość początkowa do tworzenia wielu kluczy symetrycznych, które pozwalają szyfrować i odszyfrowywać wiadomości bez konieczności ujawniania samego klucza.

Ponieważ klucz prywatny nigdy nie musi być udostępniany, a do szyfrowania i odszyfrowywania używane są różne klucze po obu stronach, nazywa się to algorytmem szyfrowania asymetrycznego.

Przykłady zastosowań:

* Alicja podpisuje wiadomość kluczem publicznym Bartka – tylko on może ją odszyfrować za pomocą swojego klucza prywatnego
* Alicja podpisuje wiadomość swoim kluczem prywatnym – każdy może zweryfikować, że wiadomość została wysłana przez Alicję, odszyfrowując ją jej kluczem publicznym, nie znając jej klucza prywatnego
* Łącząc te dwa podejścia w dwóch warstwach szyfrowania, można wysłać wiadomość zaszyfrowaną tak, że tylko Bartek może ją odszyfrować, a następnie potwierdzić, że nadawcą była rzeczywiście Alicja

Chociaż nie został wymieniony jako autor publikacji, Ralph Merkle odegrał kluczową rolę w rozwiązaniu tego, co do tej pory uważano za nierozwiązywalną zagadkę – jak nawiązać lub odnowić prywatną komunikację w otwartej i potencjalnie wrogiej sieci.

To podejście samo w sobie jest podatne na atak brute force, w którym atakujący może przejąć wspólne liczby i ostatecznie odtworzyć wspólny klucz, jeśli tylko będzie miał wystarczająco dużo czasu i zasobów, więc nie jest to kompletne rozwiązanie.

##### Protokoły dla kryptosystemów klucza publicznego

Oprócz wkładu w system klucza publicznego Diffiego-Hellmana opisany powyżej, **Ralph Merkle** przez wiele lat kontynuował pracę w tej dziedzinie i odegrał kluczową rolę w rozwoju niektórych elementów wykorzystywanych przez Bitcoina.

Kryptograficzna funkcja skrótu to algorytm matematyczny, który przyjmuje dane wejściowe dowolnej wielkości i przetwarza złożone obliczenia, aby zwrócić wartość skrótu w bitach, która zwykle jest przedstawiana jako stałej długości wyjście alfanumeryczne w formacie szesnastkowym.

* Dane wejściowe mogą mieć dowolny rozmiar
* Wynik ma zawsze stałą długość i jest deterministyczny (te same dane wejściowe zawsze tworzą ten sam skrót)
* Łatwo jest zweryfikować wynik, ale niezwykle trudno odwrócić proces, aby ustalić dane wejściowe
* Niewielka zmiana danych całkowicie zmienia wynik

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/28da97f5f2d8f33f06438fec568676ab57f84ea9-515x331.svg)

Haszowanie jest integralną częścią protokołu Bitcoina. SHA-256, używany w Bitcoinie, został stworzony przez NSA i jest przykładem kryptograficznego algorytmu haszującego.

* Każdy blok w łańcuchu jest haszowany, aby dane nie mogły zostać zmienione – zapewnia to integralność rozproszonej księgi
* Wygenerowany skrót musi spełniać kryteria „Proof of work”, aby blok został uznany za ważny
* Drzewa Merkle’a – dzięki rozgałęzieniom i haszowaniu skrótów, drzewa skrótów umożliwiają weryfikację dużych zbiorów danych przy minimalnym zużyciu pamięci
* Podpisy i klucze oparte na skrótach mogą być używane do portfeli, adresów i autoryzacji transakcji

Rozproszona weryfikacja stanów blockchaina i modele księgi tylko do dopisywania, odporne na zmiany, są możliwe dzięki jednokierunkowemu haszowaniu. Funkcje skrótu zapewniają niezawodny, deterministyczny sposób weryfikacji zdarzeń w publicznych księgach, takich jak Bitcoin, bez scentralizowanego modelu zaufania.

Twórcy tych nowych możliwości w dziedzinie kryptografii spodziewali się, że zapoczątkują one nową falę innowacji.

##### Kryptografia krzywych eliptycznych

Jedną z późniejszych innowacji była kryptografia krzywych eliptycznych.

Kryptografia krzywych eliptycznych została wprowadzona w 1985 roku przez dwóch naukowców, N. Koblitza i V. Millera. Zaproponowali oni wykorzystanie punktów zdefiniowanych przez krzywe eliptyczne zamiast skończonych pól pierwszych, tak aby założenie o problemie dyskretnego logarytmu było spełnione, jak to się zwykle robi w standardowym protokole wymiany klucza Diffiego-Hellmana. Szczegóły działania wykraczają poza zakres tej sekcji, ale ogólnie rzecz biorąc, krzywa eliptyczna to zbiór punktów spełniających określone równanie matematyczne.

Równanie krzywej eliptycznej wygląda mniej więcej tak:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

Ma to kilka przydatnych właściwości:

* Symetria względem osi poziomej. Każdy punkt na krzywej można odbić względem osi x i pozostanie on na tej samej krzywej.
* każda niepionowa prosta przetnie krzywą w maksymalnie trzech miejscach.
* Kompaktowe rozmiary kluczy są niezbędne do efektywnego przechowywania i przesyłania kluczy publicznych w blockchainie.

Te właściwości można wykorzystać do tworzenia par kluczy w podobny sposób jak w algorytmie Diffiego-Hellmana. Bitcoin używa ECDSA, czyli Elliptic Curve Digital Signature Algorithm. Jest to proces, który wykorzystuje krzywą eliptyczną i skończone pole do „podpisywania” danych w taki sposób, że osoby trzecie mogą zweryfikować autentyczność podpisu, podczas gdy podpisujący zachowuje wyłączną możliwość jego tworzenia. W przypadku bitcoina podpisywane są dane dotyczące transakcji przenoszącej własność.

Część „skończona” jest podobna do podejścia „mod” w Diffie-Hellmanie, gdzie wynik równania jest dzielony, a reszta z dzielenia służy do zapewnienia, że mieści się on w określonym zakresie liczb.
