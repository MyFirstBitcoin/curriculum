# 7.1 Jaringan Petir

Lightning Network adalah sistem pembayaran yang memungkinkan pengguna untuk mengirim dan menerima bitcoin dengan cepat dan biaya rendah. Cara kerjanya adalah dengan membuat dompet bersama di mana kedua pihak menyimpan sebagian bitcoin mereka. Setelah itu, mereka dapat melakukan transaksi tanpa batas satu sama lain tanpa perlu mencatat setiap transaksi di blockchain utama. Dengan cara ini, mereka melewati kebutuhan untuk memverifikasi dan memasukkan setiap transaksi ke dalam blok, sehingga prosesnya menjadi cepat dan hemat biaya. Biaya yang lebih rendah membuat Lightning Network dapat digunakan untuk pembayaran kecil yang tidak selalu layak dilakukan di on-chain. Setelah kedua pihak memutuskan untuk mengakhiri kerja sama, hanya saldo akhir yang dicatat di blockchain.

Bayangkan suatu hari bekerja di sebuah kafe. Karena berencana untuk tinggal cukup lama, kamu membuka tab dan membayar di muka, bukan membayar setiap kali memesan. Di akhir hari, kamu dan pemilik kafe memeriksa tab untuk menyelesaikan tagihan. Jika depositmu lebih besar dari yang kamu habiskan, kamu akan menerima kembali selisihnya; jika kamu menghabiskan lebih banyak, kamu membayar kekurangannya.

Skema ini dapat diperluas untuk melibatkan lebih banyak peserta. Misalnya, pada salah satu kunjunganmu ke kafe, kamu membawa seorang teman yang tidak dikenal oleh bartender dan tidak bisa membuka tab. Kamu menawarkan tab milikmu untuk menutupi pengeluaran temanmu, dan kalian sepakat bahwa temanmu akan menggantinya secara pribadi. Sekarang bayangkan ribuan orang melakukan hal yang sama secara bersamaan, memungkinkan orang lain menggunakan tab yang sudah ada untuk terhubung dengan lebih banyak individu lagi — seperti itulah cara Lightning Network bekerja!

Dengan Lightning, kamu dapat melakukan pembayaran kepada siapa saja di jaringan, tidak hanya kepada orang yang berbagi tab langsung denganmu — asalkan ada rute yang dapat ditemukan antara kedua pihak. Pembayaranmu dapat melewati jaringan hingga mencapai tujuannya, meskipun kamu tidak memiliki saluran terbuka langsung dengan penerima.

Mari kita lihat perbedaan antara transaksi on-chain dan off-chain.

##### Transaksi On-Chain

Ini adalah transaksi yang terjadi langsung di blockchain Bitcoin. Konfirmasinya memakan waktu sekitar 10 menit, dan biaya tergantung pada ukuran transaksi dalam virtual byte. Transaksi ini lebih aman namun lebih lambat, karena memerlukan konsensus dari jaringan.

##### Transaksi Lightning Network

Transaksi ini terjadi di jaringan terpisah yang dibangun di atas blockchain Bitcoin. Penyelesaiannya lebih cepat dan biayanya lebih rendah. Biasanya digunakan ketika kecepatan dan biaya transaksi menjadi pertimbangan utama. Dibandingkan dengan transaksi on-chain, transaksi ini kurang aman.


|  | Jaringan Bitcoin | Lightning Network |
| --- | --- | --- |
| Definisi | Jaringan digital terdesentralisasi yang menggunakan kriptografi untuk mengamankan transaksi keuangan. | Protokol pembayaran lapis kedua yang berjalan di atas blockchain Bitcoin, memungkinkan transaksi yang lebih cepat dan murah. |
| Keunggulan | Terdesentralisasi dan aman. Tidak ada chargeback atau penipuan. Dapat digunakan secara pseudonim. Diterima secara global. | Transaksi lebih cepat dan murah. Skalabilitas meningkat. Transaksi off-chain tidak membebani blockchain. |
| Kekurangan | Waktu transaksi lambat. Biaya tinggi untuk jenis transaksi tertentu. Rumit untuk pemula. | Dapat memerlukan kepercayaan pada operator saluran. Membutuhkan transaksi on-chain untuk membuka dan menutup saluran. |
