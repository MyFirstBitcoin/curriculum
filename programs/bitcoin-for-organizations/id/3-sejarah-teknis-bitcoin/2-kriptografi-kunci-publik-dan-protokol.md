# 3.2 Kriptografi Kunci Publik dan Protokol

Internet saat ini, dan sebagian besar sistem komputer modern, bergantung pada kriptografi, sebuah metode untuk menyamarkan informasi sehingga hanya penerima informasi yang dapat mendekodenya. Dasar-dasar kriptografi yang digunakan untuk mengamankan Bitcoin dapat ditelusuri kembali ke tahun 70-an.

Masalah pertama yang harus diselesaikan adalah – bagaimana mengirim rahasia bersama melalui media yang tidak aman.

Hal ini pertama kali diteliti oleh Whitfield Diffie dan Martin Hellman.

Masalahnya: dua pihak – biasanya disebut sebagai Alice dan Bob – ingin berbagi informasi rahasia melalui jaringan di mana orang lain mungkin sedang menyadap. Untuk mencapai hal ini, mereka menciptakan proses pertukaran kunci Diffie-Hellman.

Rahasia bersama ini kemudian dapat digunakan sebagai nilai benih untuk membuat banyak kunci simetris guna mengenkripsi dan mendekripsi pesan yang dikirim satu sama lain tanpa membagikan kunci itu sendiri secara terbuka.

Karena kunci privat tidak pernah harus dibagikan, dan kunci yang berbeda digunakan di setiap ujung untuk mengenkripsi dan mendekripsi, ini disebut sebagai algoritma enkripsi asimetris.

Kasus penggunaan:

* Alice menandatangani pesan dengan kunci publik Bob – yang hanya dapat didekripsi oleh Bob menggunakan kunci privatnya
* Alice menandatangani pesan dengan kunci privatnya – dengan mendekripsi menggunakan kunci publiknya, siapa pun dapat memverifikasi bahwa pesan tersebut dikirim oleh Alice, tanpa mengetahui kunci privatnya
* Dengan menggabungkan kedua pendekatan ini dengan dua lapisan enkripsi, sebuah pesan dapat dikirim secara terenkripsi sehingga hanya Bob yang dapat mendekripsinya, dan ia kemudian dapat memverifikasi bahwa pengirimnya memang Alice

Meskipun tidak tercantum sebagai penulis pada makalah tersebut, Ralph Merkle sangat berperan dalam membantu memecahkan apa yang hingga saat itu dianggap sebagai teka-teki yang tak terpecahkan – bagaimana membangun atau membangun kembali komunikasi privat melalui jaringan terbuka dan berpotensi berbahaya.

Pendekatan ini sendiri rentan terhadap serangan brute force, di mana penyerang dapat mengambil angka-angka yang dibagikan dan akhirnya merekonstruksi kunci bersama jika memiliki cukup waktu dan sumber daya, sehingga ini bukanlah jawaban lengkap jika berdiri sendiri.

##### Protokol untuk Kriptosistem Kunci Publik

Selain berkontribusi pada sistem kunci publik Diffie-Hellman yang dijelaskan di atas, **Ralph Merkle** terus berkontribusi di bidang ini selama bertahun-tahun, dan sangat berperan dalam pengembangan beberapa komponen kunci yang digunakan oleh Bitcoin.

Fungsi hash kriptografi adalah algoritma matematika yang menerima input dengan ukuran berapa pun dan memproses perhitungan kompleks untuk menghasilkan nilai hash dalam bit, yang biasanya direpresentasikan dengan output alfanumerik berukuran tetap menggunakan format heksadesimal.

* Input dapat berukuran berapa saja
* Output selalu berukuran tetap dan deterministik (input yang sama menghasilkan hash yang sama setiap kali)
* Sangat mudah untuk memverifikasi tetapi sangat sulit untuk membalik prosesnya guna menentukan inputnya
* Perubahan kecil pada data sepenuhnya mengubah outputnya

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/5e46b2740cf1e2b7b0a505361457f8d0cd9a98b4-515x331.svg)

Hashing adalah bagian integral dari protokol Bitcoin. SHA-256, yang digunakan dalam Bitcoin, diciptakan oleh NSA dan merupakan contoh algoritma hashing kriptografi.

* Setiap blok dalam rantai di-hash sehingga data tidak dapat diubah – memastikan integritas buku besar terdistribusi
* Hash yang dihasilkan harus memenuhi kriteria ‘Proof of work’ agar dapat dianggap sebagai blok yang valid
* Pohon Merkle – dengan menggunakan percabangan dan hash dari hash, pohon hash dapat memungkinkan verifikasi dataset besar dengan penyimpanan minimal
* Tanda tangan dan kunci berbasis hash dapat digunakan untuk dompet, alamat, dan otorisasi transaksi

Verifikasi terdistribusi atas status blockchain dan model buku besar hanya-tambah yang tahan terhadap revisi dimungkinkan oleh hashing satu arah. Fungsi hash menyediakan pendekatan yang andal dan deterministik untuk memverifikasi peristiwa pada buku besar publik seperti Bitcoin tanpa adanya model kepercayaan terpusat.

Kemampuan baru dalam bidang kriptografi ini diharapkan oleh para penciptanya akan membawa gelombang inovasi baru di bidang ini.

##### Kriptografi kurva eliptik

Salah satu inovasi berikutnya datang dalam bentuk kriptografi kurva eliptik.

Kriptografi kurva eliptik diperkenalkan pada tahun 1985 oleh dua ilmuwan, N. Koblitz dan V. Miller. Mereka mengusulkan gagasan menggunakan titik-titik yang didefinisikan oleh kurva eliptik, bukan bidang prima hingga, sehingga asumsi masalah Logaritma Diskrit tetap berlaku, seperti yang umum digunakan dalam protokol pertukaran kunci Diffie-Hellman standar. Rincian tentang cara kerjanya berada di luar cakupan bagian ini, tetapi secara garis besar, kurva eliptik adalah kumpulan titik yang memenuhi persamaan matematika tertentu.

Persamaan untuk kurva eliptik terlihat seperti:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

Ini memiliki beberapa sifat yang berguna:

* Simetri horizontal. Setiap titik pada kurva dapat dipantulkan ke sumbu x dan tetap berada pada kurva yang sama.
* setiap garis yang tidak vertikal akan memotong kurva di paling banyak tiga titik.
* Ukuran kunci yang ringkas sangat penting untuk efisiensi penyimpanan dan transmisi kunci publik di blockchain.

Sifat-sifat ini dapat digunakan untuk membuat pasangan kunci dengan cara yang mirip dengan algoritma Diffie-Hellman. Bitcoin menggunakan ECDSA, yang merupakan singkatan dari Elliptic Curve Digital Signature Algorithm. Ini adalah proses yang menggunakan kurva eliptik dan bidang hingga untuk “menandatangani” data sedemikian rupa sehingga pihak ketiga dapat memverifikasi keaslian tanda tangan sementara penandatangan tetap memiliki kemampuan eksklusif untuk membuat tanda tangan tersebut. Pada bitcoin, data yang ditandatangani adalah transaksi yang mentransfer kepemilikan.

Bagian ‘hingga’ mirip dengan pendekatan ‘mod’ pada Diffie-Hellman, di mana output dari persamaan dibagi dan sisanya digunakan untuk memastikan bahwa hasilnya berada dalam rentang angka tertentu.
