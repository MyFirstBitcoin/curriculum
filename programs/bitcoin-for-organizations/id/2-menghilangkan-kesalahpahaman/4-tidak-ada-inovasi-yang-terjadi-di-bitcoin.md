# 2.4 Tidak ada inovasi yang terjadi di Bitcoin

> Penciptaan seribu hutan ada dalam satu biji pohon ek.   
_Ralph Waldo Emerson_

Para kritikus sering mencoba mengklaim bahwa Bitcoin adalah teknologi yang 'usang' atau 'mati' karena tidak sering mengubah protokol lapisan dasarnya seperti blockchain pesaing. Klaim ini mengabaikan baik alasan mengapa perubahan pada Bitcoin diadopsi secara perlahan maupun banyaknya inovasi yang terjadi untuk meningkatkan skala jaringan di lapisan yang lebih tinggi, seperti Lightning Network. Klaim ini juga mengabaikan bahwa banyak teknologi kita yang paling fleksibel dan tahan lama juga tidak berkembang dengan cepat di lapisan dasarnya.

Sebagai contoh, tidak ada inovasi yang terjadi pada Transmission Control Protocol (TCP), yang menjadi dasar internet. TCP pertama kali dibuat pada tahun 1974. Terakhir kali TCP diperbarui adalah pada tahun 1982. TCP melakukan apa yang perlu dilakukan. Memang tidak sempurna, dan ada perdebatan apakah kita perlu meningkatkan IPv4 untuk mendukung perkembangan internet di masa depan. Namun, mengatakan bahwa tidak ada inovasi di internet sejak 1982 adalah klaim yang luar biasa. Semua inovasi ini terjadi 'di atas' TCP, bukan 'di dalamnya'.

Sebagian besar inovasi yang terjadi bukanlah 'di dalam' Bitcoin, melainkan 'di atas' Bitcoin. Suatu hari nanti kemungkinan tidak akan ada lagi inovasi 'di dalam' Bitcoin, dan itu seharusnya menjadi tujuan, bukan kritik, karena hal itu mencerminkan betapa fundamentalnya Bitcoin dalam mendukung ekonomi global dengan menyediakan fondasi bagi uang yang sehat, global, netral, dan tanpa izin. Uang yang sehat baik dalam arti ekonomi, yaitu memiliki pasokan tetap dan buku besar yang tidak dapat diubah, maupun sehat secara teknologi karena tidak berubah dan telah berjalan selama bertahun-tahun tanpa gangguan. Bitcoin telah mencapai waktu aktif 100% selama 10 tahun terakhir.

Namun, akan menjadi perhatian jika tidak ada inovasi yang terjadi 'di atas' Bitcoin. Mari kita lihat hal itu selama 10 tahun terakhir:



#### 'Di dalam' Bitcoin

Segregated Witness (SegWit) diimplementasikan pada tahun 2017 untuk melindungi dari malleabilitas transaksi dan meningkatkan kapasitas blok. SegWit juga merupakan prasyarat penting agar lightning dan beberapa side chain dapat bekerja secara efisien.

Taproot diimplementasikan pada tahun 2021 untuk memungkinkan pengelompokan dan validasi beberapa tanda tangan dengan menggabungkan tanda tangan Schnorr, memperkenalkan bahasa skrip untuk memungkinkan fungsionalitas yang lebih kompleks, serta meningkatkan privasi dan ketahanan sensor pada transaksi.



#### 'Di atas' Bitcoin

##### Liquid Sidechain

Sidechain Liquid diimplementasikan pada tahun 2018. Liquid, seperti sidechain lainnya, adalah buku besar blockchain terpisah yang terhubung ke blockchain utama Bitcoin, sesuai dengan seperangkat aturan yang telah ditentukan. Aturan-aturan ini cukup fleksibel untuk memungkinkan rantai Liquid berkembang dan mengadopsi peningkatan desain dan skalabilitas seiring waktu. Namun, keterkaitan dengan blockchain Bitcoin memastikan batas pasokan total 21 juta bitcoin tetap konsisten di kedua rantai.

Aset di Liquid, L-BTC, dipatok dua arah ke bitcoin di rantai utama. Ada kompromi biaya, kecepatan, privasi, dan keamanan yang membuat L-BTC ideal untuk beberapa aplikasi. Biaya, kecepatan, dan privasi semuanya meningkat dengan L-BTC, dengan mengorbankan kepercayaan pada organisasi yang membentuk Liquid Federation, yang bersama-sama mengendalikan proses multisig 11 dari 15 untuk mematok masuk dan keluar L-BTC ke bitcoin dan sebaliknya.

##### Lightning Network

Lightning Network diimplementasikan pada tahun 2018. Lightning dirancang sebagai jaringan pembayaran peer to peer dalam bentuk grafik node yang terhubung melalui channel; ini bukan blockchain. Bitcoin dikunci oleh operator node di blockchain utama agar dapat digunakan di Lightning Network, memastikan hanya bitcoin 'asli' yang digunakan. Node kemudian dapat membuka channel likuiditas melalui smart contract multisig satu sama lain. Pembayaran menemukan rute melalui jaringan dari sumber ke tujuan, mengoptimalkan biaya dengan syarat likuiditas yang cukup tersedia di arah yang benar di setiap langkah rute. Lightning Network sangat meningkatkan biaya, kecepatan, dan privasi dengan mengorbankan keamanan (atau peningkatan kepercayaan yang dibutuhkan) dan peningkatan kompleksitas. Namun, jaringan ini memang ditujukan untuk pembayaran harian dengan volume tinggi dan nilai rendah, sehingga kompromi ini dianggap sangat wajar untuk jutaan transaksi hariannya (sumber: River, 2023).

##### Chaumian eCash Mints

Fedimints dapat dianggap sebagai jaringan lightning yang dibatasi komunitas. Mereka dirancang untuk memanfaatkan kepercayaan yang sudah ada dalam komunitas tertentu (misalnya keluarga, desa, kelompok pertemanan) sebagai imbalan untuk menyederhanakan kompleksitas dan meningkatkan privasi bagi pengguna. Mereka adalah protokol modular dan open source untuk menyimpan dan bertransaksi bitcoin dalam konteks komunitas. Mereka dapat berinteraksi dengan Lightning Network itu sendiri.

**Cashu** adalah token pembawa yang dapat disimpan di perangkat seperti ponsel; desainnya bertujuan untuk mereplikasi manfaat uang tunai fisik namun dalam bentuk digital. Cashu adalah contoh Chaumian eCash yang dibangun di atas Bitcoin dan meningkatkan privasi serta ketahanan sensor serta mengurangi kompleksitas dengan imbalan kepercayaan pada mint eCash yang digunakan. Mint Cashu menerbitkan token eCash, yang mewakili bitcoin, yang dapat dibelanjakan pengguna tanpa mengungkapkan identitas mereka. Cashu dapat berinteraksi dengan Lightning Network.

Kemungkinan akan ada banyak lagi aplikasi layer 2 yang dibangun di masa depan, dengan banyak aplikasi layer 3 yang pada gilirannya dibangun di atas masing-masing aplikasi tersebut.

Sebagai contoh dari banyaknya aplikasi luar biasa yang dibangun di atas Lightning, berikut adalah kutipan dari Laporan Riset Lightning Network oleh River.

![The Lightning Network Industry Market Map 2023](https://cdn.sanity.io/images/vje9ehw2/staging/a5d3bdf5b343b7ae7e44663cf6e56a76a4bdec2d-501x706.svg)
