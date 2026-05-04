# 3.4 Hashcash

Hashcash, bu alandaki erken yenilikçilerden biri olan Adam Back tarafından oluşturuldu. Adam, internet üzerinde serbest piyasalara ve gizliliğe büyük ilgi duyuyordu ve Cypherpunks e-posta listesine rastladı, oraya katıldı ve aktif bir katılımcı oldu.

Dijital paraya çok ilgi duyuyordu ve grubun Chaum ile birlikte DigiCash üzerinde daha yakın çalışabileceğine dair bazı önerilerde bulundu, ancak bunlar bir sonuca ulaşmadı. Daha sonra dikkatini başka bir ortaya çıkan probleme, yani e-posta spam’ine çevirdi. O ve diğer Cypherpunk’lar, spam sorununa bir çözüm bulmak istiyordu; spam gönderenlerin binlerce e-postayı kolayca oluşturup ağları tıkaması çok kolaydı. Onun yenilikçi çözümü, herhangi bir veriyi belirli uzunlukta benzersiz ve rastgele bir karakter dizisine dönüştürmeye yarayan kriptografi özelliği olan hashleme üzerine kuruluydu. Bu, e-postanın geçerli sayılması ve ağda iletilebilmesi için dijital bir ‘pul’ eklenmesini gerektiriyordu. Gerçek bir e-posta için önemsiz bir maliyet, ancak bir spam gönderen için caydırıcıydı.

Hashcash’in getirdiği temel yenilik, gerçek dünya kaynaklarını – hesaplama gücünü – dijital bir ağa bağlamasıydı. O zamana kadar dijital kaynaklar sınırsızca çoğaltılabiliyorken, oluşturulan ‘hashcash’ miktarı insanların buna harcamaya istekli olduğu enerjiyle sınırlıydı.

Çözüm, Adam’ın dijital bir para sisteminde olması gerektiğine inandığı bazı kriterleri karşılasa da; anonim, dayanıklı ve güvene dayalı olmayan bir yapıdaydı, her hashcash tekrar kullanılamıyor ve gerçekten kıt değildi. Bu sorunların harici üçüncü taraflar kullanılarak nasıl çözülebileceğine dair başka yollar önerdi.

##### BitGold

Nick Szabo, Hashcash ve iş ispatı (proof of work) kavramı üzerine inşa ederek, Hashcash’in yayımlanmasından bir yıl sonra, 1998’de bir e-posta listesinde alternatif bir çözüm önerdi.

Çözüme yaklaşsa da, bu önerinin hâlâ birkaç zorluğu vardı.

* Hash sahipliğinin kaydını kim tutacak ve onlara nasıl güvenilecek?
* Hashleme genellikle zamanla ucuzlayacaktı, bu HashCash için de bir zorluktu.

Bağlantılı hash’ler zaman damgalı olacağından, hashlemenin o zamanki zorluğunun tarihsel olarak izlenmesini önerdi; daha eski bir hash, maliyetler düştüğü için daha yeni bir hashe göre daha fazla işlem gücü gerektirecekti. Ne yazık ki bu, hash’lerin ‘değiştirilebilir’ yani eşit değerde olmayacağı anlamına geliyordu ki bu da dijital paranın temel bir özelliği olarak görülüyordu. Bunu çözmek için Nick, BitGold’un üzerinde çalışacak ve farklı hash gruplarını aynı değerde toplayabilecek bir tür ‘serbest bankacılık’ önerdi.

##### B-Money

Bit Gold önerisinden kısa bir süre sonra, Wei Dai benzer bir çözüm önerdi. Cypherpunk’lar için zaten birkaç başka araç geliştirmişti ve dijital para hakkında kendi fikirleri vardı.

Onun önerisi, Bit Gold’a benziyordu; dijital imzalarla para transferi yapılıyordu ve işlemlerin kayıtları, her birine atanan açık anahtarlar ve para birimi miktarlarını içeren bir defterde tutuluyordu. Bit-Gold’da olduğu gibi, güvenilir üçüncü taraflar güvenlik açığı olarak görülüyordu ve elektronik para sisteminin bakiyeleri, işlemleri izlemek veya çifte harcamayı önlemek için tek bir varlığa dayanmaması gerektiğine inanılıyordu.

Wei-Dai, bu sorunlara birkaç çözüm önerdi; bunlardan biri, defteri merkezi bir varlık(lar) yerine TÜM düğümlerin tutmasıydı. Tüm kullanıcılar kendi defterlerini ve her işlemin geçerliliğini kontrol ederse, tüm düğümler güncel kaldığı sürece defterler ağ genelinde senkronize kalacaktı. Bu kadar dağıtık bir sistemin bozulması zor olurdu.

Wei Dai, bunun Bizans generalleri problemini (1) çözmediğini fark etti; çünkü düğümler kolayca senkronizasyonu kaybedebilir veya basitçe yalan söyleyebilirdi. Alternatif olarak, defteri tutan bir alt küme ‘güvenilir’ sunucuların olması ve bu sunucuları dürüst tutmak için finansal teşvikler oluşturulması gibi yöntemler önerdi.

Para politikası için, B-Money’nin satın alma gücünü bir tür dış tüketici fiyat endeksine sabitlemeyi önerdi. Aynı miktarda B-Money’nin zaman içinde endeksin eşit bir payını alabilmesini, böylece bir miktar fiyat istikrarı sağlamayı istedi. Yani, herkes geçerli bir hash sağlayarak yeni para birimi üretebilecekti, ancak hash üretmenin zorluğu zamanla işlemci maliyetlerine ve fiyat endeksine göre değişebilecekti, böylece her birim ‘değişmez’ olacaktı.
