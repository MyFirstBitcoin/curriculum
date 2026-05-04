# 3.6 Dovadă de lucru reutilizabilă

Hal Finney este un alt membru faimos al mișcării Cypherpunk, care a fost foarte interesat de dezvoltarea banilor electronici și activ pe lista de discuții.

El a decis să încerce din nou dezvoltarea unui sistem de bani electronici bazat pe proof-of-work. Până în acest moment, rezultatul hash era unic pentru fiecare tranzacție, însă ideea lui era să creeze „dovezi de lucru reutilizabile”.

Dezavantajul acestei abordări este serverul centralizat, care trebuie să fie de încredere pentru a nu cheltui dublu sau pentru a nu fi închis. Pentru a evita acest lucru, Hal a propus folosirea unui software liber și open source care putea fi găzduit pe o componentă hardware securizată și validat independent.

Soluția se confrunta totuși cu unele dintre aceleași probleme ca și celelalte propuneri:

* Problema „oului și găinii” în ceea ce privește adoptarea, unde lipsește un stimulent pentru ca utilizatorii să dorească să solicite jetoane, iar vânzătorii nu vor să se conecteze la sistem decât dacă utilizatorii doresc să plătească cu aceste jetoane.
* POW este, de asemenea, probabil să devină mai ieftin în timp pe măsură ce performanța calculatoarelor se îmbunătățește, ceea ce sugerează că piața ar fi, în cele din urmă, inundată cu unități de monedă RPOW.

> Dacă legea lui Moore continuă să fie valabilă, costul creării unui jeton (POW) va scădea într-un ritm constant, exponențial. Ține cont că aceasta nu este monedă și nu este destinată să fie un depozit de valoare, ci mai degrabă o reprezentare ușor de schimbat a efortului de calcul._Hal Finney_

Aceste caracteristici au limitat atractivitatea și, implicit, adoptarea proiectului, iar în ciuda tuturor eforturilor sale, proiectul a ajuns să fie încă o încercare eșuată de a crea bani electronici.
