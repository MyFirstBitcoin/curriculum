# 8 - Cara Kerja Bitcoin

Durasi: 90 menit

Ide Inti: Keamanan Bitcoin bergantung pada ide teknis yang sederhana namun kuat seperti kunci, tanda tangan, hashing, dan UTXO, yang memungkinkan kepemilikan dan verifikasi tanpa otoritas pusat.

#### Tujuan Pembelajaran

Pada akhir pelajaran ini, siswa diharapkan dapat:

* Menjelaskan bagaimana kunci publik dan privat membantu mengamankan kepemilikan dan transaksi Bitcoin.
* Menguraikan apa itu tanda tangan digital dan bagaimana tanda tangan tersebut membuktikan bahwa suatu transaksi telah disetujui oleh pemilik yang sah.
* Menjelaskan, dengan istilah sederhana, apa arti kriptografi, enkripsi, dan dekripsi dalam konteks Bitcoin.
* Mendefinisikan hashing dan menjelaskan mengapa fungsi hash penting untuk keamanan dan integritas data Bitcoin.
* Mengidentifikasi sifat dasar dari fungsi hash, seperti keluaran dengan panjang tetap, sifat satu arah, dan kepekaan terhadap perubahan kecil pada input.
* Menjelaskan model UTXO dan bagaimana bitcoin dibelanjakan, diterima, dan dikembalikan sebagai kembalian melalui output transaksi.
* Menguraikan bagaimana node membantu mencegah pengeluaran ganda dengan memeriksa apakah suatu output sudah pernah dibelanjakan.

#### Alat & Sumber Daya

##### Alat Bantu Visual

* Bab 8 - Cara Kerja Bitcoin

##### Pustaka Pendukung

* Kartu Referensi Kosakata — Bab 8 — Istilah: kriptografi, hash, UTXO, tanda tangan digital, kunci privat/publik, pohon merkle, blockchain
* Pustaka Miskonsepsi — Bab 8 — Alamat: "frasa seed yang hilang bisa dipulihkan," "kunci privat = kata sandi," "blockchain itu anonim"
* Penjelasan Teknis & Pendalaman — Fungsi hash, kunci publik/privat, model UTXO, keamanan Proof of Work

#### Aktivitas

* Transaksi dalam Aksi
* Menjelajahi Mempool

#### Pengajaran Daring

* Gunakan papan tulis digital dan gambar setiap konsep secara langsung daripada hanya mengandalkan penjelasan lisan.
* Ajarkan satu ide teknis pada satu waktu dan sering-seringlah berhenti untuk pertanyaan pengecekan.
* Gunakan visual untuk kunci, tanda tangan, hash, dan UTXO agar siswa dapat mengikuti strukturnya.
* Tetap fokus pada konsep dan hindari terlalu dalam ke matematika atau jargon.

#### Persiapan

* Siapkan dan laminasi diagram: pasangan kunci publik/privat, tanda tangan digital, model UTXO, hashing (fungsi satu arah).
* Tandai penjelajah blockchain dan kalkulator hash SHA-256; pilih 2-3 transaksi Bitcoin nyata untuk dijelaskan langkah demi langkah.
* Siapkan catatan papan tulis untuk menjelaskan input, output, dan bagaimana transaksi dikonfirmasi di blockchain.

#### Prosedur

Pelajaran ini memberikan siswa pandangan pertama tentang sisi teknis Bitcoin tanpa mengasumsikan pengetahuan teknis sebelumnya. Panduan ini sekarang mengikuti struktur ringkas yang sama seperti Diploma, dengan kriptografi dikelompokkan di bawah satu judul dan UTXO dikelompokkan di bawah judul lainnya.

##### 8.0 Pendahuluan, 8 menit

Mulailah dengan menetapkan ekspektasi:

* Apa yang membuat Bitcoin aman jika tidak ada bank sentral yang mengendalikannya?
* Bagaimana jaringan dapat mengetahui apakah seseorang benar-benar memiliki bitcoin yang ingin mereka kirim?
* Apa yang sebenarnya terjadi di balik layar ketika seseorang melakukan transaksi Bitcoin?

Jelaskan bahwa bab ini berfokus pada fondasi teknis dasar Bitcoin, khususnya kunci, tanda tangan, hashing, dan UTXO. Juga yakinkan siswa bahwa mereka tidak perlu menjadi insinyur untuk memahami logika dasarnya. Bab ini sendiri menegaskan hal tersebut dengan membandingkan Bitcoin dengan internet, banyak orang menggunakannya setiap hari tanpa benar-benar memahami setiap lapisan di bawahnya.

##### 8.1 Keamanan melalui Kriptografi, 57 menit

**Bitcoin sebagai Buku Besar yang Disimpan di Banyak Komputer**

Mulailah dengan penjelasan sederhana dari bab ini tentang jaringan Bitcoin:

* Bitcoin adalah catatan transaksi
* catatan itu disimpan di banyak komputer yang disebut node
* buku besar itu bersifat publik dan pseudonim
* buku besar itu menampilkan alamat dan riwayat transaksi, bukan detail identitas pribadi

Bagian ini membantu siswa menghubungkan kembali dengan apa yang sudah mereka ketahui dari bab-bab sebelumnya. Bitcoin tidak didasarkan pada akun tersembunyi di dalam bank. Bitcoin didasarkan pada buku besar bersama yang dapat diverifikasi oleh banyak peserta. sangat membantu di sini karena menampilkan pengguna, dompet, dan jaringan Bitcoin yang lebih luas terhubung ke buku besar publik.

**Kunci Publik dan Privat**

Sekarang masuk ke kriptografi.

Jelaskan bahwa setiap pengguna Bitcoin memiliki:

* kunci privat, yang harus tetap dirahasiakan
* sebuah kunci publik, yang dapat dibagikan

Jelaskan tujuan mereka dengan istilah sederhana:

* kunci privat membuktikan kendali dan mengotorisasi pengeluaran
* kunci publik membantu orang lain memverifikasi bahwa transaksi telah diotorisasi dengan benar

Poin pengajaran yang kuat dari bab ini adalah bahwa Bitcoin menggunakan kriptografi kunci publik/privat, bukan model lama di mana dua orang harus terlebih dahulu berbagi kunci rahasia yang sama. Hal ini penting karena memungkinkan verifikasi yang aman tanpa memaksa pengguna mengungkapkan rahasia yang melindungi dana mereka.

Anda dapat menjelaskannya seperti ini:

* kunci privat seperti bukti rahasia bahwa bitcoin itu milik Anda
* kunci publik adalah bagian dari apa yang memungkinkan jaringan memverifikasi otorisasi Anda
* siapa pun yang mengendalikan kunci privat mengendalikan kemampuan untuk membelanjakan bitcoin

Berhati-hatilah di sini agar tidak membuat bahasa enkripsi menjadi terlalu rumit. Poin terpenting untuk siswa adalah kepemilikan dan otorisasi.

**Tanda Tangan Digital dan Otorisasi Transaksi**

Sekarang jelaskan apa yang terjadi ketika seseorang mengirim bitcoin.

Gunakan urutan dari bab ini:

* seorang pengguna membuat transaksi
* pengirim menghasilkan tanda tangan digital menggunakan kunci privat mereka
* transaksi disiarkan ke jaringan
* node memverifikasi bahwa tanda tangan tersebut valid
* setelah diverifikasi dan dikonfirmasi, kepemilikan dipindahkan di buku besar

Tegaskan bahwa tanda tangan digital bukanlah hal yang sama dengan mengetik nama. Ini adalah bukti kriptografi bahwa pemilik sebenarnya telah mengotorisasi transaksi. Ini adalah salah satu mekanisme inti yang memungkinkan Bitcoin berfungsi tanpa otoritas pusat yang menyetujui transaksi secara manual. Diagramnya berguna karena menunjukkan proses penandatanganan dan verifikasi secara visual, serta jalur transaksi dari pengirim hingga validasi jaringan.

Kalimat yang baik untuk kelas adalah:

Transaksi Bitcoin tidak disetujui karena bank mengatakannya. Transaksi diterima karena jaringan dapat memverifikasi bukti kriptografi yang valid.

**Hashing dan Fungsi Satu Arah**

Selanjutnya, jelaskan tentang hashing.

Mulai dengan sederhana:

* sebuah fungsi mengambil input dan menghasilkan output
* fungsi satu arah mudah dijalankan ke satu arah, tetapi secara realistis mustahil untuk dibalik
* fungsi hash mengambil data dengan ukuran berapa pun dan mengubahnya menjadi output dengan panjang tetap yang disebut hash

Gunakan salah satu analogi dari bab ini, mana pun yang paling jelas untuk audiens Anda:

* analogi smoothie untuk fungsi satu arah
* analogi sidik jari untuk hash
* analogi partitur musik untuk memeriksa apakah sesuatu berubah

Analogi sidik jari mungkin yang paling jelas untuk sebagian besar kelas:

* hash seperti sidik jari digital untuk data
* jika input berubah sedikit saja, hash berubah total
* ini membantu komputer memeriksa integritas dan mendeteksi pemalsuan

Kemudian jelaskan mengapa hashing penting di Bitcoin:

* transaksi di-hash
* jaringan menggunakan hash untuk membantu memverifikasi integritas
* jika sebuah transaksi diubah, hash-nya juga berubah
* ini membantu melindungi buku besar dari manipulasi yang tidak terdeteksi

Visual pada halaman 7 hingga 10 sangat berguna di sini. Bab ini menunjukkan baik ide output dengan panjang tetap maupun prinsip "perubahan kecil, hasil benar-benar berbeda", yang merupakan salah satu konsep terpenting untuk dipahami siswa.

**Sifat Dasar Fungsi Hash**

Jelaskan secara singkat sifat-sifat yang disorot dalam bab ini, tanpa membuatnya terasa terlalu akademis:

* Deterministik: input yang sama memberikan output yang sama setiap saat
* Satu arah / tahan pra-citra: Anda tidak dapat membalik proses ini secara realistis
* Sensitif terhadap perubahan: bahkan perubahan input kecil menghasilkan output yang sangat berbeda
* Tahan tabrakan: sangat sulit menemukan dua input berbeda dengan output yang sama
* Cepat diverifikasi: fungsi ini efisien dijalankan dan diperiksa

Anda tidak perlu siswa menghafal setiap istilah, tetapi mereka harus memahami intinya: hashing memberi Bitcoin cara yang andal untuk mengidentifikasi data dan mendeteksi perubahan.

##### 8.2 Model UTXO, 25 menit

**Model UTXO**

Sekarang masuk ke bagian utama kedua dari bab ini: UTXO, atau Unspent Transaction Outputs (Output Transaksi yang Belum Dibelanjakan).

Jelaskan dengan istilah sederhana menggunakan analogi uang tunai dari bab ini:

* bitcoin tidak dilacak seperti saldo rekening bank saja
* sebaliknya, bitcoin terdiri dari bagian-bagian yang dapat dibelanjakan yang disebut UTXO
* ketika Anda membelanjakan bitcoin, Anda menggunakan satu atau lebih UTXO yang sudah ada sebagai input
* UTXO baru kemudian dibuat sebagai output

Gunakan contoh dari bab ini:

* jika Anda memiliki UTXO 10 BTC
* dan Anda mengirim 6 BTC
* UTXO baru sebesar 6 BTC dikirim ke penerima
* UTXO kembalian baru kembali kepada Anda
* sebagian kecil dibayarkan sebagai biaya penambang

Itu membantu siswa melihat bahwa Bitcoin bekerja lebih mirip dengan membelanjakan uang tunai dan menerima kembalian daripada hanya mengurangi angka dari satu baris rekening. Diagram sangat kuat di sini karena secara visual menunjukkan satu UTXO dipecah menjadi output penerima, output kembalian, dan biaya.

Buat dua poin kunci ini menjadi eksplisit:

* saldo dompet Anda adalah jumlah dari semua UTXO Anda
* ketika Anda membelanjakan, UTXO lama dikonsumsi dan UTXO baru dibuat

**Mencegah Pengeluaran Ganda**

Tutup materi dengan menjelaskan salah satu implikasi terpenting dari model UTXO.

Jika seseorang mencoba membelanjakan output yang sama dua kali, node akan menolak percobaan kedua karena mereka memelihara buku besar dan dapat memverifikasi apakah UTXO tersebut sudah dibelanjakan. Inilah cara Bitcoin mencegah pengeluaran ganda tanpa perlu perusahaan pembayaran pusat untuk mengelola catatan. Contoh ini sangat berguna karena menjelaskan proses Alice menggabungkan UTXO, mengirim dana ke Bob, menerima kembalian, dan transaksi yang terkonfirmasi memperbarui buku besar di seluruh node.

Cara yang jelas untuk mengatakannya di kelas adalah:

Bitcoin mencegah pengeluaran ganda karena jaringan melacak output mana yang masih belum dibelanjakan dan mana yang sudah digunakan.

###### Penutup dan Cek Pemahaman

Tutup dengan beberapa pertanyaan cepat:

* Apa perbedaan antara public key dan private key?
* Apa yang dibuktikan oleh tanda tangan digital?
* Mengapa hashing berguna dalam Bitcoin?
* Apa yang terjadi jika sebuah transaksi diubah setelah di-hash?
* Apa itu UTXO dalam istilah sederhana?
* Bagaimana jaringan mencegah seseorang membelanjakan bitcoin yang sama dua kali?

#### Catatan Pengajar

Bab ini mengandung lebih banyak istilah teknis dibandingkan bab sebelumnya, jadi utamakan kejelasan, analogi, dan pengulangan.

Tujuannya bukan membuat siswa menjadi pengembang. Tujuannya adalah membantu mereka memahami mengapa keamanan Bitcoin bekerja.

Poin terkuat yang harus diprioritaskan jika waktu terbatas adalah:

* private key vs public key
* tanda tangan digital
* apa fungsi hashing
* UTXO sebagai bagian bitcoin yang dapat dibelanjakan
* bagaimana pengeluaran ganda dicegah

Visual yang paling berguna di bab ini adalah:

* diagram user-wallet-network
* visual tanda tangan digital
* contoh hashing dan diagram output panjang tetap di halaman 7 sampai 10
* diagram UTXO di halaman 10 sampai 12

##### Seperti Apa Hasil yang Baik

* Penting untuk memperlakukan kriptografi sebagai fondasi, bukan misteri, gunakan banyak visual, hindari matematika yang mendalam, hubungkan kembali ke bab sebelumnya, dan uji pemahaman dengan aplikasi seperti "Jika seseorang mengubah satu transaksi, apa yang rusak?"
* Pengajar harus sabar dengan siswa yang kesulitan, berpikir secara visual dan menggambar semuanya, jujur tentang apa yang tidak perlu dipahami siswa, bersedia mengatakan "Saya tidak tahu tapi begini cara kita mencari tahu," dan tetap memberi semangat sepanjang proses.
* Siswa memahami mengapa Bitcoin tidak bisa diretas karena dilindungi oleh matematika, menghargai desain sistem yang elegan, merasa nyaman dengan kompleksitas meskipun tidak perlu tahu semua detail, percaya diri bertanya tanpa takut dihakimi, dan menyadari mereka telah naik tingkat dalam memahami sesuatu yang kebanyakan orang tidak tahu.
* Capaian Pembelajaran akan tercapai jika siswa dapat menjelaskan dasar-dasar kriptografi seperti fungsi satu arah dan tanda tangan digital tanpa matematika mendalam, memahami model UTXO yang menunjukkan bahwa Anda memiliki koin bukan akun, mengenali hashing sebagai fondasi keamanan Bitcoin, memahami anatomi transaksi termasuk tanda tangan dan konfirmasi, menjelaskan mengapa Bitcoin tidak dapat diubah, dan mampu bertanya kritis tentang potensi serangan atau kerentanan.

##### Manajemen Waktu

Jika waktu terbatas, prioritaskan:

* Kunci privat vs kunci publik
* Tanda tangan digital
* Apa yang dilakukan hashing
* UTXO sebagai bagian bitcoin yang dapat dibelanjakan
* Bagaimana double-spending dicegah

Jika sudah di depan, luangkan waktu untuk:

* Diagram pengguna-dompet-jaringan dan model keamanan visual
* Visual tanda tangan digital: proses kriptografi secara rinci
* Merkle tree dan keamanan rantai
* Vektor serangan tingkat lanjut dan mengapa mereka gagal

##### Jika Siswa Kesulitan

* Kriptografi terasa mengancam → "Kamu menggunakannya setiap hari; Bitcoin menggunakannya dengan cara yang sama."
* Hashing sebagai konsep → Analogi sidik jari; unik, tidak bisa diubah tanpa mengubah hash.
* Tanda tangan digital → "Membuktikan otorisasi tanpa mengungkapkan kata sandi."
