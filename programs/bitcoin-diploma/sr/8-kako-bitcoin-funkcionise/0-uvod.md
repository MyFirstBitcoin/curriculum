# 8.0 Uvod

> Bitcoin nije „neregulisan“; njime upravlja algoritam umesto državnih birokratija. Nekorumpiran.  
_Andreas M. Antonopoulos_

U ovom modulu detaljnije ćemo pogledati tehničku stranu Bitcoina. Jednostavnim rečima objašnjavamo kriptografiju koja štiti protokol i kako funkcionišu transakcije. Neki pojmovi mogu delovati tehnički, ali ne brinite. Mnogi ljudi svakodnevno koriste internet, a da ne razumeju u potpunosti kako on radi.

Učenje tehničke strane Bitcoina je dug put koji nije neophodan za svakoga. Iako podstičemo dalje učenje, ovaj modul se fokusira na ključne osnove.

Bitcoin mreža je zajednički zapis transakcija koji se čuva na mnogim računarima koji se zovu čvorovi (nodes). Ovaj zapis, poznat kao Bitcoin knjiga (ledger), je pseudoniman. Ne sadrži lične podatke poput imena ili godina, već samo podatke o transakcijama i Bitcoin adresama. Knjiga prati svaku transakciju od početka blockchaina.

##### Mehanika Bitcoin protokola

* Dokaz o radu
* Kriptografski vremenski žigovi
* Podešavanje težine
* Arhitektura peer-to-peer mreže
* Hash funkcije i Merkleova stabla
* Kriptografija javnog ključa
* Prepolovljavanje bloka (block subsidy halving)
