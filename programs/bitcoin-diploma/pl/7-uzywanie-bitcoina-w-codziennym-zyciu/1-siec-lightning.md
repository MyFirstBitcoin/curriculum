# 7.1 Sieć Lightning

Lightning Network to system płatności, który pozwala użytkownikom szybko i tanio wysyłać oraz odbierać bitcoiny. Działa poprzez utworzenie wspólnego portfela, w którym obie strony deponują część swoich bitcoinów. Następnie mogą dokonywać nieograniczonej liczby transakcji między sobą bez konieczności zapisywania każdej z nich w głównym łańcuchu bloków. Dzięki temu omijają potrzebę weryfikacji i dołączania każdej pojedynczej transakcji do bloku, co sprawia, że proces jest zarówno szybki, jak i opłacalny. Niższe opłaty oznaczają, że Lightning Network może być używany do drobnych płatności, które nie zawsze są opłacalne w sieci głównej. Gdy strony zdecydują się zakończyć współpracę, tylko końcowe saldo zostaje zapisane w blockchainie.

Wyobraź sobie dzień pracy w kawiarni. Planując zostać na dłużej, otwierasz rachunek i wpłacasz zaliczkę zamiast płacić za każde zamówienie osobno. Pod koniec dnia ty i właściciel przeglądacie rachunek, aby go rozliczyć. Jeśli twoja wpłata była większa niż wydatki, otrzymujesz różnicę z powrotem; jeśli wydałeś więcej, dopłacasz brakującą kwotę.

Ten schemat można rozszerzyć na większą liczbę uczestników. Na przykład podczas jednej z wizyt w kawiarni przyprowadzasz przyjaciela, którego barman nie zna i nie może otworzyć mu rachunku. Oferujesz swojemu przyjacielowi skorzystanie z twojego rachunku, a w zamian umawiacie się, że rozliczycie się prywatnie. Teraz wyobraź sobie tysiące osób robiących to samo jednocześnie, pozwalając innym korzystać z istniejących rachunków, aby łączyć się z jeszcze większą liczbą osób — tak właśnie działa Lightning Network!

Dzięki Lightning możesz dokonywać płatności do każdego użytkownika w sieci, nie tylko do osoby, z którą masz bezpośredni rachunek — pod warunkiem, że można znaleźć trasę między obiema stronami. Twoja płatność może przechodzić przez sieć, aż dotrze do odbiorcy, nawet jeśli nie masz otwartego kanału bezpośrednio z nim.

Przyjrzyjmy się różnicy między transakcjami on-chain a off-chain.

##### Transakcje on-chain

To transakcje, które odbywają się bezpośrednio w blockchainie Bitcoina. Potwierdzenie trwa około 10 minut, a opłaty zależą od wielkości transakcji w bajtach wirtualnych. Są bardziej bezpieczne, ale wolniejsze, ponieważ wymagają konsensusu sieci.

##### Transakcje w Lightning Network

Te transakcje odbywają się w osobnej sieci zbudowanej na bazie blockchaina Bitcoina. Rozliczają się szybciej i z niższymi opłatami. Są często używane tam, gdzie liczy się szybkość i koszt transakcji. W porównaniu do transakcji on-chain są mniej bezpieczne.


|  | Sieć Bitcoin | Lightning Network |
| --- | --- | --- |
| Definicja | Zdecentralizowana cyfrowa sieć wykorzystująca kryptografię do zabezpieczania transakcji finansowych. | Protokół płatności drugiej warstwy działający na blockchainie Bitcoina, umożliwiający szybsze i tańsze transakcje. |
| Zalety | Zdecentralizowana i bezpieczna. Brak obciążeń zwrotnych i oszustw. Możliwość użycia pseudonimów. Akceptacja na całym świecie. | Szybsze i tańsze transakcje. Większa skalowalność. Transakcje off-chain nie obciążają blockchaina. |
| Wady | Wolny czas realizacji transakcji. Wysokie opłaty przy niektórych rodzajach transakcji. Złożoność dla początkujących. | Może wymagać zaufania do operatorów kanałów. Wymaga transakcji on-chain do otwarcia i zamknięcia kanałów. |
