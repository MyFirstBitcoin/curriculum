# 3.2 Kriptografi Kunci Awam dan Protokol

Internet hari ini, dan kebanyakan sistem komputer moden, bergantung pada kriptografi, iaitu kaedah menyembunyikan maklumat supaya hanya penerima maklumat tersebut boleh menyahkodnya. Asas-asas kriptografi yang digunakan untuk mengamankan Bitcoin boleh dikesan kembali ke tahun 70-an.

Isu pertama yang perlu diselesaikan ialah – bagaimana untuk menghantar rahsia bersama melalui medium yang tidak selamat.

Perkara ini pertama kali dikaji oleh Whitfield Diffie dan Martin Hellman.

Masalahnya: dua pihak – biasanya dirujuk sebagai Alia dan Bob – ingin berkongsi maklumat rahsia melalui rangkaian di mana orang lain mungkin sedang mengintip. Untuk mencapai ini, mereka mencipta proses pertukaran kunci Diffie-Hellman.

Rahsia bersama ini kemudian boleh digunakan sebagai nilai benih untuk mencipta banyak kunci simetri untuk menyulit dan menyahkod mesej yang dihantar antara satu sama lain tanpa perlu berkongsi kunci itu secara terbuka.

Oleh kerana kunci peribadi tidak pernah perlu dikongsi, dan kunci yang berbeza digunakan di setiap hujung untuk menyulit dan menyahkod, ini dipanggil algoritma penyulitan asimetri.

Kes penggunaan:

* Alia menandatangani mesej dengan kunci awam Bob – hanya Bob yang boleh menyahkodnya menggunakan kunci peribadinya
* Alia menandatangani mesej dengan kunci peribadinya – dengan menyahkod menggunakan kunci awamnya, sesiapa sahaja boleh mengesahkan bahawa mesej itu dihantar oleh Alia, tanpa mengetahui kunci peribadinya
* Dengan menggabungkan kedua-dua pendekatan ini dengan dua lapisan penyulitan, satu mesej boleh dihantar dalam bentuk yang disulitkan supaya hanya Bob boleh menyahkodnya, dan dia kemudian boleh mengesahkan bahawa pengirimnya memang Alia

Walaupun tidak dikreditkan dalam kertas kerja tersebut, Ralph Merkle sangat berperanan dalam membantu menyelesaikan apa yang dianggap sebagai teka-teki yang tidak dapat diselesaikan sebelum ini – bagaimana untuk mewujudkan atau mewujudkan semula komunikasi peribadi melalui rangkaian terbuka dan berpotensi bermusuhan.

Pendekatan ini sendiri terdedah kepada serangan brute force, di mana penyerang boleh mengambil nombor yang dikongsi dan akhirnya mencipta semula kunci bersama jika diberikan masa dan sumber yang mencukupi, jadi ia bukanlah jawapan yang lengkap secara sendirian.

##### Protokol untuk Sistem Kriptografi Kunci Awam

Selain menyumbang kepada sistem kunci awam Diffie-Hellman yang diterangkan di atas, **Ralph Merkle** terus menyumbang dalam bidang ini selama bertahun-tahun, dan sangat berperanan dalam pembangunan beberapa komponen utama yang digunakan oleh Bitcoin.

Fungsi hash kriptografi ialah algoritma matematik yang mengambil input bersaiz apa pun dan memproses pengiraan kompleks untuk menghasilkan nilai hash dalam bit, yang biasanya diwakili oleh output alfanumerik panjang tetap menggunakan format heksadesimal.

* Input boleh bersaiz apa sahaja
* Output sentiasa mempunyai panjang tetap dan deterministik (input yang sama menghasilkan hash yang sama setiap kali)
* Ia mudah untuk disahkan tetapi amat sukar untuk diterbalikkan prosesnya bagi menentukan input asal
* Sedikit perubahan pada data akan mengubah output sepenuhnya

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/5e46b2740cf1e2b7b0a505361457f8d0cd9a98b4-515x331.svg)

Hashing adalah bahagian penting dalam protokol Bitcoin. SHA-256, yang digunakan dalam Bitcoin, dicipta oleh NSA dan merupakan contoh algoritma hashing kriptografi.

* Setiap blok dalam rantaian di-hash supaya data tidak boleh diubah – memastikan integriti lejar teragih
* Hash yang dijana perlu memenuhi kriteria ‘Bukti kerja’ untuk dianggap sebagai blok yang sah
* Pokok Merkle – dengan menggunakan cabang dan hash kepada hash, pokok hash boleh membolehkan pengesahan set data besar dengan storan minimum
* Tandatangan dan Kunci Berasaskan Hash boleh digunakan untuk dompet, alamat dan kebenaran transaksi

Pengesahan teragih bagi status blockchain dan model lejar tambah-sahaja yang tahan semakan semula menjadi mungkin dengan penggunaan hash sehala. Fungsi hash menyediakan pendekatan yang boleh dipercayai dan deterministik untuk mengesahkan peristiwa pada lejar awam seperti Bitcoin tanpa model kepercayaan berpusat.

Keupayaan baharu dalam bidang kriptografi ini dijangka oleh penciptanya akan membawa gelombang inovasi baharu dalam bidang ini.

##### Kriptografi lengkung eliptik

Salah satu inovasi kemudian datang dalam bentuk kriptografi lengkung eliptik.

Kriptografi lengkung eliptik diperkenalkan pada tahun 1985 oleh dua saintis, N. Koblitz dan V. Miller. Mereka mencadangkan idea menggunakan titik-titik yang ditakrifkan oleh lengkung eliptik dan bukannya medan perdana terhingga supaya andaian masalah Logaritma Diskret kekal, seperti yang biasa digunakan dalam protokol pertukaran kunci Diffie-Hellman standard. Perincian bagaimana ia berfungsi adalah di luar skop bahagian ini, tetapi secara ringkasnya, lengkung eliptik ialah set titik yang memenuhi persamaan matematik tertentu.

Persamaan untuk lengkung eliptik kelihatan seperti:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

Ini mempunyai beberapa ciri berguna:

* Simetri mendatar. Mana-mana titik pada lengkung boleh dipantulkan ke atas paksi-x dan masih berada pada lengkung yang sama.
* sebarang garis bukan menegak akan memotong lengkung pada maksimum tiga tempat.
* Saiz kunci yang padat adalah penting untuk penyimpanan dan penghantaran kunci awam yang cekap dalam blockchain.

Ciri-ciri ini boleh digunakan untuk mencipta pasangan kunci dengan cara yang serupa dengan algoritma Diffie-Hellman. Bitcoin menggunakan ECDSA, singkatan kepada Elliptic Curve Digital Signature Algorithm. Ia adalah proses yang menggunakan lengkung eliptik dan medan terhingga untuk "menandatangani" data dengan cara pihak ketiga boleh mengesahkan keaslian tandatangan tersebut sementara penandatangan mengekalkan keupayaan eksklusif untuk mencipta tandatangan itu. Dengan bitcoin, data yang ditandatangani ialah transaksi yang memindahkan pemilikan.

Bahagian 'terhingga' adalah serupa dengan pendekatan 'mod' dalam Diffie-Hellman, di mana output persamaan dibahagi dan bakinya digunakan untuk memastikan ia berada dalam julat nombor tertentu.
