# 2.3 Bitcoin jest zbyt wolny, aby być globalną walutą

> Wizjonerzy widzą przyszłość pracowników pracujących zdalnie, interaktywnych bibliotek i multimedialnych sal lekcyjnych. Mówią o elektronicznych zebraniach miejskich i wirtualnych społecznościach... Prawda jest taka, że żadna baza danych online nie zastąpi twojej codziennej gazety, żaden CD-ROM nie zastąpi kompetentnego nauczyciela i żadna sieć komputerowa nie zmieni sposobu działania rządu.  
_Clifford Stroll_

17 lat później Newsweek zakończył wydawanie drukowane i stał się dostępny wyłącznie online. Wyobraź sobie, że żyjesz w 1974 roku, kiedy po raz pierwszy stworzono Transmission Control Protocol (TCP).

Nikt nie przewidział smartfona, z wszystkimi jego aplikacjami, trzymanego w dłoni. Nikt nie przewidział systemu nawigacji satelitarnej w twoim samochodzie.

Internet nie pojawił się nagle, lecz stopniowo jako ewolucja protokołów i warstw. Te ewolucje opierały się na TCP, ale głównie go nie zmieniały.

> Patrząc na przejście do przyszłych platform komunikacyjnych, widzę, że piękno protokołów internetowych polega na oddzieleniu warstw pomiędzy usługą a technologią.  
_Michael K Powell_



##### Porównaj ewolucję Bitcoina z ewolucją internetu

TCP był konieczny, ale niewystarczający dla powstania wszystkiego innego w internecie. Ewolucja Bitcoina wydaje się podążać podobną ścieżką. Otwarte systemy wydają się być bardziej odporne i skuteczne, gdy są rozwijane warstwowo, chociaż może upłynąć dużo czasu między położeniem początkowych fundamentów a powszechną adopcją. Rozwiązania typu „wszystko w jednym” nie wydają się być tak skuteczne w otwartych systemach, jak te budowane warstwowo na protokołach. Tak jak nikt nie musiał przebudowywać internetu, bo nie można było przesyłać filmów przez TCP, tak prawdopodobnie będzie z Bitcoinem.

Już teraz istnieje wiele protokołów warstwy 2 działających na Bitcoinie, a na nich działa wiele aplikacji (zobacz sekcję 201.4 po więcej szczegółów na ten temat).

Zamiast skupiać się na tym, czego bitcoin i sieć Bitcoin nie potrafią dziś zrobić, pomyśl o tym, co już dziś jest możliwe, i porównaj to z tym, co było możliwe 10 lat temu. Wykonaj to ćwiczenie z internetem z lat 1985–1995, a następnie zobacz, jak bardzo internet przyspieszył przez kolejne 30 lat i jakie aplikacje stały się możliwe. Wykorzystaj tę wiedzę, aby wyobrazić sobie, jak Bitcoin może wyglądać za kolejne 10 lat, albo nawet 30, jeśli twoja wyobraźnia sięga tak daleko.



##### Porównaj Bitcoina z istniejącym globalnym systemem pieniężnym

Główne twierdzenie, że Bitcoin jest zbyt wolny, by być globalnym pieniądzem, jest prawdopodobnie prawdziwe, jeśli ograniczymy się do podstawowej warstwy Bitcoina. Prawdą jest też, że podstawowa warstwa naszych obecnych systemów pieniężnych jest zbyt wolna, by być globalnym pieniądzem, jeśli podobne ograniczenie oznaczałoby brak infrastruktury płatniczej budowanej przez prywatne banki i usługi płatnicze, takie jak Visa i Mastercard. Nasz obecny system jest zbudowany warstwowo, więc możemy oczekiwać, że przyszłość będzie wyglądać podobnie. Niektóre kompromisy projektowe, takie jak między zaufaniem, szybkością a kosztem, mogą się przenosić między systemami dostarczającymi te same rozwiązania, choć są one zbudowane do przesyłania różnych tokenów wartości.

Niektóre z istniejących warstw 2 na Bitcoinie bezpośrednio rozwiązują problem szybkości, na przykład Liquid i Lightning Network (zobacz sekcję 201.4 po więcej szczegółów). Liquid jest szybszy i tańszy niż blockchain Bitcoina, a Lightning Network jest jeszcze szybszy i tańszy niż Liquid. Rozwój wielu warstw 2, każdej z innymi kompromisami, jest czymś oczekiwanym i zdrowym.

Prawdopodobnie pojawi się więcej warstw 2 i 3 oraz eksplozja aplikacji korzystających z nich, tak jak to miało miejsce podczas ewolucji internetu.



##### Motywacja

Gdy pojawia się ta krytyka, warto zastanowić się, czy krytyk nie ma innych motywacji. Na przykład, czy nie ma nowego lub innego projektu blockchain? Może to być analogiczne do próby sprzedaży lepszego Transmission Control Protocol.

Dylemat skalowalności, czyli Blockchain Trilemma, został po raz pierwszy przedstawiony przez Vitalika Buterina w 2017 roku. Mówi on, że w projektowaniu blockchaina zawsze istnieje kompromis między decentralizacją, bezpieczeństwem a skalowalnością. Każdy, kto podnosi zarzut, że Bitcoin jest zbyt wolny i że ma szybsze rozwiązanie w blockchainie warstwy 1, poświęca część bezpieczeństwa lub decentralizacji, aby to osiągnąć. Taki kompromis może mieć sens dla blockchaina zaprojektowanego do innych celów, ale dla globalnego pieniądza kolejność priorytetów musi być następująca:


> **Light**
>
> * **Decentralizacja**
>   * Umożliwia usunięcie zaufanych pośredników
> * **Bezpieczeństwo**
>   * Powstrzymuje złych aktorów przed manipulowaniem transakcjami lub księgą
> * **Skalowalność**
>   * Pozwala systemowi skalować się ekonomicznie pod względem liczby użytkowników i szybkości


Pierwsze dwie cechy tworzą środowisko dla emisji bez twórców, płatności bez pośredników i przechowywania bez zarządców.

Bitcoin dokonuje właściwego wyboru spośród trzech cech projektowych blockchaina, biorąc pod uwagę, że jego docelowym zastosowaniem jest globalny pieniądz, a kompromisy w zakresie skalowalności i szybkości łagodzi poprzez warstwy.

> Satoshi odkrył, jak chronić integralność cyfrowego pieniądza bez zaufanych pośredników – nie są potrzebni twórcy, pośrednicy ani zarządcy.  
_Resistance Money, 2024, Bailey, Retter, Warmke_
