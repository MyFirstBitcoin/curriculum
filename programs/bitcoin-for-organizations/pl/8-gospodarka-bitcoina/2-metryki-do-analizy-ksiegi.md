# 8.2 Metryki do analizy księgi

Ponieważ przejrzystość Bitcoina jest inna niż w tradycyjnych systemach finansowych — gdzie większość przepływów pieniężnych odbywa się za zamkniętymi drzwiami instytucji — powstaje bogate pole do analityki on-chain, gdzie dane na poziomie sieci stają się soczewką do zrozumienia zachowań użytkowników, przepływów pieniężnych i długoterminowych trendów. Te wskaźniki mogą pomóc odpowiedzieć na konkretne pytania, takie jak: jak aktywnie wykorzystywana jest sieć, czy monety są akumulowane czy wyprzedawane oraz czy sieć staje się bardziej bezpieczna.

Zrozumienie tych wskaźników jest pomocne nie tylko dla użytkowników Bitcoina, ale także dla badaczy i decydentów poszukujących wglądu w ten wyjątkowo przejrzysty system finansowy.

Ta sekcja zawiera kilka najczęściej używanych wskaźników do analizy aktywności Bitcoina pogrupowanych w podkategorie. Nie jest to lista wyczerpująca. Odwiedź [www.bitcoinmagazinepro.com/charts](https://www.bitcoinmagazinepro.com/charts) aby zobaczyć pełniejszą listę i opisy.



#### 8.2.1 Wskaźniki adresów

Wskaźniki adresów są przydatne do monitorowania w czasie, ponieważ wskazują poziom aktywności w sieci Bitcoin. Na przykład, gdy Bitcoin jest coraz szerzej przyjmowany, liczba aktywnych adresów rośnie. Możemy to przeanalizować dalej, wyodrębniając liczbę adresów, które posiadają minimalnie określoną ilość Bitcoina, na przykład 0,1 BTC, w określonym przedziale czasu, np. w ciągu roku. Choć daje to obraz adopcji Bitcoina w czasie, jest to niedoskonałe, ponieważ jedna osoba może posiadać wiele adresów Bitcoina. Z drugiej strony giełdy lub ETF-y mogą wyglądać jak pojedyncze podmioty, gdy przechowują środki dla wielu osób.

![Bitcoin: Addresses Hodling > X BTC by Year](https://cdn.sanity.io/images/vje9ehw2/staging/b88a9239820e45ed50ce00812170e2bb4d02b5d2-1407x766.png)

_Adresy hodlujące Bitcoina > X BTC według roku. Źródło: Bitcoin Magazine Pro._

Porównując adresy z aktualną ceną rynkową BTC, można zobaczyć procent wszystkich adresów Bitcoina, które są na plusie. Pozwala to śledzić nastroje rynkowe, ponieważ widzimy, jaka część rynku trzyma BTC z zyskiem lub stratą.

Na przykład, **Procent niezrealizowanego zysku** na poniższym wykresie pokazuje odsetek wszystkich adresów w księdze z niezrealizowanym zyskiem mierzonym w dolarach amerykańskich. Zauważ, że ponieważ wykres poniżej został wykonany blisko historycznego maksimum Bitcoina, procent adresów wykazujących niezrealizowany zysk jest bliski stu procent. Widzimy też, że długotrwałe okresy, gdy Procent niezrealizowanego zysku znajduje się poniżej jednej odchylenia standardowego od średniej, są rzadkie. Dlatego spadek poniżej tej linii może sugerować dobry moment wejścia dla kupujących.

![Percent Unrealised Profit](https://cdn.sanity.io/images/vje9ehw2/staging/f306f03f31ce4faada8bf34137dd76f9d550697a-1041x491.png)

_Procent niezrealizowanego zysku. Źródło: checkonchain.com_



#### 8.2.2 Wskaźniki on-chain

Wskaźniki on-chain są przydatne, ponieważ dają wgląd w zachowanie sieci, wykraczający poza to, co pokazują same ceny i wskaźniki adresów. Pomagają analitykom zrozumieć działania i nastroje różnych typów uczestników, takich jak długoterminowi posiadacze i krótkoterminowi traderzy, śledząc, jak monety są przechowywane, przemieszczane lub wyceniane w czasie. Te wskaźniki wykorzystują przejrzystość księgi, by ujawnić ukryte dynamiki rynku, takie jak akumulacja, dystrybucja czy nawet przekonanie inwestorów. Dzięki temu są szczególnie przydatne do identyfikowania trendów strukturalnych, oceny, czy rynek jest przegrzany lub niedowartościowany, oraz przewidywania punktów zwrotnych w cyklu rynkowym.

Na przykład, analizując wartość posiadanych BTC od czasu ostatniej transakcji, możemy wywnioskować, czy rynek znajduje się w stanie stresu (jak może to mieć miejsce podczas głębokiego dołka cyklu). Ten wskaźnik znany jest jako **Cena zrealizowana** i daje nam „średni koszt nabycia” wszystkich BTC w obiegu. Jeśli cena rynkowa spada poniżej Ceny zrealizowanej, oznacza to, że większość adresów trzyma Bitcoina na papierowej stracie.

Grupując dalej dane z księgi na przedziały wiekowe, możemy pokazać, jak ilość BTC przemieszcza się między adresami w czasie, co tworzy faliste wzory na wykresie znane jako **fale HODL**.

![Bitcoin HODL Waves](https://cdn.sanity.io/images/vje9ehw2/staging/ce108e45a1a7217e081101e4a276ee2d9e95a22e-1129x577.png)

_Fale HODL Bitcoina. Źródło: Bitcoin Magazine Pro._

Fale HODL pokazują, co robią długoterminowi, średnioterminowi i krótkoterminowi posiadacze ze swoimi BTC. Na przykład, na powyższym wykresie krótkoterminowi posiadacze są pokazani na czerwono i pomarańczowo i widać skoki aktywności, gdy ta grupa masowo kupuje blisko szczytów rynkowych. Z drugiej strony widać, że bardzo długoterminowi posiadacze (na fioletowo i niebiesko) stale zwiększają swój udział w sieci, co wskazuje na silne przekonanie tych grup. Wykres nie jest doskonały, ponieważ niektóre monety mogą przechodzić ze starych na nowe adresy pod kontrolą tego samego użytkownika. Jednak daje ciekawy obraz przekonania długoterminowych posiadaczy.

Innym sposobem badania „mądrych pieniędzy” długoterminowych posiadaczy jest analiza **Coin Days Destroyed** (CDD). Pojęcie „Coin Days” to iloczyn liczby BTC i liczby dni od ostatniego ruchu tych monet. Na przykład 5 BTC, które nie były ruszane przez 100 dni, zgromadziło 500 coin days, a 10 BTC nieprzemieszczane przez 10 dni to 100 coin days. W ten sposób nadajemy większą wagę monetom trzymanym dłużej. Gdy te monety zostaną przesłane, te coin days są „niszczone”. Wskaźnik ten pokazuje wzrosty CDD w okresach znaczących ruchów cenowych, co daje analitykom możliwość oddzielenia rutynowej aktywności rynkowej od istotnych zmian w nastrojach długoterminowych posiadaczy.

Innym wskaźnikiem, który może pomóc określić, czy rynek niedowartościowuje lub przewartościowuje BTC, jest stosunek wartości rynkowej do wartości zrealizowanej, czyli **MVRV**. Oblicza się go po prostu jako stosunek wartości rynkowej (liczba BTC w obiegu pomnożona przez cenę rynkową) do wartości zrealizowanej (suma wszystkich BTC od czasu ich ostatniego ruchu). Wysokie MVRV sugeruje, że więcej monet jest na plusie (często widoczne blisko szczytów rynkowych), a niskie MVRV oznacza, że wiele monet jest trzymanych ze stratą (widoczne blisko dołków rynkowych).



#### 8.2.3 Wskaźniki wydobycia

Wskaźniki wydobycia są przydatne do zrozumienia bezpieczeństwa, bodźców ekonomicznych i ogólnego stanu sieci Bitcoin. Takie wskaźniki jak hashrate, przychody górników, trudność i stosunek opłat pokazują, ile mocy obliczeniowej zabezpiecza blockchain i jak dobrze górnicy są wynagradzani za swoją działalność.

Najczęściej przywoływanym wskaźnikiem zdrowia sieci i siły jej bezpieczeństwa jest **Hashrate** sieci Bitcoin. Ponieważ proces wydobycia zabezpiecza sieć i potwierdza, że transakcje w księdze są ważne, im większa moc obliczeniowa (lub moc haszująca), tym trudniej byłoby złośliwemu aktorowi przejąć i zaatakować sieć.

![Bitcoin Hashrate](https://cdn.sanity.io/images/vje9ehw2/staging/fcb4a24c431a37580d3d6c4ec62b664e7e41c362-1134x584.png)

_Hashrate Bitcoina. Źródło: Bitcoin Magazine Pro._

Powyższy wykres pokazuje, że w maju 2025 roku całkowita moc obliczeniowa sieci wynosi około 900 TeraHash/s (900 bilionów kryptograficznych obliczeń „hash” na sekundę). Jeśli hashrate rośnie, oznacza to, że sieć staje się bardziej bezpieczna, co jest uspokajające dla użytkowników.

Wskaźnik Puell Multiple (stworzony przez Davida Puella) patrzy na cykl rynkowy z perspektywy górników i ich przychodów. Wskaźnik oblicza się, dzieląc dzienną emisję BTC (w USD) przez 365-dniową średnią kroczącą wartości dziennej emisji. Pomaga on zidentyfikować okresy stresu lub ulgi dla górników. Historycznie, wartość powyżej 3 poprzedzała spadki wartości rynkowej BTC, ponieważ wskazuje, że górnicy są bardzo dochodowi. Wartość poniżej 0,5 oznacza stres i historycznie wskazywała na dołki rynkowe wartości BTC.
