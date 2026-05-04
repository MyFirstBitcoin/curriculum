# 3.6 Znovupoužitelné důkazy o vykonané práci

Hal Finney je dalším slavným členem hnutí Cypherpunk, který se velmi zajímal o vývoj elektronických peněz a byl aktivní na e-mailové konferenci.

Rozhodl se znovu pokusit o vývoj systému elektronických peněz založeného na proof-of-work. Až do tohoto bodu byl hash výstup jedinečný pro každou transakci, ale jeho nápadem bylo vytvořit „znovupoužitelné důkazy o práci“.

Nevýhodou tohoto přístupu je centralizovaný server, kterému je třeba důvěřovat, že nebude provádět dvojí útratu nebo nebude vypnut. Aby toto obešel, Hal navrhl použití svobodného a otevřeného softwaru, který by mohl běžet na bezpečné hardwarové komponentě a být nezávisle ověřován.

Řešení stále čelilo některým stejným problémům jako ostatní návrhy:

* Problém „slepice a vejce“ při získávání uživatelů, kdy chybí motivace pro uživatele žádat o tokeny a pro prodejce připojit se k systému, pokud uživatelé nechtějí platit těmito tokeny.
* Proof-of-work pravděpodobně také časem zlevní, jak se zlepšuje výpočetní výkon, což naznačuje, že trh by byl nakonec zaplaven měnovými jednotkami RPOW.

> Pokud bude platit Moorův zákon, náklady na vytvoření (POW) tokenu budou klesat stabilním, exponenciálním tempem. Mějte na paměti, že toto nejsou peníze a není to určeno jako uchovatel hodnoty, ale spíše jako snadno směnitelná reprezentace výpočetního úsilí.  
 _Hal Finney_

Tyto vlastnosti omezily atraktivitu a tím i rozšíření projektu, a navzdory jeho nejlepším snahám projekt skončil jako další neúspěšný pokus o vytvoření elektronických peněz.
