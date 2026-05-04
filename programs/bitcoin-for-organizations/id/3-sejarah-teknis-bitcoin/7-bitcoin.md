# 3.7 Bitcoin

Setelah bertahun-tahun dan berbagai upaya yang gagal, para Cypherpunks sebagian besar mulai kehilangan minat pada ide mata uang digital tanpa izin, ketika Adam Back menerima email yang berisi tautan ke draft white paper berjudul 'uang elektronik tanpa pihak ketiga' dari seseorang anonim yang menyebut dirinya Satoshi Nakamoto.

Untuk merangkum sampai titik ini, kita setidaknya sudah memiliki ide-ide berikut:

* Tanda tangan kriptografi yang dapat memberikan tingkat privasi dan anonimitas
* Konsep mata uang tanpa jaminan (B-Money)
* Usulan (namun belum ada cara) untuk membatasi penerbitan mata uang baru
* Koin digital yang kepemilikannya diatribusikan melalui kunci publik (B-Money) dan dapat dipindahkan dengan tanda tangan serta dialihkan berdasarkan alamat penerima (RPOW dan Hashcash)
* Semua node memelihara salinan buku besar yang sepenuhnya terdistribusi (B-Money) (pada saat itu dianggap tidak praktis)
* Protokol penanda waktu– menggunakan hashing pohon Merkle untuk menyediakan kronologi kejadian yang dapat dibuktikan secara matematis dan sulit dipalsukan jika semua pengguna menyimpan catatan yang sama
* Proof of work untuk mengaitkan upaya dunia nyata ke dalam sistem (namun menggunakan hash itu sendiri sebagai mata uang)
* Jaringan yang sepenuhnya terdesentralisasi di mana semua peer setara dan dapat keluar masuk jaringan (BitTorrent)
* Konsep mengaitkan hash baru ke hash sebelumnya (Bit Gold dan penanda waktu)

Yang masih kurang pada saat itu meliputi:

* Solusi yang layak untuk menyelesaikan masalah 'jenderal Bizantium'
* Metode untuk membatasi jumlah uang yang beredar meskipun terjadi peningkatan perangkat keras secara terus-menerus
* Skema insentif bagi orang untuk berpartisipasi (masalah ayam dan telur)

Perbedaan besar lainnya antara upaya-upaya terbaru dan Bitcoin adalah bahwa Satoshi telah mengerjakan kodenya selama beberapa waktu sesuai etos asli 'Cypherpunks menulis kode' sebelum mengumumkannya di milis, tidak seperti Bit Gold dan B-Money yang lebih bersifat konseptual.

Apa inovasi yang membedakan Bitcoin dari upaya-upaya uang elektronik sebelumnya?

Proof of work akan digunakan sebagai mekanisme konsensus dan cara untuk memberikan keamanan serta imutabilitas: Alih-alih menggunakan hash sebagai bentuk uang, hash akan digunakan dalam proses konseptual baru yang disebut penambangan, di mana sebuah node akan mengelompokkan serangkaian transaksi, menambahkan angka acak, lalu menerapkan hashing pada 'blok' data tersebut. Blok yang valid yang memenuhi persyaratan hash kemudian akan diumumkan ke jaringan. Blok-blok ini akan dihubungkan satu sama lain menggunakan hash dari blok sebelumnya di setiap blok, dan blockchain terpanjang akan digunakan jika terjadi tiebreaker di mana node yang berbeda memvalidasi dan mengumumkan blok yang berbeda pada waktu yang sama sehingga terjadi pemisahan rantai. Proof of work menjadi penentu tiebreaker terdistribusi untuk menyelesaikan masalah jenderal Bizantium.

Para penambang ini juga diberikan insentif untuk menyediakan CPU yang dibutuhkan dalam melakukan proof-of-work dengan diberikan bitcoin baru untuk setiap blok. Jumlah Bitcoin yang mereka dapatkan juga diprogram untuk berkurang kira-kira setiap 4 tahun hingga seluruh Bitcoin telah tercipta, menciptakan batas keras pada total Bitcoin yang akan pernah beredar yaitu 21 juta.

Ide paling orisinal adalah cara Satoshi menyelesaikan masalah berapa banyak uang yang diciptakan seiring peningkatan perangkat keras dan semakin banyak daya yang dapat digunakan pada jaringan. Penanda waktu dari sejumlah blok tertentu (2016) akan dirata-ratakan, dan jika blok-blok tersebut tercipta terlalu cepat, hash yang dibutuhkan untuk membuat blok baru akan dibuat lebih sulit, jika terlalu lambat akan dibuat lebih mudah. Ini dibangun ke dalam protokol terdesentralisasi yang dijalankan semua node sehingga penambang yang mengabaikannya akan membuang energi untuk menambang blok tanpa manfaat karena akan ditolak oleh jaringan lainnya. Penyesuaian ini memastikan penciptaan blok baru tetap sesuai jadwal penerbitan yang direncanakan, dan memberikan insentif bagi penambang untuk 'bermain sesuai aturan'.

####   
Ringkasan

Banyak bagian dari teka-teki tentang apa yang diperlukan untuk membangun sistem uang elektronik peer-to-peer terdesentralisasi berdasarkan prinsip uang sehat sudah ada sebelum Satoshi merilis whitepaper-nya dan segera setelah rilis awal kode.

> Sifat Bitcoin sedemikian rupa sehingga setelah versi 0.1 dirilis, desain intinya telah ditetapkan secara permanen untuk sepanjang masa hidupnya  
_Satoshi Nakamoto_

Meskipun banyak ide perbaikan (BIP) telah diusulkan dan diadopsi, Bitcoin telah berjalan di latar belakang sejak 2009 mengikuti protokol yang dirancang dalam rilis awal dan hampir tanpa gangguan. Semua perbaikan dilakukan dengan tetap menjaga kompatibilitas ke belakang dengan semua versi sebelumnya.



##### Catatan

1. Untuk penjelasan tentang masalah Jenderal Bizantium - lihat [https://id.wikipedia.org/wiki/Byzantine_fault](https://en.wikipedia.org/wiki/Byzantine_fault)
