# 3.7 Bitcoin

Po wielu latach i nieudanych próbach Cypherpunks w większości zaczęli tracić zainteresowanie ideą cyfrowej waluty bez zezwoleń, gdy Adam Back otrzymał e-mail z linkiem do szkicu whitepaper zatytułowanego „electronic cash without a third party” od anonimowej osoby podającej się za Satoshi Nakamoto.

Podsumowując na tym etapie, mamy przynajmniej następujące idee:

* Podpisy kryptograficzne, które mogłyby zapewnić pewien poziom prywatności i anonimowości
* Koncepcja waluty bez pokrycia (B-Money)
* Propozycje (ale brak środków) ograniczające emisję nowej waluty
* Cyfrowe monety, których własność była przypisywana przez klucze publiczne (B-Money) i mogły być przenoszone przez podpisywanie oraz przypisywane na nowo na podstawie adresu odbiorcy (RPOW i Hashcash)
* Wszystkie węzły utrzymują kopię całkowicie rozproszonej księgi (B-Money) (wówczas odrzucone jako niepraktyczne)
* Protokół znakowania czasem – wykorzystanie haszowania drzewa Merkle’a do zapewnienia matematycznie udowadnialnej chronologii zdarzeń, którą trudno sfałszować, jeśli wszyscy użytkownicy przechowują te same zapisy
* Proof of work, aby powiązać rzeczywisty wysiłek z systemem (ale używając samego hasha jako waluty)
* Całkowicie zdecentralizowane sieci, w których wszyscy uczestnicy są równi i mogą dowolnie dołączać i opuszczać sieć (BitTorrent)
* Koncepcja powiązania nowych hashy z poprzednimi (Bit Gold i znakowanie czasem)

Czego wówczas brakowało:

* Realnego rozwiązania problemu „bizantyjskich generałów”
* Metody ograniczenia ilości pieniędzy w obiegu mimo ciągłych ulepszeń sprzętu
* Systemu zachęt do udziału (problem jajka i kury)

Drugą istotną różnicą między ostatnimi próbami a Bitcoinem było to, że Satoshi pracował nad kodem przez pewien czas, zgodnie z prawdziwą etyką „Cypherpunks piszą kod”, zanim ogłosił go na listach dyskusyjnych, w przeciwieństwie do Bit Gold i B-Money, które były bardziej koncepcyjne.

Jaka była innowacja, która wyróżniła Bitcoina na tle wcześniejszych prób stworzenia elektronicznej gotówki?

Proof of work miał być używany jako mechanizm konsensusu oraz sposób zapewnienia bezpieczeństwa i niezmienności: Zamiast używać hasha jako formy pieniądza, miał być wykorzystywany przez nowy proces koncepcyjny zwany kopaniem, gdzie węzeł grupował zestaw transakcji, dodawał losową liczbę, a następnie stosował haszowanie do „bloku” danych. Prawidłowy blok spełniający wymagania hasha był następnie ogłaszany w sieci. Bloki te były ze sobą powiązane poprzez hash poprzedniego bloku w każdym z nich, a najdłuższy łańcuch bloków był używany w przypadku remisu, gdy różne węzły weryfikowały i ogłaszały różne bloki jednocześnie, tworząc rozgałęzienia łańcucha. Proof of work stał się rozproszonym rozstrzygaczem remisów, rozwiązując problem bizantyjskich generałów.

Ci górnicy otrzymywali również zachętę do udostępniania mocy obliczeniowej wymaganej do przeprowadzenia proof-of-work poprzez przydzielanie im nowych bitcoinów za każdy blok. Ilość Bitcoinów, którą otrzymują, jest również zaprogramowana tak, aby zmniejszała się mniej więcej co 4 lata, aż wszystkie Bitcoiny zostaną wykopane, co tworzy twardy limit całkowitej liczby Bitcoinów, które kiedykolwiek będą w obiegu – 21 milionów.

Najbardziej oryginalnym pomysłem był sposób, w jaki rozwiązano problem ilości tworzonej waluty w miarę ulepszania sprzętu i zwiększania mocy sieci. Znaczniki czasu ustalonej liczby bloków (2016) były uśredniane, a jeśli były tworzone zbyt szybko, wymagany hash do utworzenia nowego bloku był utrudniany, jeśli zbyt wolno – ułatwiany. Było to wbudowane w zdecentralizowany protokół, który uruchamiają wszystkie węzły, więc każdy górnik ignorujący to traciłby energię na wydobycie bloku bez korzyści, ponieważ zostałby on odrzucony przez resztę sieci. Ta korekta zapewnia, że tworzenie nowych bloków pozostaje zgodne z planowanym harmonogramem emisji i motywuje górników do „grania według zasad”.

####   
Podsumowanie

Wiele elementów układanki potrzebnych do zbudowania zdecentralizowanego, peer-to-peer systemu elektronicznej gotówki opartego na zasadach zdrowego pieniądza było już gotowych, zanim Satoshi opublikował swój whitepaper i wkrótce po początkowym wydaniu kodu.

> Natura Bitcoina jest taka, że po wydaniu wersji 0.1 podstawowy projekt został ustalony na resztę jego istnienia  
_Satoshi Nakamoto_

Chociaż zaproponowano i przyjęto wiele pomysłów na ulepszenia (BIP), Bitcoin działa w tle od 2009 roku, podążając za protokołem zaprojektowanym w początkowym wydaniu i praktycznie bez zakłóceń. Wszystkie ulepszenia zostały wprowadzone przy zachowaniu kompatybilności wstecznej ze wszystkimi poprzednimi wersjami.



##### Notatki

1. Wyjaśnienie problemu bizantyjskich generałów – zobacz [https://pl.wikipedia.org/wiki/Problem_bizantyjskich_genera%C5%82%C3%B3w](https://en.wikipedia.org/wiki/Byzantine_fault)
