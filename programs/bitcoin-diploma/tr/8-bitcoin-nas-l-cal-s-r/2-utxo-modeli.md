# 8.2 UTXO Modeli

##### UTXO'lar nedir?

Garip ismine aldanıp korkmayın. UTXO'ları, cüzdanınızdaki banknotlar ve madeni paralar gibi, bitcoin parçaları olarak düşünebilirsiniz. Örneğin, 180 TL'lik bir ürünü 300 TL'lik bir banknotla öderseniz, 120 TL para üstü alırsınız. Bitcoin de benzer şekilde çalışır.

Sahip olduğunuz tüm bitcoin, farklı UTXO'lardan oluşur. Bitcoin gönderdiğinizde, cüzdanınız bu parçaların bir veya birkaçını ödemede kullanır.

Harcadığınız parça, gönderdiğiniz miktardan büyükse, kalan değer yeni bir UTXO olarak size para üstü şeklinde geri döner. Aynı anda, alıcıya da gönderdiğiniz bitcoin'i temsil eden yeni bir UTXO ulaşır.

Cüzdan bakiyeniz, kontrol ettiğiniz tüm UTXO'ların toplam değeridir.


> **Callout – Gizlilik**
>
> UTXO'larınızı başkalarına göstermemelisiniz çünkü birisi bunları bildiğinde, işlemlerinizi takip edebilir ve sonunda ne kadar paranız olduğunu öğrenebilir.


###### Örnek

1. Ayşe, Barış'a 5 BTC göndermek istiyor.
1. Cüzdanı, toplamda 6 BTC değerinde olan iki UTXO'sunu kullanır.
1. İşlem, **5 BTC'yi Barış'a gönderir**, Barış'ın cüzdanında yeni bir UTXO oluşturur.
1. Kalan **0,99 BTC para üstü olarak Ayşe'ye geri döner**, işlem ücreti olarak **0,01 BTC ödedikten sonra**.
1. İşlem onaylandıktan sonra, Bitcoin defterine eklenir ve Ayşe'nin kullandığı UTXO'lar harcanmış olarak işaretlenir, böylece tekrar kullanılamazlar.

###### Kaynaklar


[▶ “How Bitcoin Works under the Hood” videosunu izleyin](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
