# 8.2 Metrik untuk Menganalisis Lejar

Oleh kerana ketelusan Bitcoin berbeza daripada sistem kewangan tradisional — di mana kebanyakan aliran wang berlaku di sebalik pintu institusi yang tertutup — ia membuka ruang kepada bidang analitik on-chain yang kaya, di mana data peringkat rangkaian menjadi lensa untuk memahami tingkah laku pengguna, aliran wang dan trend jangka panjang. Metrik-metrik ini boleh membantu menjawab soalan khusus, seperti sejauh mana rangkaian digunakan secara aktif, sama ada syiling sedang dikumpul atau dijual, dan sama ada rangkaian menjadi lebih selamat.

Memahami metrik-metrik ini bukan sahaja berguna untuk pengguna Bitcoin, tetapi juga untuk penyelidik atau pembuat dasar yang ingin mendapatkan pandangan tentang sistem kewangan yang sangat telus ini.

Bahagian ini mengandungi beberapa metrik yang biasa digunakan untuk menganalisis aktiviti Bitcoin yang dikelompokkan mengikut sub kategori. Ia bukan senarai yang menyeluruh. Lawati [www.bitcoinmagazinepro.com/charts](https://www.bitcoinmagazinepro.com/charts) untuk senarai dan penerangan yang lebih lengkap.



#### 8.2.1 Metrik Alamat

Metrik alamat berguna untuk dipantau dari semasa ke semasa kerana ia menunjukkan tahap aktiviti di rangkaian Bitcoin. Sebagai contoh, apabila Bitcoin semakin diterima pakai, bilangan alamat aktif meningkat. Kita boleh meneliti perkara ini dengan melihat bilangan alamat yang memegang jumlah minimum Bitcoin tertentu, contohnya 0.1 BTC, dalam tempoh masa tertentu, seperti satu tahun. Walaupun ini memberikan gambaran tentang penerimaan Bitcoin dari masa ke masa, ia tidak sempurna kerana seseorang individu boleh memegang beberapa alamat Bitcoin. Sebaliknya, bursa atau ETF mungkin kelihatan sebagai satu entiti apabila memegang dana untuk sejumlah besar individu.

![Bitcoin: Addresses Hodling > X BTC by Year](https://cdn.sanity.io/images/vje9ehw2/staging/b88a9239820e45ed50ce00812170e2bb4d02b5d2-1407x766.png)

_Alamat yang Memegang Bitcoin > X BTC mengikut Tahun. Sumber: Bitcoin Magazine Pro._

Dengan membandingkan alamat dengan harga pasaran semasa BTC, adalah mungkin untuk melihat peratusan keseluruhan alamat Bitcoin yang berada dalam keuntungan. Ini membolehkan kita menjejaki sentimen pasaran kerana kita dapat melihat berapa bahagian pasaran yang masih memegang BTC dengan keuntungan atau kerugian.

Sebagai contoh, carta **Peratusan Keuntungan Belum Direalisasi** di bawah menunjukkan bahagian semua alamat lejar dengan keuntungan belum direalisasi yang diukur dalam dolar AS. Perhatikan bahawa, kerana carta di bawah diambil hampir pada paras tertinggi sepanjang masa Bitcoin, peratusan alamat yang menunjukkan keuntungan belum direalisasi hampir seratus peratus. Kita juga dapat melihat bahawa tempoh panjang Peratusan Keuntungan Belum Direalisasi di bawah satu sisihan piawai daripada purata adalah jarang berlaku. Oleh itu, penurunan di bawah garis ini mungkin menunjukkan titik masuk yang baik untuk pembeli.

![Percent Unrealised Profit](https://cdn.sanity.io/images/vje9ehw2/staging/f306f03f31ce4faada8bf34137dd76f9d550697a-1041x491.png)

_Peratusan Keuntungan Belum Direalisasi. Sumber: checkonchain.com_



#### 8.2.2 Penunjuk On-Chain

Penunjuk on-chain berguna kerana ia menawarkan pandangan tentang tingkah laku rangkaian, melangkaui apa yang boleh ditunjukkan oleh harga dan metrik alamat sahaja. Ia membantu penganalisis memahami tindakan dan sentimen pelbagai jenis peserta, seperti pemegang jangka panjang berbanding pedagang jangka pendek dengan menjejaki bagaimana syiling dipegang, dipindahkan, atau dinilai dari masa ke masa. Penunjuk ini memanfaatkan sifat telus lejar untuk mendedahkan dinamik pasaran tersembunyi seperti pengumpulan, pengagihan, atau keyakinan pelabur. Ini menjadikannya sangat berguna untuk mengenal pasti trend struktur, menilai sama ada pasaran terlalu panas atau di bawah nilai, dan menjangkakan titik perubahan dalam kitaran pasaran.

Sebagai contoh, dengan meneliti nilai pegangan BTC sejak kali terakhir ia dipindahkan, kita boleh membuat kesimpulan sama ada pasaran berada dalam tekanan (seperti yang mungkin berlaku semasa paras terendah kitaran utama). Metrik ini dikenali sebagai **Harga Direalisasi** dan memberikan kita 'kos purata' semua BTC dalam edaran. Jika harga pasaran jatuh di bawah Harga Direalisasi, ini menunjukkan bahawa secara agregat majoriti alamat memegang kerugian atas kertas.

Dengan mengelompokkan data lejar mengikut jalur umur, kita boleh menunjukkan bagaimana jumlah BTC bergerak antara alamat dari masa ke masa, yang menghasilkan corak seperti gelombang pada carta yang dikenali sebagai **gelombang HODL**.

![Bitcoin HODL Waves](https://cdn.sanity.io/images/vje9ehw2/staging/ce108e45a1a7217e081101e4a276ee2d9e95a22e-1129x577.png)

_Gelombang HODL Bitcoin. Sumber: Bitcoin Magazine Pro._

Gelombang HODL menunjukkan apa yang dilakukan oleh pemegang jangka panjang, sederhana dan pendek dengan BTC mereka. Sebagai contoh, dalam carta di atas, pemegang jangka pendek ditunjukkan dalam warna merah dan jingga dan kita dapat melihat lonjakan aktiviti apabila kumpulan ini berlumba membeli berhampiran puncak pasaran. Di hujung yang lain, kita dapat melihat bahawa pemegang jangka sangat panjang (dalam ungu dan biru) semakin meningkat dalam bahagian keseluruhan rangkaian, menunjukkan keyakinan tinggi dalam kalangan kumpulan ini. Carta ini tidak sempurna kerana beberapa syiling boleh bergerak dari alamat lama ke alamat baru di bawah kawalan pengguna yang sama. Namun, ia memberikan pandangan menarik tentang keyakinan pemegang jangka panjang.

Satu lagi cara untuk meneliti 'wang bijak' pemegang jangka panjang adalah dengan melihat **Coin Days Destroyed** (CDD). Konsep 'Coin Days' ialah gandaan bilangan BTC dengan hari sejak syiling itu terakhir dipindahkan. Sebagai contoh, 5 BTC yang tidak bergerak selama 100 hari telah mengumpul 500 coin days dan 10 BTC yang tidak bergerak selama 10 hari telah mengumpul 100 coin days. Dengan cara ini, kita memberikan pemberat tambahan kepada syiling yang dipegang lebih lama. Apabila syiling itu dipindahkan, coin days tersebut 'dimusnahkan'. Penunjuk ini menunjukkan peningkatan CDD pada masa pergerakan harga yang ketara, yang memberikan penganalisis cara untuk membezakan aktiviti pasaran rutin daripada perubahan bermakna dalam sentimen pemegang jangka panjang.

Satu lagi metrik yang mungkin membantu mengenal pasti sama ada pasaran menilai BTC di bawah atau melebihi nilai ialah Market-Value to Realised Value atau **MVRV**. Ia dikira dengan mudah sebagai nisbah Nilai Pasaran (bilangan BTC dalam edaran didarab dengan harga pasaran) dibahagi dengan Nilai Direalisasi (jumlah semua BTC sejak kali terakhir ia dipindahkan). MVRV yang tinggi mencadangkan lebih banyak syiling berada dalam keuntungan (sering dilihat berhampiran puncak pasaran) dan MVRV yang rendah menunjukkan banyak syiling dipegang dalam kerugian (dilihat berhampiran paras terendah pasaran).



#### 8.2.3 Metrik Perlombongan

Metrik perlombongan berguna untuk memahami keselamatan, insentif ekonomi dan kesihatan keseluruhan rangkaian Bitcoin. Metrik seperti hashrate, pendapatan pelombong, kesukaran, dan nisbah yuran mendedahkan berapa banyak kuasa pengiraan yang melindungi blockchain dan sejauh mana pelombong diberi ganjaran untuk aktiviti mereka.

**Hashrate** rangkaian Bitcoin mungkin merupakan penunjuk yang paling kerap dirujuk tentang kesihatan rangkaian dan kekuatan keselamatan. Oleh kerana proses perlombongan melindungi rangkaian dan mengesahkan bahawa transaksi di lejar adalah sah, semakin tinggi tahap kuasa pengiraan (atau hashing), semakin sukar bagi pihak berniat jahat untuk mengatasi dan menyerang rangkaian.

![Bitcoin Hashrate](https://cdn.sanity.io/images/vje9ehw2/staging/fcb4a24c431a37580d3d6c4ec62b664e7e41c362-1134x584.png)

_Hashrate Bitcoin. Sumber: Bitcoin Magazine Pro._

Carta di atas menunjukkan bahawa, pada Mei 2025, jumlah kuasa pengiraan rangkaian berada sekitar 900 TeraHash/s (900 Trilion pengiraan 'hash' kriptografi sesaat). Jika hashrate meningkat, ini menunjukkan rangkaian menjadi lebih selamat, yang meyakinkan pengguna.

Puell Multiple (dicipta oleh David Puell) melihat kitaran pasaran dari perspektif pelombong dan pendapatan mereka. Metrik ini dikira dengan membahagikan pengeluaran harian BTC (dalam USD) dengan purata bergerak 365 hari nilai pengeluaran harian. Metrik ini membantu mengenal pasti tempoh tekanan atau kelegaan pelombong. Secara sejarah, gandaan melebihi 3 telah mendahului penurunan nilai pasaran BTC, kerana ia menunjukkan pelombong sangat menguntungkan. Nilai di bawah 0.5 menunjukkan tekanan dan secara sejarah menandakan paras terendah pasaran untuk nilai BTC.
