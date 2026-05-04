# 9.3 İşlemler Nasıl Çalışır

Artık açık ve özel anahtarları, ayrıca düğümlerin ve madencilerin rollerini anladığınıza göre, bir Bitcoin işleminin baştan sona nasıl çalıştığını burada görebilirsiniz.

1. Ahmet, bitcoin'i Kerem'e göndermek istiyor. Kerem’in adresi, gönderilecek miktar ve bir ücret ile bir işlem oluşturuyor.
1. Ahmet, sahipliğini kanıtlamak için işlemi özel anahtarıyla imzalıyor.
1. İşlemi Bitcoin ağına yayıyor.
1. Düğümler işlemi alır ve kurallara uyup uymadığını kontrol eder; imzayı doğrular ve Ahmet’in yeterli bitcoin’i olup olmadığını denetler.
1. Geçerliyse, işlem ağda paylaşılır ve bekleyen işlemlerin beklediği mempool’a eklenir.
1. Madenciler, mempool’dan işlemleri seçer ve çıkarmaya çalıştıkları bloğa ekler.
1. Bir madenci bir bloğu başarıyla çıkardığında, bu blok ağa paylaşılır ve diğer düğümler tarafından kontrol edilir.
1. Geçerliyse, blok blokzincire eklenir. Kerem bitcoin’i alır.
1. Daha fazla blok eklendikçe, işlem onay alır ve daha güvenli hale gelir.

Bir bloğa dahil edildikten sonra, işlem onaylanır. Ahmet bu bitcoin’i tekrar harcayamaz ve Kerem aldığı bitcoin’i yeni bir işlemde harcayabilir.


> **Note**
>
> İşlem ve ücret seçildi → Cüzdan tarafından imzalandı ve gönderildi → Düğümler tarafından dağıtıldı → Madenci işlemi blok şablonuna ekledi → Madenci İş Kanıtı yarışmasını kazandı → Yeni blok doğrulandı → Yeni blok düğümler tarafından dağıtıldı


###### Kaynaklar


[▶ YouTube](https://www.youtube.com/watch?v=xc_TxlByxeY)
