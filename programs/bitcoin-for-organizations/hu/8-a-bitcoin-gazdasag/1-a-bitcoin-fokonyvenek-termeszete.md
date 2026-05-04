# 8.1 A Bitcoin főkönyvének természete

A Bitcoin tranzakciós főkönyve (más néven timechain vagy blockchain) egy nyilvánosan elérhető, időbélyeggel ellátott nyilvántartás minden érvényes tranzakcióról, amely valaha is megtörtént a hálózaton. A hagyományos pénzügyi rendszerben a belső tranzakciók csak az arra jogosult résztvevők, például bankok, szabályozó hatóságok vagy adatkezelők (mint a SWIFT, BACS vagy SEPA) számára láthatók. A hagyományos rendszerekben a fizetési adatokhoz való hozzáférés erősen korlátozott és költséges lehet.

Ezzel szemben a Bitcoin hálózatban bárki, akinek van internetkapcsolata, megtekintheti az összes tranzakciót, a legnagyobb értéktől egészen az egyes Satoshikig. A résztvevők valós időben követhetik a teljes bitcoin készletet, figyelhetik a címek és tárcák aktivitását, valamint megtekinthetik a bányász jutalmakat és a díjak alakulását. Bár a főkönyvön látható tevékenység a nyilvános kulcscímekhez kötött, nem pedig egyéni személyazonossághoz, nagy adathalmazokat lehet összeállítani a költési szokásokról, így mindenki valós időben kutathatja és elemezheti a gazdasági aktivitást. Ahogy a hálózat növekszik és egyre inkább elfogadják a gazdasági igazság forrásaként, csökkenhet a kormányzati szervek és harmadik fél szolgáltatók szerepe a statisztikai elemzések és költési jelentések készítésében.



#### 8.1.1 Node-ok és Block Explorerek

Bárki, aki önállóan szeretné ellenőrizni a Bitcoin főkönyvét és hozzáférni az adataihoz, futtasson egy teljes node-ot. A teljes node-ot gyakran a Bitcoin gazdaságban való részvétel és ellenőrzés legalapvetőbb módjaként írják le. Ez világszerte elérhető nyílt forráskódú szoftverként, amely futtatásakor letölti és érvényesíti a teljes Bitcoin főkönyvet a 2009 januárjában közzétett „Genesis Block”-tól egészen a jelenlegi napig. Emellett támogatja a Bitcoin hálózat biztonságát azzal, hogy segít ellenőrizni az új tranzakciókat, amelyek bekerülnek a főkönyvbe. A főkönyvhöz ilyen módon hozzáférve a teljes node az igazság forrásaként szolgál a hálózat kutatói és könyvvizsgálói számára. A Bitcoin felhasználók számára pedig a teljes node egy „önrendelkező” kaput jelent a Bitcoin gazdaság tranzakciós információihoz, mivel növeli a magánszférát és a biztonságot azzal, hogy megszünteti a harmadik fél szolgáltatóktól való függőséget.

Míg a teljes node-ok a nyers adatokat töltik le, a block explorerek, mint például a mempool.space vagy a blockstream.info, vizuális felületet kínálnak a főkönyvi tevékenységek kereséséhez és értelmezéséhez. A block explorer lehetővé teszi az egyes tranzakciók követését, valamint a tárcák egyenlegének és előzményeinek megtekintését. Megjeleníti továbbá a bányászati tevékenység mutatóit, például a blokk jutalmakat és a tranzakciós díjakat.

A teljes node-ok és a block explorerek együtt azok az eszközök, amelyek a Bitcoin hálózat átláthatóságát használhatóvá teszik.



#### 8.1.2 Tevékenység: A Bitcoin főkönyv felfedezése

1. Nyisd meg [mempool.space](https://mempool.space) és fedezd fel a kezdőlapot.
  * Mi a legfrissebb blokk magassága?
  * Mennyi jelenleg a tranzakciós díj (alacsony, közepes és magas prioritás)?
  * Hány tranzakció várakozik a mempoolban a következő blokkra?
1. Nyisd meg a főkönyv legfrissebb blokkját.
  * Hány tranzakció került bele?
  * Nevezd meg a blokk bányászát!
  * Mennyi volt a blokk jutalma?
1. Nyiss meg egy tranzakciót a blokkban.
  * Hány inputja és outputja van a tranzakciónak?
  * Mekkora a tranzakció értéke BTC-ben és USD-ben?

Beszéljétek meg, miben különbözik a pénz mozgása a hagyományos rendszerben, és hogyan használja egy vállalkozás vagy kormányzat ezt a fajta átláthatóságot.
