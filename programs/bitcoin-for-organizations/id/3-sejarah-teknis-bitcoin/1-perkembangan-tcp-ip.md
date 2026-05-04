# 3.1 Perkembangan TCP/IP

Sebagian besar dari kita sudah akrab dengan protokol TCP/IP yang digunakan saat ini sebagai fondasi internet. Asal-usulnya bermula pada akhir tahun 70-an ketika para ilmuwan mengeksplorasi desain alternatif untuk Arpanet – jaringan yang bahkan lebih awal yang dirancang oleh Departemen Pertahanan AS untuk memungkinkan berbagi sumber daya antar komputer jarak jauh. TCP/IP menjadi standar protokol untuk Arpanet pada tahun 1983, yang kemudian membuatnya menjadi model jaringan yang dominan pada akhir tahun 1990-an dan menjadi fondasi bagi internet tempat Bitcoin berjalan saat ini.


| Model OSI | TCP/IP |
| --- | --- |
| Aplikasi | Aplikasi |
| Presentasi | Aplikasi |
| Sesi | Aplikasi |
| Transport | Transport |
| Jaringan | Jaringan |
| Data Link | Data Link |
| Fisik | Fisik |


Pada saat yang sama ketika model TCP/IP sedang dikembangkan, kerangka kerja serupa namun lebih komprehensif juga sedang dikembangkan oleh International Standards Organisation (ISO) dan industri Telekomunikasi (CCITT). Proses untuk mengembangkan protokol baru atau mengusulkan perubahan berjalan lambat dan rumit dibandingkan dengan pendekatan yang lebih terdesentralisasi yang digunakan untuk mengembangkan TCP/IP, sehingga pendekatan ini menjadi dominan hingga hari ini.

##### Permintaan Perubahan

Setiap pengembangan yang diusulkan terhadap protokol yang ada atau ide untuk protokol baru dapat diajukan dalam model TCP/IP melalui **Permintaan Perubahan** proses. Proses ini melalui tahapan persetujuan, yang dikelola oleh Internet Engineering Task Force (IETF), dan menjadi open source setelah disetujui agar siapa pun dapat mengimplementasikan dan mengadopsinya. Beberapa contoh penting:

* 1969 RFC 1 Mendokumentasikan bagaimana paket akan dikirim di Arpanet
* 1981 RFC791 mendefinisikan protokol Internet V4 – masih banyak digunakan hingga saat ini
* 1982 RFC 821 Simple Mail Transfer Protocol
* 1987 Domain Name System – bagaimana nama domain dihubungkan ke alamat IP
* 1999 RDC 2616 Hypertext Transfer Protocol – penting untuk menjelajah web


> **Callout**
>
> The **Usulan Peningkatan Bitcoin** (BIP) mengikuti pendekatan yang mirip dengan RFC, namun berfokus murni pada peningkatan Bitcoin itu sendiri, bukan pada pengembangan protokol baru atau alternatif. Bitcoin juga mengadopsi model berlapis ini, dan Anda akan melihat protokol tambahan yang dijelaskan sebagai lapisan dua atau tiga.


Dengan cara yang sama seperti lapisan dasar model TCP/IP yang relatif sedikit berubah dalam beberapa dekade terakhir, dengan inovasi terjadi di lapisan yang lebih tinggi, lapisan dasar Bitcoin juga diperkirakan akan berubah sangat lambat pada titik ini, dengan solusi penskalaan seperti Lightning dan Liquid terjadi di atasnya.

Contoh yang baik tentang bagaimana protokol lapisan dasar menjadi sulit diubah seiring waktu adalah IPv6. Perkiraan habisnya ruang alamat pada IPv4 menciptakan kebutuhan akan protokol baru. Standar draf pertama dibuat pada tahun 1998, tetapi baru diratifikasi sebagai standar internet pada tahun 2017. Meskipun IPv6 memecahkan banyak masalah pada IPv4 dan jauh lebih siap untuk masa depan, adopsinya di industri masih sangat lambat hingga hari ini. Selama waktu ini, banyak protokol baru telah didefinisikan di lapisan atas untuk mendukung multimedia, email, dan sebagainya.

##### Blok bangunan yang digunakan oleh Bitcoin

Pemisahan masalah interkonektivitas ini memungkinkan protokol dikembangkan secara independen dari lapisan di atas dan di bawahnya. Alih-alih harus menciptakan solusi ulang untuk setiap lapisan, jaringan Bitcoin dapat mengandalkan kemampuan dasar jaringan yang disediakan pada lapisan fisik dan data link.


| Lapisan | TCP/IP Asli |
| --- | --- |
| Aplikasi | Menggunakan Domain Name System (DNS) untuk mengidentifikasi node tetangga. Port 8333 menandakan protokol Bitcoin. |
| Transport | UDP untuk komunikasi FIBRE antar penambang untuk latensi rendah. TCP untuk komunikasi P2P antar node. |
| Transport | Routing TOR: Memungkinkan anonimitas dan privasi. Protokol Broadcast: Mengarahkan lalu lintas di seluruh jaringan. |
| Link | Beroperasi di atas media apa pun (misal, Ethernet, Wi-Fi, dll.) |
| Fisik | Transmisi fisik melalui nirkabel, Ethernet, atau antarmuka perangkat keras lainnya. |


##### Bitcoin adalah protokol netral untuk mentransfer nilai seperti halnya HTTPS adalah protokol untuk mentransfer informasi

* **HTTPS**: Situs Web Aman
* **SMTP**: Kirim Email
* **FTP**: Transfer file
* **DNS**: Kelola nama domain
* **BTC**: Menyimpan dan mentransfer nilai

Bitcoin memungkinkan nilai untuk dipindahkan secara andal dan tanpa memerlukan pihak ketiga antara orang atau perangkat di seluruh Internet. Hal ini diperkirakan akan membuka nilai yang sangat besar.
