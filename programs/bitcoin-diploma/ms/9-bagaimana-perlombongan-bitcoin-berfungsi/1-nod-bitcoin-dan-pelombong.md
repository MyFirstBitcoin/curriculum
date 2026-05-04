# 9.1 Nod Bitcoin dan Pelombong

Node Bitcoin mungkin kedengaran teknikal, tetapi ia hanyalah perisian yang menyimpan salinan blockchain Bitcoin pada komputer. Blockchain ialah rekod bersama bagi semua transaksi Bitcoin.

Apabila anda menjalankan node sendiri, anda mengesahkan transaksi Bitcoin sendiri tanpa perlu mempercayai orang lain. Ini memberi anda lebih kebebasan dan membantu mengekalkan rangkaian Bitcoin yang terdesentralisasi.

Anda boleh menganggap node Bitcoin seperti pegawai trafik digital dengan beberapa tugas penting.

1. Ia menyimpan salinan blockchain, iaitu sejarah semua transaksi Bitcoin.
1. Node berhubung dengan node lain di seluruh dunia dan berkongsi maklumat. Salah satu contohnya ialah senarai transaksi baharu yang menunggu untuk disahkan, yang dipanggil mempool.
1. Node memeriksa setiap transaksi agar mematuhi peraturan Bitcoin. Jika transaksi tidak sah, node akan menolaknya.

Node juga membantu node baharu menyertai rangkaian dengan berkongsi blockchain dengan mereka. Namun, setiap node baharu tetap memeriksa semua peraturan secara bebas.

Sesiapa sahaja boleh menjalankan node dengan memasang perisian seperti Bitcoin Core dan memuat turun blockchain. Setelah ia disediakan, node akan terus menerima blok baharu kira-kira setiap 10 minit dan mengesahkannya sebelum menambahkannya ke salinan blockchainnya.

Menjalankan node membantu menjadikan rangkaian Bitcoin lebih selamat dan terdesentralisasi, kerana lebih ramai orang mengesahkan sistem secara bebas.

#### Apa Itu Node Bitcoin?

> Tujuan perlombongan bukanlah untuk mencipta bitcoin baharu; itu hanyalah sistem insentif. Perlombongan ialah mekanisme yang mendesentralisasikan keselamatan Bitcoin.  
_Andreas M. Antonopoulos_


> **Callout**
>
> Pelombong mengumpulkan transaksi yang belum disahkan, membentuk satu blok, dan menggunakan tenaga untuk mencari kunci yang menambah dan mengamankan blok tersebut.


Pelombong bersaing untuk menambah blok transaksi seterusnya ke dalam blockchain. Untuk melakukannya, mereka mesti mencari nombor khas yang menghasilkan hash blok yang sah. Anda boleh membayangkannya seperti mencari kunci yang betul di antara berbilion kemungkinan. Pelombong pertama yang menemui hash yang betul memenangi perlumbaan dan mendapat hak untuk menambah blok mereka ke dalam blockchain.

Apabila pelombong menemui hash yang sah, mereka berkongsi blok mereka dengan rangkaian. Pelombong lain dengan cepat mengesahkan bahawa penyelesaiannya betul. Jika betul, blok itu akan ditambah ke dalam blockchain, membantu memastikan lejar awam Bitcoin selamat.

Pelombong memperoleh bitcoin dengan dua cara:

* **Ganjaran blok:** Bitcoin baharu dicipta dan diberikan kepada pelombong yang berjaya menambah satu blok ke dalam blockchain.
* **Yuran transaksi:** Apabila orang menghantar bitcoin, mereka menyertakan sedikit yuran. Pelombong yang menambah blok akan menerima yuran daripada transaksi yang dimasukkan dalam blok itu.

#### Halving Bitcoin


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12.5 BTC | 6.25 BTC | 3.125 BTC |



> **Callout**
>
> Ganjaran pelombong untuk melengkapkan satu blok akan dibahagi dua setiap 210,000 blok, kira-kira setiap empat tahun.


Bitcoin mempunyai jumlah maksimum tetap sebanyak 21,000,000 bitcoin, tetapi semuanya tidak dicipta ketika Bitcoin bermula. Sebaliknya, bitcoin baharu diperkenalkan secara beransur-ansur ke dalam edaran melalui **perlombongan**.

Apabila pelombong berjaya menambah blok transaksi baharu ke rangkaian Bitcoin, mereka menerima **ganjaran blok** dalam bentuk bitcoin. Pada awal kewujudan Bitcoin, ganjaran ini ialah 50 bitcoin setiap blok. Ganjaran ini menggalakkan orang ramai menggunakan kuasa pengkomputeran dan elektrik untuk membantu mengamankan rangkaian.

Kira-kira setiap 210,000 blok (lebih kurang setiap 4 tahun), ganjaran blok akan dibahagi dua. Peristiwa ini dipanggil **halving**. Halving memperlahankan penciptaan bitcoin baharu dan membantu memastikan jumlah keseluruhan tidak akan melebihi 21 juta. Lama-kelamaan, ini menjadikan bitcoin semakin sukar didapati.


> **Definition – Bekalan dalam edaran**
>
> **Bekalan dalam edaran** merujuk kepada jumlah keseluruhan mata wang yang tersedia. Untuk Bitcoin, jumlah bekalan dalam edaran ialah bilangan syiling yang telah dilombong dan berada dalam edaran pada bila-bila masa.


![ Bitcoin Supply Schedule](https://cdn.sanity.io/images/vje9ehw2/staging/500839e9cfd856e298c941a4a11b73975b59bc3f-292x200.svg)


> **Definition – Jadual bekalan Bitcoin**
>
> **Jadual bekalan Bitcoin** ialah pelan tetap dan terbuka untuk pengeluaran bitcoin baharu ke dalam edaran, yang direka untuk mengekalkan kekurangan Bitcoin dari masa ke masa.


Selepas setiap peristiwa halving, ganjaran bitcoin yang diterima pelombong untuk menambah satu blok akan dibahagi dua. Ini mengurangkan kadar penciptaan bitcoin baharu.

Pelombong masih memperoleh yuran transaksi daripada transaksi yang dimasukkan dalam blok yang mereka lombong. Lama-kelamaan, yuran ini dijangka menjadi bahagian utama pendapatan pelombong.

Halving telah dibina dalam protokol Bitcoin dan berlaku secara automatik kira-kira setiap empat tahun. Disebabkan ini, jadual bekalan Bitcoin adalah boleh diramal dan telus.

Jadual ini menunjukkan halving yang akan datang, termasuk tarikh anggaran, nombor blok apabila ia berlaku, ganjaran blok baharu, dan peratusan jumlah bekalan bitcoin yang telah dilombong.


| Peristiwa | Tarikh | Blok | Ganjaran | Dilombong |
| --- | --- | --- | --- | --- |
| Halving ke-5 | 2028 | 1,050,000 | 1.5625 BTC | 98.44 % |
| Halving ke-6 | 2032 | 1,260,000 | 0.78125 BTC | 99.22 % |
| Halving ke-7 | 2036 | 1,470,000 | 0.390625 BTC | 99.61 % |


Semakin banyak bitcoin dilombong, bekalan yang beredar akan terus meningkat sehingga had maksimum 21,000,000 bitcoin tercapai, yang dijangka sekitar tahun 2140. Oleh kerana semakin sedikit bitcoin baharu dicipta dari masa ke masa, jika permintaan meningkat, harga Bitcoin boleh naik. Ini juga menggalakkan pelombong untuk terus mengamankan rangkaian dengan menyumbangkan kuasa pengiraan mereka.

#### Apakah itu hash blok yang sah dalam Bitcoin?

Dalam Bitcoin, pelombong bersaing untuk mencari kod khas yang dipanggil **hash blok**. Kod ini mengenal pasti satu blok transaksi dan membolehkan ia ditambah ke dalam rantaian blok.

Setiap blok mengandungi maklumat tentang transaksi terkini dan juga termasuk hash blok sebelumnya. Ini menghubungkan setiap blok bersama, membentuk satu rantaian dari blok pertama (Genesis Block) hingga ke blok yang paling terkini.

Hash berfungsi seperti **cap jari digital** untuk data dalam blok tersebut. Jika sebarang maklumat dalam blok diubah, cap jari itu juga akan berubah. Ini memudahkan sesiapa sahaja untuk mengesahkan bahawa sejarah transaksi blockchain tidak diubah dan membantu memastikan rangkaian selamat.


> **Callout**
>
> Satoshi Nakamoto, pencipta Bitcoin, telah melombong Genesis Block, yang membuka sejumlah 50 bitcoin.


#### Perlumbaan untuk Melombong Blok

Pelombong bersaing untuk mencari hash blok yang sah. Pelombong pertama yang menemuinya boleh menambah blok baharu ke dalam blockchain dan menerima ganjaran bitcoin.

Untuk menjadi sah, hash blok mesti lebih rendah daripada nombor yang ditetapkan oleh rangkaian yang dipanggil sasaran kesukaran. Oleh kerana hash adalah rawak, pelombong mesti terus mencuba input yang berbeza sehingga mereka menemui satu yang berfungsi.

Jika terlalu ramai pelombong bersaing, blok akan ditemui terlalu cepat. Jika terlalu sedikit pelombong yang mengambil bahagian, blok akan mengambil masa terlalu lama untuk ditemui. Untuk memastikan sistem berjalan lancar, Bitcoin secara automatik melaraskan tahap kesukaran setiap 2,016 blok (kira-kira setiap dua minggu).

Pelarasan ini memastikan bahawa, secara purata, satu blok baharu ditambah ke dalam blockchain kira-kira setiap 10 minit.


> **Definition – Definisi tahap kesukaran**
>
> Tahap **kesukaran** dalam perlombongan Bitcoin mengukur betapa sukarnya untuk mencari hash blok yang sah. Rangkaian melaraskan kesukaran ini setiap 2,016 blok (kira-kira setiap dua minggu) supaya blok baharu ditambah ke dalam blockchain kira-kira setiap 10 minit. Semakin tinggi kesukaran, semakin sukar untuk pelombong mencari blok yang sah.


Dengan menemui hash blok yang sah, seorang pelombong membuktikan mereka telah melakukan kerja yang diperlukan untuk menambah blok baharu ke dalam blockchain. Proses ini dipanggil **Bukti Kerja** (PoW). Ia adalah mekanisme keselamatan yang membolehkan Bitcoin mengesahkan transaksi dan menambah blok baharu ke dalam blockchain. Pelombong yang menemui hash sah terlebih dahulu akan mendapat ganjaran dalam bentuk bitcoin, yang termasuk ganjaran blok dan yuran transaksi daripada transaksi yang dimasukkan dalam blok tersebut.

Bukti Kerja (PoW) membantu memastikan Bitcoin selamat dengan menjadikannya sangat mahal untuk sesiapa sahaja cuba menipu atau mengambil alih rangkaian. Sebaliknya, adalah jauh lebih menguntungkan untuk mematuhi peraturan.

Pelombong memainkan empat peranan utama:

1. **Mengumpul transaksi**: Pelombong memilih transaksi yang telah dihantar ke rangkaian dan meletakkannya ke dalam blok calon.
1. **Melakukan Bukti Kerja**: Pelombong bersaing untuk menyelesaikan teka-teki matematik yang sukar dengan mencari hash blok yang sah.
1. **Siar blok**: Pelombong pertama yang menemui penyelesaian yang sah akan berkongsi blok baru dengan rangkaian.
1. **Dapatkan ganjaran**: Jika blok itu sah, ia akan ditambah ke dalam rantaian blok dan pelombong menerima bitcoin yang baru dicipta serta yuran transaksi.

Ramai pelombong di seluruh dunia cuba mencipta blok seterusnya pada masa yang sama. Apabila seorang pelombong menemui penyelesaian yang sah, rangkaian akan memeriksa blok tersebut. Jika semuanya betul, ia akan ditambah ke dalam rantaian blok. Blok-blok lain yang bersaing akan dibuang. Proses ini memastikan rangkaian sentiasa bersetuju dan mengelakkan perbelanjaan berganda.

* Pelombong ialah komputer yang membantu menyelenggara dan mengemas kini lejar Bitcoin.
* Mereka mengumpul transaksi dan mengumpulkannya ke dalam satu blok. Kemudian mereka menjalankan data blok tersebut melalui algoritma hash untuk mencipta kod unik yang dipanggil hash.
* Pelombong mengulangi proses ini berkali-kali, mencari hash yang memenuhi peraturan Bitcoin. Pelombong pertama yang menemui hash yang sah akan mendapat bitcoin baru sebagai ganjaran, dan blok mereka akan ditambah ke dalam rantaian blok.
* Hash setiap blok juga menghubungkannya dengan blok sebelumnya. Jika seseorang cuba mengubah transaksi lepas, hash tidak akan sepadan lagi, dan rangkaian akan menolak rantaian yang diubah. Inilah yang memastikan lejar Bitcoin selamat.
