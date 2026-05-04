# 2.7 Bitcoin nie jest naprawdę zdecentralizowany

> Złożoność kryptowalut wynika z prób decentralizacji — poprzez rozproszenie władzy i zarządzania w systemie teoretycznie nie ma potrzeby istnienia zaufanych pośredników, takich jak instytucje finansowe. Taka była idea początkowego white paper Bitcoin, który zaproponował kryptograficzne rozwiązanie umożliwiające przesyłanie płatności bez udziału instytucji finansowych czy innych zaufanych pośredników. Jednak Bitcoin bardzo szybko stał się scentralizowany i obecnie zależy od niewielkiej grupy programistów oraz pul wydobywczych, aby funkcjonować  
_Międzynarodowy Fundusz Walutowy_

Jak pokazuje powyższy cytat z dość niedawnego wpisu Międzynarodowego Funduszu Walutowego, główny nurt branży finansowej wciąż twierdzi, że Bitcoin nie jest zdecentralizowany, a także myli Bitcoin z innymi aktywami kryptowalutowymi.

##### Wprowadzenie

![Trilemma](https://cdn.sanity.io/images/vje9ehw2/staging/7aad0804113eed4fedacf20ecfb4fbd9666eb0c4-161x167.svg)

Decentralizacja jest kluczowym aspektem Bitcoina. Możliwość utrzymania zasad protokołu, takich jak rzadkość i dystrybucja, bez centralnej władzy sprawia, że może on pełnić rolę pieniądza bez pozwolenia dla globalnego społeczeństwa.

Jak zauważył Satoshi w swojej korespondencji online, zdecentralizowane usługi takie jak BitTorrent „dawały sobie radę” z rządowymi represjami, w przeciwieństwie do usług z określonym właścicielem i scentralizowanymi serwerami. Wyraźnie martwił się o potencjalne ryzyko, że rządy lub inne podmioty mogą zamknąć lub w inny sposób negatywnie wpłynąć na Bitcoin.

W tym kontekście interesuje nas decentralizacja:

* Rozwoju i zarządzania kodem uruchamiającym protokół; kto może zmieniać zasady?
* Funkcji wydobycia, która tworzy nowe bloki zgodnie z zasadami i weryfikuje pod kątem podwójnego wydania
* Węzłów, które weryfikują transakcje pod kątem ważności i przechowują kopię łańcucha bloków

##### Programiści

Bitcoin to protokół open-source, do którego każdy ma dostęp — można go przeglądać, pobierać, kopiować lub sugerować zmiany. Jest dostępny w bibliotece GitHub, a kod źródłowy został pierwotnie uruchomiony w 2009 roku przez Satoshiego Nakamoto. Każdy może pobrać kod i uruchomić węzeł, z których większość działa na oryginalnym oprogramowaniu Bitcoin Core, które było aktualizowane z biegiem czasu.

![How Does an idea Make Its Way Into Bitcoin Core?](https://cdn.sanity.io/images/vje9ehw2/staging/49f70d059c9dbe19a6e4500e9abd8db66ca97bff-1300x1439.png)

_Źródło: https://river.com/learn/what-is-bitcoin-core/_

Rozwój Bitcoin Core podąża za najlepszymi praktykami rozwoju open source. W dowolnym momencie może być dowolna liczba programistów piszących lub przeglądających zmiany w kodzie. Muszą oni wysłuchać uwag operatorów węzłów i górników, a także użytkowników, zanim wprowadzą jakąkolwiek istotną zmianę w kodzie, która zostanie przejrzana i zatwierdzona, jak pokazano na powyższym schemacie, zanim trafi do kodu.

Zasady Bitcoina są następnie zakodowane w tym oprogramowaniu Bitcoin Core, które działa na każdym węźle. Każdy może zaproponować zmianę zasad – zasady to kod, ale nie są _tylko_ kodem, są _uzgodnionym_ kodem. Jeśli zostaną zmienione jednostronnie, nowy kod nie jest już częścią konsensusu i nie jest już częścią Bitcoina. Zmiana czegoś w Bitcoinie i pozostanie w konsensusie jest trudna. Proponowane zmiany w kodzie dzielą się na trzy kategorie:

* W ramach istniejących zasad: Drobne ulepszenia, takie jak poprawki literówek, lepszy interfejs użytkownika czy zarządzanie danymi, mogą należeć do tej kategorii i stosunkowo łatwo uzyskać akceptację.
* Dodanie nowej zasady, która wprowadza ograniczenia do istniejących zasad – na przykład zmniejszenie rozmiaru bloku. Nazywa się to „miękkim forkiem”. Węzły, które nie wdrożą zmiany kodu i pozostaną przy starej wersji, nadal będą mogły uczestniczyć w sieci.
* Dodanie nowej zasady, która łamie obecne zasady, np. zwiększenie rozmiaru bloku. Węzły, które nie zaktualizują kodu, odrzucą blok utworzony w większym rozmiarze jako nieważny. Nazywa się to „twardym forkiem” i powoduje rozdzielenie łańcucha między węzłami działającymi na oryginalnym i nowym kodzie oraz tworzy nową monetę. Miało to miejsce wcześniej, ale nie przyniosło długoterminowego sukcesu nowej monecie, ponieważ większość węzłów zdecydowała się pozostać przy oryginalnym kodzie.

Dlatego żadna pojedyncza osoba ani grupa nie może jednostronnie zmienić kodu Bitcoina bez uzyskania konsensusu, w przeciwnym razie ryzykuje rozdzielenie łańcucha i powstanie nowej monety według innego zestawu zasad.

##### Wydobycie

Funkcja wydobycia weryfikuje transakcje tak jak każdy inny węzeł w sieci, ale następnie zużywa energię potrzebną do utworzenia nowego bloku, który spełnia zasady konsensusu zapisane w kodzie. Sukces pozwala górnikowi uzyskać nagrody w postaci opłat transakcyjnych i nagród w Bitcoinie (w chwili pisania 3,125 monety za blok).

Wydobycie zwykle odbywa się w tzw. pulach wydobywczych, gdzie ludzie łączą moc obliczeniową (hashrate), aby zwiększyć szanse na wydobycie bloku i podzielić się nagrodami. Istnieje ryzyko, że jedna lub więcej takich pul może się połączyć, aby osiągnąć 51% dominacji w wydobyciu i zasadniczo przeforsować własne zasady walidacji sieci, by podwójnie wydać monety. Wymagałoby to jednak ogromnych zasobów i kosztów, a indywidualni górnicy mogą w każdej chwili łatwo przejść do innej puli. Taki atak prawdopodobnie spowodowałby też załamanie wartości bitcoina, ponieważ byłoby oczywiste, że integralność sieci została naruszona. Atakujący musiałby więc szybko zamienić zdobyte bitcoiny na walutę fiducjarną, zanim wartość spadnie. To sprawia, że długotrwały atak jest jeszcze trudniejszy do utrzymania, a więc bardziej opłaca się górnikowi lub operatorowi puli przestrzegać zasad i próbować wydobywać ważne bloki.

Geograficzne rozproszenie funkcji wydobycia jest również ważne, aby np. rządy nie mogły przejąć mocy wydobywczej lub jej wyłączyć. Na przykład niedawny zakaz wydobycia w Chinach pokazał, że Bitcoin potrafi się dostosować i przetrwać taką interwencję rządową, szybko adaptując się i odzyskując moc obliczeniową po jej utracie.

##### Węzły

W przeciwieństwie do wydobycia, które wymaga znacznych nakładów finansowych, aby skutecznie konkurować w wyścigu o nowe bloki, czy rozwoju kodu, który wymaga umiejętności programistycznych, uruchomienie węzła to coś, co każdy zainteresowany utrzymaniem decentralizacji Bitcoina może zrobić.

Węzły uruchamiają oprogramowanie Bitcoin Core i egzekwują zasady zawarte w kodzie, aby upewnić się, że górnicy nie oszukują, np. przyznając sobie większą nagrodę za blok niż dozwolona. Egzekwują także limit podaży 21 milionów, co jest kluczowe dla utrzymania rzadkości Bitcoina. Aby jakikolwiek rząd lub zły aktor mógł zatrzymać Bitcoina, musiałby zniszczyć każdą pojedynczą kopię łańcucha bloków, która obecnie działa na tysiącach węzłów na całym świecie — co jest niemal niemożliwe.

##### Ludzie

Kolejnym aspektem potencjalnej centralizacji są ludzie. Każda inna „altcoina” ma lidera — kogoś, kogo można potencjalnie zmusić do popierania zmian niekorzystnych dla Bitcoina. Satoshi Nakamoto pozostał wystarczająco długo, by upewnić się, że Bitcoin jest na drodze do sukcesu, po czym zniknął na dobre, pozostawiając go w rękach innych, by rozwijali i ulepszali oprogramowanie.

A co z osobami posiadającymi duże ilości Bitcoina? Wczesni inwestorzy, którzy trzymali swoje monety i ich nie stracili, są teraz bardzo zamożni. Warto zauważyć, że tak może być, ale nie daje im to większego wpływu na system niż komukolwiek innemu, w przeciwieństwie do monet „proof of stake”, gdzie wcześni użytkownicy, którzy już są bogaci w tej monecie, zyskują przewagę w podejmowaniu decyzji i dystrybucji przyszłych monet. To nieuchronnie prowadziło lub doprowadzi do centralizacji z czasem.

##### Podsumowanie

Jakie potencjalne zagrożenia może próbować ograniczyć decentralizacja?

* Rządowe wyłączenie lub zakazanie Bitcoina
* Niepożądane zmiany w kodzie, które faworyzują jedną grupę interesów w Bitcoinie, np. zwiększenie nagrody za blok
* Wymuszenie zmian w protokole przez rząd lub złych aktorów w celu wpłynięcia na kierunek rozwoju protokołu
* Możliwość przejęcia sieci przez pulę górników i „podwójnego wydania” Bitcoina – atak 51%

Jak widzimy, połączenie węzłów, programistów i górników, a także zastosowanie mechanizmu „proof of work”, decentralizuje Bitcoina na tyle, że te potencjalne zagrożenia nie są uznawane za poważne. Społeczność będzie musiała nadal monitorować sytuację, aby tak pozostało.
