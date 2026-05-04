# 2.7 Bitcoin tidak benar-benar terdesentralisasi

> Kompleksitas kripto muncul dari upaya desentralisasi—dengan mendistribusikan kekuasaan dan tata kelola dalam sistem, secara teori tidak diperlukan perantara tepercaya seperti institusi keuangan. Itulah premis dari white paper Bitcoin awal, yang menawarkan solusi kriptografi yang dimaksudkan untuk memungkinkan pembayaran dikirim tanpa melibatkan institusi keuangan atau perantara tepercaya lainnya. Namun, Bitcoin menjadi terpusat dengan sangat cepat dan sekarang bergantung pada sekelompok kecil pengembang perangkat lunak dan pool penambangan untuk berfungsi  
_Dana Moneter Internasional_

Seperti yang ditunjukkan oleh kutipan di atas dari postingan cukup baru oleh Dana Moneter Internasional, industri keuangan arus utama terus mengklaim bahwa Bitcoin tidak terdesentralisasi, serta seringkali mencampuradukkan Bitcoin dengan aset kripto lainnya.

##### Pendahuluan

![Trilemma](https://cdn.sanity.io/images/vje9ehw2/staging/c9b1abab260a73f4e8c91d45b6656c233053d4d3-161x167.svg)

Desentralisasi adalah aspek penting dari Bitcoin. Kemampuan untuk mempertahankan aturan protokol seperti kelangkaan dan distribusi tanpa otoritas pusat memastikan bahwa Bitcoin dapat berfungsi sebagai uang tanpa izin untuk masyarakat global.

Seperti yang dicatat Satoshi dalam korespondensi onlinenya, layanan terdesentralisasi seperti BitTorrent 'masih bertahan' terhadap penindasan Pemerintah, dibandingkan dengan layanan yang memiliki pemilik yang teridentifikasi dan server terpusat. Ia jelas khawatir tentang potensi risiko Pemerintah atau kepentingan lain yang dapat menutup atau mempengaruhi Bitcoin secara negatif.

Dalam konteks ini, kita tertarik pada desentralisasi dari:

* Pengembangan dan pengelolaan kode yang menjalankan protokol; siapa yang diizinkan mengubah aturan?
* Fungsi penambangan yang membuat blok baru sesuai dengan aturan dan memvalidasi terhadap pengeluaran ganda
* Node yang memvalidasi transaksi untuk keabsahan dan menyimpan salinan blockchain

##### Pengembang

Bitcoin adalah protokol open-source yang siapa saja bebas untuk melihat, mengunduh, menyalin, atau mengusulkan perubahan. Kode ini tersedia di perpustakaan GitHub, dengan kode sumber yang awalnya diluncurkan pada tahun 2009 oleh Satoshi Nakamoto. Siapa saja bebas mengunduh kode dan menjalankan node, yang sebagian besar menjalankan perangkat lunak Bitcoin Core asli, yang telah diperbarui seiring waktu.

![How Does an idea Make Its Way Into Bitcoin Core?](https://cdn.sanity.io/images/vje9ehw2/staging/49f70d059c9dbe19a6e4500e9abd8db66ca97bff-1300x1439.png)

_Sumber: https://river.com/learn/what-is-bitcoin-core/_

Pengembangan Bitcoin Core mengikuti praktik terbaik pengembangan open source. Setiap saat, bisa ada sejumlah pengembang yang menulis atau meninjau perubahan kode. Mereka perlu mendengarkan kekhawatiran operator node dan penambang, serta basis pengguna sebelum membuat perubahan penting pada kode, yang akan ditinjau dan disetujui seperti yang ditunjukkan pada diagram alur di atas sebelum akhirnya masuk ke dalam kode.

Aturan Bitcoin kemudian dikodekan dalam perangkat lunak Bitcoin Core ini, yang berjalan di setiap node. Siapa saja dapat mengusulkan perubahan pada aturan – aturan tersebut adalah kode, tetapi mereka bukanlah_hanya_kode, mereka adalah_kode yang disepakati bersama_Jika diubah secara sepihak, kode baru tersebut tidak lagi menjadi bagian dari konsensus dan tidak lagi menjadi bagian dari Bitcoin. Mengubah sesuatu pada Bitcoin dan tetap berada dalam konsensus adalah hal yang rumit. Usulan perubahan kode terbagi dalam tiga kategori:

* Dalam aturan yang ada: Peningkatan kecil seperti perbaikan ejaan, UI yang lebih baik, atau manajemen data dapat masuk dalam kategori ini dan relatif mudah untuk disetujui.
* Menambahkan aturan baru yang menambah pembatasan pada aturan—seperti mengurangi ukuran blok. Ini disebut sebagai 'soft fork'. Node yang memilih untuk tidak menerapkan perubahan kode dan tetap pada rilis lama masih dapat berpartisipasi dalam jaringan.
* Menambahkan aturan baru yang melanggar aturan saat ini, misalnya peningkatan ukuran blok. Node yang tidak memperbarui ke kode baru akan menolak blok yang dibuat dengan ukuran lebih besar sebagai tidak valid. Ini disebut sebagai 'hard fork' dan akan menciptakan pemisahan rantai antara node yang menjalankan kode asli dan kode baru serta menciptakan koin baru. Ini pernah terjadi sebelumnya tetapi tidak pernah menghasilkan keberhasilan jangka panjang untuk koin baru karena mayoritas node memutuskan untuk tetap pada kode asli.

Oleh karena itu, satu pihak atau sekelompok orang tidak dapat secara sepihak mengubah kode Bitcoin tanpa mendapatkan kesepakatan konsensus, atau mereka berisiko terjadi pemisahan rantai dan penciptaan koin baru dengan seperangkat aturan yang berbeda.

##### Penambangan

Fungsi penambangan memvalidasi transaksi seperti node lain di jaringan, tetapi kemudian akan mengeluarkan energi yang diperlukan untuk membuat blok baru yang memenuhi aturan konsensus dalam kode. Keberhasilan memungkinkan penambang mendapatkan imbalan dalam bentuk biaya transaksi dan hadiah Bitcoin (saat penulisan 3,125 koin per blok).

Penambangan biasanya dilakukan oleh 'Pool' penambangan di mana orang-orang menggabungkan kekuatan penambangan atau hash rate mereka untuk meningkatkan peluang berhasil menambang blok dan berbagi imbalan. Ada bahaya bahwa satu atau lebih pool penambangan dapat bergabung untuk mencapai dominasi 51% dalam penambangan dan pada dasarnya mengesampingkan protokol validasi jaringan demi keuntungan mereka untuk melakukan pengeluaran ganda. Ini akan membutuhkan sumber daya yang sangat besar dengan biaya tinggi, dan penambang individu dapat dengan mudah berpindah ke pool penambangan lain kapan saja. Serangan semacam itu juga kemungkinan besar akan menyebabkan nilai bitcoin jatuh, karena akan jelas bahwa integritas jaringan telah dikompromikan. Penyerang karena itu harus segera mengonversi bitcoin yang didapat ke fiat sebelum nilainya turun. Hal ini membuat serangan sulit dipertahankan dalam jangka panjang, sehingga lebih menguntungkan bagi penambang atau operator pool untuk mematuhi aturan dan mencoba menambang blok yang valid.

Distribusi geografis dari fungsi penambangan juga penting untuk menghindari, misalnya, pemerintah mengambil alih kapasitas penambangan atau menutupnya. Sebagai contoh, larangan penambangan baru-baru ini oleh Tiongkok menunjukkan kemampuan Bitcoin untuk beradaptasi dan bertahan dari intervensi pemerintah semacam itu, beradaptasi dan pulih dengan cepat dari hilangnya hash power yang diakibatkan.

##### Node

Berbeda dengan penambangan, yang membutuhkan investasi finansial signifikan untuk dapat bersaing secara efektif dalam perlombaan menambang blok baru, atau pengembangan kode yang membutuhkan keahlian pemrograman, menjalankan node adalah sesuatu yang dapat dilakukan siapa saja yang tertarik membantu menjaga desentralisasi Bitcoin.

Node menjalankan perangkat lunak Bitcoin Core dan menegakkan aturan yang ada dalam kode untuk memastikan penambang tidak curang, misalnya dengan memberikan hadiah blok lebih besar dari yang diizinkan. Node juga menegakkan batas pasokan 21 juta, yang sangat penting untuk menjaga kelangkaan Bitcoin. Agar pemerintah atau pihak jahat dapat menghentikan Bitcoin, mereka harus menghancurkan setiap salinan blockchain, yang saat ini berjalan di ribuan node yang tersebar di seluruh dunia, sebuah tugas yang hampir mustahil.

##### Orang

Aspek lain dari potensi sentralisasi adalah manusia. Setiap 'alt-coin' lain memiliki sosok pemimpin—seseorang yang berpotensi dapat dipaksa untuk mendukung perubahan yang tidak sesuai dengan kepentingan terbaik Bitcoin. Satoshi Nakamoto tetap ada cukup lama untuk memastikan Bitcoin berada di jalur kesuksesan sebelum menghilang untuk selamanya, meninggalkannya di tangan orang lain untuk mengembangkan dan menyesuaikan perangkat lunak.

Bagaimana dengan pemegang Bitcoin dalam jumlah besar? Investor awal, yang telah menyimpan koin mereka dan tidak kehilangannya, akan sangat kaya saat ini. Penting untuk dicatat bahwa hal ini memang mungkin terjadi, tetapi itu tidak memberi mereka pengaruh lebih besar pada sistem dibandingkan orang lain, tidak seperti koin 'proof of stake' di mana para pengadopsi awal yang sudah kaya dalam koin tersebut mendapatkan keuntungan dalam pengambilan keputusan dan distribusi koin di masa depan. Hal ini telah atau pasti akan menyebabkan sentralisasi seiring waktu.

##### Kesimpulan

Apa saja potensi ancaman yang dapat diupayakan untuk diminimalkan oleh desentralisasi?

* Pemerintah menutup atau melarang Bitcoin
* Perubahan kode yang tidak diinginkan yang menguntungkan satu kepentingan dalam Bitcoin, misalnya meningkatkan hadiah blok
* Pemaksaan protokol oleh pemerintah atau pihak jahat untuk mempengaruhi arah protokol
* Kemampuan sekelompok penambang untuk mengambil alih jaringan dan melakukan 'double-spend' Bitcoin – serangan 51%

Seperti yang dapat kita lihat, kombinasi node, pengembang kode, dan penambang, serta penggunaan mekanisme 'proof of work', mendesentralisasi Bitcoin pada tingkat yang cukup sehingga potensi ancaman ini tidak dianggap sebagai kekhawatiran besar. Komunitas perlu terus memantau situasi untuk memastikan hal ini tetap terjadi.
