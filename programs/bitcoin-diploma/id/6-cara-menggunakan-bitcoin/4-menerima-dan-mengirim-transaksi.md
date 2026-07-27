# 6.4 Menerima dan Mengirim Transaksi

Transaksi Bitcoin adalah pemindahan kepemilikan bitcoin kepada pemilik baru. Perlu dicatat bahwa yang dipindahkan bukanlah koin fisik, melainkan kepemilikannya: dengan kata lain, hak untuk membelanjakannya. Setiap kali sebuah transaksi diterima ke dalam sebuah blok, semua node di jaringan memperbarui salinan lokal mereka dari buku besar publik untuk mencerminkan perubahan kepemilikan tersebut. Dalam hal ini, transaksi Bitcoin lebih mirip dengan transaksi properti (seperti real estat atau properti lain) daripada transaksi tunai.

Untuk "mengirim" bitcoin, pengirim menandatangani sebuah pesan dengan kunci privat mereka, memberi sinyal kepada jaringan bahwa pemilik sah bitcoin telah memindahkan kepemilikannya kepada penerima.

Bitcoin tersebut sekarang akan terikat pada alamat penerima, memberikan mereka kepemilikan atas bitcoin tersebut, sehingga hanya pemilik baru yang dapat membelanjakannya dengan menggunakan kunci privat mereka.

Transaksi Bitcoin baru dimulai dari dompet di seluruh dunia, namun tidak ada pemroses pembayaran pusat. Sebagai gantinya, para penambang bersaing untuk mencatat transaksi ke dalam buku besar.

Misalkan Joko berutang 0,5 BTC kepada Eliana dan siap membayarnya kembali. Keduanya memiliki dompet digital.

1. Eliana membagikan alamatnya kepada Joko.
1. Joko menggunakan perangkat lunak dompetnya untuk membuat transaksi, yang mencakup alamat Eliana, jumlah yang akan ditransfer (0,5 BTC), dan biaya untuk penambang. Biaya yang lebih tinggi membuat transaksi lebih mungkin dimasukkan oleh penambang ke dalam blok berikutnya.
1. Setelah menandatangani transaksi, transaksi tersebut disiarkan ke jaringan, di mana transaksi tersebut diverifikasi oleh node-node. Mereka memeriksa apakah Joko memiliki dana yang cukup dan merupakan pemilik sah koin yang ingin ia belanjakan. Jika tidak, transaksi langsung ditolak.
1. Setelah transaksi diverifikasi, penambang memilih apakah akan menambahkan transaksi ke blok berikutnya, biasanya berdasarkan biaya yang dipilih. Setelah transaksi masuk ke dalam blok, transaksi tersebut ditambahkan ke blockchain dan dana dipindahkan ke alamat Eliana.
1. Kepemilikan telah berpindah ke Eliana. Sekarang ia dapat menggunakan kunci privatnya untuk membelanjakan dana tersebut.

_Penting untuk dicatat bahwa setelah transaksi selesai, transaksi tersebut tidak dapat dibatalkan._


> **Light – Bagaimana Cara Kerja Transaksi Bitcoin**
>
> 1. Seseorang meminta transaksi
> 1. Transaksi disiarkan ke komputer P2P (node-node)
> 1. Penambang memverifikasi transaksi
> 1. Transaksi digabungkan untuk membentuk sebuah blok data
> 1. Blok baru ditambahkan ke blockchain yang sudah ada
> 1. Transaksi selesai



> **Light – Menerima Transaksi Bitcoin**
>
> Untuk menerima bitcoin, Anda perlu memberikan alamat publik Bitcoin kepada pengirim. Ini adalah rangkaian unik huruf dan angka yang mewakili dompet Anda dan digunakan untuk mengidentifikasinya di jaringan Bitcoin.
>
> Anda dapat menemukan alamat publik Anda dengan membuka dompet Bitcoin Anda dan mencari opsi “Terima” atau “Deposit” bitcoin.
>
> Anda kemudian dapat membagikan alamat Bitcoin Anda dengan beberapa cara:
>
> 1. **Salin dan tempel alamat**: Anda dapat menyalin alamat dengan menyorotnya dan menekan "Salin", lalu menempelkannya ke email atau pesan.
> 1. **Bagikan tautan ke dompet Bitcoin Anda**: Beberapa dompet Bitcoin memungkinkan Anda membuat tautan ke dompet Anda yang dapat Anda bagikan kepada pengirim. Mereka kemudian dapat mengklik tautan tersebut untuk mengakses dompet Anda dan mengirim bitcoin.
> 1. **Bagikan kode QR**: Jika pengirim memiliki ponsel pintar dengan aplikasi dompet Bitcoin terpasang, mereka dapat memindai kode QR untuk mendapatkan alamat Bitcoin Anda.


Setelah pengirim memiliki alamat Anda, mereka dapat mengirimkan bitcoin kepada Anda dengan memasukkan alamat Anda dan jumlah yang ingin dikirim. Bitcoin kemudian dikirim dari dompet mereka ke dompet Anda.

Transaksi dikonfirmasi oleh Jaringan Bitcoin dan biasanya memakan waktu sekitar 10 menit. Untuk keamanan lebih, disarankan menunggu dua konfirmasi, yang memakan waktu sekitar 20 menit.


> **Light – Mengirim Transaksi Bitcoin**
>
> Untuk mengirim bitcoin, Anda memerlukan beberapa hal: dompet Bitcoin, alamat publik penerima, dan jumlah bitcoin yang ingin Anda kirim.
>
> 1. Buka dompet Bitcoin Anda.
> 1. Arahkan ke tombol “Kirim” dan tempel alamat penerima di kolom "Kepada". Sebagai alternatif, Anda juga dapat memindai kode QR jika penerima menyediakannya.
> 1. Masukkan jumlah bitcoin yang ingin Anda kirim di kolom “Jumlah”.
> 1. Periksa kembali alamat penerima dan jumlah yang akan dikirim. Ingat, transaksi tidak dapat dibatalkan!
> 1. Sebelum mengklik “Konfirmasi dan Kirim”, kami sarankan Anda memeriksa kembali detail transaksi sekali lagi untuk memastikan Anda mengirim jumlah bitcoin yang benar ke alamat yang benar.
> 1. Siarkan transaksi dan tunggu jaringan mengonfirmasi transaksi tersebut.
>
> Sekarang Anda tahu cara mengevaluasi, memilih, dan menyiapkan dompet Bitcoin yang bersifat self-custodial. Mengirim dan menerima bitcoin di jaringan Bitcoin disebut sebagai transaksi “on-chain”. Ini karena transaksi terjadi di jaringan utama Bitcoin dan dicatat di blockchain.
>
> Transaksi on-chain adalah cara teraman untuk bertransaksi dengan bitcoin karena verifikasi terdesentralisasi yang disediakan oleh jaringan.
>
> Namun, transaksi on-chain lebih lambat dan bisa jauh lebih mahal daripada opsi lain (yang akan kita bahas di Modul 7) karena adanya biaya penambang.


#### Aktivitas: Transaksi dalam Aksi


https://qr.myfirstbitcoin.org/transactions.pdf

_Activity: Transactions_


**Ini adalah latihan kerja sama yang menyederhanakan peran dasar orang-orang yang terlibat dalam transaksi Bitcoin.**

###### Poin-Poin Penting

1. Ada empat jenis peserta dalam setiap transaksi bitcoin: pengirim, penerima, penambang, dan operator node.
1. Pengirim harus menyetujui (menandatangani secara kriptografi) **jumlah bitcoin** yang akan dikirim DAN **alamat spesifik** yang akan dikirimi.
1. Penerima harus memberikan **alamat yang valid** kepada pengirim DAN memverifikasi bahwa transaksi telah berhasil dikonfirmasi di blockchain.
1. Penambang memastikan semua kriteria valid sebelum menambahkan transaksi ke blok-blok berikutnya.
1. Operator node memverifikasi bahwa blok yang ditambang valid sebelum memperbarui versi blockchain (buku besar) mereka.

###### Tips Siswa

Bergiliran menjalankan keempat peran untuk merasakan apa yang dilakukan setiap peserta.
