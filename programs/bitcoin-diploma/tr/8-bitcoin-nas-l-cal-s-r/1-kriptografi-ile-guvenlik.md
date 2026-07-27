# 8.1 Kriptografi ile Güvenlik

> Bitcoin bize kesin bir vaat sunar: program tam olarak belirtildiği gibi çalışacaktır.  
_Andreas M. Antonopoulos_

#### Açık/Özel Anahtar Kriptografisi


> **Definition – Kriptografi Tanımı**
>
> **Kriptografi** bilgiyi yalnızca doğru kişilerin okuyabileceği bir sır haline getirme uygulamasıdır.


* **Şifreleme** bilgiyi yalnızca doğru anahtara sahip birinin okuyabileceği şekilde kodlanmış bir forma dönüştürme işlemidir.
* **Şifre Çözme** bu kodlanmış bilgiyi tekrar okunabilir bir hale getirme işlemidir.

Geleneksel kriptografide, özel olarak iletişim kurmak isteyen iki kişi önceden aynı gizli anahtarı paylaşmak zorundadır; bu, paylaşılan bir şifreye benzer. Bir kişi bu anahtarı mesajı şifrelemek için kullanır ve göndermeden önce şifreler, diğer kişi ise aynı anahtarı kullanarak mesajın şifresini çözüp okur.

Bu sistemdeki sorun, iki kişinin de gizli anahtarı önceden paylaşmak zorunda olmasıdır. Eğer başka biri bu anahtara erişirse, yakalanan tüm mesajları okuyabilir.

Bitcoin, kullanıcıların önceden gizli anahtar paylaşmasına gerek olmayan açık anahtarlı kriptografi adı verilen farklı bir yöntemle bu sorunu çözer.

Açık/özel anahtar kriptografisi, sır paylaşma sorununu çözer. Bir şifre paylaşmak yerine, her kişinin iki anahtarı vardır: bir açık anahtar ve bir özel anahtar.

* **açık anahtar** herkesle paylaşılabilir.
* **özel anahtar** her zaman gizli tutulmalıdır.

Ahmet, Arel'e bir şey göndermek isterse, Arel’in açık anahtarını kullanabilir. Bunu yalnızca Arel, kendi özel anahtarıyla açabilir. Mesajı biri ele geçirse bile, özel anahtar olmadan okuyamaz veya kullanamaz.

Bitcoin'de bu sistem dijital imzalar oluşturmak için kullanılır. Dijital imza, bir özel anahtarın sahibinin bir işlemi onayladığını kanıtlar; tıpkı bir belgeye imza atmak gibi. Bu, Bitcoin işlemlerinin üçüncü bir tarafa güvenmeden güvenli ve doğrulanabilir olmasını sağlar.

Bitcoin işlemleri, bitcoin sahipliğinin bir adresten başka bir adrese aktarılmasını içerir.

Şifreleme, yalnızca gerçek bitcoin sahibinin parasını başkasına gönderme yetkisine sahip olmasını sağlamak için kullanılır. Bu, mülkiyetlerinin kötü niyetli kişilere karşı korunmasını sağlar.

Ek bir koruma önlemi olarak, her Bitcoin işlemi otomatik olarak BENZERSİZ bir dijital imza alır. Bu benzersiz dijital imza, ağın bitcoin’in gerçek sahibi tarafından gönderildiğini doğrulamasına yardımcı olan, kurcalamaya karşı dayanıklı bir teknolojiyle desteklenir.


> **Dark**
>
> Her kullanıcının iki anahtarı vardır: bir **özel anahtar**, bu **gizli tutulur**, ve bir **açık anahtar** ki bu **başkalarıyla paylaşılabilir**. **Özel anahtar** bir kimlik ve sahiplik kanıtı olarak hizmet eder, şu mesajı doğrular: “Bu adres bana ait ve üzerinde kontrolüm var.”


###### Bir Bitcoin İşlemi Nasıl Çalışır

1. **İşlemin Oluşturulması**: Bir kullanıcı, alıcının adresi ve gönderilecek bitcoin miktarı gibi ayrıntıları belirterek bir Bitcoin işlemi başlatır.
1. **Dijital İmza Oluşturma**: Gönderen, benzersiz bir **dijital imza** kendi **özel anahtarını** kullanarak oluşturur. Bu imza, işlemin özgünlüğünü doğrulayan benzersiz bir koddur.
1. **İşlemin Yayınlanması**: İmzalanan işlem, bitcoin sahipliğinin gönderen kişiden alıcıya aktarılmak istendiğini belirterek Bitcoin ağına yayınlanır.
1. **Ağda Doğrulama**: Bitcoin ağındaki düğümler işlemi alır ve alıcının **açık anahtarını** imzanın doğruluğunu doğrulamak için. işlemin. Aynı anda, gönderenin **açık anahtarını** doğrulamak için **dijital imzayı**.
1. **Bitcoin ağında onaylama**: Doğrulama başarılı olursa, işlem deftere eklenir; bu defter, tüm işlemlerin güvenli ve şeffaf bir kaydıdır. Onaylandıktan sonra, bitcoin'in sahipliği resmi olarak gönderen kişiden alıcıya aktarılır.


> **Callout – Özet**
>
> **dijital imza**, gönderenin **özel anahtarı** ile oluşturulur ve işlemin bitcoin sahibinin izniyle yapıldığını kanıtlar. Bitcoin ağı bu kanıtı doğrulayabilir ve işlemi kaydedebilir.


#### Hashleme Açıklaması

Lütfen teknik terimler ve matematiksel kavramlar sizi korkutmasın. Herkesin matematiğe bayılmadığını biliyoruz, ancak kendinizi şaşırtabilir ve en karmaşık fikirlerin bile biraz çabayla anlaşılabileceğini görebilirsiniz.


> **Definition – Fonksiyonun Tanımı**
>
> Bir **fonksiyon**, bazı bilgileri alıp onu yeni bir şeye dönüştüren bir makine gibidir. Fonksiyona verdiğiniz bilgi **girdidir**. Fonksiyonun oluşturduğu yeni bilgi ise **çıktıdır**. Fonksiyonlar, bilgisayarların görevleri yerine getirmesine ve sorunları çözmesine yardımcı olur.


##### Fonksiyon nedir?

Bir fonksiyon, bir girdi alıp bir çıktı üreten talimatlar bütünüdür. Bunu bir tarif gibi düşünebilirsiniz: Belirli malzemelerle adımları izlersiniz ve her zaman öngörülebilir bir sonuca ulaşırsınız.

Bitcoin'de fonksiyonlar, işlemleri işlemek ve doğrulamak için kullanılır. Birisi bitcoin gönderdiğinde, kriptografik fonksiyonlar işlemin geçerli olup olmadığını kontrol etmeye, gönderenin yeterli bakiyesi olup olmadığını onaylamaya ve Bitcoin defterindeki bakiyeleri güncellemeye yardımcı olur. Doğrulandıktan ve bir bloğa eklendikten sonra, işlem blok zincirinde kalıcı kaydın bir parçası olur.

##### Tek Yönlü Fonksiyon Nedir?

Tek yönlü fonksiyon, bir yönde hesaplaması kolay, ancak tersine çevirmesi son derece zor olan özel bir fonksiyon türüdür. Örneğin, malzemeleri karıştırıp bir smoothie yapmak kolaydır, ancak smoothie'yi tekrar orijinal malzemelerine ayıramazsınız.

Bitcoin güvenliği tek yönlü fonksiyonlara dayanır. Bunlar, açık ve özel anahtar kriptografisinde kullanılır; insanların açık anahtarlarını paylaşmasına olanak tanırken, özel anahtarlarını gizli tutar. Açık anahtar görünür olsa bile, ondan özel anahtarı elde etmek imkansızdır. Bu, Bitcoin işlemlerini güvenli kılan şeydir.

##### Hash Fonksiyonu Nedir?

Bir **hash fonksiyonu**, gizli bir kod makinesi gibidir. Bir mesajı alır ve onu bir koda dönüştürür.

###### Bitcoin İşlemlerinde Hashleme Nasıl Çalışır?

Bitcoin'de, her işlem blok zincirine eklenmeden önce bir hash'e dönüştürülür. Hash, işlemin benzersiz dijital parmak izidir. Birisi işlemin çok küçük bir kısmını bile değiştirmeye çalışırsa, hash tamamen değişir. Bu, ağın müdahaleyi kolayca tespit etmesini sağlar.

###### Bitcoin Güvenliğinde Hashlemenin Rolü

Hashleme, işlemleri doğrulamayı kolay ve sessizce değiştirmeyi imkansız hale getirerek Bitcoin ağını korur. Her işlemin kendine özgü bir hash'i olduğu için, ağ bir şeyin değiştirilip değiştirilmediğini hızla tespit edebilir.

Bir hash fonksiyonu, veriyi alır ve hash adı verilen sabit uzunlukta bir sayı ve harf dizisine dönüştürür. Aynı girdi her zaman aynı hash'i üretir, ancak girdideki çok küçük bir değişiklik bile tamamen farklı bir sonuç oluşturur. Bu özellik, bilgisayarların verinin değişmediğini kontrol etmesini sağlar.


> **Definition – Hashlemenin Tanımı**
>
> **Hashleme**, dijital veriler için bir parmak izi oluşturmak gibidir. Dijital bir mesajı alıp sabit uzunlukta bir koda dönüştürme işlemidir ve bu kod benzersiz bir tanımlayıcı görevi görür. Nasıl ki bir parmak izi bir kişiyi tanımlayabiliyorsa, bir hash de dijital bir mesajı tanımlayabilir.


**çıktı**, yani hash, orijinal bilginin uzunluğu ne olursa olsun her zaman aynı uzunluktadır. Bitcoin, **SHA-256** ve **RIPEMD160** adlı birkaç özel hash fonksiyonu kullanır.

Aşağıda birkaç örnek verilmiştir:

* SHA256 ile bir dizgenin hash'i **merhaba dünya**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* Metnin SHA256 özeti **merhaba dünya.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Girdi üzerinde yapılan küçük bir değişikliğin çıktıyı tamamen değiştirdiğine dikkat edin, ilk örnekle karşılaştırıldığında
* İndirilebilir iso dosyasının SHA256 özeti **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Bu girdi devasa bir dosya olmasına rağmen, çıktı yine de aynı sabit uzunlukta

Hashleme işlemini, bir müzik parçasının özünü yakalayan bir nota gibi de düşünebilirsiniz. Nasıl ki bir nota bir melodinin benzersiz bir temsiliyse, bir hash değeri de bir verinin benzersiz bir temsilidir.

Bir müzisyen, bir müzik parçasının notasını gerçek performansla karşılaştırarak performansın doğru olup olmadığını anlayabilir. Benzer şekilde, alınan verinin hash değeri ile orijinal hash değeri karşılaştırılarak, verinin iletim sırasında değiştirilip değiştirilmediği anlaşılabilir.

Bir müzik performansındaki küçük bir sapma bile melodinin farklı duyulmasına neden olabileceği gibi, orijinal veride yapılan en ufak bir değişiklik bile farklı bir hash değeriyle sonuçlanır. Bu, hashlemeyi bir Bitcoin işleminin bütünlüğünü ve doğruluğunu sağlamak için güçlü bir araç haline getirir.

Şunun şifrelenmesi işlemi **açık anahtar** hashleme yoluyla, bilgiyi sabit uzunlukta ve okunamaz bir formata dönüştürerek güvenliği artırmak için kullanılır. Bitcoin, açık adresler üretmek için SHA-256 ve RIPEMD160 algoritmalarını kullanır. Ortaya çıkan çıktı, **açık anahtar** için benzersiz bir tanımlayıcı görevi görür ve defterde saklanan işlemlerin bütünlüğünü ve güvenliğini sağlamaya yardımcı olur. Bilgi bu şekilde şifrelendiğinde, yetkisiz kişilerin veriye erişmesi ve müdahale etmesi daha zor hale gelir.

##### Bir hash fonksiyonunun özellikleri

* **Deterministik**: Aynı malzemeler her zaman aynı smoothie'yi üretir. Aynı şekilde, aynı veri her zaman aynı hash'i üretir.
* **Ön-görüntü direnci**: Elinizde sadece smoothie varsa, tam olarak hangi meyvelerin kullanıldığını anlayamazsınız. Benzer şekilde, sadece hash varsa, orijinal veriyi belirleyemezsiniz.
* **Çığ etkisi**: Malzemelerin çok küçük bir kısmını değiştirmek bile tamamen farklı bir smoothie oluşturur. Hashlemede, veride yapılan çok küçük bir değişiklik tamamen farklı bir hash üretir.
* **Çakışma direnci**: Aynı smoothie'yi üreten iki farklı malzeme seti bulmak son derece zordur. Aynı şekilde, iki farklı veri parçasının aynı hash'i üretmesi son derece olası değildir.
* **Doğrulaması hızlı**: Smoothie yapmak hızlıdır ve sonucun smoothie olup olmadığını kontrol etmek kolaydır. Hash fonksiyonları hızlı hesaplanır ve herkesin kolayca doğrulamasını sağlar.

#### Etkinlik: SHA 256 Hash Oluştur


https://tools.keycdn.com/sha256-online-generator

_SHA256 Online Generator_


Hashlemenin nasıl çalıştığını merak ediyor musunuz? Herhangi bir kelime, cümle veya seçtiğiniz bir girdiden anında SHA256 hash oluşturmak için QR kodunu tarayın. Hash fonksiyonları dijital parmak izleri gibidir: tek yönlüdürler, yani bir şey hash'lenince geri çevrilemez. Deneyin ve kendiniz görün!
