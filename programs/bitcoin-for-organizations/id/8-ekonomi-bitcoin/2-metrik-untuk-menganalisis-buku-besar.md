# 8.2 Metrik untuk Menganalisis Buku Besar

Karena transparansi Bitcoin berbeda dengan sistem keuangan tradisional — di mana sebagian besar aliran uang terjadi di balik pintu institusi yang tertutup — hal ini memunculkan bidang analitik on-chain yang kaya, di mana data tingkat jaringan menjadi lensa untuk memahami perilaku pengguna, aliran uang, dan tren jangka panjang. Metode-metode ini dapat membantu menjawab pertanyaan spesifik, seperti seberapa aktif jaringan digunakan, apakah koin sedang diakumulasi atau dijual, dan apakah jaringan menjadi lebih aman.

Memahami metrik-metrik ini bermanfaat tidak hanya bagi pengguna Bitcoin, tetapi juga bagi peneliti atau pembuat kebijakan yang mencari wawasan tentang sistem keuangan yang sangat transparan ini.

Bagian ini berisi beberapa metrik yang umum digunakan untuk menganalisis aktivitas Bitcoin yang dikelompokkan ke dalam subkategori. Ini bukan daftar yang komprehensif. Kunjungi [www.bitcoinmagazinepro.com/charts](https://www.bitcoinmagazinepro.com/charts) untuk daftar dan deskripsi yang lebih lengkap.



#### 8.2.1 Metrik Alamat

Metrik alamat berguna untuk dipantau dari waktu ke waktu karena menunjukkan tingkat aktivitas di jaringan Bitcoin. Misalnya, seiring adopsi Bitcoin yang meningkat, jumlah alamat aktif juga bertambah. Kita dapat menelusuri lebih lanjut dengan memisahkan jumlah alamat yang memiliki jumlah minimum Bitcoin tertentu, misalnya 0,1 BTC, dalam periode waktu tertentu, seperti satu tahun. Meskipun ini memberikan gambaran adopsi Bitcoin dari waktu ke waktu, metode ini tidak sempurna karena satu individu dapat memiliki beberapa alamat Bitcoin. Sebaliknya, bursa atau ETF dapat muncul sebagai satu entitas saat menyimpan dana untuk banyak individu.

![Bitcoin: Addresses Hodling > X BTC by Year](https://cdn.sanity.io/images/vje9ehw2/staging/b88a9239820e45ed50ce00812170e2bb4d02b5d2-1407x766.png)

_Alamat yang Menyimpan Bitcoin > X BTC per Tahun. Sumber: Bitcoin Magazine Pro._

Dengan membandingkan alamat dengan harga pasar BTC saat ini, kita dapat melihat persentase keseluruhan alamat Bitcoin yang sedang untung. Ini memungkinkan kita melacak sentimen pasar karena kita dapat melihat berapa proporsi pasar yang masih memegang BTC dalam kondisi untung atau rugi.

Sebagai contoh, grafik **Persentase Keuntungan yang Belum Direalisasi** di bawah ini menunjukkan proporsi semua alamat di buku besar yang memiliki keuntungan yang belum direalisasi dalam dolar AS. Perlu dicatat, karena grafik di bawah diambil mendekati harga tertinggi sepanjang masa Bitcoin, persentase alamat yang menunjukkan keuntungan yang belum direalisasi hampir seratus persen. Kita juga dapat melihat bahwa periode panjang Persentase Keuntungan yang Belum Direalisasi di bawah satu standar deviasi dari rata-rata adalah hal yang tidak biasa. Oleh karena itu, penurunan di bawah garis ini dapat menunjukkan titik masuk yang baik bagi pembeli.

![Percent Unrealised Profit](https://cdn.sanity.io/images/vje9ehw2/staging/f306f03f31ce4faada8bf34137dd76f9d550697a-1041x491.png)

_Persentase Keuntungan yang Belum Direalisasi. Sumber: checkonchain.com_



#### 8.2.2 Indikator On-Chain

Indikator on-chain berguna karena memberikan wawasan tentang perilaku jaringan, melampaui apa yang dapat ditunjukkan oleh harga dan metrik alamat saja. Indikator ini membantu analis memahami tindakan dan sentimen berbagai jenis partisipan, seperti pemegang jangka panjang versus trader jangka pendek, dengan melacak bagaimana koin disimpan, dipindahkan, atau dinilai dari waktu ke waktu. Indikator-indikator ini memanfaatkan sifat transparan buku besar untuk mengungkap dinamika pasar tersembunyi seperti akumulasi, distribusi, atau bahkan keyakinan investor. Hal ini membuatnya sangat berguna untuk mengidentifikasi tren struktural, menilai apakah pasar sedang panas berlebihan atau undervalued, dan mengantisipasi titik balik dalam siklus pasar.

Misalnya, dengan memeriksa nilai kepemilikan BTC sejak terakhir kali ditransaksikan, kita dapat menyimpulkan apakah pasar sedang dalam tekanan (seperti yang mungkin terjadi selama titik terendah siklus utama). Metrik ini dikenal sebagai **Harga Realisasi** dan memberikan kita 'biaya rata-rata' dari semua BTC yang beredar. Jika harga pasar turun di bawah Harga Realisasi, ini menunjukkan bahwa secara agregat mayoritas alamat sedang menanggung kerugian di atas kertas.

Dengan mengelompokkan data buku besar lebih lanjut ke dalam rentang usia, kita dapat menunjukkan bagaimana jumlah BTC berpindah antar alamat dari waktu ke waktu, yang menciptakan pola seperti gelombang pada grafik yang dikenal sebagai **Gelombang HODL**.

![Bitcoin HODL Waves](https://cdn.sanity.io/images/vje9ehw2/staging/ce108e45a1a7217e081101e4a276ee2d9e95a22e-1129x577.png)

_Gelombang HODL Bitcoin. Sumber: Bitcoin Magazine Pro._

Gelombang HODL menunjukkan apa yang dilakukan pemegang jangka panjang, menengah, dan pendek dengan BTC mereka. Misalnya, pada grafik di atas, pemegang jangka pendek ditunjukkan dengan warna merah dan oranye dan kita dapat melihat lonjakan aktivitas saat kelompok ini bergegas membeli di dekat puncak pasar. Di sisi lain, kita dapat melihat bahwa pemegang jangka sangat panjang (ungu dan biru) secara konsisten meningkatkan pangsa mereka di jaringan, menunjukkan keyakinan tinggi di antara kelompok ini. Grafik ini tidak sempurna karena beberapa koin dapat berpindah dari alamat lama ke alamat baru yang masih dikendalikan oleh pengguna yang sama. Namun, grafik ini tetap memberikan gambaran menarik tentang keyakinan pemegang jangka panjang.

Cara lain untuk meneliti 'uang pintar' dari pemegang jangka panjang adalah dengan melihat **Coin Days Destroyed** (CDD). Konsep 'Coin Days' adalah hasil perkalian jumlah BTC dengan hari sejak koin terakhir dipindahkan. Misalnya, 5 BTC yang tidak bergerak selama 100 hari telah mengumpulkan 500 coin days dan 10 BTC yang tidak bergerak selama 10 hari telah mengumpulkan 100 coin days. Dengan cara ini, kita memberikan bobot lebih pada koin yang disimpan lebih lama. Ketika koin tersebut dipindahkan, coin days tersebut 'dihancurkan'. Indikator ini menunjukkan peningkatan CDD pada saat terjadi pergerakan harga yang signifikan, yang memberikan analis cara untuk membedakan aktivitas pasar rutin dari perubahan signifikan dalam sentimen pemegang jangka panjang.

Metrik lain yang dapat membantu mengidentifikasi apakah pasar sedang menilai BTC terlalu rendah atau terlalu tinggi adalah Market-Value to Realised Value atau **MVRV**. Ini dihitung dengan sederhana sebagai rasio Nilai Pasar (jumlah BTC yang beredar dikalikan harga pasar) dibagi dengan Nilai Realisasi (jumlah semua BTC sejak terakhir dipindahkan). MVRV yang tinggi menunjukkan lebih banyak koin dalam kondisi untung (sering terlihat di puncak pasar) dan MVRV yang rendah menunjukkan banyak koin yang disimpan dalam kondisi rugi (terlihat di dasar pasar).



#### 8.2.3 Metrik Penambangan

Metrik penambangan berguna untuk memahami keamanan, insentif ekonomi, dan kesehatan keseluruhan jaringan Bitcoin. Metrik seperti hashrate, pendapatan penambang, tingkat kesulitan, dan rasio biaya mengungkapkan seberapa besar kekuatan komputasi yang mengamankan blockchain dan seberapa baik penambang diberi kompensasi atas aktivitas mereka.

**Hashrate** dari jaringan Bitcoin mungkin merupakan indikator yang paling sering disebutkan terkait kesehatan jaringan dan kekuatan keamanannya. Karena proses penambangan mengamankan jaringan dan memastikan transaksi di buku besar valid, semakin besar tingkat kekuatan komputasi (atau hashing) yang ada, semakin sulit bagi aktor jahat untuk menguasai dan menyerang jaringan.

![Bitcoin Hashrate](https://cdn.sanity.io/images/vje9ehw2/staging/fcb4a24c431a37580d3d6c4ec62b664e7e41c362-1134x584.png)

_Hashrate Bitcoin. Sumber: Bitcoin Magazine Pro._

Grafik di atas menunjukkan bahwa, pada Mei 2025, total kekuatan komputasi jaringan berada di sekitar 900 TeraHash/s (900 triliun perhitungan kriptografi 'hash' per detik). Jika hashrate meningkat, ini menunjukkan bahwa jaringan menjadi lebih aman, yang memberikan rasa aman bagi pengguna.

Puell Multiple (dikembangkan oleh David Puell) melihat siklus pasar dari sudut pandang penambang dan pendapatan mereka. Metrik ini dihitung dengan membagi penerbitan harian BTC (dalam USD) dengan rata-rata pergerakan 365 hari dari nilai penerbitan harian. Metrik ini membantu mengidentifikasi periode tekanan atau kelonggaran bagi penambang. Secara historis, nilai di atas 3 telah mendahului penurunan nilai pasar BTC, karena menunjukkan penambang sangat menguntungkan. Nilai di bawah 0,5 menunjukkan tekanan dan secara historis menandakan titik terendah pasar untuk nilai BTC.
