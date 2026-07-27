# 6.2 Pengantar Dompet

Tidak seperti uang fisik, bitcoin sebenarnya tidak disimpan di dalam dompet Bitcoin. Sebaliknya, bitcoin berada di buku besar terdistribusi yang terus diverifikasi dan diamankan oleh jaringan Bitcoin. Jadi, bagaimana Anda bisa memiliki bitcoin?

Anda memiliki kepemilikan atas bitcoin Anda hanya jika Anda mengendalikan kunci privat yang memungkinkan Anda menandatangani transaksi dan mentransfer kepemilikan bitcoin Anda kepada orang lain. Inilah yang disebut dengan mengirim bitcoin.

Mari kita lihat dua konsep yang kita maksud saat menggunakan istilah **dompet**:

* Sebuah kunci privat utama, seperti kata sandi, dari mana kunci publik Anda, seperti alamat email, dihasilkan. Anda dapat membagikan alamat publik Anda kepada orang lain untuk menerima dan mengirim bitcoin, tetapi Anda tidak boleh membagikan kunci privat Anda!
* Antarmuka seluler atau desktop yang digunakan untuk berinteraksi dengan jaringan Bitcoin, memeriksa saldo bitcoin Anda, mengirim dan menerima transaksi, serta menyiarkannya ke jaringan. Berbagai jenis dompet, beserta manfaat dan komprominya, akan dijelaskan di bagian berikutnya.

#### Dompet Swakustodi vs Kustodian

Sebelum membahas lebih detail tentang berbagai jenis dompet Bitcoin dan karakteristiknya, mari kita buat perbedaan penting antara dompet swakustodi dan kustodian. Setiap jenis memiliki manfaat, risiko, dan tingkat kendali atas bitcoin yang berbeda. Swakustodi berarti pengguna memegang kunci privat dan benar-benar mengendalikan bitcoinnya; pada dompet kustodian, pihak ketiga memegang bitcoin untuk pengguna.


| Jenis | Kendali | Manfaat | Risiko |
| --- | --- | --- | --- |
| Swakustodi | Pengguna | Kendali penuh atas dana dan transaksi, tidak ada proses persetujuan atau pembekuan akun, tidak ada kendali perusahaan atau pemerintah, terlindungi dari penyitaan. | Tidak ada pemulihan jika frasa pemulihan hilang, tanggung jawab penuh ada pada pengguna. |
| Kustodian | Penyedia pihak ketiga | Pemulihan mudah jika akses hilang, dukungan pelanggan lebih mudah. | Dana terhubung ke Internet, lebih rentan terhadap peretasan. Kustodian dapat membekukan akun. |


Dalam dompet swakustodi (juga disebut dompet non-kustodian), Anda adalah satu-satunya yang memiliki kunci ke dompet dan Anda memiliki kendali penuh atas apa yang masuk dan keluar. Sebaliknya, pada dompet kustodian, orang lain memegang kunci privat, sehingga mereka memiliki akses penuh untuk memindahkan bitcoin apa pun yang dikendalikan penyedia tersebut atas nama Anda.

* Swakustodi seperti menjadi bank bagi diri sendiri. Transaksi tidak tunduk pada pengawasan dan kendali
* Swakustodi memastikan pihak ketiga tidak dapat menyita bitcoin Anda.
* Swakustodi memberikan ketenangan pikiran di masa-masa ketidakpastian, karena Anda tahu bitcoin Anda aman.

Penting untuk memilih jenis dompet yang tepat sesuai kebutuhan masing-masing individu. Terkadang, orang sulit membedakan apakah mereka memasang dompet swakustodi atau kustodian. Tabel ini menunjukkan perbedaan dalam proses instalasi.


| Jenis | Langkah 1: Pilih | Langkah 2: Instal | Langkah 3: Buat | Langkah 4: Amankan |
| --- | --- | --- | --- | --- |
| Swakustodi | Pilih dompet swakustodi | Ikuti petunjuk dompet | Buat frasa pemulihan | Simpan frasa pemulihan di tempat yang aman |
| Kustodian | Pilih dompet kustodian | Ikuti petunjuk dompet | Buat akun | T/A |


“**Bukan kunci Anda, bukan koin Anda**” adalah ungkapan populer di kalangan pemegang bitcoin. Ini merujuk pada gagasan bahwa jika Anda tidak memiliki kendali langsung atas kunci privat yang terkait dengan dompet Bitcoin Anda, Anda tidak benar-benar memiliki koin tersebut.

Siapa pun yang mengakses kunci privat Anda memiliki kepemilikan atas bitcoin Anda. Inilah sebabnya mengapa sangat penting untuk melindunginya dengan menjauhkannya dari mata-mata! Kita akan melihat beberapa cara untuk melakukannya nanti di buku ini.

Untuk bagian selanjutnya, kita hanya akan membahas dompet swakustodi, di mana pengguna memiliki kunci mereka sendiri dan memiliki kendali penuh atas bitcoinnya.

Jangan khawatir jika ini tampak rumit atau Anda belum memahami semuanya — ini adalah sebuah perjalanan, dan Anda akan lebih mengerti seiring Anda mulai menggunakan Bitcoin!

#### Berbagai Jenis Dompet Bitcoin

Di mana kunci privat Anda dibuat dan disimpan menentukan bagaimana kita mendeskripsikan dompet Bitcoin. Jika kunci ada di ponsel Anda, itu adalah **dompet seluler**. Jika disimpan dengan aman di perangkat khusus, itu adalah **hardware wallet**.


| Tipe | Deskripsi | Keuntungan | Kekurangan | Contoh Pengguna |
| --- | --- | --- | --- | --- |
| Dompet Online | Diakses melalui peramban web | Dapat diakses dari perangkat apa pun yang terhubung ke internet | Kurang aman karena dapat diretas atau dikompromikan | Perlu sering mengakses dompetnya dan tidak menyimpan banyak dana |
| Dompet Seluler | Diinstal di perangkat seluler | Mudah digunakan | Dapat hilang jika perangkat dicuri atau diretas | Perlu melakukan transaksi saat bepergian dan tidak menyimpan banyak dana |
| Dompet Desktop | Diinstal di komputer desktop | Praktis dan dapat diakses dari mana saja | Dapat diretas jika komputer terinfeksi malware | Ingin menyimpan bitcoin dalam jumlah besar dan nyaman menggunakan komputer desktop |
| Hardware Wallet | Perangkat fisik yang menyimpan bitcoin secara offline | Lebih aman daripada dompet online dan dapat digunakan secara offline | Dana bisa tidak dapat dipulihkan | Ingin menyimpan bitcoin dalam jumlah besar dan bersedia membayar demi keamanan tambahan |


Karena kunci dapat dipindahkan dari satu perangkat ke perangkat lain, “status” dompet Bitcoin Anda tidak tetap. Misalnya, jika saya membuat kunci dompet di komputer dan kemudian memindahkannya ke ponsel, maka “dompet desktop” menjadi “dompet seluler.”

Saat menyimpan bitcoin Anda, bukan hanya soal siapa yang mengendalikan kunci — ada banyak risiko lain yang perlu dipertimbangkan. Itulah mengapa penting untuk menemukan solusi penyimpanan yang aman sekaligus nyaman. Ketika Anda menganalisis kelebihan dan kekurangan berbagai jenis dompet, Anda akan belajar bahwa tidak ada dompet yang ideal untuk memenuhi semua kebutuhan.

##### Hal yang perlu dipertimbangkan saat memilih dompet

* **Keamanan**: Pastikan dompet memiliki langkah-langkah keamanan yang kuat.
* **Privasi**: Pertimbangkan apakah dompet memerlukan informasi pribadi.
* **Kemudahan penggunaan**: Pilih dompet yang mudah digunakan dan dinavigasi.
* **Kompatibilitas**: Pastikan dompet kompatibel dengan perangkat Anda.
* **Biaya**: Bandingkan biaya yang dikenakan oleh berbagai dompet.
* **Reputasi**: Periksa reputasi pengembang untuk memastikan mereka dapat dipercaya.
* **Kontrol**: Beberapa dompet memberi Anda lebih banyak kontrol atas kunci privat Anda.

##### Open Source vs Closed Source

Faktor penting lain yang perlu diingat saat memilih dompet Bitcoin adalah mengetahui apakah aplikasi atau perangkat lunak tersebut open-source. Ini penting karena proyek open-source memungkinkan komunitas untuk meninjau kode dan melanjutkan proyek jika tim pengembang berhenti mengerjakannya. Sama seperti kode Bitcoin yang sepenuhnya terbuka untuk semua orang tinjau, gunakan, dan modifikasi, begitu juga seharusnya kode dompet yang Anda gunakan untuk mengelola bitcoin Anda.

#### Aktivitas: Diskusi dan evaluasi dompet Bitcoin


https://bitcoin.org/en/choose-your-wallet

_QR Code: Choose your wallet_


Kunjungi situs web berikut: [https://bitcoin.org/en/choose-your-wallet](https://bitcoin.org/en/choose-your-wallet)

Gunakan pengetahuan baru Anda tentang dompet Bitcoin untuk memilih dompet yang paling sesuai dengan kebutuhan Anda berdasarkan kriteria yang telah kita bahas hari ini.
