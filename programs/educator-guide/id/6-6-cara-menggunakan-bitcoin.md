# 6 - Cara Menggunakan Bitcoin

Durasi: 90 menit

Ide Inti: Menggunakan Bitcoin secara on-chain mengajarkan siswa bagaimana kepemilikan, swakustodi, dan verifikasi bekerja dalam praktik, mengubah teori menjadi aksi keuangan langsung.

#### Tujuan Pembelajaran

Pada akhir pelajaran ini, siswa diharapkan dapat:

* Mengidentifikasi cara umum memperoleh dan menukar bitcoin, termasuk metode peer-to-peer dan pertukaran terpusat.
* Menjelaskan perbedaan antara dompet swakustodi dan kustodian, serta mengapa swakustodi penting dalam Bitcoin.
* Menguraikan tujuan dari private key, alamat publik, seed phrase, dan antarmuka dompet.
* Membandingkan berbagai jenis dompet dan mengevaluasi kelebihan dan kekurangannya berdasarkan keamanan, kenyamanan, privasi, dan kendali.
* Mengatur dompet Bitcoin di ponsel dan menjelaskan proses pemulihan dasar.
* Mendemonstrasikan cara menerima dan mengirim transaksi bitcoin on-chain.

Menerapkan prinsip "Jangan Percaya, Verifikasi" pada pemilihan dompet, transaksi, dan penggunaan Bitcoin secara umum.

#### Alat & Sumber Daya

##### Alat Bantu Visual

* Bab 6 - Cara Menggunakan Bitcoin

##### Perpustakaan Pendukung

* Kartu Referensi Kosakata — Bab 6 — Istilah: dompet, private key, alamat publik, seed phrase, kustodian, swakustodi, UTXO, biaya transaksi
* Bagan Perbandingan & Lembar Referensi — Perbandingan jenis dompet (kustodian, mobile, hardware, kertas)
* Penjelasan Teknis & Pendalaman — Kunci publik/pribadi, model UTXO, konfirmasi transaksi
* Pendalaman Keamanan Private Key — Seed phrase, derivasi kunci, metode cadangan, vektor serangan
* Panduan Anatomi Transaksi — Contoh langkah demi langkah cara kerja transaksi Bitcoin
* Daftar Periksa Praktik Keamanan Terbaik — Sebelum mulai, membuat dompet, menerima, mengirim, pencegahan phishing

#### Aktivitas

* Transaksi dalam Aksi
* Lomba Estafet Lightning
* Menjelajahi Mempool

#### Pengajaran Daring

* Jelaskan sejak awal apakah siswa hanya menonton demo atau ikut mengatur dompet mereka sendiri.
* Gunakan tangkapan layar yang besar dan mudah dibaca untuk setiap langkah pengaturan dompet.
* Berhenti sejenak setelah setiap langkah dan minta siswa mengonfirmasi pemahaman di chat sebelum melanjutkan.
* Berikan peringatan langsung sebelum bagian seed phrase dan ingatkan siswa untuk tidak pernah membagikan informasi sensitif secara online.

#### Persiapan

* Unduh dan uji aplikasi dompet ponsel (Blue Wallet atau Muun); siapkan tangkapan layar langkah-langkah utama pengaturan.
* Siapkan panduan pengaturan dompet (unduh → buat → cadangkan seed → terima) untuk referensi.
* Pastikan jaringan/WiFi berfungsi; siapkan alamat demo dan kode QR untuk ditampilkan.

#### Prosedur

Pelajaran ini bergerak dari teori ke praktik langsung. Sekarang strukturnya langsung sesuai dengan struktur Diploma sehingga akuisisi, dompet, pengaturan, transaksi, dan verifikasi muncul di bawah judul utama yang sama seperti panduan siswa. Dukungan pengajaran tambahan tetap berada di dalam bagian-bagian tersebut.

##### 6.0 Pendahuluan, 8 menit

Mulailah dengan menghubungkan bab ini ke bab sebelumnya:

* Jika Bitcoin adalah uang, bagaimana orang benar-benar mendapatkannya dan menggunakannya?
* Apa artinya benar-benar mengendalikan bitcoin Anda?
* Mengapa menggunakan Bitcoin berbeda dengan menggunakan aplikasi bank?

Tegaskan bahwa bab ini tentang penggunaan praktis. Siswa tidak lagi hanya belajar apa itu Bitcoin, mereka belajar bagaimana berinteraksi langsung dengannya.

##### 6.1 Memperoleh dan Menukar Bitcoin, 12 menit

Jelaskan bahwa orang dapat memperoleh bitcoin dengan berbagai cara, termasuk:

* menerima pembayaran dalam bitcoin
* menambang bitcoin
* menukar fiat dengan bitcoin secara langsung
* menukar fiat dengan bitcoin secara online

Kemudian fokus pada dua jalur utama akuisisi yang dibahas dalam bab ini:

* peer-to-peer, secara langsung
* peer-to-peer, daring, online
* bursa terpusat

Jelaskan dengan jelas keuntungan dan kerugiannya.

Untuk P2P secara langsung, tekankan pertukaran langsung tanpa bank atau perantara, namun juga sebutkan risiko praktis saat bertemu orang untuk transaksi tunai.

Untuk P2P online, jelaskan escrow dengan istilah sederhana, sebagai cara untuk mengurangi risiko lawan transaksi sambil tetap memungkinkan pertukaran langsung antar pengguna.

Untuk bursa terpusat, jelaskan dengan jelas bahwa mereka memang nyaman, tetapi mengharuskan pengguna mempercayai sebuah perusahaan, seringkali membagikan informasi pribadi, dan meninggalkan dana di bawah kendali pihak ketiga sampai ditarik. Ini adalah tempat yang baik untuk menegaskan kembali bahwa kenyamanan sering kali datang dengan pengorbanan privasi dan kedaulatan.

##### 6.2 Pengantar Dompet Bitcoin, 35 menit

**Apa Itu Dompet Bitcoin Sebenarnya**

Luruskan kesalahpahaman umum sejak awal: bitcoin tidak disimpan di dalam aplikasi dompet seperti uang tunai fisik di dalam tas.  
Bitcoin itu sendiri ada di buku besar yang dikelola oleh jaringan. Yang dikendalikan pengguna adalah kemampuan untuk membelanjakannya melalui kunci privat.

Kemudian jelaskan dua hal yang sering dimaksud orang dengan "dompet":

* sistem kunci privat, dari mana alamat dihasilkan
* aplikasi atau antarmuka yang digunakan untuk berinteraksi dengan jaringan

Gunakan analogi email dari bab ini jika membantu:

* alamat publik = seperti alamat email yang bisa Anda bagikan
* kunci privat = seperti kata sandi yang harus Anda lindungi

Tegaskan dengan sangat jelas di sini: siapa pun yang mengendalikan kunci privat, mengendalikan bitcoinnya. Itu adalah konsep inti yang harus dipahami siswa.

**Dompet Swakustodi vs Dompet Kustodian**

Ini adalah salah satu bagian terpenting dari bab ini.

Jelaskan perbedaannya dengan jelas:

* Dompet swakustodi: pengguna mengendalikan kunci privat
* Dompet kustodian: pihak ketiga mengendalikan kunci privat atas nama pengguna

Kemudian jelaskan keuntungan dan kerugiannya:

Swakustodi

* kontrol penuh atas dana
* tidak ada proses persetujuan
* perlindungan terhadap penyitaan sewenang-wenang
* tanggung jawab lebih besar
* tidak ada pemulihan mudah jika frasa benih hilang

Kustodian

* pemulihan dan dukungan lebih mudah
* lebih sederhana untuk pemula
* lebih rentan terhadap pembekuan akun, peretasan, dan kendali pihak ketiga
* pengguna sebenarnya tidak benar-benar memegang bitcoin

Ini adalah saat yang tepat untuk menekankan frasa:

"Bukan kunci Anda, bukan koin Anda."

Siswa harus meninggalkan bagian ini dengan memahami tidak hanya slogannya, tetapi juga apa artinya dalam praktik.

**Jenis-Jenis Dompet yang Berbeda dan Cara Memilihnya**

Perkenalkan jenis dompet yang dibahas di bab ini:

* dompet daring
* dompet seluler
* dompet desktop
* dompet perangkat keras
* dompet kertas

Jangan menganggap salah satu sebagai yang sempurna. Sebaliknya, jelaskan bahwa masing-masing memiliki kompromi antara:

* keamanan
* privasi
* kenyamanan
* kompatibilitas
* biaya
* kontrol
* reputasi

Juga jelaskan dengan jelas bahwa kami menyarankan untuk memperhatikan apakah perangkat lunak dompet bersifat open-source, karena alat open-source dapat ditinjau, diaudit, dan dilanjutkan oleh komunitas. Hal ini terhubung langsung dengan prinsip verifikasi dalam Bitcoin.

##### 6.3 Menyiapkan Dompet Bitcoin di Ponsel, 10 menit

Bimbing siswa melalui proses dasar yang ditunjukkan dalam bab ini:

* unduh dompet
* buat dompet baru
* buat dan tulis frasa pemulihan
* konfirmasi frasa pemulihan
* tambahkan keamanan ekstra jika tersedia
* buka dompet dan temukan fungsi terima

Buat peringatan tentang frasa seed sangat jelas:

* jika frasa seed hilang, akses ke dana bisa hilang
* jika orang lain mendapatkan frasa seed, mereka bisa mengambil dana

Jika siswa melakukan ini secara langsung, pendidik harus berhenti di setiap langkah dan memastikan semua orang memahami apa yang mereka lakukan. Jika kelas lebih bersifat konseptual, bagian ini dapat dijelaskan sebagai penjelasan alur, bukan dilakukan secara langsung. Opsi pemulihan yang ditunjukkan dalam bab ini juga berguna untuk menjelaskan bahwa dompet dapat dipulihkan jika frasa seed dicadangkan dengan benar.

##### 6.4 Menerima dan Mengirim Transaksi, 17 menit

**Menerima dan Mengirim Transaksi On-chain**

Sekarang jelaskan bagaimana transaksi on-chain bekerja.

Untuk menerima bitcoin:

* buka dompet
* ketuk terima atau deposit
* salin alamat, bagikan tautan, atau tunjukkan kode QR

Untuk mengirim bitcoin:

* buka dompet
* tempel atau pindai alamat penerima
* masukkan jumlah
* periksa ulang semua detail
* siarkan transaksi
* tunggu konfirmasi

Jelaskan poin-poin kunci ini dengan jelas:

* transaksi memindahkan kepemilikan, bukan koin fisik
* transaksi tidak dapat dibatalkan
* node memverifikasi validitas
* penambang memasukkan transaksi ke dalam blok
* biaya memengaruhi prioritas konfirmasi
* transaksi on-chain umumnya aman, tetapi lebih lambat dan seringkali lebih mahal dibandingkan transaksi Lightning

Diagram alur transaksi dalam bab ini sangat berguna di sini, karena membantu siswa memvisualisasikan jalur dari permintaan dompet hingga konfirmasi jaringan.

**Transaksi dalam Aksi dan Latihan Berbasis Peran**

Gunakan struktur latihan kooperatif dari bab ini untuk memperkuat pemahaman. Jelaskan empat peran yang terlibat:

* pengirim
* penerima
* penambang
* operator node

Pendekatan sederhana di kelas adalah membagi peran dan menjalani satu transaksi langkah demi langkah. Ini membantu siswa melihat bahwa transaksi Bitcoin bukanlah sihir, melainkan proses terkoordinasi yang melibatkan persetujuan, verifikasi, dimasukkan ke dalam blok, dan pembaruan buku besar.

Tujuan di sini bukanlah kedalaman teknis. Tujuannya adalah membantu siswa memahami siapa melakukan apa dalam sebuah transaksi dan mengapa verifikasi itu penting.

##### 6.5 Jangan Percaya, Verifikasi, 8 menit

Jelaskan bahwa ini berlaku untuk:

* dompet
* bursa
* aplikasi
* detail transaksi
* klaim tentang "keuntungan mudah"
* proyek yang berpura-pura seperti Bitcoin

Jelaskan dengan jelas bahwa Bitcoin mengharuskan pengguna untuk berpikir kritis, memverifikasi apa yang mereka gunakan, dan menghindari kepercayaan buta. Jelaskan juga mengapa alat open-source penting dalam konteks ini: alat tersebut memungkinkan verifikasi secara independen.

###### Penutup dan Cek Pemahaman

Tutup dengan beberapa pertanyaan cepat:

* Apa perbedaan antara dompet kustodian dan dompet self-custodial?
* Mengapa frasa benih (seed phrase) sangat penting?
* Apa yang terjadi saat Anda mengirim transaksi on-chain?
* Mengapa transaksi on-chain lebih lambat dibanding beberapa pembayaran Bitcoin lainnya?
* Apa arti "Jangan Percaya, Verifikasi" dalam praktiknya?

#### Catatan Pengajar

Bab ini sangat praktis, jadi utamakan kejelasan, keamanan, dan pengulangan.

Siswa tidak perlu menguasai semua jenis dompet dalam satu kelas. Tujuan utamanya adalah:

* memahami dasar-dasar dompet
* memahami self-custody (penyimpanan mandiri)
* mempelajari alur transaksi dasar
* mengadopsi pola pikir verifikasi yang bertanggung jawab

Berhati-hatilah secara khusus saat membahas frasa benih dan pengaturan dompet. Siswa harus memahami bahwa ini bukan detail kecil, melainkan dasar dari kepemilikan Bitcoin.

Visual dan aktivitas yang paling berguna di bab ini adalah:

* perbandingan self-custodial vs kustodian
* tabel perbandingan jenis dompet
* latihan pengaturan dompet langkah demi langkah
* diagram alur transaksi
* aktivitas transaksi berbasis peran

##### Contoh Praktik Baik

* Penting agar siswa benar-benar mengatur dompet atau menonton demo yang hati-hati, menjadikan frasa benih sebagai inti dengan "12 kata ini ADALAH Bitcoin Anda," menguji skenario seperti "Apa yang terjadi jika Anda kehilangan ponsel?", dan berlatih mengenali phishing.
* Pengajar harus menjadi pembimbing langsung yang sudah pernah melakukan ini sebelumnya, sadar keamanan tanpa paranoid, dan jujur tentang tingkat kesulitan serta pembelajaran yang diperlukan.
* Siswa merasa telah mempelajari keterampilan nyata yang bisa digunakan, memahami bahwa frasa benih itu nyata dan penting, bukan sekadar konsep abstrak, merasa mampu menyimpan Bitcoin sendiri, dan memahami bahwa desentralisasi membutuhkan tanggung jawab pribadi.
* Capaian Pembelajaran akan tercapai jika siswa dapat mengatur dompet dan memahami perbedaan kunci publik dan privat, memahami perbandingan kustodian dan self-custody, menjelaskan cara kerja transaksi termasuk input, output, dan biaya, menunjukkan kesadaran keamanan termasuk perlindungan frasa benih, serta mampu mengajukan pertanyaan kritis tentang kepemilikan dan kontrol.

##### Manajemen Waktu

Jika waktu terbatas, prioritaskan:

* Memahami dasar-dasar dompet
* Memahami self-custody
* Mempelajari alur transaksi dasar
* Mengadopsi pola pikir verifikasi yang bertanggung jawab

Jika waktu lebih, luangkan waktu untuk:

* Tabel perbandingan self-custodial vs kustodian
* Tabel perbandingan jenis dompet
* Latihan pengaturan dompet langkah demi langkah dengan demo langsung
* Diagram alur transaksi dengan perhitungan biaya
* Praktik keamanan lanjutan dan pertimbangan dompet perangkat keras

##### Jika Siswa Mengalami Kesulitan

* Frasa benih sebagai "nyata" → "Frasa ini ADALAH bitcoin Anda; tidak ada layanan pelanggan."
* Kunci publik vs privat → Analogi email (alamat vs kata sandi).
* Mengapa ini sulit → "Anda yang mengendalikan; Anda yang bertanggung jawab." Akui adanya trade-off.
