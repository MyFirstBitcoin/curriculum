# 3.2 Açık Anahtar Kriptografisi ve Protokoller

Günümüzde İnternet ve çoğu modern bilgisayar sistemi, bilgiyi yalnızca alıcısının çözebileceği şekilde gizleyen bir yöntem olan kriptografiye dayanır. Bitcoin'i güvence altına almak için kullanılan kriptografinin temelleri 70’li yıllara kadar uzanır.

Çözülmesi gereken ilk sorun – paylaşılan bir sırrı güvensiz bir ortamda nasıl iletebiliriz?

Bu konuya ilk olarak Whitfield Diffie ve Martin Hellman eğildi.

Sorun şu: İki taraf – genellikle Alice ve Bob olarak adlandırılır – başkalarının dinleyebileceği bir ağ üzerinden gizli bilgi paylaşmak ister. Bunu başarmak için Diffie-Hellman anahtar değişim sürecini oluşturdular.

Bu paylaşılan sır daha sonra, anahtarın kendisini açıkta paylaşmadan birbirlerine mesaj göndermek için şifreleme ve şifre çözme işlemlerinde kullanılacak çok sayıda simetrik anahtar oluşturmak için tohum değeri olarak kullanılabilir.

Özel anahtar asla paylaşılmak zorunda olmadığından ve her iki uçta da şifreleme ve şifre çözme için farklı anahtarlar kullanıldığından, bu asimetrik şifreleme algoritması olarak adlandırılır.

Kullanım alanları:

* Alice, Bob’un açık anahtarıyla bir mesajı imzalar – bu mesajı yalnızca Bob, kendi özel anahtarıyla çözebilir
* Alice, mesajı kendi özel anahtarıyla imzalar – mesajı Alice’in açık anahtarıyla çözen herkes, mesajın gerçekten Alice tarafından gönderildiğini, özel anahtarı bilmeden doğrulayabilir
* Bu iki yaklaşımı iki katmanlı şifreleme ile birleştirerek, bir mesaj yalnızca Bob’un çözebileceği şekilde şifrelenerek gönderilebilir ve Bob daha sonra gönderenin gerçekten Alice olduğunu doğrulayabilir.

Makale üzerinde adı geçmese de, Ralph Merkle, o zamana kadar çözülemez olarak görülen bu bulmacanın – açık ve potansiyel olarak düşmanca bir ağda özel iletişimi nasıl kurar veya yeniden kurarız – çözülmesinde çok önemli bir rol oynamıştır.

Bu yaklaşım kendi başına kaba kuvvet saldırısına karşı savunmasızdır; bir saldırgan paylaşılan sayıları alıp yeterli zaman ve kaynakla sonunda ortak anahtarı yeniden oluşturabilir, bu yüzden tek başına tam bir çözüm değildir.

##### Açık Anahtar Kriptosistemleri için Protokoller

Yukarıda açıklanan Diffie-Hellman açık anahtar sistemine katkıda bulunmasının yanı sıra, **Ralph Merkle** yıllarca bu alana katkı sağlamaya devam etti ve Bitcoin tarafından kullanılan bazı önemli bileşenlerin geliştirilmesinde etkili oldu.

Kriptografik bir özet fonksiyonu, herhangi bir boyuttaki girdileri alıp karmaşık hesaplamalar yaparak bit cinsinden bir özet değeri döndüren matematiksel bir algoritmadır; bu genellikle sabit uzunlukta, onaltılık biçimde gösterilen alfasayısal bir çıktı ile temsil edilir.

* Girdiler herhangi bir boyutta olabilir
* Çıktı her zaman sabit uzunluktadır ve deterministiktir (aynı girdi her seferinde aynı özeti oluşturur)
* Doğrulaması kolaydır ancak girdiyi bulmak için işlemi tersine çevirmek son derece zordur
* Veride yapılan küçük bir değişiklik çıktıyı tamamen değiştirir

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/8e30852bec3c6852c9e334076a6ad162df0dec4b-515x331.svg)

Özetleme, Bitcoin protokolünün ayrılmaz bir parçasıdır. Bitcoin’de kullanılan SHA-256, NSA tarafından oluşturulmuştur ve kriptografik özetleme algoritmasına bir örnektir.

* Zincirdeki her blok özetlenir, böylece veriler değiştirilemez – bu da dağıtık defterin bütünlüğünü sağlar.
* Oluşturulan özetin, geçerli bir blok olarak kabul edilmesi için ‘İş Kanıtı’ kriterlerini karşılaması gerekir.
* Merkle ağaçları – dallanma ve özetlerin özetlerini kullanarak, özet ağaçları büyük veri kümelerinin minimum depolama ile doğrulanmasını sağlar.
* Özet tabanlı İmzalar ve Anahtarlar, cüzdanlar, adresler ve işlemlerin yetkilendirilmesi için kullanılabilir.

Blokzincir durumlarının dağıtık doğrulanması ve yalnızca eklenebilir, değişime dirençli defter modelleri tek yönlü özetleme sayesinde mümkün olur. Özet fonksiyonları, merkezi bir güven modeli olmadan Bitcoin gibi halka açık defterlerde olayların doğrulanması için güvenilir, deterministik bir yaklaşım sunar.

Kriptografi alanındaki bu yeni yeteneklerin, yaratıcıları tarafından bu alanda yeni bir inovasyon dalgası başlatması bekleniyordu.

##### Eliptik eğri kriptografisi

Bu sonraki yeniliklerden biri, eliptik eğri kriptografisi şeklinde ortaya çıktı.

Eliptik eğri kriptografisi, 1985 yılında iki bilim insanı N. Koblitz ve V. Miller tarafından tanıtıldı. Standart Diffie-Hellman anahtar değişim protokolünde yaygın olarak kullanılan sonlu asal alanlar yerine, eliptik eğrilerle tanımlanan noktaların kullanılmasını ve Ayrık Logaritma problemi varsayımının burada da geçerli olmasını önerdiler. Bunun nasıl çalıştığının detayları bu bölümün kapsamı dışında olsa da, genel olarak eliptik eğri, belirli bir matematiksel denklemi sağlayan noktalar kümesidir.

Bir eliptik eğri için denklem aşağıdaki gibi görünür:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

Bunun bazı faydalı özellikleri vardır:

* Yatay simetri. Eğri üzerindeki herhangi bir nokta x eksenine göre yansıtıldığında aynı eğri üzerinde kalır.
* herhangi bir dikey olmayan doğru, eğriyi en fazla üç noktada keser.
* Kompakt anahtar boyutları, blokzincirde açık anahtarların verimli şekilde saklanması ve iletilmesi için gereklidir.

Bu özellikler, Diffie-Hellman algoritmasına benzer şekilde anahtar çiftleri oluşturmak için kullanılabilir. Bitcoin, Eliptik Eğri Dijital İmza Algoritması'nın (ECDSA) kısaltması olan ECDSA’yı kullanır. Bu, eliptik eğri ve sonlu bir alan kullanarak verileri öyle bir şekilde 'imzalama' sürecidir ki, üçüncü taraflar imzanın doğruluğunu teyit edebilirken, imzalayan kişi imzayı oluşturma yetkisini elinde tutar. Bitcoin’de imzalanan veri, sahipliği devreden işlemdir.

‘Sonlu’ kısmı, Diffie-Hellman’daki ‘mod’ yaklaşımına benzer; denklemin çıktısı bölünür ve kalan, sayılar aralığına sığması için kullanılır.
