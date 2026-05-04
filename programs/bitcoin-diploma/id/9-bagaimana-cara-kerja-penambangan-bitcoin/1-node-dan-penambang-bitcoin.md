# 9.1 Node dan Penambang Bitcoin

Node Bitcoin mungkin terdengar teknis, tetapi sebenarnya hanyalah perangkat lunak yang menyimpan salinan blockchain Bitcoin di sebuah komputer. Blockchain adalah catatan bersama dari semua transaksi Bitcoin.

Ketika Anda menjalankan node sendiri, Anda memverifikasi transaksi Bitcoin secara mandiri, bukan mempercayai orang lain. Ini memberi Anda lebih banyak kemandirian dan membantu menjaga jaringan Bitcoin tetap terdesentralisasi.

Anda bisa membayangkan node Bitcoin seperti petugas lalu lintas digital dengan beberapa tugas penting.

1. Node menyimpan salinan blockchain, yaitu riwayat semua transaksi Bitcoin.
1. Node terhubung dengan node lain di seluruh dunia dan saling berbagi informasi. Salah satu contohnya adalah daftar transaksi baru yang menunggu konfirmasi, yang disebut mempool.
1. Node memeriksa bahwa setiap transaksi mengikuti aturan Bitcoin. Jika sebuah transaksi tidak valid, node akan menolaknya.

Node juga membantu node baru bergabung ke jaringan dengan membagikan blockchain kepada mereka. Namun, setiap node baru tetap memeriksa semua aturan secara mandiri.

Siapa pun dapat menjalankan node dengan menginstal perangkat lunak seperti Bitcoin Core dan mengunduh blockchain. Setelah terpasang, node akan terus menerima blok baru kira-kira setiap 10 menit dan memverifikasinya sebelum menambahkannya ke salinan blockchain miliknya.

Menjalankan node membantu membuat jaringan Bitcoin lebih aman dan terdesentralisasi, karena semakin banyak orang yang memverifikasi sistem secara mandiri.

#### Apa Itu Node Bitcoin?

> Tujuan penambangan bukanlah menciptakan bitcoin baru; itu adalah sistem insentif. Penambangan adalah mekanisme yang membuat keamanan Bitcoin menjadi terdesentralisasi.  
_Andreas M. Antonopoulos_


> **Callout**
>
> Penambang mengumpulkan transaksi yang belum dikonfirmasi, membentuk sebuah blok, dan menggunakan energi untuk menemukan kunci yang menambah dan mengamankan blok tersebut.


Penambang bersaing untuk menambahkan blok transaksi berikutnya ke blockchain. Untuk melakukan ini, mereka harus menemukan angka khusus yang menghasilkan hash blok yang valid. Anda bisa membayangkannya seperti mencari kunci yang tepat di antara miliaran kemungkinan. Penambang pertama yang menemukan hash yang benar memenangkan perlombaan dan berhak menambahkan bloknya ke blockchain.

Ketika seorang penambang menemukan hash yang valid, mereka membagikan bloknya ke jaringan. Penambang lain dengan cepat memverifikasi bahwa solusinya benar. Jika benar, blok tersebut ditambahkan ke blockchain, membantu menjaga keamanan buku besar publik Bitcoin.

Penambang mendapatkan bitcoin dengan dua cara:

* **Hadiah blok:** Bitcoin baru diciptakan dan diberikan kepada penambang yang berhasil menambahkan blok ke blockchain.
* **Biaya transaksi:** Ketika orang mengirim bitcoin, mereka menyertakan biaya kecil. Penambang yang menambahkan blok akan menerima biaya dari transaksi yang termasuk dalam blok tersebut.

#### Halving Bitcoin


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12,5 BTC | 6,25 BTC | 3,125 BTC |



> **Callout**
>
> Hadiah penambang untuk menyelesaikan satu blok akan berkurang setengah setiap 210.000 blok, sekitar setiap empat tahun.


Bitcoin memiliki suplai maksimum tetap sebesar 21.000.000 bitcoin, tetapi semuanya tidak langsung tercipta saat Bitcoin dimulai. Sebaliknya, bitcoin baru secara bertahap diperkenalkan ke dalam peredaran melalui **penambangan**.

Ketika penambang berhasil menambahkan blok transaksi baru ke jaringan Bitcoin, mereka menerima **hadiah blok** dalam bentuk bitcoin. Pada masa awal Bitcoin, hadiah ini adalah 50 bitcoin per blok. Hadiah ini mendorong orang untuk menggunakan daya komputasi dan listrik demi membantu mengamankan jaringan.

Sekitar setiap 210.000 blok (kira-kira setiap 4 tahun), hadiah blok akan dipotong setengah. Peristiwa ini disebut **halving**. Halving memperlambat penciptaan bitcoin baru dan membantu memastikan bahwa total suplai tidak akan pernah melebihi 21 juta. Seiring waktu, ini membuat bitcoin semakin langka.


> **Definition – Suplai beredar**
>
> **Suplai beredar** mengacu pada jumlah total mata uang yang tersedia. Pada Bitcoin, total suplai beredar adalah jumlah koin yang telah ditambang dan beredar pada waktu tertentu.


![ Bitcoin Supply Schedule](https://cdn.sanity.io/images/vje9ehw2/staging/49a6077467494fa7e97ce4942852c72e6842b52d-292x200.svg)


> **Definition – Jadwal suplai Bitcoin**
>
> **Jadwal suplai Bitcoin** adalah rencana yang telah ditentukan dan bersifat publik untuk pelepasan bitcoin baru ke dalam peredaran, yang dirancang untuk menjaga kelangkaan Bitcoin dari waktu ke waktu.


Setelah setiap peristiwa halving, hadiah bitcoin yang diterima penambang untuk menambahkan blok akan dipotong setengah. Ini mengurangi laju penciptaan bitcoin baru.

Penambang tetap mendapatkan biaya transaksi dari transaksi yang termasuk dalam blok yang mereka tambang. Seiring waktu, biaya ini diperkirakan akan menjadi bagian pendapatan penambang yang lebih besar.

Halving sudah tertanam dalam protokol Bitcoin dan terjadi secara otomatis sekitar setiap empat tahun sekali. Karena hal ini, jadwal suplai Bitcoin dapat diprediksi dan transparan.

Tabel berikut menunjukkan halving yang akan datang, termasuk perkiraan tanggal, nomor blok saat halving terjadi, hadiah blok baru, dan persentase total suplai bitcoin yang sudah ditambang.


| Peristiwa | Tanggal | Blok | Hadiah | Sudah Ditambang |
| --- | --- | --- | --- | --- |
| Halving ke-5 | 2028 | 1.050.000 | 1,5625 BTC | 98,44 % |
| Halving ke-6 | 2032 | 1.260.000 | 0,78125 BTC | 99,22 % |
| Halving ke-7 | 2036 | 1.470.000 | 0,390625 BTC | 99,61 % |


Seiring semakin banyak bitcoin yang ditambang, suplai yang beredar terus bertambah hingga mencapai batas maksimum 21.000.000 bitcoin, yang diperkirakan akan tercapai sekitar tahun 2140. Karena jumlah bitcoin baru yang diciptakan semakin sedikit dari waktu ke waktu, jika permintaan meningkat, harga Bitcoin bisa naik. Hal ini juga mendorong para penambang untuk terus mengamankan jaringan dengan memberikan daya komputasi mereka.

#### Apa itu hash blok yang valid di Bitcoin?

Dalam Bitcoin, para penambang bersaing untuk menemukan kode khusus yang disebut **hash blok**. Kode ini mengidentifikasi satu blok transaksi dan memungkinkan blok tersebut ditambahkan ke blockchain.

Setiap blok berisi informasi tentang transaksi terbaru dan juga mencakup hash dari blok sebelumnya. Ini menghubungkan setiap blok satu sama lain, membentuk rantai dari blok pertama (Genesis Block) hingga blok yang paling baru.

Hash bekerja seperti **sidik jari digital** untuk data di dalam blok. Jika ada informasi di dalam blok yang diubah, sidik jari tersebut juga akan berubah. Hal ini memudahkan siapa saja untuk memverifikasi bahwa riwayat transaksi blockchain tidak diubah dan membantu menjaga keamanan jaringan.


> **Callout**
>
> Satoshi Nakamoto, pencipta Bitcoin, menambang Genesis Block, yang menghasilkan total 50 bitcoin.


#### Perlombaan Menambang Blok

Para penambang bersaing untuk menemukan hash blok yang valid. Penambang pertama yang menemukannya berhak menambahkan blok baru ke blockchain dan menerima hadiah bitcoin.

Agar valid, hash blok harus lebih kecil dari angka yang ditetapkan jaringan yang disebut target kesulitan. Karena hash bersifat acak, penambang harus terus mencoba berbagai input sampai menemukan yang berhasil.

Jika terlalu banyak penambang yang bersaing, blok akan ditemukan terlalu cepat. Jika terlalu sedikit penambang yang berpartisipasi, blok akan memerlukan waktu terlalu lama untuk ditemukan. Untuk menjaga sistem tetap berjalan lancar, Bitcoin secara otomatis menyesuaikan tingkat kesulitan setiap 2.016 blok (sekitar dua minggu sekali).

Penyesuaian ini memastikan bahwa, rata-rata, satu blok baru ditambahkan ke blockchain setiap sekitar 10 menit.


> **Definition – Definisi tingkat kesulitan**
>
> **tingkat kesulitan** dalam penambangan Bitcoin mengukur seberapa sulit menemukan hash blok yang valid. Jaringan menyesuaikan tingkat kesulitan ini setiap 2.016 blok (sekitar dua minggu sekali) agar blok baru dapat ditambahkan ke blockchain sekitar setiap 10 menit. Semakin tinggi tingkat kesulitan, semakin sulit bagi penambang untuk menemukan blok yang valid.


Dengan menemukan hash blok yang valid, seorang penambang membuktikan bahwa mereka telah melakukan pekerjaan yang diperlukan untuk menambahkan blok baru ke blockchain. Proses ini disebut **Proof of Work** (PoW). Ini adalah mekanisme keamanan yang memungkinkan Bitcoin mengonfirmasi transaksi dan menambahkan blok baru ke blockchain. Penambang yang pertama kali menemukan hash yang valid akan mendapatkan hadiah dalam bentuk bitcoin, yang mencakup hadiah blok dan biaya transaksi dari transaksi yang ada di blok tersebut.

Proof of Work (PoW) membantu menjaga keamanan Bitcoin dengan membuatnya sangat mahal bagi siapa pun yang mencoba menipu atau mengambil alih jaringan. Sebaliknya, jauh lebih menguntungkan untuk mengikuti aturan.

Penambang memiliki empat peran utama:

1. **Mengumpulkan transaksi**: Penambang memilih transaksi yang telah dikirim ke jaringan dan memasukkannya ke dalam blok kandidat.
1. **Melakukan Proof of Work**: Penambang bersaing untuk memecahkan teka-teki matematika yang sulit dengan menemukan hash blok yang valid.
1. **Siaran blok**: Penambang pertama yang menemukan solusi yang valid membagikan blok baru ke jaringan.
1. **Dapatkan hadiah**: Jika blok tersebut valid, blok tersebut ditambahkan ke blockchain dan penambang menerima bitcoin baru yang dibuat beserta biaya transaksi.

Banyak penambang di seluruh dunia mencoba membuat blok berikutnya secara bersamaan. Ketika satu penambang menemukan solusi yang valid, jaringan memeriksa blok tersebut. Jika semuanya benar, blok tersebut ditambahkan ke blockchain. Blok-blok lain yang bersaing akan dibuang. Proses ini menjaga jaringan tetap sepakat dan mencegah pengeluaran ganda.

* Penambang adalah komputer yang membantu memelihara dan memperbarui buku besar Bitcoin.
* Mereka mengumpulkan transaksi dan mengelompokkannya ke dalam sebuah blok. Kemudian mereka menjalankan data blok tersebut melalui algoritma hashing untuk membuat kode unik yang disebut hash.
* Penambang mengulangi proses ini berkali-kali, mencari hash yang memenuhi aturan Bitcoin. Penambang pertama yang menemukan hash yang valid mendapatkan bitcoin baru sebagai hadiah, dan blok mereka ditambahkan ke blockchain.
* Hash setiap blok juga menghubungkannya dengan blok sebelumnya. Jika seseorang mencoba mengubah transaksi di masa lalu, hash-nya tidak akan cocok lagi, dan jaringan akan menolak rantai yang telah diubah. Inilah yang menjaga buku besar Bitcoin tetap aman.
