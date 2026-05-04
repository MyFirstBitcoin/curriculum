# 7.4 Mengirim dan Menerima Transaksi Lightning

Dengan dompet Lightning, menggunakan Bitcoin menjadi cepat, murah, dan privat, sehingga transaksi antara dua orang menjadi mudah. Kamu bisa dengan cepat mengirim dan menerima bitcoin untuk hal-hal sehari-hari seperti membeli kopi.

Mari kita lihat beberapa contoh Lightning Network dalam praktik.

###### Contoh 1

Baik Marcia maupun Eva memiliki 5 satuan mata uang. Marcia ingin mengirim 2 satuan kepada Eva. Pembayaran ini melewati Jefri, yang membantu meneruskan pembayaran melalui Lightning Network. Setelah pembayaran selesai, Eva memiliki 7 satuan dan Marcia memiliki 3.

Jefri membantu mengarahkan pembayaran, tetapi ia tidak dapat mencuri dana tersebut. Lightning Network menggunakan kriptografi untuk memastikan hanya penerima yang dimaksud yang dapat menerima pembayaran. Jefri hanya membantu pembayaran bergerak melalui jaringan.

Ini menunjukkan keunggulan utama Lightning Network: orang dapat mengirim pembayaran dengan cepat tanpa harus mempercayai perantara seperti bank.

Operator node seperti Jefri juga bisa mendapatkan biaya kecil karena membantu mengarahkan pembayaran. Dengan melakukan ini, mereka membantu jaringan tetap terdesentralisasi dan efisien.

Dibandingkan dengan transaksi Bitcoin biasa:

* **Transaksi on-chain** terjadi langsung di blockchain Bitcoin. Transaksi ini sangat aman tetapi bisa lebih lambat dan lebih mahal.
* **Transaksi Lightning** terjadi di luar rantai (off-chain) dan memungkinkan pembayaran bergerak jauh lebih cepat dan dengan biaya jauh lebih rendah.

Karena itu, Lightning sangat berguna untuk pembayaran kecil sehari-hari, sementara transaksi on-chain sering digunakan untuk transfer besar atau penyimpanan jangka panjang.

###### Contoh 2

Mina suka makan di luar dan sering mampir ke kafe favoritnya. Dengan begitu banyak pilihan pembayaran yang tersedia, ia tidak yakin mana yang terbaik. Untungnya, ia sudah belajar sedikit tentang Bitcoin dan Lightning Network. Setelah meninjau pilihannya, Mina menyadari bahwa menggunakan metode pembayaran Lightning adalah pilihan terbaik.

Mina ingin membeli kopi, tetapi membayar dengan transaksi Bitcoin biasa kadang-kadang bisa memakan waktu dan membutuhkan biaya lebih tinggi. Sebagai gantinya, ia memutuskan untuk menggunakan Lightning Network.

Lightning Network memungkinkan orang mengirim bitcoin secara instan dan dengan biaya sangat rendah. Ini membuatnya ideal untuk pembelian kecil sehari-hari seperti kopi.

Untuk mulai menggunakan Lightning, Mina mengunduh dompet Lightning di ponselnya. Ia kemudian mengirim sejumlah bitcoin dari dompet Bitcoin regulernya ke dompet Lightning miliknya. Langkah ini menggunakan transaksi Bitcoin biasa di blockchain. Setelah dana masuk ke dompet Lightning, dana tersebut bisa digunakan di Lightning Network.

Sekarang Mina bisa membayar kafe secara instan menggunakan Lightning. Pembayaran terjadi di luar blockchain utama Bitcoin, itulah sebabnya transaksi ini jauh lebih cepat dan murah dibandingkan transaksi on-chain biasa.


| Keuntungan | Lightning Network | Sistem Perbankan Tradisional |
| --- | --- | --- |
| Kecepatan | Cepat | Lambat |
| Transparansi | Transparan | Tertutup |
| Keamanan | Aman | Rentan |
| Biaya transaksi | Rendah | Tinggi |
| Inklusi keuangan | Tinggi | Terbatas |
| Skalabilitas | Tinggi | Rendah |
| Privasi | Tinggi | Sedang |
| Interoperabilitas | Tinggi | Rendah |
| Kepatuhan hukum | Sedang | Tinggi |
| Efektivitas biaya | Tinggi | Sedang |


Transaksi on-chain terjadi langsung di blockchain Bitcoin dan bisa memerlukan waktu serta biaya lebih. Transaksi Lightning terjadi di luar rantai (off-chain), memungkinkan pembayaran yang cepat dan berbiaya rendah, namun tetap menggunakan bitcoin.


| Visa, Inc. | Bitcoin On-chain | Lightning Network |
| --- | --- | --- |
| Kapasitas 65.000 transaksi per detik. | Kapasitas 7 transaksi per detik. | Kapasitas jutaan transaksi per detik. |


![Lightning Network Map](https://cdn.sanity.io/images/vje9ehw2/staging/5a760247cf4c32074c62f40aea8dc21095882740-504x245.svg)

https://mempool.space/graphs/lightning/nodes-channels-map

Ini adalah peta seluruh Lightning Network. Berkat ribuan operator node Lightning, kamu bisa mengirim sats ke siapa saja yang memiliki dompet Bitcoin Lightning, di mana pun mereka berada di dunia. Pembayaran akan sampai dalam beberapa detik dan hanya memerlukan biaya beberapa sen saja.**Coba sendiri!**

#### Aktivitas: Estafet Lightning

https://qr.myfirstbitcoin.org/lightning.pdf

**Ini adalah latihan langsung di mana siswa mengirim dan menerima sats sungguhan menggunakan Lightning Network.**

###### Poin Penting

1. Menggunakan dompet Lightning akan membangun kepercayaan dirimu untuk menerima dan mengirim sats sungguhan.
1. Perhatikan satuan. Beberapa dompet memungkinkan pengguna mengirim bitcoin ATAU sats (1/100.000.000 dari satu bitcoin).
1. Pembayaran Lightning kadang-kadang bisa tersendat dalam proses routing, terutama untuk pembayaran dalam jumlah besar. Meskipun mungkin terjadi, pengalaman seperti ini semakin jarang seiring perkembangan jaringan.

###### Tips Siswa

Verifikasi dengan instruktur kamu apakah/dan bagaimana biaya transaksi Bitcoin on-chain saat ini akan memengaruhi dompet Lightning yang kamu gunakan.
