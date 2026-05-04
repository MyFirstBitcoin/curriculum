# 3.1 Rozwój TCP/IP

Większość z nas zna dziś protokoły TCP/IP jako fundament internetu. Ich początki sięgają końca lat 70., kiedy naukowcy badali alternatywne rozwiązania dla Arpanetu – jeszcze wcześniejszej sieci stworzonej przez Departament Obrony USA w celu umożliwienia współdzielenia zasobów między odległymi komputerami. TCP/IP stał się standardowym protokołem dla Arpanetu w 1983 roku, co doprowadziło do jego dominacji jako modelu sieciowego pod koniec lat 90. i stanowi dziś podstawę internetu, na którym działa Bitcoin.


| Model OSI | TCP/IP |
| --- | --- |
| Aplikacja | Aplikacja |
| Prezentacja | Aplikacja |
| Sesja | Aplikacja |
| Transport | Transport |
| Sieć | Sieć |
| Łącze danych | Łącze danych |
| Warstwa fizyczna | Warstwa fizyczna |


W tym samym czasie, gdy rozwijano model TCP/IP, Międzynarodowa Organizacja Normalizacyjna (ISO) oraz branża telekomunikacyjna (CCITT) opracowywały podobne, lecz bardziej rozbudowane ramy. Proces tworzenia nowych protokołów lub sugerowania zmian był jednak powolny i nieporęczny w porównaniu z bardziej zdecentralizowanym podejściem stosowanym przy TCP/IP, co doprowadziło do dominacji tego drugiego rozwiązania.

##### Wniosek o zmianę

Wszelkie proponowane rozwinięcia istniejących protokołów lub pomysły na nowe mogą być zgłaszane w modelu TCP/IP poprzez **Wniosek o zmianę** proces. Przechodzą one przez proces zatwierdzania, zarządzany przez Internet Engineering Task Force (IETF), a po zatwierdzeniu stają się otwartym oprogramowaniem, co pozwala każdemu na ich wdrożenie i przyjęcie. Przykłady warte uwagi:

* 1969 RFC 1 Opisano, jak pakiety będą przesyłane w Arpanecie
* 1981 RFC791 zdefiniował protokół internetowy V4 – nadal szeroko stosowany
* 1982 RFC 821 Prosty protokół przesyłania poczty elektronicznej
* 1987 System nazw domen – sposób rozwiązywania nazw domen na adresy IP
* 1999 RDC 2616 Protokół przesyłania hipertekstu – kluczowy dla przeglądania stron WWW


> **Callout**
>
> **Bitcoin Improvement Proposal** (BIP) stosuje podobne podejście jak RFC, ale skupia się wyłącznie na ulepszeniach samego Bitcoina, a nie na rozwoju nowych lub alternatywnych protokołów. Bitcoin również czerpie z tego modelu warstwowego i zobaczysz dodatkowe protokoły opisywane jako warstwa druga lub trzecia.


Podobnie jak podstawowe warstwy modelu TCP/IP zmieniały się stosunkowo niewiele w ostatnich dekadach, a innowacje zachodziły na wyższych warstwach, tak i podstawowa warstwa Bitcoina prawdopodobnie będzie się teraz zmieniać bardzo powoli, a rozwiązania skalujące, takie jak Lightning i Liquid, będą rozwijane powyżej niej.

Dobrym przykładem tego, jak protokoły warstwy bazowej stają się trudne do zmiany z upływem czasu, jest IPv6. Oczekiwane wyczerpanie przestrzeni adresowej w IPv4 stworzyło zapotrzebowanie na nowy protokół. Pierwszy projekt standardu powstał w 1998 roku, ale został zatwierdzony jako standard internetowy dopiero w 2017 roku. Chociaż rozwiązał wiele problemów IPv4 i jest znacznie bardziej przyszłościowy, jego wdrażanie w branży przebiega bardzo powoli. W tym czasie na wyższych warstwach zdefiniowano wiele nowych protokołów umożliwiających multimedia, e-mail itp.

##### Klocki budulcowe używane przez Bitcoina

To rozdzielenie problemów związanych z łącznością pozwala na niezależny rozwój protokołów względem warstw powyżej i poniżej. Zamiast wymyślać rozwiązania na nowo dla każdej warstwy, sieć Bitcoin może polegać na podstawowych możliwościach sieci dostarczanych na warstwie fizycznej i łącza danych.


| Warstwa | Oryginalny TCP/IP |
| --- | --- |
| Aplikacja | Używa systemu nazw domen (DNS) do identyfikacji sąsiednich węzłów. Port 8333 sygnalizuje protokół Bitcoina. |
| Transport | UDP do komunikacji FIBRE między górnikami dla niskich opóźnień. TCP do komunikacji P2P między węzłami. |
| Transport | Routing TOR: Zapewnia anonimowość i prywatność. Protokół rozgłoszeniowy: Kieruje ruchem w sieci. |
| Łącze | Działa na dowolnym medium (np. Ethernet, Wi-Fi itp.) |
| Warstwa fizyczna | Transmisja fizyczna przez sieć bezprzewodową, Ethernet lub inne interfejsy sprzętowe. |


##### Bitcoin jest neutralnym protokołem do przesyłania wartości, tak jak HTTPS jest protokołem do przesyłania informacji

* **HTTPS**: Bezpieczne strony internetowe
* **SMTP**: Wysyłaj e-maile
* **FTP**: Przesyłaj pliki
* **DNS**: Zarządzaj nazwami domen
* **BTC**: Przechowuj i przesyłaj wartość

Bitcoin umożliwia niezawodne przenoszenie wartości bez konieczności korzystania z pośredników, pomiędzy ludźmi lub urządzeniami przez Internet. Oczekuje się, że to odblokuje ogromną wartość.
