# 6.4 Menerima dan Menghantar Transaksi

Transaksi Bitcoin ialah pemindahan hak milik bitcoin kepada pemilik baru. Perlu diingat bahawa bukan syiling sebenar yang dipindahkan, tetapi hak milik ke atasnya: dalam erti kata lain, hak untuk membelanjakannya. Setiap kali satu transaksi diterima ke dalam satu blok, semua nod dalam rangkaian akan mengemas kini salinan lejar awam mereka untuk mencerminkan perubahan hak milik tersebut. Dalam hal ini, transaksi Bitcoin lebih mirip dengan transaksi hartanah (atau harta lain) berbanding transaksi tunai.

Untuk "menghantar" bitcoin, penghantar menandatangani satu mesej dengan kunci peribadi mereka, menandakan kepada rangkaian bahawa pemilik sah bitcoin telah memindahkan hak milik kepada penerima.

Bitcoin kini akan terikat kepada alamat penerima, memberikan mereka hak milik bitcoin tersebut, supaya hanya pemilik baru boleh membelanjakannya dengan menggunakan kunci peribadi mereka.

Transaksi Bitcoin baru dimulakan dari dompet di seluruh dunia, tetapi tiada pemproses pembayaran pusat. Sebaliknya, pelombong bersaing untuk merekodkan transaksi dalam lejar.

Katakanlah Ahmad berhutang 0.5 BTC kepada Eliana dan sudah bersedia untuk membayarnya semula. Kedua-duanya mempunyai dompet digital.

1. Eliana berkongsi alamatnya dengan Ahmad.
1. Ahmad menggunakan perisian dompetnya untuk mencipta transaksi, yang merangkumi alamat Eliana, jumlah yang akan dipindahkan (0.5 BTC), dan yuran untuk pelombong. Yuran yang lebih tinggi meningkatkan kemungkinan pelombong akan memasukkan transaksi ke dalam blok seterusnya.
1. Selepas menandatangani transaksi, ia disiarkan ke rangkaian, di mana ia disahkan oleh nod. Mereka akan memeriksa sama ada Ahmad mempunyai dana yang mencukupi dan merupakan pemilik sah syiling yang ingin dibelanjakan. Jika tidak, mereka akan menolak transaksi serta-merta.
1. Setelah transaksi disahkan, pelombong memilih sama ada untuk menambah transaksi ke blok seterusnya, biasanya berdasarkan yuran yang dipilih. Setelah transaksi dimasukkan ke dalam blok, ia ditambah ke blockchain dan dana dipindahkan ke alamat Eliana.
1. Hak milik telah dipindahkan kepada Eliana. Kini dia boleh menggunakan kunci peribadinya untuk membelanjakan dana tersebut.

_Penting untuk diingat bahawa setelah transaksi selesai, ia tidak boleh dipulangkan semula._


> **Note – Bagaimana Transaksi Bitcoin Berfungsi**
>
> 1. Seseorang meminta satu transaksi
> 1. Transaksi disiarkan ke komputer P2P (nod)
> 1. Pelombong mengesahkan transaksi
> 1. Transaksi digabungkan untuk membentuk satu blok data
> 1. Blok baru ditambah ke blockchain sedia ada
> 1. Transaksi selesai



> **Note – Menerima Transaksi Bitcoin**
>
> Untuk menerima bitcoin, anda perlu memberikan alamat awam Bitcoin anda kepada penghantar. Ini adalah rentetan unik huruf dan nombor yang mewakili dompet anda dan digunakan untuk mengenal pasti dompet anda di rangkaian Bitcoin.
>
> Anda boleh mencari alamat awam anda dengan membuka dompet Bitcoin anda dan mencari pilihan untuk “Terima” atau “Deposit” bitcoin.
>
> Anda kemudian boleh berkongsi alamat Bitcoin anda dengan beberapa cara:
>
> 1. **Salin dan tampal alamat**: Anda boleh menyalin alamat dengan menyorotnya dan menekan "Salin", kemudian tampal ke dalam e-mel atau mesej.
> 1. **Kongsi pautan ke dompet Bitcoin anda**: Sesetengah dompet Bitcoin membenarkan anda mencipta pautan ke dompet anda yang boleh anda kongsi dengan penghantar. Mereka boleh klik pada pautan tersebut untuk mengakses dompet anda dan menghantar bitcoin.
> 1. **Kongsi kod QR**: Jika penghantar mempunyai telefon pintar dengan aplikasi dompet Bitcoin, mereka boleh mengimbas kod QR untuk mendapatkan alamat Bitcoin anda.


Setelah penghantar mempunyai alamat anda, mereka boleh menghantar bitcoin kepada anda dengan memasukkan alamat anda dan jumlah yang ingin dihantar. Bitcoin kemudian dihantar dari dompet mereka ke dompet anda.

Transaksi disahkan oleh Rangkaian Bitcoin dan biasanya mengambil masa kira-kira 10 minit. Untuk keselamatan yang lebih tinggi, disyorkan untuk menunggu dua pengesahan, yang mengambil masa kira-kira 20 minit.


> **Note – Menghantar Transaksi Bitcoin**
>
> Untuk menghantar bitcoin, anda memerlukan beberapa perkara: dompet Bitcoin, alamat awam penerima, dan jumlah bitcoin yang ingin dihantar.
>
> 1. Buka dompet Bitcoin anda.
> 1. Pergi ke butang “Hantar” dan tampal alamat penerima di medan "Kepada". Sebagai alternatif, anda juga boleh mengimbas kod QR jika penerima menyediakannya.
> 1. Masukkan jumlah bitcoin yang ingin anda hantar di medan “Jumlah”.
> 1. Periksa sekali lagi alamat penerima dan jumlah yang akan dihantar. Ingat, transaksi tidak boleh dipulangkan semula!
> 1. Sebelum klik “Sahkan dan Hantar”, kami mengesyorkan anda menyemak butiran transaksi sekali lagi untuk memastikan anda menghantar jumlah bitcoin yang betul ke alamat yang betul.
> 1. Siar transaksi dan tunggu rangkaian mengesahkan transaksi tersebut.
>
> Sekarang anda tahu cara menilai, memilih, dan menyediakan dompet Bitcoin kendiri. Menghantar dan menerima bitcoin di rangkaian Bitcoin dipanggil transaksi “on-chain”. Ini kerana transaksi berlaku di rangkaian utama Bitcoin dan direkodkan dalam blockchain.
>
> Transaksi on-chain adalah cara paling selamat untuk bertransaksi dengan bitcoin kerana pengesahan terdesentralisasi yang disediakan oleh rangkaian.
>
> Namun, transaksi on-chain adalah lebih perlahan dan boleh menjadi jauh lebih mahal daripada pilihan lain (yang akan kita bincangkan dalam Modul 7) disebabkan yuran pelombong.


#### Aktiviti: Transaksi Dalam Tindakan

https://qr.myfirstbitcoin.org/transactions.pdf

**Ini adalah latihan berkumpulan yang memudahkan peranan asas orang yang terlibat dalam satu transaksi Bitcoin.**

###### Perkara Utama

1. Terdapat empat jenis peserta dalam setiap transaksi bitcoin: penghantar, penerima, pelombong, dan pengendali nod.
1. Penghantar mesti meluluskan (menandatangani secara kriptografi) **jumlah bitcoin** untuk dihantar DAN **alamat tertentu** untuk dihantar.
1. Penerima mesti memberikan **alamat yang sah** kepada penghantar DAN mengesahkan bahawa transaksi telah berjaya disahkan di atas rantaian blok.
1. Pelombong memastikan semua kriteria adalah sah sebelum menambah transaksi ke blok masa depan.
1. Pengendali nod mengesahkan blok yang telah dilombong adalah sah sebelum mengemas kini versi rantaian blok (lejar) mereka.

###### Petua Pelajar

Bergilir-gilir melalui keempat-empat peranan untuk merasai apa yang dilakukan oleh setiap peserta.
