# 7.1 Rangkaian Lightning

Lightning Network ialah satu sistem pembayaran yang membolehkan pengguna menghantar dan menerima bitcoin dengan cepat dan kos yang rendah. Ia berfungsi dengan mewujudkan dompet bersama di mana kedua-dua pihak menyimpan sebahagian bitcoin mereka. Mereka kemudian boleh melakukan transaksi tanpa had antara satu sama lain tanpa perlu merekodkan setiap transaksi di blockchain utama. Dengan cara ini, mereka tidak perlu mengesahkan dan memasukkan setiap transaksi ke dalam blok, menjadikan proses ini lebih pantas dan menjimatkan kos. Yuran yang lebih rendah bermakna Lightning Network boleh digunakan untuk pembayaran kecil yang tidak selalu berbaloi dilakukan secara on-chain. Apabila kedua-dua pihak memutuskan untuk menamatkan kerjasama, hanya baki akhir sahaja yang direkodkan di blockchain.

Bayangkan satu hari bekerja di sebuah kafe. Merancang untuk duduk lama, anda membuka tab dan membuat prabayar, bukannya membayar setiap pesanan satu persatu. Pada akhir hari, anda dan pemilik kafe menyemak tab untuk menyelesaikan bil. Jika deposit anda lebih daripada apa yang anda belanjakan, anda akan menerima baki semula; jika anda berbelanja lebih, anda perlu membayar baki yang masih tertunggak.

Skim ini boleh dikembangkan untuk melibatkan lebih ramai peserta. Contohnya, pada salah satu lawatan anda ke kafe, anda membawa seorang rakan yang tidak dikenali oleh pelayan dan tidak boleh membuka tab. Anda menawarkan tab anda kepada rakan anda untuk menampung perbelanjaan mereka, dan bersetuju mereka akan membayar anda secara peribadi. Sekarang bayangkan ribuan orang melakukan perkara yang sama serentak, membolehkan orang lain menggunakan tab sedia ada untuk berhubung dengan lebih ramai individu — begitulah cara Lightning Network berfungsi!

Dengan Lightning, anda boleh membuat pembayaran kepada sesiapa sahaja di rangkaian, bukan hanya kepada orang yang anda kongsi tab secara langsung — asalkan terdapat laluan antara kedua-dua pihak. Pembayaran anda boleh melalui rangkaian sehingga sampai ke destinasi, walaupun anda tidak mempunyai saluran terbuka secara langsung dengan penerima.

Mari kita lihat perbezaan antara transaksi on-chain dan off-chain.

##### Transaksi On-Chain

Ini adalah transaksi yang berlaku secara langsung di blockchain Bitcoin. Ia mengambil masa kira-kira 10 minit untuk disahkan, dan yuran bergantung pada saiz transaksi dalam bait maya. Ia lebih selamat tetapi lebih perlahan, kerana memerlukan konsensus rangkaian.

##### Transaksi Lightning Network

Transaksi ini berlaku di rangkaian berasingan yang dibina di atas blockchain Bitcoin. Ia diselesaikan dengan lebih pantas dan yuran yang lebih rendah. Ia biasanya digunakan apabila faktor seperti kelajuan dan kos transaksi lebih penting. Berbanding transaksi on-chain, ia kurang selamat.


|  | Rangkaian Bitcoin | Lightning Network |
| --- | --- | --- |
| Definisi | Satu rangkaian digital terdesentralisasi yang menggunakan kriptografi untuk melindungi transaksi kewangan. | Protokol pembayaran lapisan kedua yang beroperasi di atas blockchain Bitcoin, membolehkan transaksi lebih pantas dan murah. |
| Kelebihan | Terdesentralisasi dan selamat. Tiada caj balik atau penipuan. Boleh digunakan secara pseudonim. Penerimaan global. | Transaksi lebih pantas dan murah. Skalabiliti yang lebih tinggi. Transaksi off-chain tidak membebankan blockchain. |
| Kekurangan | Masa transaksi yang perlahan. Yuran tinggi untuk jenis transaksi tertentu. Rumit untuk pemula. | Boleh memerlukan kepercayaan kepada pengendali saluran. Memerlukan transaksi on-chain untuk membuka dan menutup saluran. |
