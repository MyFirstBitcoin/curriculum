# 3.5 BitTorrent

Ett annat projekt som spelade en betydande roll i utvecklingen av kryptovalutor fram till bitcoin är BitTorrent.

År 2001 släppte Bram Cohen en design för ett protokoll som kallades BitTorrent, vilket skapades för att driva ett peer-to-peer-fildelningssystem. Han började arbeta på ett företag som hette MojoNation, som hade startats för att låta människor dela upp konfidentiella filer i krypterade delar som distribuerades på datorer som körde programvaran. En kopia av filen skulle laddas ner samtidigt från flera datorer. Även om det till slut misslyckades, introducerade det Cohen till fildelningsvärlden, där han bestämde sig för att han kunde skapa ett bättre protokoll, som bestod av:

* Swarm: en gemenskap av datorer som laddar ner eller laddar upp innehåll
* Tracker: ett dedikerat verktyg som fungerar ungefär som en sökmotor, men håller reda på filerna som finns inom swarmen. Detta gör det enkelt för användare att se och komma åt vilken fil de än behöver
* BitTorrent-klient: installeras på en dator för att få tillgång till trackern. Observera att swarmen är den enda platsen där filerna faktiskt lagras
* Ett incitamentssystem där användare som deltar i nätverket som fildelare får snabbare nedladdningar

Likheter med Bitcoin:

* Båda protokollen fungerar på peer-to-peer-basis
* Decentraliserad design
* BitTorrent-filer och Bitcoin-ledgern är distribuerade över nätverket
* Öppen källkod från början (BitTorrent blev så småningom en sluten programvara)
