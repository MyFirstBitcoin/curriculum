# 2.4 Tiada inovasi yang berlaku dalam Bitcoin

> Penciptaan seribu hutan bermula dari satu biji acorn.  
_Ralph Waldo Emerson_

Pengkritik sering cuba mendakwa bahawa Bitcoin adalah teknologi 'lama' atau 'mati' kerana ia tidak kerap mengubah protokol lapisan asas seperti blockchain pesaing. Dakwaan ini mengabaikan kedua-dua sebab mengapa perubahan pada Bitcoin diterima pakai secara perlahan dan jumlah inovasi yang berlaku untuk meningkatkan skala rangkaian pada lapisan lebih tinggi, seperti Lightning Network. Ia juga mengabaikan hakikat bahawa banyak teknologi kita yang paling fleksibel dan tahan lama juga tidak berkembang dengan cepat di lapisan asas.

Sebagai contoh, tiada inovasi berlaku dalam Transmission Control Protocol (TCP), yang menjadi asas kepada internet. TCP pertama kali dicipta pada tahun 1974. Kali terakhir TCP dikemas kini adalah pada tahun 1982. Ia menjalankan tugasnya dengan baik. Ia tidak sempurna, dan terdapat perdebatan sama ada kita perlu menaik taraf IPv4 untuk menyokong pembangunan internet masa depan. Namun, untuk mengatakan bahawa tiada inovasi dalam internet sejak 1982 adalah satu dakwaan yang luar biasa. Semua inovasi ini berlaku 'di atas' TCP, bukan 'di dalamnya'.

Sebahagian besar inovasi yang berlaku bukanlah 'di dalam' Bitcoin tetapi 'di atas' Bitcoin. Suatu hari nanti mungkin tiada lagi inovasi 'di dalam' Bitcoin, dan itu sepatutnya menjadi sasaran, bukan kritikan, kerana ia akan mencerminkan betapa asasnya Bitcoin dalam menyokong ekonomi global dengan menyediakan asas untuk wang yang neutral, global dan tanpa kebenaran. Wang yang kukuh bukan sahaja dari segi ekonomi kerana bekalannya tetap dan lejar tidak boleh diubah, tetapi juga kukuh dari segi teknologi kerana ia tidak berubah dan telah beroperasi tanpa gangguan selama bertahun-tahun. Bitcoin telah mencapai 100% masa operasi sepanjang 10 tahun yang lalu.

Namun, ia akan menjadi kebimbangan jika tiada inovasi berlaku 'di atas' Bitcoin. Mari kita lihat perkara ini sepanjang 10 tahun yang lalu:



#### 'Di dalam' Bitcoin

Segregated Witness (SegWit) telah dilaksanakan pada tahun 2017 untuk melindungi daripada kebolehubahan transaksi dan meningkatkan kapasiti blok. SegWit juga merupakan prasyarat penting untuk lightning dan beberapa sidechain berfungsi dengan cekap.

Taproot telah dilaksanakan pada tahun 2021 untuk membolehkan pengelompokan dan pengesahan pelbagai tandatangan dengan menggabungkan tandatangan Schnorr, memperkenalkan bahasa skrip untuk membolehkan fungsi yang lebih kompleks serta meningkatkan privasi dan ketahanan terhadap penapisan transaksi.



#### 'Di atas' Bitcoin

##### Liquid Sidechain

Sidechain Liquid telah dilaksanakan pada tahun 2018. Liquid, seperti sidechain lain, adalah lejar blockchain berasingan yang dihubungkan ke blockchain utama Bitcoin, mengikut set peraturan yang telah ditetapkan. Peraturan ini cukup fleksibel untuk membolehkan rantaian Liquid berkembang dan menggabungkan penambahbaikan reka bentuk dan skalabiliti dari semasa ke semasa. Namun, pautan ke blockchain Bitcoin memastikan had bekalan 21 juta bitcoin kekal konsisten di kedua-dua rantaian.

Aset dalam Liquid, L-BTC, dipaut dua hala kepada bitcoin di rantaian utama. Terdapat kompromi dari segi kos, kelajuan, privasi dan keselamatan yang menjadikan L-BTC sesuai untuk sesetengah aplikasi. Kos, kelajuan dan privasi semuanya bertambah baik dengan L-BTC, dengan pertukaran kepercayaan kepada organisasi yang membentuk Liquid Federation, yang bersama-sama mengawal proses multisig 11 daripada 15 untuk memaut masuk dan keluar L-BTC ke bitcoin dan sebaliknya.

##### Lightning Network

Lightning Network telah dilaksanakan pada tahun 2018. Lightning direka sebagai rangkaian pembayaran peer-to-peer dalam bentuk graf nod yang dihubungkan melalui saluran; ia bukan blockchain. Bitcoin dikunci oleh pengendali nod di blockchain utama untuk membolehkan ia digunakan di Lightning Network, memastikan hanya bitcoin 'sebenar' digunakan. Nod kemudian boleh membuka saluran kecairan melalui kontrak pintar multisig antara satu sama lain. Pembayaran mencari laluan melalui rangkaian dari sumber ke destinasi, mengoptimumkan kos dengan syarat kecairan mencukupi wujud dalam arah yang betul antara setiap langkah nod dalam laluan. Lightning Network meningkatkan kos, kelajuan dan privasi dengan ketara sebagai pertukaran kepada sedikit kehilangan keselamatan (atau peningkatan kepercayaan yang diperlukan) dan peningkatan kerumitan. Namun, ia bertujuan untuk pembayaran harian bernilai rendah tetapi berjumlah tinggi, jadi ini dianggap pertukaran yang sangat munasabah untuk berjuta-juta transaksi hariannya (sumber: River, 2023).

##### Chaumian eCash Mints

Fedimint boleh dianggap sebagai rangkaian lightning yang terhad kepada komuniti. Ia direka untuk memanfaatkan kepercayaan semula jadi yang wujud dalam komuniti tertentu (cth. keluarga, kampung, kumpulan sahabat) sebagai balasan untuk memudahkan kerumitan dan meningkatkan privasi pengguna. Ia adalah protokol modular dan sumber terbuka untuk menjaga dan bertransaksi bitcoin dalam konteks komuniti. Ia juga serasi dengan Lightning Network itu sendiri.

**Cashu** ialah token pembawa yang boleh disimpan pada peranti seperti telefon bimbit; reka bentuknya bertujuan untuk meniru kelebihan wang tunai fizikal tetapi dalam bentuk digital. Cashu ialah contoh Chaumian eCash yang dibina di atas Bitcoin dan meningkatkan privasi serta ketahanan terhadap penapisan serta mengurangkan kerumitan dengan pertukaran kepercayaan kepada mint eCash yang digunakan. Mint Cashu mengeluarkan token eCash, mewakili bitcoin, yang boleh dibelanjakan oleh pengguna tanpa mendedahkan identiti mereka. Cashu serasi dengan Lightning Network.

Kemungkinan besar akan terdapat banyak lagi aplikasi lapisan 2 yang akan dibina pada masa hadapan, dengan banyak aplikasi lapisan 3 pula dibina di atas setiap satu daripadanya.

Sebagai contoh kepada jumlah aplikasi yang luar biasa sedang dibina di atas Lightning, berikut adalah petikan daripada Laporan Penyelidikan Lightning Network oleh River.

![The Lightning Network Industry Market Map 2023](https://cdn.sanity.io/images/vje9ehw2/staging/a5d3bdf5b343b7ae7e44663cf6e56a76a4bdec2d-501x706.svg)
