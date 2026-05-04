# 3.4 Hashcash

Hashcash został stworzony przez Adama Backa, kolejnego z wczesnych innowatorów w tej dziedzinie. Adam bardzo interesował się wolnym rynkiem i prywatnością w internecie, natrafił na listę dyskusyjną Cypherpunks, do której dołączył i stał się aktywnym uczestnikiem.

Bardzo interesował się cyfrowymi pieniędzmi i zaproponował, aby grupa mogła potencjalnie ściślej współpracować nad DigiCash z Chaumem, ale te pomysły nie zostały zrealizowane. Następnie skupił się na innym pojawiającym się problemie – spamie e-mailowym. On i reszta Cypherpunków chcieli znaleźć rozwiązanie problemu spamu, gdzie dla spamerów było banalnie łatwe tworzenie i wysyłanie tysięcy wiadomości, które zapychają sieci. Jego innowacyjne rozwiązanie opierało się na haszowaniu – możliwości kryptograficznego przekształcenia dowolnych danych w unikalny i losowy ciąg o określonej długości, aby stworzyć cyfrowy „znaczek”, który musiał być dołączony do e-maila, by był uznany za ważny i przesłany przez sieć. To był niewielki koszt dla prawdziwego e-maila, ale zaporowy dla spamera.

Kluczową innowacją Hashcash było powiązanie zasobów ze świata rzeczywistego – mocy obliczeniowej – z siecią cyfrową. Podczas gdy zasoby cyfrowe do tej pory mogły być kopiowane bez ograniczeń, liczba „hashcash” była ograniczona przez to, ile energii ludzie byli gotowi w to zainwestować.

Chociaż rozwiązanie spełniało część kryteriów, które Adam uważał za niezbędne w systemie cyfrowej gotówki – było anonimowe, odporne i nie wymagało zaufania – każdy hashcash nie był wielokrotnego użytku i nie był naprawdę rzadki. Zaproponował inne sposoby rozwiązania tych problemów z wykorzystaniem zewnętrznych stron trzecich.

##### BitGold

Nick Szabo rozwinął koncepcję Hashcash i dowodu pracy, proponując alternatywne rozwiązanie, które opisał na liście dyskusyjnej rok po opublikowaniu Hashcash, w 1998 roku.

Chociaż było to bliżej rozwiązania, ta propozycja nadal miała kilka wyzwań.

* Kto miałby prowadzić rejestr własności hashy i jak można im ufać?
* Haszowanie generalnie stawałoby się tańsze z czasem, co było również wyzwaniem dla HashCash.

Ponieważ powiązane hashe miały być oznaczane czasowo, zaproponował pewną formę historycznego śledzenia trudności haszowania w danym momencie; wcześniejszy hash wymagałby większych kosztów przetwarzania niż późniejszy, ponieważ koszty spadały. Niestety oznaczało to, że hashe nie byłyby „zamienne”, czyli równej wartości, co jest kluczową cechą cyfrowych pieniędzy. Aby to rozwiązać, Nick zasugerował pewną formę „wolnej bankowości” działającej na BitGold, która mogłaby agregować różne grupy hashy wyceniane tak samo.

##### B-Money

Wkrótce po propozycji Bit Gold, Wei Dai zaproponował podobne rozwiązanie. Już wcześniej opracował kilka innych narzędzi dla Cypherpunków i miał własne pomysły na temat cyfrowych pieniędzy.

Jego propozycja przypominała Bit Gold tym, że wykorzystywała podpisy cyfrowe do przekazywania środków, a zapisy transakcji miały być przechowywane w rejestrze, zawierającym klucze publiczne i ilość jednostek waluty przypisanych do każdego z nich. Podobnie jak w Bit-Gold, zaufane strony trzecie były uważane za luki w bezpieczeństwie, a przekonanie było takie, że elektroniczny system gotówkowy nie powinien polegać na jednej jednostce do śledzenia sald, transakcji czy zapobiegania podwójnemu wydaniu.

Wei Dai zaproponował kilka rozwiązań tych problemów, z których jedno polegało na tym, że zamiast centralnej jednostki (lub jednostek) utrzymującej rejestr, WSZYSTKIE węzły miałyby własną kopię. Jeśli wszyscy użytkownicy sprawdzaliby własny rejestr i ważność każdej transakcji, to dopóki wszystkie węzły byłyby aktualne, rejestry powinny pozostać zsynchronizowane w całej sieci. Taki wysoce rozproszony system byłby trudny do skorumpowania.

Wei Dai zauważył, że to nie rozwiązuje problemu generałów bizantyjskich (1), ponieważ węzły mogłyby łatwo stracić synchronizację lub po prostu kłamać. Zaproponował alternatywne metody, takie jak wyznaczenie podzbioru „zaufanych” serwerów utrzymujących rejestr oraz stworzenie bodźców finansowych, by te serwery pozostały uczciwe.

Jeśli chodzi o politykę pieniężną, zaproponował powiązanie siły nabywczej B-Money z jakimś zewnętrznym indeksem cen konsumpcyjnych. Chciał, aby ta sama ilość B-Money mogła kupić równy udział w indeksie w czasie, zapewniając pewną stabilność cen. Każdy mógłby generować nowe jednostki waluty, dostarczając poprawny hash, ale trudność generowania hashy mogłaby się zmieniać w czasie w zależności od kosztów CPU i indeksu cen, tak aby każda jednostka była „niezmienna”.
