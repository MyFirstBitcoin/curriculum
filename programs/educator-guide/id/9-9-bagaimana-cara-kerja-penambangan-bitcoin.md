# 9 - Bagaimana Cara Kerja Penambangan Bitcoin

Durasi: 90 menit

Ide Inti: Penambangan Bitcoin dan validasi node bekerja sama untuk mengamankan jaringan, mengonfirmasi transaksi, dan menegakkan aturan sistem melalui Proof of Work.

#### Tujuan Pembelajaran

Pada akhir pelajaran ini, siswa diharapkan dapat:

* Menjelaskan perbedaan antara peran node Bitcoin dan peran penambang Bitcoin.
* Menggambarkan bagaimana node memvalidasi transaksi, berbagi informasi, dan membantu menegakkan aturan Bitcoin.
* Menjelaskan apa yang dilakukan penambang, termasuk memilih transaksi, membangun blok kandidat, dan bersaing untuk menemukan hash blok yang valid.
* Mendefinisikan mempool dan menjelaskan mengapa mempool berfungsi seperti ruang tunggu untuk transaksi yang belum dikonfirmasi.
* Menggambarkan bagaimana biaya transaksi memengaruhi pemilihan penambang dan kecepatan konfirmasi.
* Menjelaskan Proof of Work sebagai mekanisme yang mengamankan Bitcoin dengan membuat serangan menjadi mahal.
* Menggambarkan bagaimana penyesuaian tingkat kesulitan membantu menjaga waktu rata-rata blok sekitar 10 menit.
* Menelusuri siklus hidup penuh sebuah transaksi Bitcoin, mulai dari pembuatan dan penandatanganan hingga konfirmasi dalam sebuah blok.

#### Alat & Sumber Daya

##### Bantuan Visual

* Bab 9 - Bagaimana Cara Kerja Penambangan Bitcoin?

##### Perpustakaan Pendukung

* Kartu Referensi Kosakata — Bab 9 — Istilah: penambangan, Proof of Work, teka-teki hash, penyesuaian tingkat kesulitan, hadiah blok, mempool, serangan 51%
* Perpustakaan Miskonsepsi — Bab 9 — Membahas: "penambang menciptakan Bitcoin dari nol," "penambang mengendalikan Bitcoin," "lebih banyak penambangan = lebih tidak aman"
* Bagan Perbandingan & Lembar Referensi — Ekonomi penambangan: pendapatan, biaya, keselarasan insentif; penyesuaian tingkat kesulitan
* Penjelasan Teknis & Pendalaman — Keamanan Proof of Work; mengapa menyerang itu mahal; ambang batas 51%

#### Aktivitas

* Menjelajahi Mempool
* Transaksi dalam Aksi

#### Pengajaran Daring

* Gunakan satu diagram alur transaksi yang jelas dari penandatanganan dompet hingga konfirmasi.
* Pisahkan node dan penambang secara visual di layar sepanjang pelajaran.
* Gunakan mempool.space atau tangkapan layar untuk menunjukkan transaksi yang belum dikonfirmasi dan tekanan biaya.
* Jeda setelah setiap tahap proses penambangan dan ajukan satu pertanyaan pemahaman singkat.

#### Persiapan

* Siapkan diagram proses penambangan (mempool → pemilihan transaksi → pembuatan blok → penyesuaian tingkat kesulitan) untuk ditampilkan.
* Tandai halaman mempool.space atau blockchain.com bagian penambangan; siapkan tangkapan layar statistik penambangan dan penyesuaian tingkat kesulitan saat ini.
* Buat penjelasan visual tentang Proof of Work sebagai mekanisme keamanan; tunjukkan penyesuaian tingkat kesulitan selama 3-6 bulan terakhir.

#### Prosedur

Pelajaran ini membahas lebih dalam tentang bagaimana transaksi Bitcoin bergerak melalui jaringan dan menjadi bagian dari blockchain. Sekarang mengikuti struktur Diploma secara langsung sehingga bagian utama selaras dengan panduan siswa sambil tetap mempertahankan penjelasan lengkap untuk pendidik di setiap bagian.

##### 9.0 Pendahuluan, 8 menit

Mulailah dengan menghubungkan bab ini ke bab sebelumnya:

* Jika seorang pengguna menandatangani transaksi dengan kunci privat, apa yang terjadi selanjutnya?
* Siapa yang memeriksa apakah transaksi tersebut valid?
* Bagaimana transaksi tersebut ditambahkan ke blockchain?
* Mengapa Bitcoin membutuhkan baik node maupun penambang?

Perjelas bahwa bab ini menjelaskan bagaimana jaringan memproses transaksi dalam praktik dan bagaimana penambangan mengamankan sistem tanpa otoritas pusat.

##### 9.1 Node dan Penambang Bitcoin, 47 menit

**Node dan Penambang, Peran yang Berbeda**

Mulailah dengan memisahkan kedua peran tersebut secara jelas.

Node Bitcoin:

* menyimpan salinan blockchain
* memverifikasi apakah transaksi mengikuti aturan
* berbagi informasi dengan node lain
* membantu dompet dan perangkat lunak lain mengakses data blockchain
* dapat menolak transaksi tidak valid atau blok tidak valid

Bab ini menggambarkan node sebagai penjaga gerbang validasi, dan memperluasnya dengan analogi "petugas lalu lintas digital". Itu membantu karena menunjukkan node sebagai pemeriksa dan koordinator, bukan penguasa. Diagramnya juga menegaskan bahwa banyak node menyimpan salinan buku besar di seluruh dunia.

Penambang Bitcoin:

* mengumpulkan transaksi yang valid
* menyusun blok kandidat
* bersaing untuk menemukan hash blok yang valid
* menyiarkan blok yang valid ketika mereka menang
* menerima hadiah blok dan biaya transaksi

Poin pengajaran utama dari bab ini adalah bahwa tujuan penambangan bukan hanya untuk menciptakan bitcoin baru, tetapi untuk mendesentralisasi keamanan Bitcoin. Bitcoin baru adalah insentifnya, sementara proses penambangan itu sendiri adalah mekanisme keamanannya.

**Apa yang Sebenarnya Dilakukan Node**

Kembangkan bagian node dengan daftar fungsi node dari bab ini:

* Penjaga gerbang validasi: mereka memeriksa bahwa transaksi dan blok mengikuti aturan
* Pusat komunikasi: mereka saling terhubung dan berbagi data transaksi
* Pemeriksa kualitas: mereka menolak informasi yang tidak valid
* Informan blockchain: mereka menyediakan data ke perangkat lunak lain seperti dompet
* Penyambut node baru: mereka membantu node baru mendapatkan blockchain, sementara setiap node baru tetap memverifikasi data secara mandiri

Ini adalah saat yang tepat untuk menekankan bahwa menjalankan node memberi pengguna lebih banyak kemandirian. Alih-alih sepenuhnya bergantung pada layanan luar untuk memberi tahu mereka keadaan jaringan, mereka dapat memverifikasinya sendiri. menjelaskan poin ini dengan jelas, termasuk menyebutkan Bitcoin Core sebagai salah satu implementasi yang dapat dijalankan pengguna.

**Apa yang Sebenarnya Dilakukan Penambang**

Sekarang jelaskan penambangan dengan lebih hati-hati.

Penambang:

* mengumpulkan transaksi yang sudah diverifikasi tetapi belum dikonfirmasi
* mengelompokkan mereka ke dalam blok kandidat
* berulang kali melakukan hash data blok saat mencari hash blok yang valid
* menyiarkan blok pemenang ke jaringan
* mendapatkan hadiah jika blok diterima

Gunakan analogi "tumpukan jerami kunci yang sangat besar" dari bab ini jika membantu. Ini memberi siswa gambaran konkret tentang perlombaan penambangan. Ide utamanya bukan bahwa penambang memecahkan masalah matematika yang berguna dalam arti biasa, tetapi bahwa mereka membuktikan telah menghabiskan energi dan komputasi dunia nyata untuk mengamankan sistem.

Ini juga tempat yang tepat untuk menjelaskan hadiah penambang:

* hadiah blok: bitcoin yang baru diterbitkan
* biaya transaksi: biaya yang dilampirkan pada transaksi yang ingin dikonfirmasi pengguna

Perjelas bahwa penambang biasanya memprioritaskan transaksi dengan biaya lebih tinggi, karena itu meningkatkan hadiah mereka. Bab ini juga menjelaskan halving di sini, jadi Anda dapat mencatat secara singkat bahwa hadiah blok berkurang setiap 210.000 blok, sekitar setiap empat tahun, sesuai jadwal suplai publik Bitcoin. Halaman 5 dan 6 memuat jadwal suplai dan tabel halving mendatang, yang dapat membantu menegaskan penerbitan Bitcoin yang dapat diprediksi.

**Hash Blok Valid, Proof of Work, dan Penyesuaian Kesulitan**

Bagian ini adalah inti dari bab ini.

Jelaskan bahwa penambang sedang mencari hash blok yang valid, artinya hash blok yang memenuhi target jaringan. Bab ini menjelaskan ini sebagai menemukan angka yang lebih rendah dari target yang ditetapkan jaringan.

Kemudian jelaskan Proof of Work dengan jelas:

* penambang harus melakukan pekerjaan komputasi berulang
* yang pertama menemukan hash valid membuktikan bahwa mereka telah melakukan pekerjaan itu
* ini membuat mahal untuk menulis ulang atau menyerang buku besar
* node kemudian memverifikasi blok sebelum menerimanya

Kalimat yang kuat untuk mengajar adalah:

Proof of Work mengamankan Bitcoin dengan membuat ketidakjujuran menjadi mahal dan verifikasi menjadi mudah.

Jelaskan juga penyesuaian kesulitan:

* jaringan menyesuaikan kesulitan penambangan setiap 2.016 blok
* ini terjadi kira-kira setiap dua minggu
* tujuannya adalah menjaga waktu rata-rata blok mendekati 10 menit
* jika lebih banyak hash power bergabung ke jaringan, kesulitan naik
* jika hash power berkurang, kesulitan turun

Halaman 7 dan 8 menjelaskan proses ini dan menunjukkan bagaimana target yang lebih sulit membutuhkan lebih banyak pekerjaan. Ini membantu siswa memahami bahwa waktu Bitcoin tidak dikendalikan oleh otoritas pusat, tetapi oleh aturan protokol yang merespons secara otomatis terhadap kondisi jaringan.

##### 9.2 Apa Itu Mempool?, 15 menit

Sekarang pindah ke mempool.

Jelaskan bahwa mempool adalah ruang tunggu untuk transaksi yang valid namun belum dikonfirmasi. Ketika seorang pengguna menyiarkan transaksi, node terlebih dahulu memverifikasinya. Jika valid, mereka menambahkannya ke mempool mereka dan membagikannya ke node lain. Kemudian penambang dapat memilih dari transaksi yang menunggu tersebut saat membangun blok. Halaman 10 dan 11 menjelaskan proses ini secara langsung.

Poin penting yang perlu ditekankan:

* mempool bukanlah blockchain
* transaksi di sana masih belum terkonfirmasi
* setiap node memiliki mempool-nya sendiri
* tidak ada satu mempool universal
* transaksi dengan biaya lebih tinggi lebih mungkin dipilih lebih cepat

Bab ini juga menjelaskan alasan umum mengapa sebuah transaksi bisa tetap belum terkonfirmasi dalam waktu lama:

* biaya rendah
* kemacetan jaringan
* percobaan double-spend
* data yang salah atau tidak lengkap
* transaksi yang tidak valid

Jika bermanfaat, sebutkan aktivitas dengan mempool.space sebagai cara praktis untuk memvisualisasikan transaksi yang belum terkonfirmasi dan tingkat biaya. Juga tegaskan bahwa mempool.space hanyalah salah satu explorer, bukan mempool itu sendiri.

##### 9.3 Cara Kerja Transaksi Bitcoin, 20 menit

Sekarang satukan semuanya menggunakan urutan langkah demi langkah dari bab ini.

Versi kelas yang jelas adalah:



1. Pengirim memilih UTXO dan membuat transaksi
1. Pengirim menambahkan alamat penerima dan biaya
1. Pengirim menandatangani transaksi dengan kunci privatnya
1. Transaksi disiarkan ke jaringan
1. Node memverifikasi dan menambahkannya ke mempool mereka
1. Penambang memilihnya untuk blok kandidat
1. Penambang bersaing melalui Proof of Work
1. Satu penambang menemukan hash blok yang valid dan menyiarkan blok tersebut
1. Node memverifikasi blok dan menambahkannya ke blockchain
1. Transaksi menerima konfirmasi saat lebih banyak blok ditambahkan
1. Jelaskan poin akhir secara eksplisit:
1. setelah transaksi dimasukkan ke dalam blok yang valid, transaksi tersebut terkonfirmasi
1. input yang sudah digunakan tidak dapat digunakan lagi
1. penerima sekarang mengendalikan UTXO baru yang dibuat oleh transaksi tersebut

Diagram ringkasan sangat berguna di sini karena secara visual menghubungkan seluruh proses dari penandatanganan dompet hingga inklusi oleh penambang hingga validasi node dan distribusi blok.

###### Penutup dan Cek Pemahaman

Tutup dengan beberapa pertanyaan cepat:

* Apa perbedaan antara node dan penambang?
* Apa itu mempool?
* Mengapa beberapa transaksi terkonfirmasi lebih cepat daripada yang lain?
* Apa yang dibuktikan oleh Proof of Work?
* Mengapa Bitcoin menyesuaikan tingkat kesulitan penambangan?
* Apa langkah utama antara mengirim transaksi dan menerima konfirmasi?

#### Catatan Pengajar

Jaga agar benang merah pengajaran tetap jelas: node memverifikasi, penambang bersaing, Proof of Work mengamankan, dan mempool menampung transaksi valid sampai mereka terkonfirmasi.

Bab ini bisa terasa teknis, jadi seringlah gunakan analogi dan diagram.

Hindari membuat penambangan terdengar seperti "menciptakan bitcoin dari ketiadaan." Jelaskan dengan tepat bahwa hadiah adalah insentif, sementara proses penambangan mengamankan jaringan.

Poin terpenting yang harus diprioritaskan jika waktu terbatas adalah:



1. Peran node vs penambang
1. Mempool sebagai ruang tunggu
1. Proof of Work
1. Penyesuaian tingkat kesulitan
1. Alur transaksi dari penandatanganan hingga konfirmasi

##### Seperti Apa Penjelasan yang Baik

* Penting untuk segera memperjelas bahwa Penambang ≠ Node, menunjukkan penambangan sebagai aktivitas ekonomi dengan biaya perangkat keras nyata dan pengeluaran listrik, menggunakan penyesuaian kesulitan dan Proof of Work untuk menjelaskan mekanisme keamanan, serta menguji pemahaman dengan skenario tentang perubahan jaringan.
* Pendidik harus menggunakan angka nyata untuk mendasari diskusi, sangat jelas dan berulang-ulang tentang perbedaan antara Penambang dan Node, bersikap realistis terhadap kekhawatiran sentralisasi pada mining pool, dan menghargai tingkat kecanggihan yang sebenarnya terlibat.
* Siswa memahami bahwa penambangan adalah pekerjaan rumit yang dilakukan orang-orang cerdas karena mereka mendapatkan Bitcoin, menyadari bahwa insentif mendorong perilaku jujur karena keuntungan penambang bergantung pada keberhasilan Bitcoin, melihat sistem mengatur dirinya sendiri melalui penyesuaian tingkat kesulitan otomatis, memahami bahwa penambangan adalah bisnis nyata bukan amal, dan menghargai bahwa keamanan Bitcoin memerlukan biaya listrik dan uang sungguhan.
* Hasil Pembelajaran akan tercapai jika siswa dapat membedakan penambang yang membuat blok dari node yang memvalidasi, memahami Proof of Work sebagai mekanisme keamanan yang membuat serangan menjadi sangat mahal, mengenali penyesuaian tingkat kesulitan menjaga waktu blok sekitar 10 menit, memahami insentif penambang terkait hadiah blok dan biaya, menjelaskan mengapa serangan 51% gagal dilakukan, dan melihat penambangan sebagai aktivitas ekonomi dengan biaya dan manfaat nyata.

##### Manajemen Waktu

Jika waktu terbatas, prioritaskan:

* Peran node vs penambang (perbedaan penting)
* Mempool sebagai ruang tunggu
* Mekanisme Proof of Work
* Penyesuaian tingkat kesulitan (sistem yang mengatur diri sendiri)
* Alur transaksi dari penandatanganan hingga konfirmasi

Jika waktu lebih, luangkan waktu untuk:

* Ekonomi penambangan dan detail perangkat keras
* Dinamika mining pool dan kekhawatiran sentralisasi
* Skenario serangan 51% dan mengapa secara matematis gagal
* Keamanan jangka panjang melalui penyelarasan insentif

##### Jika Siswa Kesulitan

* Penambang vs. node (kebingungan) → "Node memvalidasi, penambang mengusulkan; wasit vs. pemain."
* Proof of Work boros → "Keamanan mahal mencegah serangan; membuatnya sia-sia."
* Penyesuaian tingkat kesulitan → "Lebih banyak penambang = blok lebih cepat = tingkat kesulitan naik; sistem bernapas."
