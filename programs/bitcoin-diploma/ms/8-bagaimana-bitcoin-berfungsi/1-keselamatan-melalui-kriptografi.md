# 8.1 Keselamatan melalui Kriptografi

> Apa yang Bitcoin berikan kepada kita ialah satu janji yang kukuh: program ini akan dijalankan tepat seperti yang ditetapkan.  
_Andreas M. Antonopoulos_

#### Kriptografi Kunci Awam/Peribadi


> **Definition – Definisi Kriptografi**
>
> **Kriptografi** ialah amalan menukar maklumat menjadi rahsia yang hanya boleh dibaca oleh orang yang betul.


* **Penyulitan** ialah proses menukar maklumat menjadi bentuk berkod supaya hanya seseorang yang mempunyai kunci yang betul boleh membacanya.
* **Penyahsulitan** ialah proses menukar maklumat berkod itu kembali menjadi sesuatu yang boleh dibaca.

Dalam kriptografi tradisional, dua orang yang ingin berkomunikasi secara peribadi mesti terlebih dahulu berkongsi kunci rahsia yang sama, seperti kata laluan bersama. Seseorang menggunakan kunci ini untuk menyulitkan mesej sebelum menghantarnya, dan orang lain menggunakan kunci yang sama untuk menyahsulit dan membacanya.

Masalah dengan sistem ini ialah kedua-dua orang mesti sudah berkongsi kunci rahsia itu. Jika orang lain mendapat akses kepada kunci itu, mereka boleh membaca mana-mana mesej yang dipintas.

Bitcoin menyelesaikan masalah ini dengan menggunakan pendekatan berbeza yang dipanggil kriptografi kunci awam, di mana pengguna tidak perlu berkongsi kunci rahsia terlebih dahulu.

Kriptografi kunci awam/peribadi menyelesaikan masalah perkongsian rahsia. Sebaliknya berkongsi kata laluan, setiap orang mempunyai dua kunci: kunci awam dan kunci peribadi.

* Kunci **awam** boleh dikongsi dengan sesiapa sahaja.
* Kunci **peribadi** mesti sentiasa dirahsiakan.

Jika Johan ingin menghantar sesuatu kepada Arel, dia boleh menggunakan kunci awam Arel. Hanya Arel boleh membukanya menggunakan kunci peribadinya. Walaupun seseorang memintas mesej itu, mereka tidak boleh membacanya atau menggunakannya tanpa kunci peribadi.

Dalam Bitcoin, sistem ini digunakan untuk mencipta tandatangan digital. Tandatangan digital membuktikan bahawa pemilik kunci peribadi telah meluluskan transaksi, sama seperti menandatangani nama anda pada dokumen. Inilah yang membolehkan transaksi Bitcoin menjadi selamat dan boleh disahkan tanpa mempercayai pihak ketiga.

Transaksi Bitcoin melibatkan pemindahan pemilikan bitcoin dari satu alamat ke alamat lain.

Penyulitan digunakan untuk memastikan hanya pemilik sebenar bitcoin mempunyai kuasa untuk menghantar wang mereka kepada orang lain. Ia memastikan harta mereka dilindungi daripada pihak berniat jahat.

Sebagai langkah perlindungan tambahan, setiap transaksi Bitcoin secara automatik mendapat tandatangan digital yang UNIK. Tandatangan digital unik ini dikuasakan oleh teknologi kalis gangguan yang membantu rangkaian mengesahkan bahawa pemilik sebenar bitcoin, dan bukannya orang lain, telah menghantarnya.


> **Dark**
>
> Setiap pengguna mempunyai dua kunci: satu **kunci peribadi**, yang **dirahsiakan**, dan satu **kunci awam** yang boleh **dikongsi dengan orang lain**. Kunci **peribadi** berfungsi sebagai bentuk pengenalan dan bukti pemilikan, mengesahkan: “Alamat ini milik saya dan saya mengawalnya.”


###### Bagaimana Transaksi Bitcoin Berfungsi

1. **Mencipta Transaksi**: Pengguna memulakan transaksi Bitcoin dengan menentukan butiran seperti alamat penerima dan jumlah bitcoin yang akan dihantar.
1. **Penjanaan Tandatangan Digital**: Penghantar menjana satu **tandatangan digital** yang unik menggunakan **kunci peribadi**. Tandatangan ini ialah kod unik yang mengesahkan ketulenan transaksi.
1. **Penyiaran Transaksi**: Transaksi yang telah ditandatangani disiarkan ke rangkaian Bitcoin, menandakan niat untuk memindahkan pemilikan bitcoin daripada penghantar kepada penerima.
1. **Pengesahan di Rangkaian**: Nod pada rangkaian Bitcoin menerima transaksi dan menggunakan **kunci awam** untuk mengesahkan keaslian tandatangan. transaksi tersebut. Pada masa yang sama, mereka menggunakan **kunci awam** untuk mengesahkan **tandatangan digital**.
1. **Pengesahan di rangkaian Bitcoin**: Jika pengesahan berjaya, transaksi akan ditambah ke lejar, yang berfungsi sebagai rekod semua transaksi yang selamat dan telus. Setelah disahkan, pemilikan bitcoin secara rasmi dipindahkan daripada penghantar kepada penerima.


> **Callout – Ringkasan**
>
> Tandatangan digital**tandatangan digital**, yang dicipta dengan **kunci peribadi** penghantar, membuktikan bahawa transaksi itu telah dibenarkan oleh pemilik bitcoin. Rangkaian Bitcoin kemudian boleh mengesahkan bukti ini dan merekodkan transaksi tersebut.


#### Penjelasan Mengenai Hashing

Jangan risau dengan istilah teknikal dan konsep matematik yang akan datang. Kami faham tidak semua orang meminati matematik, tetapi anda mungkin akan terkejut bahawa idea yang paling kompleks pun boleh difahami dengan sedikit usaha.


> **Definition – Definisi fungsi**
>
> Satu **fungsi** adalah seperti mesin yang mengambil maklumat dan menukarkannya kepada sesuatu yang baru. Maklumat yang anda berikan kepada fungsi itu ialah **input**. Maklumat baru yang dihasilkan oleh fungsi itu ialah **output**. Fungsi membantu komputer melakukan tugas dan menyelesaikan masalah.


##### Apakah itu fungsi?

Fungsi ialah satu set arahan yang mengambil input dan menghasilkan output. Anda boleh bayangkan seperti resipi: anda ikut langkah-langkah dengan bahan tertentu, dan anda sentiasa mendapat hasil yang boleh dijangka.

Dalam Bitcoin, fungsi digunakan untuk memproses dan mengesahkan transaksi. Apabila seseorang menghantar bitcoin, fungsi kriptografi membantu menyemak sama ada transaksi itu sah, mengesahkan bahawa penghantar mempunyai dana yang mencukupi, dan mengemas kini baki pada lejar Bitcoin. Setelah disahkan dan ditambah ke dalam blok, transaksi itu menjadi sebahagian daripada rekod kekal di blockchain.

##### Apakah itu fungsi sehala?

Fungsi sehala ialah sejenis fungsi khas yang mudah dikira dalam satu arah tetapi amat sukar untuk diterbalikkan. Sebagai contoh, mengisar bahan menjadi smoothie adalah mudah, tetapi anda tidak boleh memisahkan smoothie itu kembali kepada bahan asalnya.

Keselamatan Bitcoin bergantung kepada fungsi sehala. Ia digunakan dalam kriptografi kunci awam dan kunci peribadi, membolehkan orang berkongsi kunci awam sambil mengekalkan kunci peribadi secara rahsia. Walaupun kunci awam boleh dilihat, adalah mustahil untuk mendapatkan kunci peribadi daripadanya. Inilah yang menjadikan transaksi Bitcoin selamat.

##### Apakah itu fungsi hash?

Satu **fungsi hash** adalah seperti mesin kod rahsia. Ia mengambil satu mesej dan menukarkannya kepada satu kod.

###### Bagaimana Hashing Berfungsi dalam Transaksi Bitcoin

Dalam Bitcoin, setiap transaksi akan diubah menjadi hash sebelum ia ditambah ke blockchain. Hash ialah cap jari digital unik bagi transaksi tersebut. Jika sesiapa cuba mengubah walaupun sedikit bahagian transaksi, hash itu akan berubah sepenuhnya. Ini memudahkan rangkaian mengesan sebarang pengubahsuaian.

###### Peranan Hashing dalam Keselamatan Bitcoin

Hashing membantu melindungi rangkaian Bitcoin dengan menjadikan transaksi mudah untuk disahkan dan mustahil untuk diubah secara senyap. Oleh kerana setiap transaksi mempunyai hash uniknya sendiri, rangkaian boleh dengan cepat mengesan jika ada sesuatu yang telah diubah.

Fungsi hash mengambil data dan menukarkannya kepada rentetan tetap nombor dan huruf yang dipanggil hash. Input yang sama akan sentiasa menghasilkan hash yang sama, tetapi walaupun perubahan kecil pada input akan menghasilkan keputusan yang sangat berbeza. Sifat ini membolehkan komputer menyemak bahawa data tidak diubah.


> **Definition – Definisi Hashing**
>
> **Hashing** adalah seperti mencipta cap jari untuk data digital. Ia adalah proses mengambil mesej digital dan menukarkannya kepada kod panjang tetap, yang berfungsi sebagai pengecam unik. Sama seperti cap jari boleh mengenal pasti seseorang, hash boleh mengenal pasti mesej digital.


Hasilnya**output**, atau hash, sentiasa mempunyai panjang yang sama, tidak kira berapa panjang maklumat asal. Bitcoin menggunakan beberapa jenis fungsi hash tertentu yang dipanggil **SHA-256** dan **RIPEMD160**.

Beberapa contoh adalah seperti di bawah:

* SHA256 hash bagi rentetan **hello world**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* Hash SHA256 bagi rentetan **hello world.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Perhatikan bahawa perubahan kecil pada input akan mengubah output sepenuhnya berbanding dengan yang pertama
* Hash SHA256 bagi fail iso yang boleh dimuat turun **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Input ini adalah fail yang sangat besar namun outputnya masih tetap panjang tetap

Anda juga boleh menganggap hashing seperti skor muzik yang menangkap inti pati sesebuah lagu. Seperti skor muzik adalah representasi unik bagi satu melodi, nilai hash adalah representasi unik bagi sesuatu data.

Dengan membandingkan skor muzik dengan persembahan sebenar, seorang pemuzik boleh menentukan sama ada persembahan itu tepat. Begitu juga, dengan membandingkan nilai hash data yang diterima dengan nilai hash asal, seseorang boleh menentukan sama ada data telah diubah semasa penghantaran.

Seperti juga sedikit penyimpangan dalam persembahan muzik boleh menyebabkan ia kedengaran berbeza, walaupun perubahan paling kecil pada data asal akan menghasilkan nilai hash yang berbeza. Ini menjadikan hashing alat yang berkuasa untuk memastikan integriti dan keaslian transaksi Bitcoin.

Proses pengekodan **kunci awam** melalui hashing digunakan untuk meningkatkan keselamatan maklumat dengan menukarkannya kepada format tetap yang tidak boleh dibaca. Bitcoin menggunakan algoritma SHA-256 dan RIPEMD160 untuk menghasilkan alamat awam. Output yang terhasil berfungsi sebagai pengecam unik untuk **kunci awam** dan membantu memastikan integriti serta keselamatan transaksi yang disimpan dalam lejar. Dengan menyulitkan maklumat dengan cara ini, ia menjadi lebih sukar untuk individu yang tidak dibenarkan mengakses dan memanipulasi data.

##### Ciri-ciri fungsi hashing

* **Deterministik**: Bahan yang sama sentiasa menghasilkan smoothie yang sama. Begitu juga, data yang sama akan sentiasa menghasilkan hash yang sama.
* **Rintangan pra-imej**: Jika anda hanya ada smoothie, anda tidak boleh mengetahui buah-buahan yang digunakan. Begitu juga, jika anda hanya ada hash, anda tidak boleh menentukan data asal.
* **Kesan avalan**: Mengubah walaupun sedikit bahan akan menghasilkan smoothie yang sangat berbeza. Dalam hashing, perubahan kecil pada data menghasilkan hash yang sangat berbeza.
* **Rintangan perlanggaran**: Amat sukar untuk mencari dua set bahan yang berbeza tetapi menghasilkan smoothie yang sama. Begitu juga, amat tidak mungkin dua data berbeza menghasilkan hash yang sama.
* **Cepat untuk disahkan**: Membuat smoothie adalah pantas, dan mudah untuk memeriksa bahawa hasilnya adalah smoothie. Fungsi hash adalah pantas untuk dikira dan mudah untuk sesiapa sahaja sahkan.

#### Aktiviti: Jana Hash SHA 256


https://tools.keycdn.com/sha256-online-generator

_SHA256 Online Generator_


Ingin tahu bagaimana hashing berfungsi? Imbas kod QR untuk serta-merta menjana hash SHA256 daripada mana-mana perkataan, ayat, atau input pilihan anda. Fungsi hash seperti cap jari digital: ia sehala, bermakna setelah sesuatu di-hash, ia tidak boleh diundur semula. Cubalah sendiri dan lihat hasilnya!
