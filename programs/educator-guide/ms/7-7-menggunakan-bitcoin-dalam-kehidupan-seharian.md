# 7 - Menggunakan Bitcoin dalam Kehidupan Seharian

Tempoh: 90 minit

Idea Utama: Lightning Network menjadikan Bitcoin lebih praktikal untuk pembayaran harian dengan membolehkan transaksi yang lebih pantas dan murah sambil mengekalkan Bitcoin sebagai asasnya.

#### Objektif Pembelajaran

Pada akhir pelajaran ini, pelajar sepatutnya dapat:

* Terangkan apa itu Lightning Network dan mengapa ia dibina di atas Bitcoin.
* Bandingkan transaksi on-chain dan Lightning dari segi kelajuan, kos, dan kompromi keselamatan.
* Bezakan antara dompet Lightning kustodian dan kendiri, serta terangkan mengapa kawalan kendiri itu penting.
* Sediakan dompet Lightning dan huraikan peranan frasa benih dalam pemulihan dompet.
* Tunjukkan bagaimana pembayaran Lightning bergerak melalui rangkaian, walaupun dua pengguna tidak berkongsi saluran secara langsung.
* Kenal pasti cara-cara sebenar Bitcoin boleh digunakan dalam kehidupan seharian melalui Lightning, termasuk kopi, barangan runcit, pembayaran peniaga, dan perbelanjaan tempatan.
* Terangkan bagaimana alat seperti BTCPay Server, BTCMap, dan kad hadiah membantu memperluas penggunaan Bitcoin dalam amalan.
* Huraikan apa itu ekonomi bulat Bitcoin dan mengapa Lightning menjadikannya lebih berdaya maju.

#### Alat & Sumber

##### Bahan Visual

* Bab 7 - Menggunakan Bitcoin dalam Kehidupan Harian

##### Perpustakaan Sokongan

* Kad Rujukan Perkataan — Istilah: Lightning Network, saluran pembayaran, perutean, Lapisan 2, ekonomi bulat, kiriman wang
* Perpustakaan Contoh Dunia Sebenar & Kajian Kes — El Salvador, ekonomi bulat Austin, kisah penerimaan peniaga Lightning
* Carta Perbandingan & Lembaran Rujukan — Perbandingan On-Chain vs. Lightning; Perbandingan Yuran & Kelajuan antara kaedah pembayaran
* Penerangan Mudah Lightning Network — Cara saluran pembayaran berfungsi tanpa jargon; perutean; keselamatan; kes penggunaan
* Senario Pembayaran Langkah demi Langkah — Hantar kepada rakan, terima pembayaran, kiriman wang, terima sebagai pekerja bebas
* Alat Perbandingan Yuran & Kelajuan — Bila hendak guna Lightning vs. on-chain vs. perbankan (dengan contoh kos)

#### Aktiviti

* Perlumbaan Relay Lightning

#### Pengajaran Dalam Talian

* Gunakan slaid perbandingan sebelah-menyebelah untuk pembayaran on-chain dan Lightning.
* Mulakan dengan kes penggunaan sebenar seperti kopi atau kiriman wang supaya pelajar faham mengapa Lightning wujud.
* Gunakan rajah perutean tiga orang yang ringkas supaya penjelasan rangkaian kekal jelas.
* Kekalkan mekanik saluran secara ringkas kecuali kelas sudah mempunyai asas yang kukuh.

#### Persediaan

* Muat turun dompet Lightning dan sediakan tangkapan skrin yang menunjukkan kelajuan transaksi on-chain (perlahan) vs. Lightning (pantas) secara sebelah-menyebelah.
* Cari 2-3 peniaga atau komuniti sebenar yang menggunakan Lightning; tandakan BTCMap.org untuk rujukan.
* Sediakan carta perbandingan on-chain vs. Lightning (kelajuan, yuran, keselamatan, kes penggunaan) untuk diedarkan.

#### Prosedur

Pelajaran ini menunjukkan kepada pelajar bagaimana Bitcoin menjadi praktikal untuk pembayaran harian melalui Lightning Network. Panduan ini kini mengikuti struktur Diploma secara langsung supaya bahagian utama Lightning sepadan dengan panduan pelajar, manakala perbandingan, alat peniaga, dan bahan ekonomi bulat kekal di tempat yang sesuai.

##### 7.0 Pengenalan, 8 minit

Mulakan dengan menghubungkan bab ini dengan bab sebelumnya:

* Jika Bitcoin berfungsi secara on-chain, mengapa lapisan lain diperlukan?
* Apa yang berlaku apabila orang ingin membuat banyak pembayaran kecil dengan cepat?
* Sistem pembayaran jenis apa yang lebih sesuai untuk kopi, barangan runcit, atau membayar rakan?

Jelaskan bahawa bab ini memberi tumpuan kepada Bitcoin untuk kegunaan harian, terutamanya apabila kelajuan dan yuran rendah penting. Tegaskan bahawa Lightning dibina di atas Bitcoin, bukan berasingan daripadanya.

##### 7.1 Lightning Network, 25 minit

**Apa Itu Lightning Network**

Terangkan bahawa Lightning Network ialah sistem pembayaran yang dibina di atas Bitcoin yang membolehkan pengguna menghantar dan menerima bitcoin dengan cepat dan murah. Ia berfungsi dengan memindahkan banyak pembayaran kecil keluar dari blockchain utama dan hanya menyelesaikan keputusan akhir kembali ke on-chain kemudian.

Cara yang membantu untuk menerangkannya ialah dengan analogi tab kafe dari bab ini:

* daripada membayar setiap item satu demi satu secara on-chain
* dua pihak membuka saluran
* mereka mengemas kini baki semasa mereka bertransaksi
* hanya baki akhir direkodkan di blockchain apabila mereka menutup saluran

Itu menjadikan Lightning lebih pantas dan murah untuk pembayaran kecil yang kerap. Juga jelaskan bahawa pembayaran Lightning boleh melalui rangkaian, jadi pengguna tidak perlu mempunyai saluran langsung dengan setiap orang yang mereka bayar.

**On-chain vs Lightning**

Sekarang buat perbezaan ini sangat jelas.

Transaksi on-chain

* berlaku secara langsung di blockchain Bitcoin
* biasanya lebih perlahan
* bergantung pada kemasukan dan pengesahan blok
* cenderung lebih selamat
* boleh menjadi lebih mahal bergantung pada yuran

Transaksi Lightning

* berlaku di lapisan kedua yang dibina di atas Bitcoin
* diselesaikan dengan jauh lebih pantas
* biasanya jauh lebih murah
* berguna untuk pembayaran kecil dan kerap
* melibatkan kompromi berbanding penyelesaian on-chain

Pastikan perkara utama mudah: on-chain lebih kukuh untuk penyelesaian akhir, Lightning lebih kuat untuk kelajuan dan penggunaan harian yang kos rendah. Perbandingan ini sangat berguna di sini.

##### 7.2 Jenis Dompet Lightning yang Berbeza, 10 minit

Terangkan bahawa dompet Lightning menjalankan fungsi asas yang sama seperti dompet Bitcoin, menerima dan menghantar bitcoin, tetapi ia direka untuk digunakan di Rangkaian Lightning. Kemudian terangkan perbezaan utama dompet dalam bab ini:

* kawalan sendiri: pengguna mengawal kunci
* kustodian: orang lain mengawal kunci

Perjelaskan kompromi utama:

* dompet kustodian mungkin terasa lebih mudah dan senang digunakan
* tetapi pengguna bergantung pada kebenaran dan kawalan orang lain
* dompet kawalan sendiri memberi lebih pemilikan dan kedaulatan

Juga tegaskan cadangan bab ini untuk mengutamakan dompet sumber terbuka, kerana alat sumber terbuka boleh disemak, diperbaiki, dan disahkan oleh komuniti.

##### 7.3 Menyediakan Dompet Bitcoin Lightning, 10 minit

Bimbing pelajar melalui aliran asas penyediaan:

* muat turun dompet Lightning
* cipta dompet baru
* tulis frasa pemulihan
* sahkan perkataan dalam urutan yang betul
* tambah keselamatan tambahan jika dompet membenarkannya
* mula menggunakan dompet

Jelaskan dengan jelas tentang frasa seed:

* ia membolehkan pengguna mendapatkan semula akses
* jika ia hilang, akses kepada dana mungkin hilang
* jika orang lain mendapatkannya, mereka boleh mengawal dana

Bahagian ini harus benar-benar menekankan tanggungjawab dan pengendalian yang selamat, sama seperti dalam bab on-chain.

##### 7.4 Menghantar dan Menerima Transaksi Lightning, 17 minit

**Bagaimana Transaksi Lightning Berfungsi dalam Amalan**

Gunakan contoh Marcia, Jeff, dan Eve untuk menerangkan routing. Marcia tidak perlu mempunyai saluran langsung dengan Eve. Pembayarannya boleh bergerak melalui Jeff, yang bersambung ke rangkaian, dan tetap sampai kepada Eve dengan selamat.

Jelaskan perkara-perkara ini dengan jelas:

* Pembayaran Lightning boleh bergerak melalui perantara
* perantara itu membantu mengarahkan pembayaran
* proses routing tidak bermaksud pengguna mempercayai bank atau pemproses pembayaran berpusat
* rangkaian menggunakan kriptografi supaya pembayaran sampai kepada penerima yang dimaksudkan

Ini membantu pelajar faham bahawa Lightning masih peer-to-peer, walaupun pembayaran bergerak melalui struktur rangkaian yang lebih luas. Jika berguna, nyatakan bahawa bab ini juga menyebut operator nod boleh memperoleh yuran dan membantu menguatkan rangkaian dengan mengarahkan pembayaran.

**Membiayai Saluran dan Menggunakan Lightning Berulang Kali**

Terangkan contoh Mina dengan lebih lanjut:

* Mina memindahkan bitcoin dari dompet on-chain ke dompet Lightning miliknya
* ini membiayai satu saluran pembayaran
* dia kemudian boleh membuat pembayaran berulang tanpa perlu membuka semula proses setiap kali
* apabila saluran ditutup, baki akhir akan diselesaikan semula di atas rantaian

Jelaskan satu had penting: dana yang dikunci dalam saluran aktif sedang digunakan untuk Lightning dan tidak boleh digunakan secara bebas untuk transaksi di atas rantaian pada masa yang sama. Ini membantu pelajar faham bahawa Lightning sangat berkuasa, tetapi ia melibatkan struktur pembayaran yang berbeza.

##### 7.5 Membeli Kopi dan Barangan Runcit dengan Bitcoin, 20 minit

**Kes Penggunaan Harian**

Beralih daripada mekanik kepada kehidupan sebenar.

Terangkan bahawa Lightning sangat berguna untuk:

* membeli kopi
* barangan runcit
* membeli-belah
* membayar rakan
* transaksi kecil harian

Contoh Mina dalam bab ini membantu menunjukkan mengapa Lightning lebih sesuai berbanding sistem pembayaran tradisional untuk banyak situasi: ia pantas, yuran rendah, tanpa sempadan, dan boleh diakses walaupun oleh mereka yang mungkin tidak mempunyai akaun bank. Jadual perbandingan dan rajah pemprosesan pembayaran adalah alat pengajaran yang kuat di sini, terutamanya untuk menunjukkan berapa banyak perantara yang wujud dalam pembayaran kad tradisional.

**Alat Pedagang dan Membelanjakan Bitcoin di Dunia Sebenar**

Sekarang terangkan bagaimana perniagaan dan pengguna boleh menjadikan Lightning praktikal dalam kehidupan seharian.

Terangkan tiga alat utama atau laluan dalam bab ini:

BTCPay Server

* pemproses pembayaran sumber terbuka
* membolehkan peniaga menerima bitcoin secara langsung
* tiada orang tengah yang mengawal dana
* berguna untuk pembayaran perniagaan dalam talian dan bersemuka

BTCMap

* membantu pengguna mencari peniaga dan komuniti yang menerima bitcoin
* membolehkan orang mencari secara tempatan
* boleh dikemas kini oleh komuniti

Kad hadiah dan baucar

* alat peralihan untuk membelanjakan bitcoin di tempat yang belum menerima secara langsung
* membantu merapatkan jurang sementara penggunaan berkembang

Bahagian ini penting kerana ia menunjukkan kepada pelajar bahawa penggunaan Bitcoin bukan sekadar teori. Sudah ada alat sebenar yang boleh digunakan orang hari ini.

**Ekonomi Pekeliling dan Bitcoin sebagai Medium Pertukaran**

Tutup kandungan utama dengan menerangkan bahawa ekonomi pekeliling ialah komuniti di mana peserta cuba membeli dan menjual antara satu sama lain sebanyak mungkin. Diterapkan kepada Bitcoin, ini bermakna peniaga, pekerja, dan pengguna memilih untuk bertransaksi dalam bitcoin dan saling menyokong secara ekonomi.

Jelaskan mengapa Lightning penting di sini:

* pembayaran hampir serta-merta
* yuran rendah
* pembayaran kecil menjadi praktikal
* perdagangan tempatan menjadi lebih mudah untuk dikekalkan

Anda boleh sebut bahawa bab ini merujuk kepada contoh seperti Arnhem dan Bitcoin Beach, menunjukkan bahawa ekonomi pekeliling bukan sekadar hipotesis. Ia sudah wujud dan terus berkembang. Garis masa visual sangat berguna di sini

###### Penutup dan Semakan Kefahaman

Tutup dengan beberapa soalan pantas:

* Mengapa Lightning Network dibina?
* Apakah satu perbezaan utama antara pembayaran di atas rantaian dan Lightning?
* Mengapa penjagaan kendiri penting dalam dompet Lightning?
* Bagaimana seseorang boleh menerima pembayaran Lightning tanpa saluran langsung kepada setiap orang?
* Apakah itu ekonomi pekeliling Bitcoin?

#### Nota Pendidik

Pastikan benang pengajaran utama jelas: Bitcoin ialah lapisan asas, Lightning membantu menjadikan pembayaran harian lebih pantas dan murah.

Bab ini sepatutnya terasa praktikal dan konkrit, bukan terlalu teknikal.

Utamakan kefahaman berbanding mekanik saluran yang mendalam.

Perkara paling penting untuk diutamakan, jika masa terhad, ialah:

* apa itu Lightning
* pertukaran antara on-chain vs Lightning
* penjagaan dan penyediaan dompet
* pembayaran dunia sebenar
* ekonomi bulat

Visual yang paling berguna dalam bab ini ialah:

* perbandingan on-chain vs Lightning
* perbezaan dompet
* contoh penghalaan dengan Marzuki, Jeff, dan Eva
* jadual perbandingan dan carta kapasiti
* diagram pemprosesan pembayaran tradisional
* garis masa ekonomi bulat

##### Contoh Terbaik

* Penting untuk bermula dengan masalah "Bitcoin mengambil masa 10 minit dan kos RM10," terangkan Lightning sebagai lorong laju di atas Bitcoin, gunakan contoh sebenar daripada peniaga dan koridor kiriman wang, dan cipta pokok keputusan bila hendak guna on-chain berbanding Lightning.
* Pendidik harus bersikap pragmatik tentang apa yang sebenarnya diselesaikan oleh Lightning, berkongsi kisah dari lapangan di mana Bitcoin digunakan, jelaskan pertukaran khusus, dan kekal realistik tentang kadar penerimaan sambil teruja dengan kemungkinan yang ada.
* Pelajar mengalami sendiri Bitcoin berfungsi untuk pembayaran sebenar di tempat sebenar, faham bahawa kelajuan dan kos penting untuk pembayaran, bayangkan ekonomi bulat di mana Bitcoin kekal tempatan, kenal pasti bahawa Lightning ≠ Bitcoin (alat berbeza untuk tujuan berbeza), dan menjadi ingin tahu tentang sistem ekonomi yang dibina atas pembayaran Bitcoin.
* Hasil Pembelajaran akan dicapai jika pelajar boleh menerangkan Lightning Network sebagai lapisan di atas Bitcoin, faham asas saluran pembayaran dan penghalaan, lihat kes penggunaan sebenar untuk pembayaran Lightning, bandingkan on-chain dan Lightning untuk pelbagai senario, faham konsep ekonomi bulat, dan kenal pasti pertukaran khusus bagi setiap pendekatan.

##### Pengurusan Masa

Jika masa terhad, utamakan:

* Apa itu Lightning
* Pertukaran antara On-chain vs Lightning
* Pembayaran dunia sebenar
* Ekonomi bulat

Jika ada masa lebih, beri tumpuan pada:

* Mekanisme saluran pembayaran dan penghalaan
* Alat perbandingan yuran dan kelajuan
* Kajian kes ekonomi bulat di El Salvador dan Austin
* Langkah demi langkah senario pembayaran Lightning secara praktikal

##### Jika Pelajar Menghadapi Kesukaran

* Kenapa Lightning wujud → Bandingkan: 10 minit/RM10 vs. beberapa saat/sebahagian sen.
* Saluran pembayaran → Analogi buku hutang kafe; selesaikan dalaman kemudian di Bitcoin.
* Kenapa ia penting secara global → "Bagaimana jika tiada bank tetapi ada Bitcoin?"
