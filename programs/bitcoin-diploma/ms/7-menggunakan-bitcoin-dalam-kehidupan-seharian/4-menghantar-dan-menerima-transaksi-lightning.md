# 7.4 Menghantar dan Menerima Transaksi Lightning

Dengan dompet Lightning, menggunakan Bitcoin adalah pantas, murah, dan peribadi, menjadikan transaksi antara dua orang mudah. Anda boleh menghantar dan menerima bitcoin dengan cepat untuk perkara harian seperti membeli kopi.

Mari kita lihat beberapa contoh Lightning Network dalam tindakan.

###### Contoh 1

Kedua-dua Marcia dan Eve mempunyai 5 unit mata wang. Marcia ingin menghantar 2 unit kepada Eve. Pembayaran itu melalui Jeff, yang membantu menghantar pembayaran melalui Lightning Network. Selepas pembayaran selesai, Eve mempunyai 7 unit dan Marcia mempunyai 3.

Jeff membantu mengarahkan pembayaran, tetapi dia tidak boleh mencuri dana tersebut. Lightning Network menggunakan kriptografi untuk memastikan hanya penerima yang dimaksudkan boleh menerima pembayaran. Jeff hanya membantu pembayaran bergerak melalui rangkaian.

Ini menunjukkan kelebihan utama Lightning Network: orang boleh menghantar pembayaran dengan cepat tanpa mempercayai perantara seperti bank.

Pengendali nod seperti Jeff juga boleh memperoleh yuran kecil kerana membantu mengarahkan pembayaran. Dengan cara ini, mereka membantu rangkaian kekal terdesentralisasi dan cekap.

Berbanding dengan transaksi Bitcoin biasa:

* **Transaksi atas rantaian** berlaku secara langsung di blockchain Bitcoin. Ia sangat selamat tetapi boleh menjadi lebih perlahan dan mahal.
* **Transaksi Lightning** berlaku di luar rantaian dan membolehkan pembayaran bergerak dengan lebih pantas dan pada kos yang jauh lebih rendah.

Disebabkan ini, Lightning berguna untuk pembayaran kecil dan harian, manakala transaksi atas rantaian sering digunakan untuk pemindahan yang lebih besar atau penyimpanan jangka panjang.

###### Contoh 2

Mina suka makan di luar dan sering singgah di kafe kegemarannya. Dengan begitu banyak pilihan pembayaran yang berbeza, dia tidak pasti yang mana satu pilihan terbaik. Nasib baik, dia telah belajar sedikit tentang Bitcoin dan Lightning Network. Selepas meneliti pilihannya, Mina sedar bahawa menggunakan kaedah pembayaran Lightning adalah pilihan terbaik.

Mina ingin membeli kopi, tetapi membayar dengan transaksi Bitcoin biasa kadang-kadang boleh mengambil masa dan memerlukan yuran yang lebih tinggi. Sebaliknya, dia memutuskan untuk menggunakan Lightning Network.

Lightning Network membolehkan orang menghantar bitcoin serta-merta dan dengan yuran yang sangat rendah. Ini menjadikannya ideal untuk pembelian kecil dan harian seperti kopi.

Untuk mula menggunakan Lightning, Mina memuat turun dompet Lightning di telefonnya. Dia kemudian menghantar sedikit bitcoin dari dompet Bitcoin biasa ke dompet Lightning miliknya. Langkah ini menggunakan transaksi Bitcoin biasa di blockchain. Setelah dana berada dalam dompet Lightning, ia boleh digunakan di Lightning Network.

Sekarang Mina boleh membayar kafe itu serta-merta menggunakan Lightning. Pembayaran berlaku di luar blockchain utama Bitcoin, sebab itulah ia jauh lebih pantas dan murah berbanding transaksi atas rantaian biasa.


| Kelebihan | Lightning Network | Sistem Perbankan Tradisional |
| --- | --- | --- |
| Kelajuan | Pantas | Perlahan |
| Ketelusan | Telus | Tidak telus |
| Keselamatan | Selamat | Terdedah |
| Yuran transaksi | Rendah | Tinggi |
| Keterangkuman kewangan | Tinggi | Terhad |
| Kebolehkembangan | Tinggi | Rendah |
| Privasi | Tinggi | Sederhana |
| Interoperabiliti | Tinggi | Rendah |
| Pematuhan undang-undang | Sederhana | Tinggi |
| Keberkesanan kos | Tinggi | Sederhana |


Transaksi on-chain berlaku secara langsung di atas blockchain Bitcoin dan boleh mengambil lebih banyak masa serta yuran. Transaksi Lightning berlaku di luar rantai (off-chain), membolehkan pembayaran yang pantas dan kos rendah sambil masih menggunakan bitcoin.


| Visa, Inc. | Bitcoin On-chain | Lightning Network |
| --- | --- | --- |
| Kapasiti 65,000 transaksi sesaat. | Kapasiti 7 transaksi sesaat. | Kapasiti berjuta-juta transaksi sesaat. |


![Lightning Network Map](https://cdn.sanity.io/images/vje9ehw2/staging/5a760247cf4c32074c62f40aea8dc21095882740-504x245.svg)


https://mempool.space/graphs/lightning/nodes-channels-map

_Mempool.space Nodes Channels Map_


Ini adalah peta keseluruhan Lightning Network. Terima kasih kepada ribuan pengendali nod Lightning, anda boleh menghantar sats kepada mana-mana pengguna dengan dompet Bitcoin Lightning, di mana sahaja mereka berada di dunia. Pembayaran akan sampai dalam beberapa saat dan hanya akan menelan kos beberapa sen sahaja.**Cuba sendiri!**

#### Aktiviti: Perlumbaan Relay Lightning


https://qr.myfirstbitcoin.org/lightning.pdf

_Activity: Lightning_


**Ini adalah latihan praktikal di mana pelajar menghantar dan menerima sats sebenar menggunakan Lightning Network.**

###### Perkara Utama

1. Menggunakan dompet Lightning akan membina keyakinan anda untuk menerima dan menghantar sats sebenar.
1. Perhatikan unit. Sesetengah dompet membenarkan pengguna menghantar bitcoin ATAU sats (1/100,000,000 daripada satu bitcoin).
1. Pembayaran Lightning kadangkala boleh tergendala dalam proses routing, terutamanya untuk pembayaran yang lebih besar. Walaupun masih boleh berlaku, pengalaman pengguna seperti ini semakin jarang berlaku apabila rangkaian semakin matang.

###### Petua Pelajar

Sahkan dengan pengajar anda sama ada dan bagaimana yuran transaksi Bitcoin on-chain semasa akan memberi kesan kepada dompet Lightning yang anda gunakan.
