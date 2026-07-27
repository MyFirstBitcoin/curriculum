# 9.2 Mempool Nedir?

**mempool**, “bellek havuzu”nun kısaltmasıdır ve Bitcoin işlemleri için bir bekleme odası gibidir. Bitcoin gönderdiğinizde, işleminiz önce ağa yayınlanır ve mempool'a yerleştirilir.

Bunu bir restoranda sıra beklemek gibi düşünebilirsiniz. İsminiz bir listeye yazılır ve bir masa boşalana kadar beklersiniz. Aynı şekilde, işleminiz bir madenci onu bir bloğa dahil edene kadar mempool'da bekler.

Bitcoin düğümleri her yeni işlemi kontrol ederek geçerli olup olmadığını ve harcanan bitcoin'in daha önce kullanılmadığını doğrular. İşlem geçerliyse, onaylanana kadar mempool'da kalır.

Madenciler mempool'dan işlemleri seçer ve bunları yeni bloklara dahil eder. Genellikle, daha yüksek işlem ücretine sahip işlemler önce seçilir.

Bir işlem bir bloğa dahil edildiğinde, onaylanmış olur ve kalıcı olarak Bitcoin blokzincirine kaydedilir.

#### Etkinlik: Mempool'u Keşfetmek


https://qr.myfirstbitcoin.org/mempool.pdf

_Activity: Mempool_


**Bu etkinlik, öğrencileri teknik bilgi gerektirmeyen, ücretsiz ve açık kaynaklı bir araçla tanıştırır. Başlangıç seviyesinden deneyimli Bitcoin kullanıcılarına kadar herkes için faydalıdır.**

###### Ana Noktalar

1. **Mempool**, her Bitcoin düğümünün tuttuğu onaylanmamış işlemler listesini ifade eder; belirli bir hizmeti veya platformu değil.
1. Tek bir, evrensel mempool yoktur. Mempool.space bunlardan sadece biridir.
1. [Mempool.space](https://mempool.space), açık kaynaklıdır ve kullanımı kolay görsel bir blok gezgini olarak bilinir. Onaylanmamış işlemler, ücret oranları ve diğer ağ aktiviteleri hakkında gerçek zamanlı veriler sunar.

###### Öğrenci İpucu

Mempool.space blokları görselleştirmekten çok daha fazlasını yapar. Bitcoin ekosisteminin diğer bölümlerini de keşfedin: örneğin, Lightning, madencilik, hash oranı, havuzlar ve blok alanı "gözlükleri".
