# 7.2 Membangun jaringan energi terbarukan

#### 7.2.0: Pendahuluan

Bitcoin bergantung pada energi untuk mekanisme konsensus ‘proof of work’-nya, yang membantu memastikan Bitcoin tetap menjadi bentuk uang yang terdesentralisasi dan tanpa izin. Jaringan listrik menghadapi tantangan dalam mengintegrasikan bentuk energi baru dari sumber terbarukan, yang memberikan tekanan pada infrastruktur saat ini. Bab ini memberikan pengenalan singkat tentang tantangan-tantangan tersebut dan gambaran aspek-aspek penting dari Bitcoin sebelum menunjukkan bagaimana Bitcoin membantu dalam evolusi jaringan energi terbarukan.


> **Info – Bitcoin sebagai mata uang energi**
>
> Pada 4 Desember 1921, New York Tribune menerbitkan sebuah artikel yang menguraikan visi Ford untuk menggantikan emas dengan mata uang energi yang ia yakini dapat mematahkan cengkeraman elit perbankan atas kekayaan global dan mengakhiri perang. Ia bermaksud melakukan ini dengan membangun "pembangkit listrik terbesar di dunia" dan menciptakan sistem mata uang baru berdasarkan "unit daya."


Seperti yang dibayangkan Henry Ford, Bitcoin menggunakan energi untuk menciptakan dan melindungi mata uang secara independen dari kepentingan pemerintah atau korporasi mana pun. Ini menjadikannya bentuk uang global pertama yang benar-benar terdesentralisasi yang pernah ada. Cara kerja penambangan Bitcoin – istilah untuk proses menciptakan dan menambahkan blok baru ke jaringan – sangat kompetitif dan mendorong komunitas penambang Bitcoin untuk mencari sumber energi berbiaya rendah. Penambangan Bitcoin juga sangat adaptif karena dapat dengan cepat meningkatkan atau menurunkan penggunaan energi di lingkungan tertentu. Karakteristik ini sangat bermanfaat bagi jaringan listrik yang memanfaatkan sumber energi terbarukan.

##### Pentingnya Pengembangan Jaringan Energi Terbarukan

Dorongan menuju sumber energi terbarukan menciptakan serangkaian tantangan baru bagi operator jaringan, seperti sifat intermiten dan tersebarnya sumber energi, kemacetan transmisi, dan keterbatasan penyimpanan energi saat ini. Hal ini menambah tingkat kompleksitas pada operasi jaringan yang tidak ada ketika hanya menggunakan sumber energi beban dasar yang terpusat dan andal. Untuk mengatasinya, operator jaringan perlu menyelidiki teknologi jaringan pintar dan teknologi peramalan berbasis AI untuk meningkatkan efisiensi. Salah satu opsi yang digunakan saat ini adalah program respons permintaan, yang membutuhkan sumber energi yang dapat beradaptasi secara dinamis hampir secara real time untuk membantu mencocokkan permintaan dan pasokan energi. Di sinilah penambangan Bitcoin dapat membantu.



#### 7.2.1 Tantangan Integrasi Energi Terbarukan

Operator jaringan harus terus-menerus menyeimbangkan pasokan dan permintaan listrik. Jika permintaan listrik terlalu tinggi, jaringan bisa gagal, yang menyebabkan pemadaman bergilir atau bahkan pemadaman total.

Jika terlalu banyak energi yang masuk ke jaringan, ini juga dapat menyebabkan masalah seperti peningkatan panas dan kerusakan pada infrastruktur. Dalam kasus yang parah, hal ini dapat memicu penutupan otomatis demi keselamatan, memicu reaksi berantai di seluruh jaringan dan menyebabkan pemadaman bergilir atau total. Pemadaman listrik adalah peristiwa bencana yang merugikan bisnis miliaran dolar. Pemadaman juga dapat merenggut nyawa.

##### Kondisi Infrastruktur Saat Ini

Infrastruktur jaringan listrik saat ini dioptimalkan untuk sumber energi tradisional seperti bahan bakar fosil, seperti batu bara, gas, atau nuklir yang dapat memasok aliran energi yang stabil, terpusat, dan terkontrol untuk memenuhi permintaan. Hal ini membuat penyeimbangan pasokan dan permintaan relatif mudah. Dengan masuknya energi terbarukan, jaringan kini harus mengelola berbagai jenis energi yang tersebar, yang semuanya berperilaku sangat berbeda dari sumber energi yang dirancang untuknya. Sumber terbarukan seperti angin dan surya menghasilkan listrik secara intermiten. Misalnya, selama kekurangan angin, pembangkit listrik tenaga angin mungkin menghasilkan sedikit atau tidak ada listrik sama sekali, sementara selama peristiwa angin kencang turbin dapat membanjiri jaringan dengan kelebihan daya. Sistem jaringan saat ini belum mampu menangani fluktuasi ini secara efektif.

##### Respons permintaan

Ada beberapa pendekatan potensial yang dapat diambil oleh operator jaringan untuk mengatasi fluktuasi pasokan dan permintaan:

* Membangun pembangkit listrik konvensional (berbasis bahan bakar fosil) yang dapat disiagakan dengan biaya tertentu. Jika terjadi peningkatan permintaan yang tidak terduga, pembangkit ini dapat diaktifkan untuk memasok energi tambahan yang dibutuhkan.
* Membangun sumber energi terbarukan secara berlebih lalu menerapkan rencana pembatasan (curtailment) untuk mencegah sumber ini membanjiri jaringan pada saat produksi listrik tinggi tanpa permintaan yang sepadan.

Alternatif lainnya adalah mencoba mengurangi permintaan pada saat penggunaan puncak**.** Namun, operator jaringan belum pernah menemukan cara yang andal, cepat, dan dapat diskalakan untuk mengurangi permintaan sebelum adanya penambangan Bitcoin, sehingga mereka tidak punya pilihan selain berinvestasi pada pembangkit siaga atau membayar sumber energi terbarukan untuk mematikan operasinya, yang keduanya merupakan opsi mahal.

##### Energi terbuang

Tantangan menghubungkan pembangkit listrik tenaga angin ke jaringan biasanya meliputi beberapa tahap; studi akses, analisis dampak mendalam, rencana implementasi, dan perjanjian koneksi. Proses ini dapat memakan waktu bertahun-tahun. Sebagai contoh, diagram di bawah ini menunjukkan total kapasitas pembangkit angin yang menunggu penilaian jaringan pada pertengahan 2024.

![Total wind energy on the waiting list for grid connection assessment](https://cdn.sanity.io/images/vje9ehw2/staging/47c8e509b367a51a036409fe4fd0b7c845ae550a-1694x1410.png)

_Total energi angin dalam daftar tunggu untuk penilaian koneksi jaringan (Sumber: windeurope.org)_

##### Koneksi jaringan

Setelah sumber energi terbarukan dibangun, sering kali terjadi penundaan untuk menghubungkannya karena kurangnya kapasitas yang tersedia di jaringan. Hal ini menyebabkan kapasitas menganggur yang terbuang sia-sia hingga koneksi dapat dilakukan, padahal selama waktu tersebut energi yang dihasilkan dapat digunakan untuk menjalankan penambang bitcoin dan menghasilkan pendapatan.

##### Kelebihan produksi dan pembatasan (curtailment)

Setelah kapasitas ini ditambahkan ke jaringan, masalahnya berpindah ke pembatasan (curtailment). Ketika angin menghasilkan kapasitas lebih dari yang dibutuhkan pada waktu tertentu, belum ada teknologi yang tersedia untuk menyimpannya, sehingga kapasitas ini terbuang sia-sia. Untuk mengambil risiko membangun pembangkit angin, operator menerima harga yang dijamin untuk setiap energi yang dihasilkan, sehingga untuk menghindari kelebihan beban pada jaringan mereka dibayar untuk mematikan turbin angin. Sebagai contoh, konsumen di Inggris membayar £1 miliar pada tahun 2024 untuk ‘membatasi’ 6,6 Gwh kapasitas.

Pendekatan lain untuk pembatasan adalah penggunaan pembangkit listrik gas peaker. Ini adalah pembangkit listrik yang menggunakan gas alam untuk menghasilkan listrik selama periode permintaan tinggi. Mereka juga digunakan untuk menyeimbangkan jaringan listrik dengan menghasilkan daya saat permintaan tinggi atau pasokan rendah. Sesuai namanya, mereka umumnya hanya digunakan pada saat permintaan puncak, tetapi harus dipasang dan dirawat secara terus-menerus, sehingga secara efektif 'dibatasi' untuk sebagian besar waktu dalam keadaan siaga. Pada saat permintaan puncak, operator jaringan dapat menggunakannya untuk meningkatkan pasokan. Sebagai contoh, penerapan penambangan Bitcoin sebagai pengganti pembelian dan pengoperasian pembangkit gas peaker diperkirakan telah menghemat $18 miliar di Texas.

##### Modernisasi jaringan

Jaringan pintar sedang dibangun untuk mengelola campuran sumber energi yang semakin beragam ini, mengintegrasikan secara mulus baik bahan bakar fosil tradisional maupun metode terbarukan modern ke dalam satu jaringan yang fungsional. Dengan memanfaatkan teknologi canggih seperti penyimpanan baterai, jaringan pintar berpotensi menyimpan kelebihan energi dan melepaskannya sesuai kebutuhan, memungkinkan mereka menangani fluktuasi dan intermitensi energi terbarukan seperti lonjakan saat produksi tinggi dan kekurangan saat periode produksi rendah. Pada saat penulisan, ini masih dalam tahap awal pengembangan.

##### Kemajuan teknologi

Pemantauan dan analisis adalah kunci untuk menerapkan jaringan pintar dalam skala besar. Ini dimulai dengan memasang sensor dan teknologi pemantauan di lokasi pembangkit tempat energi dihasilkan. Perangkat lunak analitik kemudian menganalisis dan memprediksi tren berdasarkan data yang dikumpulkan melalui pemantauan ini, memberikan saran tentang masalah kesehatan pembangkit seperti potensi penutupan dan kegagalan untuk mempersiapkan jaringan pintar menghadapi situasi tersebut. Smart meter adalah tujuan akhir pengumpulan data, memantau penggunaan energi konsumen di sumbernya. Penerapan AI diharapkan dapat membantu mengelola kompleksitas ini, sehingga operator jaringan perlu meningkatkan keterampilan di bidang ini.

##### Ringkasan

Upaya pemerintah untuk mengimplementasikan energi terbarukan dalam skala besar ke dalam jaringan listrik memberikan tekanan pada desain jaringan yang ada, dan membutuhkan investasi besar untuk mengatasi sifat energi terbarukan yang tersebar dan dinamis. Desain saat ini sangat boros energi, sehingga meningkatkan biaya bagi industri dan konsumen. Banyak teknologi yang dibutuhkan agar hal ini berhasil masih dalam tahap pengembangan saat penulisan. Solusi yang lebih baik dibutuhkan.



#### 7.2.2 Pengantar Penambangan Bitcoin

##### Apa itu penambangan Bitcoin?

Penambangan Bitcoin adalah proses yang digunakan untuk menghasilkan unit bitcoin baru dan memverifikasi transaksi baru. Proses ini melibatkan jaringan komputer di seluruh dunia yang memverifikasi dan mengamankan blockchain – buku besar virtual yang mendokumentasikan semua transaksi dan memecahkan masalah ‘double-spend’ di mana uang yang sama bisa saja dibelanjakan dua kali.

Penambang Bitcoin adalah komputer yang menggunakan ASIC khusus (application specific integrated circuit) untuk membuat blok potensial baru dan mendapatkan kesempatan menambahkan blok baru ke buku besar dengan menghasilkan solusi kriptografi yang memenuhi kriteria tertentu. Semakin banyak penambang yang aktif di jaringan, semakin sulit solusi ini ditemukan, yang disesuaikan secara dinamis oleh bagian protokol yang disebut penyesuaian tingkat kesulitan. Imbalan untuk menambahkan blok baru adalah alokasi koin baru serta biaya blok kepada penambang yang berhasil.

Perlombaan untuk menciptakan blok berikutnya dan mendapatkan imbalan telah menciptakan jaringan penambang yang luas dan terdesentralisasi yang memburu energi murah agar dapat bersaing, dan memperkenalkan dinamika menarik dalam perlombaan menambah energi terbarukan ke jaringan listrik.

##### Kontroversi konsumsi energi

Seperti disebutkan dalam pendahuluan, penambangan Bitcoin terkait dengan penggunaan energi di dunia nyata. Penggunaan energi ini telah menjadi berita selama bertahun-tahun. Sering dikritik karena menggunakan terlalu banyak energi, tidak memanfaatkan energinya secara efisien, atau dalam kasus ekstrem, dianggap sebagai bencana iklim/energi. Namun, jaringan Bitcoin adalah dan akan selalu menjadi 'pembulatan' dalam konsumsi energi global, apakah berhasil atau tidak, dan penggunaan energinya tidak akan melebihi manfaat jangka panjangnya (seberapa tinggi atau rendah pun manfaat itu nantinya). Seperti yang akan kita lihat, karakteristik spesifik dari penggunaan energinya dapat membantu adopsi energi terbarukan.

##### Fleksibilitas geografis operasi penambangan

> Salah satu eksternalitas menarik dari koin PoW – mereka selalu menjadi pembeli energi pada harga 3-5 sen/kWH. Dan beberapa aset energi terbaik berada di luar jaringan listrik. Jaringan energi global ini membebaskan aset yang terbuang dan membuat aset baru menjadi layak. Bayangkan peta topografi 3D dunia dengan titik-titik energi murah sebagai dataran rendah dan energi mahal sebagai dataran tinggi. Saya membayangkan penambangan Bitcoin seperti segelas air yang dituangkan ke permukaan, mengisi celah-celah dan meratakannya._Nic Carter_

Pada waktu tertentu, mesin penambangan Bitcoin di seluruh dunia berusaha untuk membuat blok berikutnya, dan karena biaya terbesar bagi para penambang adalah listrik, hal ini menciptakan persaingan bagi para penambang untuk mencari dan memanfaatkan energi dari sumber termurah di mana pun mereka berada. Orang sering membayangkan penambang Bitcoin bersaing dengan industri lain untuk listrik, seolah-olah penambangan Bitcoin harus menggeser penggunaan listrik lain agar dapat beroperasi. Namun, karena penambang Bitcoin secara inheren membutuhkan sumber listrik yang sangat murah, mereka _tidak bisa_ biasanya bersaing dengan pengguna listrik biasa. Akibatnya, penambang Bitcoin mencari ketidakefisienan di seluruh dunia di mana listrik kurang dimanfaatkan dan terbuang sia-sia. Hal ini dijelaskan dengan baik pada tahun 2018 oleh Nic Carter.

##### Fleksibilitas Permintaan Operasi Penambangan

> Penambang Bitcoin adalah pembeli energi yang unik karena mereka menawarkan beban yang sangat fleksibel dan mudah dihentikan, memberikan pembayaran dalam bentuk mata uang kripto yang likuid secara global, dan sepenuhnya tidak bergantung pada lokasi, hanya membutuhkan koneksi internet. Gabungan kualitas ini membentuk aset luar biasa, yaitu pembeli energi terakhir yang dapat dihidupkan atau dimatikan kapan saja di mana saja di dunia.  
_Jack Dorsey_

Selain fleksibilitas geografis, penambang Bitcoin juga dapat memberikan fleksibilitas permintaan. Penambangan Bitcoin membuat pembangunan sumber energi terbarukan secara berlebih menjadi menguntungkan, karena memungkinkan kelebihan pasokan tersebut dimonetisasi. Setiap komunitas yang menginginkan listrik yang andal memang membutuhkan kapasitas listrik yang berlebih, dan untuk angin, surya, serta hidro hal ini bahkan lebih penting karena sifatnya yang variabel. Namun, pembangunan berlebih biasanya tidak terlalu efektif secara biaya, kecuali jika Anda dapat menggunakannya untuk sesuatu yang menguntungkan dan bermanfaat saat tidak dibutuhkan. Penambang Bitcoin adalah solusi unik untuk masalah tersebut, dapat membuat pembangunan berlebih menjadi menguntungkan, dan dengan demikian berperan secara tidak langsung sebagai solusi penyimpanan energi.

Selama sebagian besar waktu ketika pasokan lebih besar daripada permintaan, penambang Bitcoin berperan sebagai salah satu konsumen listrik di komunitas yang dapat menyalakan mesin mereka, memperoleh pendapatan, dan membayar biaya listrik mereka. Jika terjadi lonjakan permintaan listrik atau pengurangan pasokan yang dapat menyebabkan pemadaman di wilayah tersebut, para penambang tersebut dapat mematikan mesin mereka sementara.

Kontrak tarif komersial yang terstruktur dengan baik dapat membuat hal ini berjalan lancar. Perusahaan utilitas dapat menawarkan tarif terendah di wilayah tersebut kepada penambang, dengan imbalan mereka memiliki toleransi lebih tinggi terhadap variabilitas dan poin fleksibilitas kontrak lainnya.

Singkatnya, penambang Bitcoin unik karena:

* Hampir seluruh biaya operasional mereka adalah listrik
* Mereka dapat mentoleransi konsumsi yang terputus-putus
* Mereka fleksibel dengan lokasi mereka, sehingga dapat menghindari infrastruktur transmisi yang mahal dengan menempatkan diri di dekat sumber listrik.

Akibatnya, mereka dapat mengorbankan variabel yang tidak dapat dilakukan oleh sebagian besar perusahaan lain, demi mendapatkan harga listrik yang sangat murah saat listrik melimpah. Ini berarti dengan penambangan Bitcoin kini kita memiliki pembeli untuk setiap watt energi yang dihasilkan, di mana pun di dunia, 24x7.



#### 7.2.3 Studi Kasus

Secara teori, kita dapat melihat bahwa penambangan Bitcoin dapat berperan besar dalam percepatan adopsi energi terbarukan. Mari kita lihat beberapa contoh penerapannya saat ini.

##### Listrik tenaga air yang terbuang

Fasilitas pembangkit listrik tenaga air menghasilkan listrik secara terus-menerus, yang juga dapat berfluktuasi sepanjang tahun tergantung lokasi dan musim. Ini biasanya berarti listrik terbuang baik pada malam hari saat semua orang tidur, atau karena peningkatan produksi selama musim hujan, seperti di Tiongkok. Karena penambang Bitcoin dapat pergi ke sumber energi, mereka dulu berbondong-bondong ke Sichuan selama musim hujan untuk memanfaatkan energi yang seharusnya terbuang itu. Mereka melakukan ini bukan karena mereka adalah pecinta lingkungan yang altruistik, tetapi semata-mata karena murah dan tidak ada orang lain yang memanfaatkannya. Ketika Tiongkok melarang penambangan bitcoin, mereka langsung berkemas dan pergi.

Kota atau desa terpencil yang terletak di dekat sumber tenaga air potensial biasanya tidak mampu membiayai investasi yang diperlukan untuk membangun infrastruktur transmisi guna menyediakan listrik. Dalam situasi ini, penambang Bitcoin dapat mengumpulkan modal yang dibutuhkan untuk membangun fasilitas, menyediakan listrik murah bagi penduduk lokal, dan menggunakan energi cadangan untuk menjalankan fasilitas penambangan. Sekali lagi, ini bukan karena altruism, tetapi demi keuntungan; sebuah win/win bagi penambang dan komunitas lokal.

##### Penambangan Bitcoin untuk menstabilkan Jaringan Listrik

Jaringan listrik harus mengimbangi dua hal: perubahan tingkat pasokan dan perubahan tingkat permintaan. Beberapa sumber listrik sangat konsisten, seperti pembangkit listrik tenaga nuklir dasar, yang dapat berjalan 24/7. Sumber lain, seperti angin, surya, dan sebagian hidro, lebih variabel tergantung apa yang diberikan oleh Alam dalam bentuk angin, matahari, dan hujan pada periode tertentu. Karena variabilitas ini, pasokan listrik perlu dibangun secara berlebih sehingga bahkan pada hari dengan produksi pasokan yang sangat rendah pun tetap cukup untuk menyediakan listrik ke komunitas. Di Texas, rencana default adalah membangun pembangkit listrik berbahan bakar fosil sebagai cadangan untuk mengatasi peningkatan permintaan. Pendekatan alternatif yang diambil adalah menambah fleksibilitas respons permintaan dengan mengintegrasikan penambang Bitcoin ke dalam jaringan. Pendekatan ini menghemat jutaan dolar bagi warga Texas dalam investasi dan memberikan alternatif yang lebih ramah lingkungan.

##### Manfaat lain yang berdekatan

Meskipun tidak secara langsung terkait dengan infrastruktur jaringan energi terbarukan, ada solusi terkait energi lain yang dapat diberikan oleh penambangan Bitcoin:

* Gas suar: menghindari gas yang dibuang atau dibakar lepas ke atmosfer dengan menggunakannya untuk penambangan lokal.
* Gas TPA: menangkap metana di tempat pembuangan sampah dan menggunakannya untuk pembangkit listrik guna mengurangi emisi gas rumah kaca yang berbahaya
* Mendorong teknologi baru: Konversi energi termal laut (OTEC) adalah metode yang dikenal untuk memanfaatkan perbedaan suhu antara permukaan dan kedalaman laut untuk menghasilkan listrik. Ini belum pernah layak secara komersial sebelum adanya Bitcoin.
* Mendorong pengembangan listrik di negara berkembang: Seperti yang telah disinggung sebelumnya, penambang Bitcoin dapat menjadi 'penyewa utama' yang akan selalu menggunakan listrik yang dihasilkan, membenarkan investasi awal dan kemudian pindah ketika komunitas lokal berkembang dan menemukan penggunaan listrik yang lebih baik.

##### Ringkasan

Penambangan Bitcoin dapat membantu mendukung investasi dan keberlanjutan infrastruktur energi terbarukan:

* Menyerap kelebihan energi selama periode permintaan rendah
* Menstabilkan jaringan listrik dengan mencocokkan pasokan dan permintaan
* Menyediakan aliran pendapatan bagi pengembang energi terbarukan
* Membiayai proyek energi di daerah terpencil atau kurang terlayani
* Mendorong batas efisiensi energi
* Bertindak sebagai pembeli terakhir untuk energi yang seharusnya terbuang di mana saja di dunia kapan saja



#### 7.2.4 Menanggapi kekhawatiran

Kita telah melihat bagaimana penambangan Bitcoin dapat membantu pertumbuhan energi terbarukan, tetapi apa saja hambatan untuk hal ini?

##### Dampak lingkungan dan kesalahpahaman

Agar Bitcoin dapat berhasil diintegrasikan ke dalam sesuatu yang sepenting jaringan listrik, kekhawatiran tentang dampak lingkungan dan kesalahpahaman seperti penggunaan energi perlu diatasi. Organisasi seperti Bitcoinpolicy.uk bekerja keras untuk mengatasi kekhawatiran ini dengan industri dan otoritas terkait, tetapi ini sering kali merupakan perjuangan yang berat. Membantu mengedukasi pasar tentang potensi manfaat memonetisasi energi terbuang atau memanfaatkan kelebihan energi yang dihasilkan sangat penting untuk adopsi yang sukses.

##### Regulasi dan insentif untuk penambangan ramah lingkungan

Setiap negara mungkin memiliki pendekatan yang sangat berbeda terhadap adopsi penambangan, mulai dari negara seperti Bhutan yang menambang Bitcoin secara langsung, hingga negara bagian AS seperti Texas yang mengizinkan penambangan tanpa secara aktif mencoba menghentikannya, hingga Tiongkok yang mengeluarkan larangan penambangan total.

Negara lain seperti Inggris mungkin membayar jumlah besar kepada operator ladang angin untuk mematikan pembangkit listrik pada saat angin kencang. Insentif untuk integrasi penambangan Bitcoin dengan demikian terbatas dalam kasus seperti itu, meskipun hal ini akan mengubah model bisnis dari membebani konsumen menjadi memberikan keuntungan yang dapat mengurangi tagihan.

##### Hambatan Regulasi Tidak Langsung

Hambatan regulasi tidak langsung lainnya mungkin ada yang tidak secara langsung merujuk pada Bitcoin tetapi tetap dapat berdampak. Misalnya, infrastruktur yang perlu dibangun untuk ladang angin lepas pantai agar terhubung ke jaringan listrik mungkin dilarang untuk digunakan bersama dengan infrastruktur pusat data yang dibutuhkan untuk penambangan Bitcoin.



#### 7.2.5 Kesimpulan dan ajakan bertindak

* Bitcoin menyediakan layanan yang dapat digunakan orang untuk menyimpan dan mentransfer nilai. Sejauh ini, pasar dengan jutaan peserta telah memutuskan bahwa jaringan ini memiliki nilai, dan seperti halnya segala sesuatu yang bernilai, ia mengonsumsi energi.
* Penambangan Bitcoin menggunakan kurang dari 0,1% energi global, dan kekhawatiran tentang penggunaan energi yang dianggap boros kini telah sepenuhnya dijawab di pasar.
* Sebagian besar energi yang digunakan oleh penambangan Bitcoin sebenarnya adalah energi yang terbuang dan tidak dimanfaatkan. Ini karena penambang Bitcoin memiliki kemampuan unik untuk pergi ke lokasi terpencil dan menangani pasokan listrik yang tidak konsisten yang tidak dapat dimanfaatkan oleh konsumen lain.
* Bitcoin dapat membantu menstabilkan jaringan listrik, menjadi penyewa utama dengan menjadi yang pertama menggunakan dan membayar listrik hingga dapat terhubung ke jaringan dan digunakan di tempat lain, serta menyediakan respons permintaan dengan mematikan mesin dengan cepat selama periode permintaan puncak.

Pasar Bitcoin dan energi sedang mengalami konvergensi, dan kepemilikan aset kemungkinan juga akan menyatu. Potensi tumpang tindih juga ada dengan AI, yang membutuhkan keterampilan dan infrastruktur serupa dengan Bitcoin dan akan digunakan untuk mengelola jaringan listrik pintar. Perusahaan yang menyesuaikan pengembangan roadmap mereka untuk mengakomodasi tren ini akan berada pada posisi terbaik untuk mendapatkan manfaat dari perkembangan ini.



###### Lampiran - Referensi

1. [https://www.btcpolicy.org](https://www.btcpolicy.org/)
1. [https://www.da-ri.org/articles/how-bitcoin-mining-saved-texans-18-billion](https://www.da-ri.org/articles/how-bitcoin-mining-saved-texans-18-billion)
1. [https://gript.ie/uks-hidden-1billion-cost-of-wind-energy/](https://gript.ie/uks-hidden-1billion-cost-of-wind-energy/)
1. [https://www.lynalden.com/bitcoin-energy/#electricity](https://www.lynalden.com/bitcoin-energy/#electricity)
1. [https://squareup.com/gb/en/press/bcei-white-paper](https://squareup.com/gb/en/press/bcei-white-paper)
1. [https://www.mara.com/posts/bitcoin-mining-the-environment-the-positive-externalities](https://www.mara.com/posts/bitcoin-mining-the-environment-the-positive-externalities)
