# 9 - Bagaimana Perlombongan Bitcoin Berfungsi

Tempoh: 90 minit

Idea Utama: Perlombongan Bitcoin dan pengesahan nod bekerjasama untuk melindungi rangkaian, mengesahkan transaksi, dan menguatkuasakan peraturan sistem melalui Bukti Kerja (Proof of Work).

#### Objektif Pembelajaran

Pada akhir pelajaran ini, pelajar sepatutnya dapat:

* Terangkan perbezaan antara peranan nod Bitcoin dan peranan pelombong Bitcoin.
* Huraikan bagaimana nod mengesahkan transaksi, berkongsi maklumat, dan membantu menguatkuasakan peraturan Bitcoin.
* Terangkan apa yang dilakukan oleh pelombong, termasuk memilih transaksi, membina blok calon, dan bersaing untuk mencari hash blok yang sah.
* Takrifkan mempool dan terangkan mengapa ia berfungsi seperti bilik menunggu untuk transaksi yang belum disahkan.
* Huraikan bagaimana yuran transaksi mempengaruhi pemilihan pelombong dan kelajuan pengesahan.
* Terangkan Bukti Kerja (Proof of Work) sebagai mekanisme yang melindungi Bitcoin dengan menjadikan serangan mahal.
* Huraikan bagaimana pelarasan kesukaran membantu mengekalkan masa blok purata sekitar 10 minit.
* Jelaskan kitaran penuh transaksi Bitcoin, dari penciptaan dan penandatanganan hingga pengesahan dalam blok.

#### Alat & Sumber

##### Bahan Visual

* Bab 9 - Bagaimana Perlombongan Bitcoin Berfungsi?

##### Perpustakaan Sokongan

* Kad Rujukan Perkataan — Bab 9 — Istilah: perlombongan, Bukti Kerja, teka-teki hash, pelarasan kesukaran, ganjaran blok, mempool, serangan 51%
* Perpustakaan Salah Faham — Bab 9 — Menjawab: "pelombong mencipta Bitcoin dari tiada apa-apa," "pelombong mengawal Bitcoin," "lebih banyak perlombongan = kurang selamat"
* Carta Perbandingan & Lembaran Rujukan — Ekonomi perlombongan: hasil, kos, penjajaran insentif; pelarasan kesukaran
* Penjelasan Teknikal & Kupasan Mendalam — Keselamatan Bukti Kerja; mengapa serangan mahal; ambang 51%

#### Aktiviti

* Meneroka Mempool
* Transaksi dalam Tindakan

#### Pengajaran Dalam Talian

* Gunakan satu rajah aliran transaksi yang jelas dari penandatanganan dompet hingga pengesahan.
* Pastikan nod dan pelombong dipaparkan secara visual berasingan di skrin sepanjang pelajaran.
* Gunakan mempool.space atau tangkapan layar daripadanya untuk menunjukkan transaksi yang belum disahkan dan tekanan yuran.
* Berhenti seketika selepas setiap peringkat proses perlombongan dan tanya satu soalan kefahaman ringkas.

#### Persediaan

* Sediakan rajah proses perlombongan (mempool → pemilihan transaksi → penciptaan blok → pelarasan kesukaran) untuk dipaparkan.
* Tandakan halaman mempool.space atau blockchain.com bahagian perlombongan; sediakan tangkapan layar statistik perlombongan semasa dan pelarasan kesukaran.
* Cipta penjelasan visual tentang Bukti Kerja sebagai mekanisme keselamatan; tunjukkan pelarasan kesukaran sepanjang 3-6 bulan lepas.

#### Prosedur

Pelajaran ini melihat dengan lebih dekat bagaimana transaksi Bitcoin bergerak melalui rangkaian dan menjadi sebahagian daripada blockchain. Ia kini mengikuti struktur Diploma secara langsung supaya bahagian utama sejajar dengan panduan pelajar sambil masih mengekalkan penjelasan penuh untuk pendidik dalam setiap bahagian.

##### 9.0 Pengenalan, 8 minit

Mulakan dengan menghubungkan bab ini dengan bab sebelumnya:

* Jika seorang pengguna menandatangani transaksi dengan kunci peribadi, apa yang berlaku seterusnya?
* Siapa yang memeriksa sama ada transaksi itu sah?
* Bagaimana ia dimasukkan ke dalam blockchain?
* Mengapa Bitcoin memerlukan kedua-dua nod dan pelombong?

Perjelaskan bahawa bab ini menerangkan bagaimana rangkaian memproses transaksi dalam amalan dan bagaimana perlombongan melindungi sistem tanpa pihak berkuasa pusat.

##### 9.1 Nod dan Pelombong Bitcoin, 47 minit

**Nod dan Pelombong, Peranan Berbeza**

Mulakan dengan memisahkan kedua-dua peranan dengan jelas.

Nod Bitcoin:

* menyimpan salinan blockchain
* mengesahkan sama ada transaksi mengikut peraturan
* berkongsi maklumat dengan nod lain
* membantu dompet dan perisian lain mengakses data blockchain
* boleh menolak transaksi tidak sah atau blok tidak sah

Bab ini menerangkan nod sebagai penjaga pintu pengesahan, dan memperluaskan dengan analogi "pegawai trafik digital". Ini membantu kerana ia menunjukkan nod sebagai pemeriksa dan penyelaras, bukan penguasa. Rajah juga menguatkan bahawa banyak nod menyimpan salinan lejar di seluruh dunia.

Pelombong Bitcoin:

* mengumpul transaksi yang sah
* menyusun blok calon
* bersaing untuk mencari hash blok yang sah
* menyiarkan blok yang sah apabila mereka menang
* menerima ganjaran blok dan yuran transaksi

Satu perkara penting dari bab ini ialah tujuan perlombongan bukan sekadar untuk mencipta bitcoin baharu, tetapi untuk mendesentralisasikan keselamatan Bitcoin. Bitcoin baharu adalah insentif, manakala proses perlombongan itu sendiri adalah mekanisme keselamatan.

**Apa Sebenarnya Nod Lakukan**

Perluaskan bahagian nod dengan senarai fungsi nod dari bab ini:

* Penjaga pintu pengesahan: mereka memeriksa bahawa transaksi dan blok mematuhi peraturan
* Hab komunikasi: mereka berhubung antara satu sama lain dan berkongsi data transaksi
* Pemeriksa kualiti: mereka menolak maklumat yang tidak sah
* Pemberi maklumat blockchain: mereka menyediakan data kepada perisian lain seperti dompet
* Penyambut nod baharu: mereka membantu nod baharu mendapatkan blockchain, walaupun setiap nod baharu tetap mengesahkan data secara bebas

Ini adalah masa yang baik untuk menekankan bahawa menjalankan nod memberi pengguna lebih kebebasan. Daripada bergantung sepenuhnya kepada perkhidmatan luar untuk memberitahu mereka keadaan rangkaian, mereka boleh mengesahkannya sendiri. Bab ini menjelaskan perkara ini dengan jelas, termasuk menyebut Bitcoin Core sebagai salah satu pelaksanaan yang boleh dijalankan oleh pengguna.

**Apa Sebenarnya Pelombong Lakukan**

Sekarang terangkan perlombongan dengan lebih teliti.

Pelombong:

* mengumpul transaksi yang telah disahkan tetapi belum disahkan dalam blok
* mengumpulkannya ke dalam blok calon
* berulang kali menghash data blok sambil mencari hash blok yang sah
* menyiarkan blok yang menang ke rangkaian
* mendapat ganjaran jika blok diterima

Gunakan analogi "timbunan besar kunci" dari bab ini jika ia membantu. Ia memberi pelajar gambaran konkrit tentang perlumbaan perlombongan. Idea utama bukanlah pelombong menyelesaikan masalah matematik yang berguna dalam erti kata biasa, tetapi mereka membuktikan mereka telah menggunakan tenaga dan pengiraan dunia sebenar untuk melindungi sistem.

Ini juga tempat yang sesuai untuk menerangkan ganjaran pelombong:

* ganjaran blok: bitcoin yang baru diterbitkan
* yuran transaksi: yuran yang dilampirkan pada transaksi yang pengguna mahu disahkan

Perjelaskan bahawa pelombong biasanya mengutamakan transaksi dengan yuran lebih tinggi, kerana itu meningkatkan ganjaran mereka. Bab ini juga menerangkan halving di sini, jadi anda boleh menyatakan secara ringkas bahawa ganjaran blok berkurang setiap 210,000 blok, kira-kira setiap empat tahun, mengikut jadual bekalan awam Bitcoin. Muka surat 5 dan 6 mengandungi jadual bekalan dan jadual halving yang akan datang, yang boleh membantu menguatkan pengeluaran Bitcoin yang boleh diramal.

**Hash Blok Sah, Bukti Kerja, dan Pelarasan Kesukaran**

Bahagian ini adalah inti bab ini.

Terangkan bahawa pelombong sedang mencari hash blok yang sah, iaitu hash blok yang memenuhi sasaran rangkaian. Bab ini menerangkan ini sebagai mencari nombor yang lebih rendah daripada sasaran yang ditetapkan oleh rangkaian.

Kemudian terangkan Bukti Kerja dengan jelas:

* pelombong mesti melakukan kerja pengiraan berulang kali
* yang pertama menemui hash yang sah membuktikan mereka telah melakukan kerja itu
* ini menjadikan ia mahal untuk menulis semula atau menyerang lejar
* nod kemudian mengesahkan blok sebelum menerimanya

Satu ayat yang kuat untuk pengajaran ialah:

Bukti Kerja melindungi Bitcoin dengan menjadikan penipuan mahal dan pengesahan mudah.

Terangkan juga pelarasan kesukaran:

* rangkaian melaraskan kesukaran perlombongan setiap 2,016 blok
* ini berlaku kira-kira setiap dua minggu
* matlamatnya adalah untuk mengekalkan masa blok purata hampir 10 minit
* jika lebih banyak kuasa hash menyertai rangkaian, kesukaran meningkat
* jika kurang kuasa hash, kesukaran menurun

Muka surat 7 dan 8 menerangkan proses ini dan menunjukkan bagaimana sasaran yang lebih sukar memerlukan lebih banyak kerja. Ini membantu pelajar memahami bahawa masa Bitcoin tidak dikawal oleh pihak berkuasa pusat tetapi oleh peraturan protokol yang bertindak balas secara automatik kepada keadaan rangkaian.

##### 9.2 Apakah Itu Mempool?, 15 minit

Sekarang beralih ke mempool.

Terangkan bahawa mempool ialah bilik menunggu untuk transaksi yang sah tetapi belum disahkan. Apabila pengguna menyiarkan transaksi, nod terlebih dahulu mengesahkannya. Jika ia sah, mereka menambahkannya ke dalam mempool mereka dan berkongsi dengan nod lain. Kemudian pelombong boleh memilih daripada transaksi yang menunggu itu semasa membina blok. Muka surat 10 dan 11 menerangkan proses ini secara langsung.

Perkara penting untuk ditekankan:

* mempool bukanlah blockchain
* transaksi di situ masih belum disahkan
* setiap nod menyimpan mempool mereka sendiri
* tiada satu mempool sejagat yang tunggal
* transaksi dengan yuran lebih tinggi lebih berkemungkinan dipilih lebih awal

Bab ini juga menerangkan sebab-sebab biasa mengapa sesuatu transaksi mungkin kekal tidak disahkan untuk tempoh yang lama:

* yuran rendah
* kesesakan rangkaian
* cubaan perbelanjaan berganda
* data tidak betul atau tidak lengkap
* transaksi tidak sah

Jika sesuai, sebutkan aktiviti dengan mempool.space sebagai cara praktikal untuk memvisualisasikan transaksi yang belum disahkan dan kadar yuran. Juga jelaskan bahawa mempool.space hanyalah satu penjelajah, bukan mempool itu sendiri.

##### 9.3 Bagaimana Transaksi Bitcoin Berfungsi, 20 minit

Sekarang satukan semuanya menggunakan urutan langkah demi langkah dalam bab ini.

Versi bilik darjah yang jelas ialah:



1. Penghantar memilih UTXO dan mencipta transaksi
1. Penghantar menambah alamat penerima dan yuran
1. Penghantar menandatangani transaksi dengan kunci peribadi mereka
1. Transaksi disiarkan ke rangkaian
1. Nod mengesahkan dan menambahkannya ke mempool mereka
1. Pelombong memilihnya untuk blok calon
1. Pelombong bersaing melalui Proof of Work
1. Seorang pelombong menemui hash blok yang sah dan menyiarkan blok tersebut
1. Nod mengesahkan blok dan menambahkannya ke blockchain
1. Transaksi menerima pengesahan apabila lebih banyak blok ditambah
1. Jelaskan perkara terakhir dengan jelas:
1. sebaik sahaja transaksi dimasukkan dalam blok yang sah, ia disahkan
1. input yang telah digunakan tidak boleh digunakan lagi
1. penerima kini mengawal UTXO baru yang dicipta oleh transaksi itu

Rajah ringkasan sangat berguna di sini kerana ia menghubungkan secara visual keseluruhan proses dari penandatanganan dompet ke kemasukan pelombong ke pengesahan nod dan pengedaran blok.

###### Penutup dan Semakan Kefahaman

Akhiri dengan beberapa soalan pantas:

* Apakah perbezaan antara nod dan pelombong?
* Apakah itu mempool?
* Mengapa sesetengah transaksi disahkan lebih cepat daripada yang lain?
* Apa yang dibuktikan oleh Proof of Work?
* Mengapa Bitcoin melaras kesukaran perlombongan?
* Apakah langkah utama antara menghantar transaksi dan menerima pengesahan?

#### Nota Pendidik

Pastikan benang utama pengajaran jelas: nod mengesahkan, pelombong bersaing, Proof of Work mengamankan, dan mempool menyimpan transaksi sah sehingga ia disahkan.

Bab ini boleh terasa teknikal, jadi gunakan analogi dan rajah dengan kerap.

Elakkan menggambarkan perlombongan seperti "mencipta bitcoin daripada tiada." Jelaskan dengan tepat bahawa ganjaran adalah insentif, manakala proses perlombongan mengamankan rangkaian.

Perkara paling penting untuk diutamakan jika masa singkat ialah:



1. Peranan nod vs pelombong
1. Mempool sebagai ruang menunggu
1. Proof of Work
1. Pelarasan kesukaran
1. Aliran transaksi dari penandatanganan ke pengesahan

##### Contoh Pengajaran Yang Baik

* Penting untuk segera menjelaskan bahawa Pelombong ≠ Nod, tunjukkan perlombongan sebagai aktiviti ekonomi dengan kos perkakasan sebenar dan perbelanjaan elektrik, gunakan pelarasan kesukaran dan Proof of Work untuk menerangkan mekanisme keselamatan, dan uji kefahaman dengan senario tentang perubahan rangkaian.
* Pendidik harus menggunakan nombor sebenar untuk mengukuhkan perbincangan, sentiasa jelas dan berulang kali menekankan perbezaan antara Pelombong dan Nod, bersikap realistik tentang kebimbangan pemusatan dengan kolam perlombongan, dan menghormati tahap kecanggihan sebenar yang terlibat.
* Pelajar memahami bahawa perlombongan melibatkan orang bijak yang melakukan kerja kompleks kerana mereka memperoleh Bitcoin, menyedari bahawa insentif mendorong tingkah laku jujur kerana keuntungan pelombong bergantung pada kejayaan Bitcoin, melihat sistem mengawal sendiri melalui pelarasan kesukaran automatik, faham bahawa perlombongan adalah perniagaan sebenar bukan amal, dan menghargai bahawa keselamatan Bitcoin memerlukan elektrik dan wang sebenar.
* Hasil Pembelajaran akan tercapai jika pelajar dapat membezakan pelombong yang mencipta blok daripada nod yang mengesahkannya, memahami Proof of Work sebagai mekanisme keselamatan yang menjadikan serangan sangat mahal, mengenali pelarasan kesukaran mengekalkan masa blok sekitar 10 minit, memahami insentif pelombong berkaitan ganjaran blok dan yuran, menerangkan mengapa serangan 51% gagal, dan melihat perlombongan sebagai aktiviti ekonomi dengan kos dan manfaat sebenar.

##### Pengurusan Masa

Jika masa terhad, utamakan:

* Peranan nod vs pelombong (perbezaan kritikal)
* Mempool sebagai bilik menunggu
* Mekanisme Proof of Work
* Pelarasan kesukaran (sistem mengawal sendiri)
* Aliran transaksi dari penandatanganan hingga pengesahan

Jika ada masa lebih, beri tumpuan pada:

* Ekonomi perlombongan dan spesifikasi perkakasan
* Dinamik kolam perlombongan dan kebimbangan pemusatan
* Senario serangan 51% dan mengapa ia gagal secara matematik
* Keselamatan jangka panjang melalui penjajaran insentif

##### Jika Pelajar Menghadapi Kesukaran

* Pelombong vs. nod (kekeliruan) → "Nod mengesahkan, pelombong mencadangkan; pengadil vs pemain."
* Proof of Work membazir → "Keselamatan mahal menghalang serangan; menjadikannya tidak berbaloi."
* Pelarasan kesukaran → "Lebih ramai pelombong = blok lebih cepat = kesukaran meningkat; sistem bernafas."
