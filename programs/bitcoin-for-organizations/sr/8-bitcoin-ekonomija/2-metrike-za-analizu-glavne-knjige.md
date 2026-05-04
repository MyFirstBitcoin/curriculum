# 8.2 Metrike za analizu glavne knjige

Zbog toga što je transparentnost Bitcoina drugačija od tradicionalnih finansijskih sistema — gde se većina novčanih tokova odvija iza zatvorenih institucionalnih vrata — otvara se bogato polje on-chain analitike, gde podaci sa mreže postaju način za razumevanje ponašanja korisnika, novčanih tokova i dugoročnih trendova. Ove metrike mogu pomoći da se odgovori na konkretna pitanja, kao što su koliko se aktivno koristi mreža, da li se novčići akumuliraju ili prodaju, i da li mreža postaje sigurnija.

Razumevanje ovih metrika je korisno ne samo za korisnike Bitcoina, već i za istraživače ili donosioce odluka koji žele uvid u ovaj jedinstveno transparentan finansijski sistem.

Ovo poglavlje sadrži neke od najčešće korišćenih metrika za analizu aktivnosti na Bitcoinu, grupisane u podkategorije. Ovo nije sveobuhvatna lista. Posetite [www.bitcoinmagazinepro.com/charts](https://www.bitcoinmagazinepro.com/charts) za potpuniju listu i opise.



#### 8.2.1 Metrike adresa

Metrike adresa su korisne za praćenje kroz vreme jer pokazuju nivo aktivnosti na Bitcoin mreži. Na primer, kako Bitcoin postaje šire prihvaćen, broj aktivnih adresa raste. Ovo možemo dodatno analizirati tako što izdvajamo broj adresa koje drže minimalno određenu količinu Bitcoina, recimo 0,1 BTC, u određenom vremenskom periodu, kao što je jedna godina. Iako ovo daje uvid u usvajanje Bitcoina kroz vreme, nije savršeno jer jedna osoba može imati više Bitcoin adresa. S druge strane, berze ili ETF-ovi mogu izgledati kao jedan entitet dok zapravo drže sredstva za veliki broj pojedinaca.

![Bitcoin: Addresses Hodling > X BTC by Year](https://cdn.sanity.io/images/vje9ehw2/staging/b88a9239820e45ed50ce00812170e2bb4d02b5d2-1407x766.png)

_Adrese koje drže Bitcoin > X BTC po godinama. Izvor: Bitcoin Magazine Pro._

Upoređivanjem adresa sa trenutnom tržišnom cenom BTC moguće je videti procenat ukupnih Bitcoin adresa koje su u profitu. Ovo nam omogućava da pratimo tržišno raspoloženje jer možemo videti koliki deo tržišta drži BTC sa profitom ili gubitkom.

Na primer, **Procenat nerealizovanog profita** grafikon ispod prikazuje udeo svih adresa na glavnoj knjizi sa nerealizovanim profitom izraženim u američkim dolarima. Imajte na umu da, pošto je grafikon ispod napravljen blizu istorijskog maksimuma Bitcoina, procenat adresa sa nerealizovanim profitom je blizu sto posto. Takođe možemo videti da su produženi periodi kada je Procenat nerealizovanog profita ispod jedne standardne devijacije od proseka retki. Dakle, pad ispod ove linije može ukazivati na dobar trenutak za ulazak kupaca.

![Percent Unrealised Profit](https://cdn.sanity.io/images/vje9ehw2/staging/f306f03f31ce4faada8bf34137dd76f9d550697a-1041x491.png)

_Procenat nerealizovanog profita. Izvor: checkonchain.com_



#### 8.2.2 On-chain indikatori

On-chain indikatori su korisni jer nude uvid u ponašanje mreže, izvan onoga što same cene i metrike adresa mogu pokazati. Oni pomažu analitičarima da razumeju postupke i raspoloženje različitih tipova učesnika, kao što su dugoročni vlasnici naspram kratkoročnih trgovaca, prateći kako se novčići drže, premeštaju ili vrednuju kroz vreme. Ovi indikatori koriste transparentnost glavne knjige da otkriju skrivenu dinamiku tržišta kao što su akumulacija, distribucija ili čak uverenje investitora. To ih čini posebno korisnim za identifikaciju strukturnih trendova, procenu da li je tržište pregrejano ili potcenjeno i predviđanje preokreta u tržišnom ciklusu.

Na primer, posmatranjem vrednosti BTC koja se drži od poslednje transakcije, možemo zaključiti da li je tržište pod stresom (kao što može biti tokom velikog cikličnog minimuma). Ova metrika je poznata kao **Realizovana cena** i daje nam 'prosečnu osnovu troška' za sav BTC u opticaju. Ako tržišna cena padne ispod Realizovane cene, to pokazuje da većina adresa u zbiru drži gubitak na papiru.

Daljim grupisanjem podataka iz glavne knjige po starosnim grupama, možemo prikazati kako se količina BTC premešta između adresa kroz vreme, što stvara talasaste obrasce na grafikonu poznatom kao **HODL talasi**.

![Bitcoin HODL Waves](https://cdn.sanity.io/images/vje9ehw2/staging/ce108e45a1a7217e081101e4a276ee2d9e95a22e-1129x577.png)

_Bitcoin HODL talasi. Izvor: Bitcoin Magazine Pro._

HODL talasi pokazuju šta dugoročni, srednjoročni i kratkoročni vlasnici rade sa svojim BTC. Na primer, na grafikonu iznad, kratkoročni vlasnici su prikazani crvenom i narandžastom bojom i možemo videti skokove aktivnosti kada ova grupa žuri da kupuje blizu tržišnih vrhova. Sa druge strane, možemo videti da vrlo dugoročni vlasnici (ljubičasto i plavo) postepeno povećavaju svoj ukupni udeo u mreži, što ukazuje na snažno uverenje ovih grupa. Grafikon nije savršen jer neki novčići mogu preći sa stare na novu adresu pod kontrolom istog korisnika. Ipak, daje zanimljiv uvid u uverenje dugoročnih vlasnika.

Još jedan način da se ispita 'pametni novac' dugoročnih vlasnika je da se analizira **Uništeni dani novčića** (CDD). Koncept 'dana novčića' je proizvod broja BTC i broja dana od kada su novčići poslednji put pomereni. Na primer, 5 BTC koji nije pomeren 100 dana ima 500 dana novčića, a 10 BTC koji nije pomeren 10 dana ima 100 dana novčića. Na ovaj način dajemo veću težinu novčićima koji se duže drže. Kada se ti novčići pomere, ti dani novčića se 'uništavaju'. Ovaj indikator pokazuje povećanja CDD u trenucima značajnih promena cene, što analitičarima omogućava da razlikuju rutinsku tržišnu aktivnost od značajnih promena u raspoloženju dugoročnih vlasnika.

Još jedna metrika koja može pomoći da se utvrdi da li tržište potcenjuje ili precenjuje BTC je odnos tržišne vrednosti i realizovane vrednosti ili **MVRV**. Izračunava se jednostavno kao odnos tržišne vrednosti (broj BTC u opticaju pomnožen sa tržišnom cenom) podeljen sa realizovanom vrednošću (zbir svih BTC od kada su poslednji put pomereni). Visok MVRV sugeriše da je više novčića u profitu (često viđeno blizu tržišnih vrhova), a nizak MVRV ukazuje da se mnogi novčići drže sa gubitkom (viđeno blizu tržišnih minimuma).



#### 8.2.3 Metrike rudarenja

Metrike rudarenja su korisne za razumevanje sigurnosti, ekonomskih podsticaja i opšteg zdravlja Bitcoin mreže. Metrike kao što su hashrate, prihod rudara, težina i odnos naknada otkrivaju koliko računarske snage obezbeđuje blockchain i koliko su rudari nagrađeni za svoje aktivnosti.

**Hashrate** Bitcoin mreže je možda najčešće korišćen indikator zdravlja mreže i jačine sigurnosti. Pošto proces rudarenja obezbeđuje mrežu i potvrđuje da su transakcije na glavnoj knjizi validne, što je veći nivo računarske (ili hash) snage, to je teže zlonamernom akteru da nadjača i napadne mrežu.

![Bitcoin Hashrate](https://cdn.sanity.io/images/vje9ehw2/staging/fcb4a24c431a37580d3d6c4ec62b664e7e41c362-1134x584.png)

_Bitcoin Hashrate. Izvor: Bitcoin Magazine Pro._

Grafikon iznad pokazuje da u maju 2025. ukupna računarska snaga mreže iznosi oko 900 TeraHash/s (900 biliona kriptografskih 'hash' izračunavanja u sekundi). Ako hashrate raste, to pokazuje da mreža postaje sigurnija, što je ohrabrujuće za korisnike.

Puell Multiple (osmislio David Puell) posmatra tržišni ciklus iz ugla rudara i njihovih prihoda. Metrika se izračunava tako što se dnevna emisija BTC (u američkim dolarima) podeli sa 365-dnevnim pokretnim prosekom dnevne vrednosti emisije. Ova metrika pomaže da se identifikuju periodi stresa ili olakšanja za rudare. Istorijski gledano, vrednost iznad 3 je prethodila padu tržišne vrednosti BTC, jer ukazuje da su rudari veoma profitabilni. Vrednost ispod 0,5 ukazuje na stres i istorijski je označavala tržišne minimume za vrednost BTC.
