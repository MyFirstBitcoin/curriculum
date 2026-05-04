# 3.6 Újrahasználható proof of work

Hal Finney a Cypherpunk mozgalom egy másik híres tagja, aki nagyon érdeklődött az elektronikus pénz fejlesztése iránt, és aktív volt a levelezőlistán.

Úgy döntött, hogy újra megpróbálkozik egy proof-of-work alapú elektronikus pénzrendszer fejlesztésével. Eddig a hash kimenet minden tranzakcióhoz egyedi volt, de az ő ötlete az volt, hogy 'újrahasználható proof-of-work'-öket hozzon létre.

Ennek a megközelítésnek a hátránya a központosított szerver, amelyben meg kell bízni, hogy nem költ kétszer, vagy nem állítják le. Ennek megkerülésére Hal azt javasolta, hogy szabad és nyílt forráskódú szoftvert használjanak, amelyet biztonságos hardveres komponensen lehet futtatni, és függetlenül lehet ellenőrizni.

A megoldás még mindig ugyanazokkal a problémákkal szembesült, mint a többi javaslat:

* A 'tyúk vagy a tojás' probléma az elfogadottság elérésében, ahol hiányzik az ösztönző, hogy a felhasználók tokeneket akarjanak igényelni, és az eladók sem akarnak csatlakozni a rendszerhez, hacsak a felhasználók nem akarnak ezekkel a tokenekkel fizetni.
* A POW valószínűleg idővel olcsóbbá válik, ahogy a számítástechnikai teljesítmény javul, ami azt sugallja, hogy a piacot végül elárasztanák az RPOW pénzegységek.

> Ha a Moore-törvény továbbra is érvényes marad, egy (POW) token létrehozásának költsége folyamatosan, exponenciális ütemben csökkenni fog. Ne feledd, hogy ez nem pénz, és nem is értékmegőrzésre szolgál, hanem inkább a számítógépes erőfeszítés könnyen cserélhető reprezentációja._Hal Finney_

Ezek a tulajdonságok korlátozták a projekt vonzerejét és így az elterjedését is, és minden erőfeszítése ellenére a projekt végül egy újabb sikertelen kísérlet lett az elektronikus pénz létrehozására.
