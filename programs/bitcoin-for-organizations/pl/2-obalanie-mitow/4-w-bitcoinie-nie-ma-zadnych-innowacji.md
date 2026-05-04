# 2.4 W Bitcoinie nie ma żadnych innowacji.

> Stworzenie tysiąca lasów kryje się w jednym żołędziu.  
_Ralph Waldo Emerson_

Krytycy często próbują twierdzić, że Bitcoin to „stara” lub „martwa” technologia, ponieważ nie zmienia protokołu warstwy bazowej tak często jak konkurencyjne blockchainy. To twierdzenie ignoruje zarówno powody, dla których zmiany w Bitcoinie są wprowadzane powoli, jak i ilość innowacji, które mają miejsce w celu skalowania sieci na wyższych warstwach, takich jak Lightning Network. Pomija również fakt, że wiele naszych najbardziej elastycznych i trwałych technologii także nie rozwija się szybko na warstwie bazowej.

Na przykład, nie ma już innowacji w protokole Transmission Control Protocol (TCP), który stanowi podstawę internetu. TCP został stworzony w 1974 roku. Ostatnia aktualizacja TCP miała miejsce w 1982 roku. Robi to, co powinien. Nie jest doskonały i toczą się dyskusje, czy powinniśmy zaktualizować IPv4, aby wspierać przyszły rozwój internetu. Jednak stwierdzenie, że od 1982 roku nie było żadnych innowacji w internecie, byłoby niezwykłym twierdzeniem. Cała ta innowacja miała miejsce „na” TCP, a nie „w” nim.

Zdecydowana większość innowacji, które się pojawiają, nie dzieje się „w” Bitcoinie, lecz „na” Bitcoinie. Pewnego dnia prawdopodobnie nie będzie już żadnych innowacji „w” Bitcoinie — i to powinno być celem, a nie krytyką, ponieważ będzie to odzwierciedleniem tego, jak fundamentalny stał się w wspieraniu globalnej gospodarki, zapewniając fundamenty dla globalnych, neutralnych i pozbawionych zezwoleń solidnych pieniędzy. Pieniędzy, które są solidne zarówno w sensie ekonomicznym — dzięki stałej podaży i niezmiennemu rejestrowi — jak i w sensie technologicznym, ponieważ nie ulegają zmianom, a to, co działa, miało lata nieprzerwanego działania. Bitcoin już osiągnął 100% dostępności przez ostatnie 10 lat.

Jednak byłby to powód do niepokoju, gdyby nie pojawiały się żadne innowacje „na” Bitcoinie. Przyjrzyjmy się temu na przestrzeni ostatnich 10 lat:



#### „W” Bitcoinie

Segregated Witness (SegWit) został wdrożony w 2017 roku, aby chronić przed modyfikowalnością transakcji i zwiększyć pojemność bloków. SegWit był także niezbędnym krokiem do efektywnego działania Lightning Network i niektórych sidechainów.

Taproot został wdrożony w 2021 roku, aby umożliwić grupowanie i weryfikację wielu podpisów poprzez wprowadzenie podpisów Schnorra, wprowadzenie języka skryptowego pozwalającego na bardziej złożone funkcje oraz zwiększenie prywatności i odporności na cenzurę transakcji.



#### „Na” Bitcoinie

##### Liquid Sidechain

Sidechain Liquid został wdrożony w 2018 roku. Liquid, podobnie jak inne sidechainy, to osobny rejestr blockchain, który jest powiązany z głównym blockchainem Bitcoina według z góry określonych zasad. Zasady te są na tyle elastyczne, że pozwalają Liquid rozwijać się i wprowadzać ulepszenia projektowe oraz skalowalności z czasem. Jednak powiązanie z blockchainem Bitcoina zapewnia, że całkowita podaż bitcoina na poziomie 21 milionów jest spójna na obu łańcuchach.

Aktywo w Liquid, L-BTC, jest powiązane dwukierunkowo z bitcoinem na głównym łańcuchu. Istnieją kompromisy dotyczące kosztów, szybkości, prywatności i bezpieczeństwa, które sprawiają, że L-BTC jest idealny do niektórych zastosowań. Koszty, szybkość i prywatność są poprawione w przypadku L-BTC, kosztem zaufania do organizacji tworzących Liquid Federation, które wspólnie kontrolują proces multisig 11 z 15 do wpłacania i wypłacania L-BTC na bitcoina i odwrotnie.

##### Lightning Network

Lightning Network został wdrożony w 2018 roku. Lightning został zaprojektowany jako sieć płatności peer-to-peer w formie grafu węzłów połączonych kanałami; nie jest to blockchain. Bitcoin jest blokowany przez operatora węzła na głównym blockchainie, aby udostępnić go do użycia w Lightning Network, co zapewnia, że używany jest tylko „prawdziwy” bitcoin. Węzły mogą następnie otwierać kanały płynnościowe za pomocą multisig smart kontraktów między sobą. Płatności znajdują trasy przez sieć od źródła do celu, optymalizując koszty przy założeniu, że wystarczająca płynność istnieje w odpowiednim kierunku między każdym krokiem węzła na trasie. Lightning Network znacząco poprawia koszty, szybkość i prywatność kosztem utraty bezpieczeństwa (lub zwiększenia wymaganego zaufania) oraz wzrostu złożoności. Jednak jest przeznaczony do płatności o dużej liczbie i niskiej wartości na co dzień, więc jest to bardzo rozsądny kompromis dla milionów codziennych transakcji (źródło: River, 2023).

##### Chaumian eCash Mints

Fediminty można traktować jako lightning network ograniczoną do danej społeczności. Są zaprojektowane tak, aby wykorzystywać zaufanie istniejące w określonych społecznościach (np. rodziny, wioski, grupy przyjaciół) w zamian za uproszczenie złożoności i zwiększenie prywatności użytkowników. To modułowe, otwartoźródłowe protokoły do przechowywania i przesyłania bitcoina w kontekście społecznościowym. Są interoperacyjne z samą Lightning Network.

**Cashu** to token na okaziciela, który można przechowywać na urządzeniu, takim jak telefon komórkowy; projekt ma na celu odtworzenie zalet fizycznej gotówki w formie cyfrowej. Cashu to przykład Chaumian eCash zbudowanego na Bitcoinie, który zwiększa prywatność i odporność na cenzurę oraz zmniejsza złożoność w zamian za zaufanie do używanej mennicy eCash. Mennice Cashu wydają tokeny eCash reprezentujące bitcoina, które mogą być wydawane przez użytkowników bez ujawniania ich tożsamości. Cashu jest interoperacyjny z Lightning Network.

Prawdopodobnie w przyszłości powstanie wiele kolejnych aplikacji warstwy 2, a na każdej z nich kolejne aplikacje warstwy 3.

Jako przykład niesamowitej liczby aplikacji budowanych na Lightning Network, poniżej znajduje się fragment z raportu badawczego Lightning Network przygotowanego przez River.

![The Lightning Network Industry Market Map 2023](https://cdn.sanity.io/images/vje9ehw2/staging/a5d3bdf5b343b7ae7e44663cf6e56a76a4bdec2d-501x706.svg)
