# 3.7 Bitcoin

Selepas bertahun-tahun dan banyak percubaan yang gagal, kebanyakan Cypherpunks mula hilang minat terhadap idea mata wang digital tanpa kebenaran, apabila Adam Back menerima emel yang mengandungi pautan kepada draf kertas putih bertajuk 'electronic cash without a third party' daripada seorang individu tanpa nama yang memperkenalkan dirinya sebagai Satoshi Nakamoto.

Untuk merumuskan setakat ini, kita sudah mempunyai sekurang-kurangnya idea-idea berikut:

* Tandatangan kriptografi yang boleh memberikan tahap privasi dan anonimitas
* Konsep mata wang tanpa sandaran (B-Money)
* Cadangan (tetapi tiada cara) untuk mengehadkan pengeluaran mata wang baharu
* Syiling digital yang pemilikannya ditentukan oleh kunci awam (B-Money) dan boleh dipindahkan dengan menandatangani serta dialihkan berdasarkan alamat penerima (RPOW dan Hashcash)
* Semua nod menyimpan salinan lejar yang diedarkan sepenuhnya (B-Money) (pada masa itu dianggap tidak praktikal)
* Protokol penandaan masa– menggunakan penghashan pokok Merkle untuk menyediakan kronologi peristiwa yang boleh dibuktikan secara matematik dan sukar dipalsukan jika semua pengguna menyimpan rekod yang sama
* Bukti kerja untuk mengaitkan usaha dunia sebenar kepada sistem (tetapi menggunakan hash itu sendiri sebagai mata wang)
* Rangkaian yang benar-benar terdesentralisasi di mana semua rakan setara dan boleh masuk serta keluar dari rangkaian (BitTorrent)
* Konsep mengaitkan hash baharu kepada hash sebelumnya (Bit Gold dan penandaan masa)

Apa yang masih kurang pada masa ini termasuklah:

* Penyelesaian yang berdaya maju untuk menyelesaikan masalah 'Byzantine generals'
* Kaedah untuk mengehadkan jumlah wang dalam edaran walaupun perkakasan sentiasa bertambah baik
* Skim insentif untuk orang ramai mengambil bahagian (isu ayam dan telur)

Perbezaan utama lain antara percubaan terkini dan Bitcoin ialah Satoshi telah bekerja pada kod tersebut untuk beberapa waktu dalam semangat asal 'Cypherpunks write code' sebelum mengumumkannya di senarai mel, tidak seperti Bit Gold dan B-Money yang lebih bersifat konseptual.

Apakah inovasi yang membezakan Bitcoin daripada percubaan wang elektronik sebelum ini?

Bukti kerja akan digunakan sebagai mekanisme konsensus dan cara untuk menyediakan keselamatan serta ketidakbolehubahan: Daripada menggunakan hash sebagai bentuk wang, ia akan digunakan melalui proses konsep baharu yang dipanggil perlombongan, di mana satu nod akan mengumpulkan satu set transaksi, menambah nombor rawak dan kemudian mengaplikasikan penghashan kepada 'blok' data. Blok yang sah yang memenuhi keperluan hash kemudian akan diiklankan kepada rangkaian. Blok-blok ini akan dihubungkan menggunakan hash blok sebelumnya dalam setiap satu, dan rantaian blok terpanjang akan digunakan sekiranya berlaku seri di mana nod berbeza mengesahkan dan mengiklankan blok berbeza pada masa yang sama sehingga berlaku perpecahan rantai. Bukti kerja menjadi penentu seri teragih untuk menyelesaikan masalah Byzantine generals.

Pelombong-pelombong ini juga diberikan insentif untuk menyediakan CPU yang diperlukan bagi menjalankan bukti kerja dengan diberikan bitcoin baharu untuk setiap blok. Jumlah Bitcoin yang mereka terima juga diprogramkan untuk berkurang kira-kira setiap 4 tahun sehingga semua Bitcoin telah dicipta, mewujudkan had maksimum kepada jumlah Bitcoin yang akan pernah berada dalam edaran iaitu 21 juta.

Idea paling asli ialah cara beliau menyelesaikan isu berapa banyak wang yang dicipta apabila perkakasan bertambah baik dan lebih kuasa boleh digunakan pada rangkaian. Penanda masa bagi sejumlah blok tertentu (2016) akan diambil purata, dan jika ia dicipta terlalu cepat, hash yang diperlukan untuk mencipta blok baharu akan menjadi lebih sukar, jika terlalu perlahan ia akan menjadi lebih mudah. Ini dibina dalam protokol terdesentralisasi yang dijalankan oleh semua nod dan mana-mana pelombong yang mengabaikannya akan membazir tenaga untuk melombong blok tanpa faedah kerana ia akan ditolak oleh seluruh rangkaian. Pelarasan ini memastikan penciptaan blok baharu kekal mengikut jadual pengeluaran yang dirancang, dan menyediakan insentif untuk pelombong 'bermain mengikut peraturan'.

####   
Ringkasan

Kebanyakan bahagian penting untuk membina sistem wang elektronik peer-to-peer terdesentralisasi berasaskan prinsip wang kukuh telah pun tersedia sebelum Satoshi mengeluarkan kertas putihnya dan tidak lama selepas pelepasan awal kod tersebut.

> Sifat Bitcoin adalah sedemikian rupa sehingga sebaik sahaja versi 0.1 dikeluarkan, reka bentuk terasnya telah ditetapkan untuk sepanjang hayatnya  
_Satoshi Nakamoto_

Walaupun banyak idea penambahbaikan (BIP) telah dicadangkan dan diterima pakai, Bitcoin telah beroperasi di belakang tabir sejak 2009 mengikut protokol yang direka dalam pelepasan awal dan hampir tiada gangguan. Semua penambahbaikan dibuat sambil mengekalkan keserasian ke belakang dengan semua versi terdahulu.



##### Nota

1. Untuk penjelasan mengenai masalah Byzantine Generals - lihat [https://ms.wikipedia.org/wiki/Byzantine_fault](https://en.wikipedia.org/wiki/Byzantine_fault)
