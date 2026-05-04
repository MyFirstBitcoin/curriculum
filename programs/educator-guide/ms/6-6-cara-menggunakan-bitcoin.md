# 6 - Cara Menggunakan Bitcoin

Tempoh: 90 minit

Idea Utama: Menggunakan Bitcoin secara on-chain mengajar pelajar bagaimana pemilikan, penjagaan kendiri, dan pengesahan berfungsi dalam amalan, menjadikan teori kepada tindakan kewangan secara langsung.

#### Objektif Pembelajaran

Pada akhir pelajaran ini, pelajar sepatutnya boleh:

* Kenal pasti cara biasa untuk memperoleh dan menukar bitcoin, termasuk kaedah peer-to-peer dan pertukaran berpusat.
* Terangkan perbezaan antara dompet penjagaan kendiri dan dompet jagaan, serta mengapa penjagaan kendiri penting dalam Bitcoin.
* Huraikan tujuan kunci peribadi, alamat awam, frasa benih, dan antara muka dompet.
* Bandingkan pelbagai jenis dompet dan nilai kelebihan serta kekurangannya berdasarkan keselamatan, kemudahan, privasi, dan kawalan.
* Sediakan dompet Bitcoin mudah alih dan terangkan proses pemulihan asas.
* Tunjukkan cara menerima dan menghantar transaksi bitcoin on-chain.

Gunakan prinsip "Jangan Percaya, Sahkan" untuk pilihan dompet, transaksi, dan penggunaan Bitcoin secara umum.

#### Alat & Sumber

##### Bahan Visual

* Bab 6 - Cara Menggunakan Bitcoin

##### Perpustakaan Sokongan

* Kad Rujukan Perbendaharaan Kata — Bab 6 — Istilah: dompet, kunci peribadi, alamat awam, frasa benih, jagaan, penjagaan kendiri, UTXO, yuran transaksi
* Carta Perbandingan & Lembaran Rujukan — Perbandingan jenis dompet (jagaan, mudah alih, perkakasan, kertas)
* Penjelasan Teknikal & Kupasan Mendalam — Kunci awam/peribadi, model UTXO, pengesahan transaksi
* Kupasan Mendalam Keselamatan Kunci Peribadi — Frasa benih, penjanaan kunci, kaedah sandaran, vektor serangan
* Panduan Anatomi Transaksi — Contoh langkah demi langkah bagaimana transaksi Bitcoin berfungsi
* Senarai Semak Amalan Terbaik Keselamatan — Sebelum bermula, mencipta dompet, menerima, menghantar, pencegahan phishing

#### Aktiviti

* Transaksi dalam Tindakan
* Perlumbaan Relay Lightning
* Meneroka Mempool

#### Pengajaran Dalam Talian

* Jelaskan dari awal sama ada pelajar sedang menonton demonstrasi atau menyediakan dompet sendiri.
* Gunakan tangkapan skrin yang besar dan mudah dibaca untuk setiap langkah penyediaan dompet.
* Berhenti selepas setiap langkah dan minta pelajar mengesahkan kefahaman dalam sembang sebelum meneruskan.
* Beri amaran terus sebelum bahagian frasa benih dan ingatkan pelajar supaya tidak pernah berkongsi maklumat sensitif secara dalam talian.

#### Persediaan

* Muat turun dan uji aplikasi dompet mudah alih (Blue Wallet atau Muun); sediakan tangkapan skrin untuk langkah utama penyediaan.
* Sediakan panduan penyediaan dompet (muat turun → cipta → sandaran frasa benih → terima) untuk rujukan.
* Pastikan rangkaian/WiFi berfungsi; sediakan alamat demo dan kod QR untuk ditunjukkan.

#### Prosedur

Pelajaran ini bergerak dari teori ke amalan secara langsung. Ia kini sepadan terus dengan struktur Diploma supaya pemerolehan, dompet, penyediaan, transaksi, dan pengesahan muncul di bawah tajuk utama yang sama seperti panduan pelajar. Sokongan pengajaran tambahan kekal terletak dalam bahagian-bahagian tersebut.

##### 6.0 Pengenalan, 8 minit

Mulakan dengan mengaitkan bab ini dengan bab sebelumnya:

* Jika Bitcoin adalah wang, bagaimana orang sebenarnya mendapat dan menggunakannya?
* Apa maksudnya untuk benar-benar mengawal bitcoin anda?
* Mengapa menggunakan Bitcoin berbeza daripada menggunakan aplikasi bank?

Perjelaskan bahawa bab ini mengenai penggunaan praktikal. Pelajar tidak lagi hanya belajar apa itu Bitcoin, mereka belajar bagaimana untuk berinteraksi dengannya secara langsung.

##### 6.1 Memperoleh dan Menukar Bitcoin, 12 minit

Terangkan bahawa orang boleh memperoleh bitcoin dengan pelbagai cara, termasuk:

* menerima bayaran dalam bitcoin
* melombong bitcoin
* menukar fiat kepada bitcoin secara bersemuka
* menukar fiat kepada bitcoin secara dalam talian

Kemudian fokus kepada dua laluan utama pemerolehan yang dibincangkan dalam bab ini:

* peer-to-peer, secara bersemuka
* rakan-ke-rakan, dalam talian
* pertukaran berpusat

Jelaskan kompromi dengan jelas.

Untuk P2P secara bersemuka, tekankan pertukaran secara langsung tanpa bank atau perantara, tetapi juga sebutkan risiko praktikal apabila bertemu orang untuk urus niaga tunai.

Untuk P2P dalam talian, terangkan escrow dengan istilah mudah, sebagai cara untuk mengurangkan risiko rakan niaga sambil masih membenarkan pertukaran secara langsung antara rakan.

Untuk pertukaran berpusat, jelaskan bahawa ia mudah digunakan, tetapi memerlukan pengguna mempercayai sebuah syarikat, sering berkongsi maklumat peribadi, dan meninggalkan dana di bawah kawalan pihak ketiga sehingga dikeluarkan. Ini adalah tempat yang baik untuk menekankan bahawa kemudahan sering datang dengan kompromi dalam privasi dan kedaulatan.

##### 6.2 Pengenalan kepada Dompet Bitcoin, 35 minit

**Apa Sebenarnya Dompet Bitcoin**

Perjelaskan salah faham biasa dengan segera: bitcoin tidak disimpan di dalam aplikasi dompet seperti wang tunai fizikal dalam beg.  
Bitcoin wujud di lejar yang diselenggara oleh rangkaian. Apa yang dikawal oleh pengguna ialah keupayaan untuk membelanjakannya melalui kunci peribadi.

Kemudian terangkan dua perkara yang sering dimaksudkan orang dengan "dompet":

* sistem kunci peribadi, dari mana alamat dijana
* aplikasi atau antara muka yang digunakan untuk berinteraksi dengan rangkaian

Gunakan analogi e-mel dalam bab ini jika membantu:

* alamat awam = seperti alamat e-mel yang boleh anda kongsi
* kunci peribadi = seperti kata laluan yang mesti anda lindungi

Jelaskan dengan sangat jelas di sini: sesiapa yang mengawal kunci peribadi mengawal bitcoin. Itu adalah konsep teras yang mesti difahami oleh pelajar.

**Dompet Kendiri vs Dompet Jagaan**

Ini adalah salah satu bahagian paling penting dalam bab ini.

Terangkan perbezaan dengan jelas:

* Dompet kendiri: pengguna mengawal kunci peribadi
* Dompet jagaan: pihak ketiga mengawal kunci peribadi bagi pihak pengguna

Kemudian terangkan kompromi-kompromi:

Kendiri

* kawalan penuh ke atas dana
* tiada proses kelulusan
* perlindungan daripada rampasan sewenang-wenangnya
* tanggungjawab yang lebih besar
* tiada pemulihan mudah jika frasa benih hilang

Jagaan

* pemulihan dan sokongan lebih mudah
* lebih mudah untuk pemula
* lebih terdedah kepada pembekuan akaun, penggodaman, dan kawalan pihak ketiga
* pengguna sebenarnya tidak memegang bitcoin itu

Ini adalah masa yang sesuai untuk menekankan frasa:

"Bukan kunci anda, bukan syiling anda."

Pelajar harus meninggalkan bahagian ini dengan memahami bukan sahaja slogan itu, tetapi apa maksudnya dalam amalan.

**Jenis-jenis Dompet Berbeza dan Cara Memilih Satu**

Perkenalkan jenis dompet yang dibincangkan dalam bab ini:

* dompet dalam talian
* dompet mudah alih
* dompet desktop
* dompet perkakasan
* dompet kertas

Jangan anggap mana-mana satu sebagai sempurna. Sebaliknya, terangkan bahawa setiap satu melibatkan kompromi antara:

* keselamatan
* privasi
* kemudahan
* keserasian
* yuran
* kawalan
* reputasi

Juga jelaskan bahawa kami mengesyorkan untuk memberi perhatian sama ada perisian dompet adalah sumber terbuka, kerana alat sumber terbuka boleh disemak, diaudit, dan diteruskan oleh komuniti. Ini berkait rapat dengan prinsip pengesahan dalam Bitcoin.

##### 6.3 Menyediakan Dompet Bitcoin Mudah Alih, 10 minit

Bimbing pelajar melalui proses asas yang ditunjukkan dalam bab ini:

* muat turun dompet
* cipta dompet baru
* jana dan tulis frasa pemulihan
* sahkan frasa pemulihan
* tambah keselamatan tambahan jika ada
* buka dompet dan cari fungsi terima

Buat amaran frasa benih sangat jelas:

* jika frasa benih hilang, akses kepada dana mungkin hilang
* jika orang lain mendapat frasa benih, mereka boleh mengambil dana tersebut

Jika pelajar melakukan ini secara praktikal, pendidik harus berhenti di setiap langkah dan pastikan semua orang faham apa yang mereka lakukan. Jika kelas lebih bersifat konseptual, bahagian ini boleh diterangkan sebagai panduan langkah demi langkah dan bukan dilakukan secara langsung. Pilihan pemulihan yang ditunjukkan dalam bab ini juga berguna untuk menerangkan bahawa dompet boleh dipulihkan jika frasa benih disandarkan dengan betul.

##### 6.4 Menerima dan Menghantar Transaksi, 17 minit

**Menerima dan Menghantar Transaksi On-chain**

Sekarang terangkan bagaimana transaksi on-chain berfungsi.

Untuk menerima bitcoin:

* buka dompet
* tekan terima atau deposit
* salin alamat, kongsi pautan, atau tunjukkan kod QR

Untuk menghantar bitcoin:

* buka dompet
* tampal atau imbas alamat penerima
* masukkan jumlah
* semak semua butiran dengan teliti
* siarkan transaksi
* tunggu pengesahan

Jelaskan perkara utama ini:

* transaksi memindahkan pemilikan, bukan syiling fizikal
* transaksi tidak boleh dipulangkan semula
* nod mengesahkan kesahihan
* pelombong memasukkan transaksi ke dalam blok
* yuran mempengaruhi keutamaan pengesahan
* transaksi on-chain biasanya selamat, tetapi lebih perlahan dan sering lebih mahal berbanding transaksi Lightning

Rajah aliran transaksi dalam bab ini sangat berguna di sini, kerana ia membantu pelajar membayangkan laluan dari permintaan dompet ke pengesahan rangkaian.

**Transaksi dalam Tindakan dan Latihan Berdasarkan Peranan**

Gunakan struktur latihan koperatif dari bab ini untuk mengukuhkan pemahaman. Terangkan empat peranan yang terlibat:

* penghantar
* penerima
* pelombong
* pengendali nod

Pendekatan mudah di dalam kelas ialah menetapkan peranan dan melalui satu transaksi langkah demi langkah. Ini membantu pelajar melihat bahawa transaksi Bitcoin bukanlah magik, ia adalah proses terkoordinasi yang melibatkan kelulusan, pengesahan, kemasukan ke dalam blok, dan kemas kini lejar.

Matlamat di sini bukanlah kedalaman teknikal. Ia adalah untuk membantu pelajar memahami siapa yang melakukan apa dalam transaksi dan mengapa pengesahan itu penting.

##### 6.5 Jangan Percaya, Sahkan, 8 minit

Terangkan bahawa ini terpakai kepada:

* dompet
* pertukaran
* aplikasi
* butiran transaksi
* tuntutan tentang "keuntungan mudah"
* projek yang berpura-pura seperti Bitcoin

Jelaskan dengan jelas bahawa Bitcoin memerlukan pengguna untuk berfikir secara kritikal, mengesahkan apa yang mereka gunakan, dan mengelakkan kepercayaan membuta tuli. Terangkan juga mengapa alat sumber terbuka penting dalam konteks ini: ia membolehkan pengesahan secara bebas.

###### Penutup dan Semakan Kefahaman

Akhiri dengan beberapa soalan pantas:

* Apakah perbezaan antara dompet kustodian dan dompet kendiri (self-custodial)?
* Mengapa frasa benih (seed phrase) sangat penting?
* Apa yang berlaku apabila anda menghantar transaksi di atas rantaian (on-chain)?
* Mengapa transaksi di atas rantaian lebih perlahan berbanding beberapa pembayaran Bitcoin lain?
* Apa maksud "Jangan Percaya, Sahkan" dalam amalan?

#### Nota Pendidik

Bab ini sangat praktikal, jadi utamakan kejelasan, keselamatan, dan pengulangan.

Pelajar tidak perlu menguasai setiap jenis dompet dalam satu kelas. Matlamat utama ialah:

* memahami asas dompet
* memahami penjagaan kendiri (self-custody)
* mempelajari aliran asas transaksi
* mengamalkan sikap pengesahan yang bertanggungjawab

Berhati-hati terutamanya apabila membincangkan frasa benih dan tetapan dompet. Pelajar harus faham bahawa ini bukan perkara kecil, ia adalah asas pemilikan Bitcoin.

Visual dan aktiviti yang paling berguna dalam bab ini ialah:

* perbandingan dompet kendiri vs kustodian
* jadual kompromi jenis dompet
* latihan tetapan dompet langkah demi langkah
* diagram aliran transaksi
* aktiviti transaksi berasaskan peranan

##### Contoh Amalan Terbaik

* Penting untuk pelajar benar-benar menyediakan dompet atau menonton demonstrasi yang teliti, jadikan frasa benih sebagai tumpuan utama dengan "12 perkataan ini IALAH Bitcoin anda," uji senario seperti "Apa berlaku jika anda hilang telefon?", dan berlatih mengenal pasti penipuan phishing.
* Pendidik harus menjadi pembimbing yang berpengalaman, peka keselamatan tanpa paranoia, dan jujur tentang tahap kesukaran serta pembelajaran yang diperlukan.
* Pelajar merasakan mereka telah mempelajari kemahiran sebenar yang boleh digunakan, faham bahawa frasa benih itu nyata dan penting, bukan sesuatu yang abstrak, rasa mampu memegang Bitcoin sendiri, dan faham bahawa desentralisasi memerlukan tanggungjawab peribadi.
* Hasil Pembelajaran akan dicapai jika pelajar boleh menyediakan dompet dan memahami perbezaan kunci awam dan peribadi, memahami kompromi penjagaan antara dompet kustodian dan kendiri, menerangkan bagaimana transaksi berfungsi termasuk input, output, dan yuran, menunjukkan kesedaran keselamatan termasuk perlindungan frasa benih, dan bertanya soalan kritikal tentang pemilikan dan kawalan.

##### Pengurusan Masa

Jika masa terhad, utamakan:

* Memahami asas dompet
* Memahami penjagaan kendiri
* Mempelajari aliran asas transaksi
* Mengamalkan sikap pengesahan yang bertanggungjawab

Jika ada masa lebih, beri tumpuan pada:

* Jadual perbandingan dompet kendiri vs kustodian
* Jadual kompromi jenis dompet
* Latihan tetapan dompet langkah demi langkah dengan demo langsung
* Diagram aliran transaksi dengan pengiraan yuran
* Amalan keselamatan lanjutan dan pertimbangan dompet perkakasan

##### Jika Pelajar Menghadapi Kesukaran

* Frasa benih sebagai "nyata" → "Frasa ini IALAH bitcoin anda; tiada khidmat pelanggan."
* Kunci awam vs. peribadi → Analogi emel (alamat vs. kata laluan).
* Mengapa ia sukar → "Anda mengawalnya; anda bertanggungjawab." Akui kompromi.
