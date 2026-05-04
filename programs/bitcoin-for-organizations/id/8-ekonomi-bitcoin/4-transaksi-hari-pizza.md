# 8.4 Transaksi Hari Pizza

Sejauh ini, modul ini telah berfokus pada penggunaan sifat terbuka dari buku besar Bitcoin untuk menyusun metrik yang berguna dari data transaksi yang teragregasi. Namun, dimungkinkan untuk menggunakan data buku besar dan penjelajah blok untuk memeriksa transaksi dunia nyata dan melacak pergerakan dana di dalam jaringan.

Setiap tahun pada tanggal 22 Mei, komunitas Bitcoin mengenang Laszlo Hanyecz, yang menjadi orang pertama yang dilaporkan menggunakan bitcoin untuk membeli barang fisik. Pada 18 Mei 2010, Hanyecz mengumumkan di forum Bitcointalk.org bahwa ia sedang mencari pizza dan bersedia membayar dengan BTC. Ia menawarkan 10.000 BTC kepada siapa saja yang bersedia melakukan transaksi tersebut. Ia menunggu beberapa hari, hingga akhirnya mahasiswa berusia 19 tahun, Jeremy Sturdivant, memenuhi permintaan tersebut dan mengirimkan dua pizza besar.

Transaksi **Hari Pizza** dapat dilihat oleh siapa saja dan memiliki ID transaksi sebagai berikut:

`a1075db55d416d3ca199f55b6084e2115b9345e16c5cf302fc80e9d5fbf5d48d`

Memasukkan ID transaksi ini ke [mempool.space](https://mempool.space) mengungkapkan hal-hal berikut:

![Transaction](https://cdn.sanity.io/images/vje9ehw2/staging/d9b23ca4a14b433f0540a0920a1a1eb9662cad37-1126x268.png)



Tanggal dan waktu transaksi: 22 Mei 2010

Biaya transaksi jaringan: 99.000.000 sats (pada saat itu setara dengan kurang dari 1 sen AS. Pada Mei 2025, nilainya $95.072,67)

Tinggi Blok: 57.043

Jumlah Konfirmasi: 838.645 (ini adalah jumlah blok yang ditambahkan ke buku besar setelah transaksi ini)

![Inputs & Outputs](https://cdn.sanity.io/images/vje9ehw2/staging/dde2d64b67678116d039740c63ba279c27cc8703-1149x571.png)



![Address](https://cdn.sanity.io/images/vje9ehw2/staging/c6d7be3be795a922e7850718408570234b206615-573x253.png)

Jumlah Input Transaksi: 131

Jumlah Output Transaksi: 1

Dengan mengklik kunci publik output (berakhiran `XaxFyQ`) yang kita tahu dimiliki oleh Jeremy Sturdivant yang menerima 10.000 BTC untuk dua pizza, akan terlihat hal-hal berikut:

Alamat ini saat ini memiliki saldo 0,00257879 BTC dan tampaknya telah terlibat dalam 14 transaksi, yang terbaru terjadi pada 13 Desember 2024.



#### 8.4.1 Aktivitas: Diskusi Kelompok

1. Jelaskan manfaat (misalnya audit, akuntabilitas) atau risiko (misalnya masalah privasi) bagi individu atau bisnis yang menggunakan sistem transaksi yang transparan dan terbuka seperti ini.
1. Bagaimana transparansi keuangan seperti ini dapat memengaruhi industri seperti amal, pengadaan pemerintah, remitansi, atau penegakan hukum?
1. Haruskah sistem perbankan tradisional menawarkan tingkat visibilitas yang serupa? Akankah mereka dipaksa oleh pasar?
