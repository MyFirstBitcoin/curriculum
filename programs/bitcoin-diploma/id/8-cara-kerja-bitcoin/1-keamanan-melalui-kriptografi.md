# 8.1 Keamanan melalui Kriptografi

> Apa yang diberikan Bitcoin kepada kita adalah janji yang kuat: program akan dijalankan persis seperti yang ditentukan.  
_Andreas M. Antonopoulos_

#### Kriptografi Kunci Publik/Privat


> **Definition – Definisi Kriptografi**
>
> **Kriptografi** adalah praktik mengubah informasi menjadi rahasia yang hanya bisa dibaca oleh orang yang tepat.


* **Enkripsi** adalah proses mengubah informasi menjadi bentuk kode sehingga hanya seseorang dengan kunci yang benar yang dapat membacanya.
* **Dekripsi** adalah proses mengubah informasi yang sudah dikodekan itu kembali menjadi sesuatu yang dapat dibaca.

Dalam kriptografi tradisional, dua orang yang ingin berkomunikasi secara pribadi harus terlebih dahulu berbagi kunci rahasia yang sama, mirip seperti berbagi kata sandi. Seseorang menggunakan kunci ini untuk mengenkripsi pesan sebelum mengirimkannya, dan orang lain menggunakan kunci yang sama untuk mendekripsi dan membacanya.

Masalah dengan sistem ini adalah kedua orang harus sudah berbagi kunci rahasia. Jika orang lain mendapatkan akses ke kunci itu, mereka dapat membaca pesan yang disadap.

Bitcoin memecahkan masalah ini dengan pendekatan berbeda yang disebut kriptografi kunci publik, di mana pengguna tidak perlu berbagi kunci rahasia terlebih dahulu.

Kriptografi kunci publik/privat memecahkan masalah berbagi rahasia. Alih-alih berbagi kata sandi, setiap orang memiliki dua kunci: kunci publik dan kunci privat.

* **kunci publik** dapat dibagikan kepada siapa saja.
* **kunci privat** harus selalu dijaga kerahasiaannya.

Jika Joko ingin mengirim sesuatu ke Arel, dia dapat menggunakan kunci publik milik Arel. Hanya Arel yang dapat membukanya menggunakan kunci privat miliknya. Bahkan jika seseorang menyadap pesan tersebut, mereka tidak dapat membacanya atau menggunakannya tanpa kunci privat.

Dalam Bitcoin, sistem ini digunakan untuk membuat tanda tangan digital. Tanda tangan digital membuktikan bahwa pemilik kunci privat telah menyetujui suatu transaksi, mirip seperti menandatangani nama Anda di sebuah dokumen. Inilah yang membuat transaksi Bitcoin menjadi aman dan dapat diverifikasi tanpa harus mempercayai pihak ketiga.

Transaksi Bitcoin melibatkan pemindahan kepemilikan bitcoin dari satu alamat ke alamat lain.

Enkripsi digunakan untuk memastikan bahwa hanya pemilik asli bitcoin yang memiliki wewenang untuk mengirim uang mereka ke orang lain. Ini memastikan properti mereka terlindungi dari pihak jahat.

Sebagai langkah perlindungan tambahan, setiap transaksi Bitcoin secara otomatis mendapatkan tanda tangan digital yang UNIK. Tanda tangan digital unik ini didukung oleh teknologi anti-manipulasi yang membantu jaringan memverifikasi bahwa pemilik asli bitcoin, dan bukan orang lain, yang telah mengirimkannya.


> **Info**
>
> Setiap pengguna memiliki dua kunci: **kunci privat**, yang **disimpan secara rahasia**, dan **kunci publik** yang dapat **dibagikan kepada orang lain**. **Kunci privat** berfungsi sebagai bentuk identifikasi dan bukti kepemilikan, yang menegaskan: “Alamat ini milik saya dan saya memiliki kendali atasnya.”


###### Bagaimana Cara Kerja Transaksi Bitcoin

1. **Membuat Transaksi**: Seorang pengguna memulai transaksi Bitcoin dengan menentukan detail seperti alamat penerima dan jumlah bitcoin yang akan dikirim.
1. **Pembuatan Tanda Tangan Digital**: Pengirim membuat **tanda tangan digital** yang unik menggunakan **kunci privat**. Tanda tangan ini adalah kode unik yang memverifikasi keaslian transaksi.
1. **Menyebarkan Transaksi**: Transaksi yang sudah ditandatangani disebarkan ke jaringan Bitcoin, menandakan niat untuk memindahkan kepemilikan bitcoin dari pengirim ke penerima.
1. **Verifikasi di Jaringan**: Node di jaringan Bitcoin menerima transaksi dan menggunakan **kunci publik** untuk memverifikasi keaslian tanda tangan dari transaksi. Secara bersamaan, mereka menggunakan **kunci publik** untuk memverifikasi **tanda tangan digital**.
1. **Konfirmasi di jaringan Bitcoin**: Jika verifikasi berhasil, transaksi akan ditambahkan ke buku besar, yang berfungsi sebagai catatan aman dan transparan dari semua transaksi. Setelah dikonfirmasi, kepemilikan bitcoin secara resmi berpindah dari pengirim ke penerima.


> **Callout – Ringkasan**
>
> Tanda tangan digital**tanda tangan digital**, yang dibuat dengan **kunci privat** pengirim, membuktikan bahwa transaksi tersebut telah disetujui oleh pemilik bitcoin. Jaringan Bitcoin kemudian dapat memverifikasi bukti ini dan mencatat transaksi tersebut.


#### Penjelasan Hashing

Jangan merasa terintimidasi oleh istilah teknis dan konsep matematika di depan. Kami paham bahwa tidak semua orang menyukai matematika, tapi Anda mungkin akan terkejut bahwa bahkan ide yang paling rumit pun bisa dipahami dengan sedikit usaha.


> **Definition – Definisi fungsi**
>
> Sebuah **fungsi** itu seperti mesin yang menerima beberapa informasi dan mengubahnya menjadi sesuatu yang baru. Informasi yang Anda berikan ke fungsi disebut **input**. Informasi baru yang dihasilkan fungsi disebut **output**. Fungsi membantu komputer melakukan tugas dan memecahkan masalah.


##### Apa itu fungsi?

Fungsi adalah serangkaian instruksi yang menerima input dan menghasilkan output. Anda bisa menganggapnya seperti resep: Anda mengikuti langkah-langkah dengan bahan tertentu, dan Anda selalu mendapatkan hasil yang dapat diprediksi.

Dalam Bitcoin, fungsi digunakan untuk memproses dan memverifikasi transaksi. Ketika seseorang mengirim bitcoin, fungsi kriptografi membantu memeriksa bahwa transaksi valid, memastikan pengirim memiliki dana yang cukup, dan memperbarui saldo di buku besar Bitcoin. Setelah diverifikasi dan ditambahkan ke blok, transaksi menjadi bagian dari catatan permanen di blockchain.

##### Apa itu fungsi satu arah?

Fungsi satu arah adalah jenis fungsi khusus yang mudah dihitung ke satu arah tetapi sangat sulit untuk dibalik. Misalnya, mencampur bahan menjadi smoothie itu mudah, tetapi Anda tidak bisa memisahkan smoothie kembali ke bahan aslinya.

Keamanan Bitcoin bergantung pada fungsi satu arah. Fungsi ini digunakan dalam kriptografi kunci publik dan privat, memungkinkan orang membagikan kunci publik sambil menjaga kunci privat tetap rahasia. Meskipun kunci publik terlihat, tidak mungkin mendapatkan kunci privat darinya. Inilah yang membuat transaksi Bitcoin aman.

##### Apa itu fungsi hash?

Fungsi hash**fungsi hash** itu seperti mesin kode rahasia. Fungsi ini menerima pesan dan mengubahnya menjadi kode.

###### Bagaimana Hashing Bekerja dalam Transaksi Bitcoin

Dalam Bitcoin, setiap transaksi diubah menjadi hash sebelum ditambahkan ke blockchain. Hash adalah sidik jari digital unik dari transaksi tersebut. Jika seseorang mencoba mengubah sedikit saja bagian dari transaksi, hash akan berubah total. Ini memudahkan jaringan untuk mendeteksi adanya perubahan.

###### Peran Hashing dalam Keamanan Bitcoin

Hashing membantu melindungi jaringan Bitcoin dengan membuat transaksi mudah diverifikasi dan mustahil untuk diam-diam diubah. Karena setiap transaksi memiliki hash unik, jaringan dapat dengan cepat mendeteksi jika ada yang diubah.

Fungsi hash menerima data dan mengubahnya menjadi rangkaian angka dan huruf tetap yang disebut hash. Input yang sama akan selalu menghasilkan hash yang sama, tetapi perubahan sekecil apa pun pada input akan menghasilkan hasil yang benar-benar berbeda. Sifat ini memungkinkan komputer memeriksa bahwa data tidak diubah.


> **Definition – Definisi Hashing**
>
> **Hashing** itu seperti membuat sidik jari untuk data digital. Ini adalah proses mengambil pesan digital dan mengubahnya menjadi kode dengan panjang tetap, yang berfungsi sebagai pengenal unik. Seperti sidik jari dapat mengidentifikasi seseorang, hash dapat mengidentifikasi pesan digital.


Output**output**, atau hash, selalu memiliki panjang yang sama, tidak peduli seberapa panjang informasi aslinya. Bitcoin menggunakan beberapa jenis fungsi hash tertentu yang disebut **SHA-256** dan **RIPEMD160**.

Beberapa contoh di bawah ini:

* Hash SHA256 dari string **halo dunia**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* Hash SHA256 dari string **halo dunia.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Perhatikan bahwa perubahan kecil pada input menghasilkan output yang benar-benar berbeda jika dibandingkan dengan yang pertama
* Hash SHA256 dari file iso yang dapat diunduh **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Input ini adalah file yang sangat besar namun outputnya tetap memiliki panjang tetap

Anda juga bisa membayangkan hashing seperti partitur musik yang menangkap esensi dari sebuah lagu. Seperti halnya partitur adalah representasi unik dari sebuah melodi, nilai hash adalah representasi unik dari sebuah data.

Dengan membandingkan partitur sebuah lagu dengan penampilan aslinya, seorang musisi dapat menentukan apakah penampilannya akurat. Demikian pula, dengan membandingkan nilai hash dari data yang diterima dengan nilai hash aslinya, seseorang dapat menentukan apakah data tersebut telah diubah selama transmisi.

Seperti halnya sedikit penyimpangan dalam penampilan musik dapat membuatnya terdengar berbeda, bahkan perubahan terkecil pada data asli akan menghasilkan nilai hash yang berbeda. Ini membuat hashing menjadi alat yang kuat untuk memastikan integritas dan keaslian transaksi Bitcoin.

Proses pengkodean **public key** melalui hashing digunakan untuk meningkatkan keamanan informasi dengan mengubahnya menjadi format tetap yang tidak dapat dibaca. Bitcoin menggunakan algoritma SHA-256 dan RIPEMD160 untuk menghasilkan alamat publik. Output yang dihasilkan berfungsi sebagai pengenal unik untuk **public key** dan membantu memastikan integritas serta keamanan transaksi yang disimpan di buku besar. Dengan mengenkripsi informasi seperti ini, menjadi lebih sulit bagi pihak yang tidak berwenang untuk mengakses dan memanipulasi data.

##### Sifat-sifat fungsi hashing

* **Deterministik**: Bahan yang sama selalu menghasilkan smoothie yang sama. Dengan cara yang sama, data yang sama akan selalu menghasilkan hash yang sama.
* **Pre-image resistance**: Jika Anda hanya memiliki smoothie-nya, Anda tidak dapat mengetahui buah apa saja yang digunakan. Demikian juga, jika Anda hanya memiliki hash, Anda tidak dapat menentukan data aslinya.
* **Efek avalanche**: Mengubah sedikit saja bahan akan menghasilkan smoothie yang benar-benar berbeda. Dalam hashing, perubahan sangat kecil pada data menghasilkan hash yang benar-benar berbeda.
* **Collision resistance**: Sangat sulit menemukan dua set bahan berbeda yang menghasilkan smoothie yang persis sama. Dengan cara yang sama, sangat kecil kemungkinannya dua data berbeda menghasilkan hash yang sama.
* **Cepat untuk diverifikasi**: Membuat smoothie itu cepat, dan mudah untuk memeriksa bahwa hasilnya memang smoothie. Fungsi hash cepat dihitung dan mudah diverifikasi oleh siapa saja.

#### Aktivitas: Hasilkan Hash SHA 256

https://tools.keycdn.com/sha256-online-generator

Penasaran bagaimana hashing bekerja? Pindai kode QR untuk langsung menghasilkan hash SHA256 dari kata, kalimat, atau input apa pun yang Anda pilih. Fungsi hash seperti sidik jari digital: mereka satu arah, artinya setelah sesuatu di-hash, tidak bisa dibalik. Coba sendiri dan lihat hasilnya!
