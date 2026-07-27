# 3.0 Wprowadzenie

> **Dark – Streszczenie White Paper Bitcoin**
>
> **Czysto peer-to-peerowa wersja elektronicznej gotówki** pozwoliłaby na przesyłanie płatności online bezpośrednio od jednej osoby do drugiej bez pośrednictwa instytucji finansowej. **Podpisy cyfrowe stanowią część rozwiązania**, ale główne korzyści zostają utracone, jeśli **zaufana trzecia strona** jest nadal wymagana, aby zapobiec podwójnemu wydawaniu. Proponujemy rozwiązanie problemu podwójnego wydawania z wykorzystaniem **sieci peer-to-peer**. **Sieć znaczy czasem transakcje** poprzez haszowanie ich do ciągłego łańcucha **dowodu pracy opartego na haszach,** tworząc zapis, którego nie można zmienić bez ponownego wykonania **dowodu pracy**. Najdłuższy łańcuch służy nie tylko jako dowód kolejności zaobserwowanych zdarzeń, ale także jako dowód, że pochodzi on z największej puli mocy obliczeniowej CPU. Dopóki większość mocy CPU jest kontrolowana przez węzły, które nie współpracują w celu ataku na sieć, będą one generować najdłuższy łańcuch i wyprzedzać atakujących. **Sama sieć wymaga minimalnej struktury. Wiadomości są rozgłaszane w miarę możliwości, a węzły mogą opuszczać i dołączać do sieci według własnej woli**, akceptując najdłuższy łańcuch dowodu pracy jako dowód tego, co się wydarzyło podczas ich nieobecności.


Bitcoin nie pojawił się znikąd, lecz powstał na bazie pracy wielu osób z poprzednich dekad. Ten moduł przybliży fundamenty internetu, na których opiera się Bitcoin, a także badania i rozwój uznane w whitepaperze.

W latach 70. grupa osób zauważyła, że rząd USA w szczególności próbował ograniczyć dostęp do kryptografii, i postanowiła zadbać o to, by ta technologia była dostępna dla wszystkich ludzi, aby mogli chronić swoją prywatność w internecie. Niektórzy z tych wczesnych pionierów skupiali się również na potencjalnych korzyściach płynących z cyfrowego systemu „solidnych pieniędzy”, który mógłby służyć do przechowywania i wymiany wartości w rodzącym się internecie. Friedrich Hayek – czołowy przedstawiciel ekonomii austriackiej – już przed erą internetu wyobrażał sobie, jak mogłaby wyglądać idealna waluta oparta na wolnorynkowej konkurencji, ale uznał, że jest to technicznie i politycznie niewykonalne. Oprócz cyfrowej prywatności, ta grupa, która przekształciła się w Cypherpunks, próbowała zrealizować wizję Hayeka dotyczącą cyfrowych pieniędzy, lecz te próby kończyły się niepowodzeniem aż do momentu, gdy Satoshi opublikował swoje pomysły na liście mailingowej.

* Protokół TCP/IP (1976)
* Protokoły dla kryptosystemów z kluczem publicznym – Ralph Merkle (1980)
* Digicash – David Chaum (1989)
* Cyfrowe znakowanie czasem (lata 90.)
* Hashcash – Adam Back (1997)
* BitTorrent – Bram Cohen (2001)
* Reusable POW – Hal Finney (2004)
* Whitepaper Bitcoin – Satoshi Nakamoto (2008)

Kluczowy wpływ na rozwój Bitcoina miało pojawienie się ruchu Cypherpunk w latach 90. Opracowali oni kilka technologii kryptograficznych, w tym kryptografię z kluczem publicznym, umożliwiającą użytkownikom bezpieczną i prywatną komunikację oraz wymianę informacji. Wiele z opisanych tu osiągnięć i zaangażowanych osób należało do tej grupy.

Potrzeba cyfrowej gotówki została również zidentyfikowana i podjęto kilka prób jej stworzenia, ale miały one ograniczenia, które uniemożliwiły im sukces. Geniusz Satoshiego Nakamoto polegał na tym, że połączył te możliwości, a wraz z własnymi innowacjami zbudował na ich podstawie protokół Bitcoin używany do dziś. W kolejnych sekcjach przyjrzymy się niektórym z tych osiągnięć i wyjaśnimy, jak wpłynęły one na projekt Bitcoina. Omówimy także, jakie elementy układanki brakowały, które Satoshi zdołał rozwiązać.
