# 7 - Gunakan Bitcoin dalam Kehidupan Sehari-hari

Durasi: 90 menit

Ide Inti: Lightning Network membuat Bitcoin lebih praktis untuk pembayaran sehari-hari dengan memungkinkan transaksi yang lebih cepat dan murah, sambil tetap menjadikan Bitcoin sebagai dasarnya.

#### Tujuan Pembelajaran

Pada akhir pelajaran ini, siswa diharapkan dapat:

* Menjelaskan apa itu Lightning Network dan mengapa dibangun di atas Bitcoin.
* Membandingkan transaksi on-chain dan Lightning dari segi kecepatan, biaya, dan kompromi keamanan.
* Membedakan antara dompet Lightning kustodian dan swadaya, serta menjelaskan mengapa swadaya itu penting.
* Mengatur dompet Lightning dan menjelaskan peran frasa benih (seed phrase) dalam pemulihan dompet.
* Mendemonstrasikan bagaimana pembayaran Lightning bergerak melalui jaringan, bahkan ketika dua pengguna tidak memiliki saluran langsung.
* Mengidentifikasi cara-cara nyata Bitcoin dapat digunakan dalam kehidupan sehari-hari melalui Lightning, termasuk untuk kopi, belanja kebutuhan pokok, pembayaran merchant, dan pengeluaran lokal.
* Menjelaskan bagaimana alat seperti BTCPay Server, BTCMap, dan kartu hadiah membantu memperluas penggunaan Bitcoin dalam praktik.
* Menggambarkan apa itu ekonomi sirkular Bitcoin dan mengapa Lightning membuatnya lebih memungkinkan.

#### Alat & Sumber Daya

##### Alat Bantu Visual

* Bab 7 - Menggunakan Bitcoin dalam Kehidupan Sehari-hari

##### Perpustakaan Dukungan

* Kartu Referensi Kosakata — Istilah: Lightning Network, saluran pembayaran, routing, Layer 2, ekonomi sirkular, remitansi
* Perpustakaan Contoh Dunia Nyata & Studi Kasus — El Salvador, ekonomi sirkular Austin, kisah adopsi merchant Lightning
* Bagan Perbandingan & Lembar Referensi — Perbandingan On-Chain vs. Lightning; Perbandingan Biaya & Kecepatan antar metode pembayaran
* Penjelasan Sederhana Lightning Network — Cara kerja saluran pembayaran tanpa jargon; routing; keamanan; kasus penggunaan
* Simulasi Skenario Pembayaran — Langkah demi langkah: mengirim ke teman, menerima pembayaran, remitansi, menerima sebagai pekerja lepas
* Alat Perbandingan Biaya & Kecepatan — Kapan menggunakan Lightning vs. on-chain vs. perbankan (dengan contoh biaya)

#### Aktivitas

* Lomba Estafet Lightning

#### Pengajaran Daring

* Gunakan slide perbandingan berdampingan untuk pembayaran on-chain dan Lightning.
* Mulailah dengan kasus penggunaan nyata seperti kopi atau remitansi agar siswa memahami mengapa Lightning ada.
* Gunakan diagram routing tiga orang yang sederhana agar penjelasan jaringan tetap jelas.
* Jaga penjelasan mekanisme saluran tetap ringan kecuali kelas sudah memiliki dasar yang kuat.

#### Persiapan

* Unduh dompet Lightning dan siapkan tangkapan layar yang menunjukkan kecepatan transaksi on-chain (lambat) vs. Lightning (cepat) secara berdampingan.
* Riset 2-3 merchant atau komunitas nyata yang menggunakan Lightning; tandai BTCMap.org sebagai referensi.
* Siapkan bagan perbandingan on-chain vs. Lightning (kecepatan, biaya, keamanan, kasus penggunaan) untuk dibagikan.

#### Prosedur

Pelajaran ini menunjukkan kepada siswa bagaimana Bitcoin menjadi praktis untuk pembayaran sehari-hari melalui Lightning Network. Panduan ini sekarang mengikuti struktur Diploma secara langsung sehingga bagian utama Lightning sesuai dengan panduan siswa, sementara perbandingan, alat merchant, dan materi ekonomi sirkular tetap berada di tempatnya.

##### 7.0 Pendahuluan, 8 menit

Mulailah dengan menghubungkan bab ini ke bab sebelumnya:

* Jika Bitcoin sudah berjalan on-chain, mengapa dibutuhkan lapisan lain?
* Apa yang terjadi ketika orang ingin melakukan banyak pembayaran kecil dengan cepat?
* Sistem pembayaran seperti apa yang lebih cocok untuk kopi, belanja kebutuhan pokok, atau membayar teman?

Tegaskan bahwa bab ini berfokus pada penggunaan Bitcoin untuk kebutuhan sehari-hari, terutama ketika kecepatan dan biaya rendah sangat penting. Jelaskan bahwa Lightning dibangun di atas Bitcoin, bukan terpisah darinya.

##### 7.1 Lightning Network, 25 menit

**Apa Itu Lightning Network**

Jelaskan bahwa Lightning Network adalah sistem pembayaran yang dibangun di atas Bitcoin yang memungkinkan pengguna mengirim dan menerima bitcoin dengan cepat dan murah. Ini bekerja dengan memindahkan banyak pembayaran kecil dari blockchain utama dan hanya mencatat hasil akhirnya kembali ke on-chain nanti.

Cara yang membantu untuk menjelaskannya adalah dengan analogi tab kafe dari bab ini:

* alih-alih membayar setiap item satu per satu secara on-chain
* dua pihak membuka saluran
* mereka memperbarui saldo saat bertransaksi
* hanya saldo akhir yang dicatat di blockchain saat mereka menutup saluran

Itu membuat Lightning lebih cepat dan murah untuk pembayaran kecil yang sering. Juga jelaskan bahwa pembayaran Lightning dapat dirutekan melalui jaringan, sehingga pengguna tidak perlu memiliki saluran langsung dengan setiap orang yang mereka bayar.

**On-chain vs Lightning**

Sekarang buat perbedaannya sangat jelas.

Transaksi on-chain

* terjadi langsung di blockchain Bitcoin
* umumnya lebih lambat
* bergantung pada inklusi dan konfirmasi blok
* cenderung lebih aman
* bisa lebih mahal tergantung pada biaya transaksi

Transaksi Lightning

* terjadi di lapisan kedua yang dibangun di atas Bitcoin
* diselesaikan jauh lebih cepat
* biasanya biayanya jauh lebih murah
* berguna untuk pembayaran kecil dan sering
* melibatkan kompromi dibandingkan dengan penyelesaian on-chain

Jaga agar poin utamanya sederhana: on-chain lebih kuat untuk penyelesaian akhir, Lightning lebih unggul untuk kecepatan dan penggunaan sehari-hari yang murah. Perbandingan ini sangat berguna di sini.

##### 7.2 Jenis Dompet Lightning yang Berbeda, 10 menit

Jelaskan bahwa dompet Lightning menjalankan fungsi dasar yang sama seperti dompet Bitcoin, yaitu menerima dan mengirim bitcoin, tetapi dirancang untuk digunakan di Jaringan Lightning. Kemudian jelaskan perbedaan utama dompet dalam bab ini:

* self-custodial: pengguna mengendalikan kunci privat
* custodial: orang lain yang mengendalikan kunci privat

Perjelas inti komprominya:

* dompet kustodian mungkin terasa lebih mudah dan nyaman
* tetapi pengguna bergantung pada izin dan kendali orang lain
* dompet self-custodial memberi lebih banyak kepemilikan dan kedaulatan

Juga tegaskan kembali rekomendasi bab ini untuk lebih memilih dompet open-source, karena alat open-source dapat ditinjau, diperbaiki, dan diverifikasi oleh komunitas.

##### 7.3 Menyiapkan Dompet Bitcoin Lightning, 10 menit

Pandulah siswa melalui alur pengaturan dasar:

* unduh dompet Lightning
* buat dompet baru
* tuliskan frasa pemulihan
* konfirmasi kata-kata dalam urutan yang benar
* tambahkan keamanan ekstra jika dompet mendukungnya
* mulai gunakan dompet

Jelaskan dengan sangat jelas tentang seed phrase:

* ini adalah yang memungkinkan pengguna memulihkan akses
* jika hilang, akses ke dana bisa hilang
* jika orang lain mendapatkannya, mereka bisa mengendalikan dana

Bagian ini harus sangat menekankan tanggung jawab dan penanganan yang aman, sama seperti di bab on-chain.

##### 7.4 Mengirim dan Menerima Transaksi Lightning, 17 menit

**Bagaimana Transaksi Lightning Bekerja dalam Praktik**

Gunakan contoh Marcia, Jeff, dan Eve untuk menjelaskan routing. Marcia tidak perlu memiliki saluran langsung dengan Eve. Pembayarannya dapat melewati Jeff, yang terhubung ke jaringan, dan tetap sampai ke Eve dengan aman.

Jelaskan poin-poin ini dengan jelas:

* Pembayaran Lightning dapat melewati perantara
* perantara tersebut membantu merutekan pembayaran
* proses routing tidak berarti pengguna mempercayai bank atau prosesor pembayaran terpusat
* jaringan menggunakan kriptografi sehingga pembayaran sampai ke penerima yang dimaksud

Ini membantu siswa memahami bahwa Lightning tetap peer-to-peer, bahkan ketika pembayaran melewati struktur jaringan yang lebih luas. Jika perlu, tunjukkan bahwa bab ini juga menyebutkan operator node dapat memperoleh biaya dan membantu memperkuat jaringan dengan merutekan pembayaran.

**Mendanai Saluran dan Menggunakan Lightning Berulang Kali**

Jelaskan contoh Mina lebih lanjut:

* Mina memindahkan bitcoin dari dompet on-chain ke dompet Lightning miliknya
* ini mendanai sebuah saluran pembayaran
* dia kemudian dapat melakukan pembayaran berulang tanpa harus membuka ulang proses setiap kali
* ketika kanal ditutup, saldo akhir diselesaikan kembali di on-chain

Jelaskan satu batasan penting: dana yang terkunci di kanal aktif sedang digunakan untuk Lightning dan tidak tersedia secara bebas untuk penggunaan on-chain terpisah pada saat yang sama. Ini membantu siswa memahami bahwa Lightning itu kuat, tetapi melibatkan struktur pembayaran yang berbeda.

##### 7.5 Membeli Kopi dan Bahan Makanan dengan Bitcoin, 20 menit

**Kasus Penggunaan Sehari-hari**

Beralih dari mekanisme ke kehidupan nyata.

Jelaskan bahwa Lightning sangat berguna untuk:

* membeli kopi
* bahan makanan
* berbelanja
* membayar teman
* transaksi kecil sehari-hari

Contoh Mina dalam bab ini membantu menunjukkan mengapa Lightning lebih cocok daripada jalur pembayaran tradisional untuk banyak situasi: cepat, biaya rendah, tanpa batas, dan dapat diakses bahkan oleh orang yang mungkin tidak memiliki rekening bank. Tabel perbandingan dan diagram pemrosesan pembayaran sangat membantu di sini, terutama untuk menunjukkan berapa banyak perantara yang ada dalam pembayaran kartu tradisional.

**Alat Pedagang dan Membelanjakan Bitcoin di Dunia Nyata**

Sekarang jelaskan bagaimana bisnis dan pengguna dapat membuat Lightning menjadi praktis dalam kehidupan sehari-hari.

Bahas tiga alat utama atau jalur dalam bab ini:

BTCPay Server

* prosesor pembayaran open-source
* memungkinkan pedagang menerima bitcoin secara langsung
* tidak ada perantara yang mengendalikan dana
* berguna untuk pembayaran bisnis online dan tatap muka

BTCMap

* membantu pengguna menemukan pedagang dan komunitas yang menerima bitcoin
* memungkinkan orang mencari secara lokal
* dapat diperbarui oleh komunitas

Kartu hadiah dan voucher

* alat transisi untuk membelanjakan bitcoin di tempat yang belum menerima secara langsung
* membantu menjembatani kesenjangan sambil adopsi tumbuh

Bagian ini penting karena menunjukkan kepada siswa bahwa penggunaan Bitcoin bukan hanya teori. Sudah ada alat nyata yang bisa digunakan orang hari ini.

**Ekonomi Sirkular dan Bitcoin sebagai Alat Tukar**

Tutup konten utama dengan menjelaskan bahwa ekonomi sirkular adalah komunitas di mana para pesertanya berusaha untuk saling membeli dan menjual sebanyak mungkin. Diterapkan pada Bitcoin, ini berarti pedagang, pekerja, dan pengguna memilih untuk bertransaksi dengan bitcoin dan saling mendukung secara ekonomi.

Jelaskan mengapa Lightning penting di sini:

* pembayaran hampir instan
* biaya rendah
* pembayaran kecil menjadi praktis
* perdagangan lokal menjadi lebih mudah dipertahankan

Anda dapat menyebutkan bahwa bab ini menunjuk pada contoh seperti Arnhem dan Bitcoin Beach, menunjukkan bahwa ekonomi sirkular bukanlah hal yang hipotetis. Mereka sudah ada dan terus berkembang. Garis waktu visual sangat berguna di sini

###### Penutup dan Cek Pemahaman

Tutup dengan beberapa pertanyaan singkat:

* Mengapa Lightning Network dibangun?
* Apa satu perbedaan utama antara pembayaran on-chain dan Lightning?
* Mengapa self-custody penting dalam dompet Lightning?
* Bagaimana seseorang dapat menerima pembayaran Lightning tanpa kanal langsung ke setiap orang?
* Apa itu ekonomi sirkular Bitcoin?

#### Catatan Pengajar

Jaga benang utama pengajaran tetap jelas: Bitcoin adalah lapisan dasar, Lightning membantu membuat pembayaran sehari-hari lebih cepat dan murah.

Bab ini harus terasa praktis dan konkret, tidak terlalu teknis.

Prioritaskan pemahaman daripada mekanisme kanal yang mendalam.

Poin terkuat yang harus diprioritaskan, jika waktu terbatas, adalah:

* apa itu Lightning
* pertukaran antara on-chain vs Lightning
* penitipan dan pengaturan dompet
* pembayaran di dunia nyata
* ekonomi sirkular

Visual paling berguna di bab ini adalah:

* perbandingan on-chain vs Lightning
* perbedaan dompet
* contoh routing dengan Marcia, Jeff, dan Eve
* tabel perbandingan dan grafik kapasitas
* diagram pemrosesan pembayaran tradisional
* linimasa ekonomi sirkular

##### Seperti Apa yang Baik

* Penting untuk memulai dengan permasalahan "Bitcoin butuh 10 menit dan biaya $2," jelaskan Lightning sebagai jalur cepat di atas Bitcoin, gunakan contoh nyata dari pedagang dan koridor remitansi, serta buat pohon keputusan kapan menggunakan on-chain atau Lightning.
* Pendidik harus bersikap pragmatis tentang apa yang benar-benar diselesaikan oleh Lightning, membagikan kisah nyata dari lapangan di mana Bitcoin digunakan, menjelaskan secara jelas pertukaran spesifik, dan tetap realistis tentang adopsi sambil tetap antusias dengan kemungkinan yang ada.
* Siswa mengalami melihat Bitcoin benar-benar digunakan untuk pembayaran nyata di tempat nyata, memahami bahwa kecepatan dan biaya penting untuk pembayaran, membayangkan ekonomi sirkular di mana Bitcoin tetap lokal, mengenali bahwa Lightning ≠ Bitcoin (alat berbeda untuk tujuan berbeda), dan menjadi penasaran tentang sistem ekonomi yang dibangun di atas pembayaran Bitcoin.
* Hasil Pembelajaran akan tercapai jika siswa dapat menjelaskan Lightning Network sebagai lapisan di atas Bitcoin, memahami dasar-dasar saluran pembayaran dan routing, melihat kasus penggunaan nyata untuk pembayaran Lightning, membandingkan on-chain dan Lightning untuk skenario berbeda, memahami konsep ekonomi sirkular, dan mengenali pertukaran spesifik dari setiap pendekatan.

##### Manajemen Waktu

Jika waktu terbatas, prioritaskan:

* Apa itu Lightning
* Pertukaran antara on-chain vs Lightning
* Pembayaran di dunia nyata
* Ekonomi sirkular

Jika waktu lebih, luangkan waktu untuk:

* Mekanisme saluran pembayaran dan routing
* Alat perbandingan biaya dan kecepatan
* Studi kasus ekonomi sirkular El Salvador dan Austin
* Simulasi skenario pembayaran Lightning secara praktis

##### Jika Siswa Kesulitan

* Mengapa Lightning ada → Bandingkan: 10 menit/$2 vs. detik/sepersekian sen.
* Saluran pembayaran → Analogi nota kafe; selesaikan secara internal lalu di Bitcoin.
* Mengapa ini penting secara global → "Bagaimana jika tidak ada bank tapi punya Bitcoin?"
