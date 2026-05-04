# 8 - Bagaimana Bitcoin Berfungsi

Tempoh: 90 minit

Idea Utama: Keselamatan Bitcoin bergantung pada idea teknikal yang ringkas tetapi berkuasa seperti kunci, tandatangan, hashing, dan UTXO, yang membolehkan pemilikan dan pengesahan tanpa pihak berkuasa pusat.

#### Objektif Pembelajaran

Pada akhir pelajaran ini, pelajar sepatutnya dapat:

* Terangkan bagaimana kunci awam dan kunci peribadi membantu melindungi pemilikan dan transaksi Bitcoin.
* Huraikan apa itu tandatangan digital dan bagaimana ia membuktikan bahawa satu transaksi telah dibenarkan oleh pemilik yang sah.
* Terangkan, dalam istilah mudah, maksud kriptografi, penyulitan, dan penyahsulitan dalam konteks Bitcoin.
* Takrifkan hashing dan huraikan mengapa fungsi hash penting untuk keselamatan dan integriti data Bitcoin.
* Kenal pasti ciri asas fungsi hash, seperti output panjang tetap, sifat sehala, dan kepekaan terhadap perubahan kecil pada input.
* Terangkan model UTXO dan bagaimana bitcoin dibelanjakan, diterima, dan dipulangkan sebagai baki melalui output transaksi.
* Huraikan bagaimana nod membantu mencegah perbelanjaan berganda dengan memeriksa sama ada satu output telah dibelanjakan.

#### Alat & Sumber

##### Bahan Visual

* Bab 8 - Bagaimana Bitcoin Berfungsi

##### Perpustakaan Sokongan

* Kad Rujukan Perkataan — Bab 8 — Istilah: kriptografi, hash, UTXO, tandatangan digital, kunci peribadi/awam, pokok merkle, rantaian blok
* Perpustakaan Salah Faham — Bab 8 — Menangani: "frasa seed yang hilang boleh dipulihkan," "kunci peribadi = kata laluan," "blockchain adalah tanpa nama"
* Penerangan Teknikal & Penjelasan Mendalam — Fungsi hash, kunci awam/peribadi, model UTXO, keselamatan Proof of Work

#### Aktiviti

* Transaksi dalam Tindakan
* Meneroka Mempool

#### Pengajaran Dalam Talian

* Gunakan papan putih digital dan lukis setiap konsep secara langsung berbanding hanya bergantung pada penjelasan lisan.
* Ajar satu idea teknikal pada satu masa dan berhenti seketika untuk soalan semakan.
* Gunakan visual untuk kunci, tandatangan, hash, dan UTXO supaya pelajar boleh mengikuti strukturnya.
* Pastikan matlamatnya bersifat konseptual dan elakkan terlalu mendalam dalam matematik atau jargon.

#### Persediaan

* Sediakan dan laminasi rajah: pasangan kunci awam/peribadi, tandatangan digital, model UTXO, hashing (fungsi sehala).
* Tandakan penjelajah blockchain dan kalkulator hash SHA-256; pilih 2-3 transaksi Bitcoin sebenar untuk diterangkan langkah demi langkah.
* Sediakan nota papan putih untuk menerangkan input, output, dan bagaimana transaksi disahkan pada blockchain.

#### Prosedur

Pelajaran ini memberi pelajar pandangan pertama tentang aspek teknikal Bitcoin tanpa mengandaikan pengetahuan teknikal terdahulu. Panduan ini kini mengikuti struktur padat yang sama seperti Diploma, dengan kriptografi dikumpulkan di bawah satu tajuk dan UTXO dikumpulkan di bawah satu lagi.

##### 8.0 Pengenalan, 8 minit

Mulakan dengan menetapkan jangkaan:

* Apa yang menjadikan Bitcoin selamat jika tiada bank pusat yang mengawalnya?
* Bagaimana rangkaian boleh tahu sama ada seseorang benar-benar memiliki bitcoin yang mereka cuba hantar?
* Apa sebenarnya yang berlaku di sebalik tabir apabila seseorang membuat transaksi Bitcoin?

Jelaskan bahawa bab ini memberi tumpuan kepada asas teknikal Bitcoin, terutamanya kunci, tandatangan, hashing, dan UTXO. Juga yakinkan pelajar bahawa mereka tidak perlu menjadi jurutera untuk memahami logik asas. Bab ini sendiri menjelaskan perkara ini dengan membandingkan Bitcoin dengan internet, ramai orang menggunakannya setiap hari tanpa memahami setiap lapisan di bawahnya.

##### 8.1 Keselamatan melalui Kriptografi, 57 minit

**Bitcoin sebagai Lejar yang Disimpan di Banyak Komputer**

Mulakan dengan rangka kerja mudah bab ini tentang rangkaian Bitcoin:

* Bitcoin ialah rekod transaksi
* rekod itu disimpan di banyak komputer yang dipanggil nod
* lejar itu adalah awam dan pseudonim
* ia menunjukkan alamat dan sejarah transaksi, bukan butiran identiti peribadi

Bahagian ini membantu pelajar mengaitkan kembali dengan apa yang mereka sudah tahu dari bab-bab terdahulu. Bitcoin tidak berdasarkan akaun tersembunyi dalam bank. Ia berdasarkan lejar bersama yang boleh disahkan oleh ramai peserta. sangat membantu di sini kerana ia menunjukkan pengguna, dompet, dan rangkaian Bitcoin yang lebih luas bersambung ke lejar awam.

**Kunci Awam dan Peribadi**

Sekarang beralih ke kriptografi.

Terangkan bahawa setiap pengguna Bitcoin mempunyai:

* kunci peribadi, yang mesti dirahsiakan
* kunci awam, yang boleh dikongsi

Jelaskan tujuan mereka dalam istilah yang mudah:

* kunci peribadi membuktikan kawalan dan membenarkan perbelanjaan
* kunci awam membantu orang lain mengesahkan bahawa transaksi telah dibenarkan dengan betul

Satu perkara pengajaran yang kuat dari bab ini ialah Bitcoin menggunakan kriptografi kunci awam/peribadi, bukan model lama di mana dua orang mesti berkongsi kunci rahsia yang sama terlebih dahulu. Ini penting kerana ia membolehkan pengesahan yang selamat tanpa memaksa pengguna mendedahkan rahsia yang melindungi dana mereka.

Anda boleh menerangkannya seperti ini:

* kunci peribadi adalah seperti bukti rahsia bahawa bitcoin itu milik anda
* kunci awam adalah sebahagian daripada apa yang membolehkan rangkaian mengesahkan kebenaran anda
* sesiapa yang mengawal kunci peribadi mengawal keupayaan untuk membelanjakan bitcoin

Berhati-hati di sini supaya tidak terlalu mempersulit bahasa penyulitan. Perkara paling penting untuk pelajar ialah pemilikan dan kebenaran.

**Tandatangan Digital dan Kebenaran Transaksi**

Sekarang terangkan apa yang berlaku apabila seseorang menghantar bitcoin.

Gunakan urutan bab ini:

* seorang pengguna mencipta transaksi
* penghantar menjana tandatangan digital menggunakan kunci peribadi mereka
* transaksi disiarkan ke rangkaian
* nod mengesahkan bahawa tandatangan itu sah
* setelah disahkan dan disahkan, pemilikan dipindahkan pada lejar

Jelaskan bahawa tandatangan digital bukanlah perkara yang sama seperti menaip nama. Ia adalah bukti kriptografi bahawa pemilik sebenar telah membenarkan transaksi. Ini adalah salah satu mekanisme teras yang membolehkan Bitcoin berfungsi tanpa pihak berkuasa pusat meluluskan transaksi secara manual. Rajah sangat berguna kerana ia menunjukkan proses menandatangani dan pengesahan secara visual, serta laluan transaksi dari penghantar ke pengesahan rangkaian.

Satu ayat yang baik untuk kelas ialah:

Transaksi Bitcoin tidak diluluskan kerana bank berkata begitu. Ia diterima kerana rangkaian boleh mengesahkan bukti kriptografi yang sah.

**Hashing dan Fungsi Sehala**

Seterusnya, terangkan tentang hashing.

Mulakan dengan mudah:

* satu fungsi mengambil input dan menghasilkan output
* fungsi sehala mudah dijalankan dalam satu arah, tetapi secara realistik mustahil untuk diterbalikkan
* fungsi hash mengambil data dari sebarang saiz dan menukarkannya kepada output panjang tetap yang dipanggil hash

Gunakan salah satu analogi dalam bab ini, mana-mana yang paling jelas untuk audiens anda:

* analogi smoothie untuk fungsi sehala
* analogi cap jari untuk hash
* analogi skor muzik untuk memeriksa sama ada sesuatu telah berubah

Analogi cap jari mungkin paling jelas untuk kebanyakan kelas:

* hash adalah seperti cap jari digital untuk data
* jika input berubah walaupun sedikit, hash berubah sepenuhnya
* ini membantu komputer memeriksa integriti dan mengesan pengubahsuaian

Kemudian terangkan mengapa hashing penting dalam Bitcoin:

* transaksi di-hash
* rangkaian menggunakan hash untuk membantu mengesahkan integriti
* jika transaksi diubah, hash juga berubah
* ini membantu melindungi lejar daripada manipulasi yang tidak disedari

Visual pada halaman 7 hingga 10 sangat berguna di sini. Bab ini menunjukkan kedua-dua idea output panjang tetap dan prinsip "perubahan kecil, hasil yang sangat berbeza", yang merupakan salah satu konsep paling penting untuk pelajar fahami.

**Ciri Asas Fungsi Hash**

Terangkan secara ringkas ciri-ciri yang diketengahkan dalam bab ini, tanpa menjadikannya terlalu akademik:

* Deterministik: input yang sama memberikan output yang sama setiap kali
* Sehala / rintangan pra-imej: anda tidak boleh secara realistik membalikkan proses ini
* Sensitif kepada perubahan: walaupun perubahan kecil pada input menghasilkan output yang sangat berbeza
* Rintangan perlanggaran: sangat sukar untuk mencari dua input berbeza dengan output yang sama
* Cepat untuk disahkan: fungsi ini cekap untuk dijalankan dan diperiksa

Anda tidak perlu pelajar menghafal setiap istilah, tetapi mereka harus faham maksud umum: hashing memberikan Bitcoin cara yang boleh dipercayai untuk mengenal pasti data dan mengesan perubahan.

##### 8.2 Model UTXO, 25 minit

**Model UTXO**

Sekarang kita beralih ke bahagian utama kedua dalam bab ini: UTXO, atau Unspent Transaction Outputs.

Terangkan dengan istilah mudah menggunakan analogi tunai dalam bab ini:

* bitcoin tidak dijejak seperti baki akaun bank sahaja
* sebaliknya, ia terdiri daripada bahagian-bahagian yang boleh dibelanjakan yang dipanggil UTXO
* apabila anda membelanjakan bitcoin, anda menggunakan satu atau lebih UTXO sedia ada sebagai input
* UTXO baru kemudian dicipta sebagai output

Gunakan contoh dari bab ini:

* jika anda mempunyai UTXO 10 BTC
* dan anda menghantar 6 BTC
* UTXO baru 6 BTC diberikan kepada penerima
* UTXO baki (change) baru akan kembali kepada anda
* sebahagian kecil dibayar sebagai yuran pelombong

Ini membantu pelajar melihat bahawa Bitcoin berfungsi lebih seperti membelanjakan wang tunai dan menerima baki, berbanding hanya menolak nombor dari satu baris akaun. Rajah sangat berguna di sini kerana ia secara visual menunjukkan satu UTXO dipecahkan kepada output penerima, output baki, dan yuran.

Jelaskan dua perkara utama dengan jelas:

* baki dompet anda ialah jumlah semua UTXO anda
* apabila anda membelanjakan, UTXO lama digunakan dan UTXO baru dicipta

**Mencegah Perbelanjaan Berganda**

Akhiri kandungan dengan menerangkan salah satu implikasi terpenting model UTXO.

Jika seseorang cuba membelanjakan output yang sama dua kali, nod akan menolak cubaan kedua kerana mereka menyelenggara lejar dan boleh mengesahkan sama ada UTXO itu telah dibelanjakan. Inilah cara Bitcoin mencegah perbelanjaan berganda tanpa memerlukan syarikat pembayaran pusat untuk mengurus rekod. Contoh ini sangat berguna kerana ia menunjukkan langkah demi langkah bagaimana Alice menggabungkan UTXO, menghantar dana kepada Bob, menerima baki, dan transaksi yang disahkan mengemaskini lejar di seluruh nod.

Cara jelas untuk menyatakannya di kelas ialah:

Bitcoin mencegah perbelanjaan berganda kerana rangkaian menjejak output yang masih belum dibelanjakan dan yang telah digunakan.

###### Penutup dan Semakan Kefahaman

Akhiri dengan beberapa soalan pantas:

* Apakah perbezaan antara kunci awam dan kunci peribadi?
* Apa yang dibuktikan oleh tandatangan digital?
* Mengapa hashing berguna dalam Bitcoin?
* Apa yang berlaku jika satu transaksi diubah selepas ia di-hash?
* Apakah itu UTXO dalam istilah mudah?
* Bagaimana rangkaian menghalang seseorang daripada membelanjakan bitcoin yang sama dua kali?

#### Nota Pendidik

Bab ini mengandungi lebih banyak istilah teknikal berbanding bab-bab sebelumnya, jadi utamakan kejelasan, analogi, dan pengulangan.

Matlamatnya bukan untuk menjadikan pelajar sebagai pembangun. Matlamatnya ialah membantu mereka faham mengapa keselamatan Bitcoin berfungsi.

Perkara terpenting untuk diutamakan jika masa terhad ialah:

* kunci peribadi vs kunci awam
* tandatangan digital
* apa fungsi hashing
* UTXO sebagai bahagian bitcoin yang boleh dibelanjakan
* bagaimana perbelanjaan berganda dicegah

Visual paling berguna dalam bab ini ialah:

* rajah pengguna-dompet-rangkaian
* visual tandatangan digital
* contoh hashing dan rajah output panjang tetap di halaman 7 hingga 10
* rajah UTXO di halaman 10 hingga 12

##### Contoh Terbaik

* Penting untuk menganggap kriptografi sebagai asas, bukan misteri, gunakan visual secara meluas, elakkan matematik mendalam, kaitkan semula dengan bab-bab terdahulu, dan uji kefahaman dengan aplikasi seperti "Jika seseorang mengubah satu transaksi, apa yang rosak?"
* Pendidik harus bersabar dengan pelajar yang menghadapi kesukaran, berfikir secara visual dan melukis segala-galanya, jujur tentang apa yang pelajar tidak perlu faham, bersedia untuk berkata "Saya tidak tahu tetapi inilah cara kita boleh cari jawapannya," dan sentiasa memberi galakan.
* Pelajar faham mengapa Bitcoin tidak boleh digodam kerana ia dilindungi oleh matematik, menghargai reka bentuk sistem yang elegan, selesa dengan kerumitan walaupun tidak perlu tahu setiap perincian, yakin bertanya soalan tanpa rasa takut, dan sedar mereka telah meningkat kefahaman dalam sesuatu yang kebanyakan orang tidak tahu.
* Hasil Pembelajaran akan tercapai jika pelajar boleh menerangkan asas kriptografi seperti fungsi sehala dan tandatangan digital tanpa matematik mendalam, faham model UTXO yang menunjukkan anda memiliki syiling bukan akaun, mengenal pasti hashing sebagai asas keselamatan Bitcoin, faham anatomi transaksi termasuk tandatangan dan pengesahan, menerangkan mengapa Bitcoin tidak boleh diubah, dan bertanya soalan kritikal tentang potensi serangan atau kelemahan.

##### Pengurusan Masa

Jika masa singkat, utamakan:

* Kunci peribadi vs kunci awam
* Tandatangan digital
* Apa yang dilakukan oleh hashing
* UTXO sebagai bahagian bitcoin yang boleh dibelanjakan
* Bagaimana perbelanjaan berganda dicegah

Jika ada masa lebih, beri tumpuan pada:

* Rajah pengguna-dompet-rangkaian dan model keselamatan visual
* Visual tandatangan digital: proses kriptografi terperinci
* Pokok Merkle dan keselamatan rantaian
* Vektor serangan lanjutan dan mengapa ia gagal

##### Jika Pelajar Menghadapi Kesukaran

* Kriptografi nampak mengancam → "Anda menggunakannya setiap hari; My First Bitcoin menggunakannya dengan cara yang sama."
* Hashing sebagai konsep → Analogi cap jari; unik, tidak boleh diubah tanpa mengubah hash.
* Tandatangan digital → "Membuktikan kebenaran tanpa mendedahkan kata laluan."
