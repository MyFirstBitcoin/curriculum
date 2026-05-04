# 3.1 Perkembangan TCP/IP

Kebanyakan daripada kita sudah biasa dengan protokol TCP/IP yang digunakan hari ini sebagai asas kepada internet. Asal-usulnya bermula pada akhir tahun 70-an apabila para saintis meneroka reka bentuk alternatif kepada Arpanet – rangkaian yang lebih awal lagi yang diwujudkan oleh Jabatan Pertahanan A.S. untuk membolehkan perkongsian sumber antara komputer yang jauh. TCP/IP menjadi piawaian protokol untuk Arpanet pada tahun 1983, yang membawa kepada penguasaannya sebagai model rangkaian utama menjelang akhir tahun 1990-an dan menjadi asas kepada internet yang digunakan oleh Bitcoin hari ini.


| Model OSI | TCP/IP |
| --- | --- |
| Aplikasi | Aplikasi |
| Persembahan | Aplikasi |
| Sesi | Aplikasi |
| Pengangkutan | Pengangkutan |
| Rangkaian | Rangkaian |
| Pautan Data | Pautan Data |
| Fizikal | Fizikal |


Pada masa yang sama model TCP/IP sedang dibangunkan, satu rangka kerja yang serupa tetapi lebih menyeluruh sedang dibangunkan oleh Pertubuhan Piawaian Antarabangsa (ISO) dan industri Telekomunikasi (CCITT). Proses untuk membangunkan protokol baru atau mencadangkan perubahan adalah perlahan dan rumit berbanding pendekatan yang lebih terdesentralisasi yang digunakan untuk membangunkan TCP/IP, menyebabkan pendekatan ini menjadi dominan hari ini.

##### Permintaan Perubahan

Sebarang pembangunan yang dicadangkan kepada protokol sedia ada atau idea untuk yang baru boleh dicadangkan dalam model TCP/IP melalui **Permintaan Perubahan** proses. Ia melalui proses kelulusan, yang diuruskan oleh Internet Engineering Task Force (IETF), dan menjadi sumber terbuka setelah diluluskan supaya sesiapa sahaja boleh melaksana dan menggunakannya. Beberapa contoh penting:

* 1969 RFC 1 Mendokumentasikan bagaimana paket akan dihantar dalam Arpanet
* 1981 RFC791 mentakrifkan protokol Internet V4 – masih digunakan secara meluas hari ini
* 1982 RFC 821 Protokol Pemindahan Mel Mudah
* 1987 Sistem Nama Domain – bagaimana nama domain diselesaikan kepada alamat IP
* 1999 RDC 2616 Protokol Pemindahan Hiperteks – penting untuk melayari web


> **Callout**
>
> The **Bitcoin Improvement Proposal** (BIP) mengikuti pendekatan yang serupa dengan RFC, tetapi memberi tumpuan sepenuhnya kepada penambahbaikan untuk Bitcoin itu sendiri dan bukannya pembangunan protokol baru atau alternatif. Bitcoin juga mengambil inspirasi daripada model berlapis ini, dan anda akan melihat protokol tambahan yang digambarkan sebagai lapisan dua atau tiga.


Sama seperti lapisan asas model TCP/IP yang berubah sangat sedikit dalam beberapa dekad kebelakangan ini, dengan inovasi berlaku di lapisan lebih tinggi, lapisan asas Bitcoin dijangka berubah dengan sangat perlahan pada ketika ini, dengan penyelesaian penskalaan seperti Lightning dan Liquid berlaku di atasnya.

Contoh yang baik bagaimana protokol lapisan asas menjadi sukar untuk diubah dari masa ke masa ialah IPv6. Jangkaan kehabisan ruang alamat dalam IPv4 mencipta permintaan untuk protokol baru. Draf piawaian pertama dicipta pada tahun 1998, tetapi hanya disahkan sebagai piawaian internet pada tahun 2017. Walaupun ia menyelesaikan banyak masalah dengan IPv4 dan jauh lebih tahan masa depan, ia masih mengalami kadar penggunaan yang sangat perlahan dalam industri hari ini. Dalam tempoh ini, banyak protokol baru telah ditakrifkan di lapisan atas untuk membolehkan multimedia, e-mel dan sebagainya.

##### Blok binaan yang digunakan oleh Bitcoin

Pemecahan masalah keterhubungan ini membolehkan protokol dibangunkan secara bebas daripada lapisan di atas dan di bawahnya. Daripada perlu mencipta semula penyelesaian untuk setiap lapisan, rangkaian Bitcoin boleh bergantung kepada keupayaan asas rangkaian yang disampaikan di lapisan fizikal dan pautan data.


| Lapisan | TCP/IP Asal |
| --- | --- |
| Aplikasi | Menggunakan Sistem Nama Domain (DNS) untuk mengenal pasti nod jiran. Port 8333 menandakan protokol Bitcoin. |
| Pengangkutan | UDP untuk komunikasi FIBRE antara pelombong bagi kependaman rendah. TCP untuk komunikasi P2P antara nod. |
| Pengangkutan | Penghalaan TOR: Membolehkan anonimiti dan privasi. Protokol Siaran: Menghala trafik merentasi rangkaian. |
| Pautan | Beroperasi melalui mana-mana medium (cth., Ethernet, Wi-Fi, dll.) |
| Fizikal | Penghantaran fizikal melalui tanpa wayar, Ethernet, atau antara muka perkakasan lain. |


##### Bitcoin ialah protokol neutral untuk memindahkan nilai seperti HTTPS ialah protokol untuk memindahkan maklumat

* **HTTPS**: Laman Web Selamat
* **SMTP**: Hantar Emel
* **FTP**: Pindahkan fail
* **DNS**: Urus nama domain
* **BTC**: Simpan dan pindahkan nilai

Bitcoin membolehkan nilai dipindahkan dengan boleh dipercayai dan tanpa memerlukan pihak ketiga antara individu atau peranti di seluruh Internet. Ini dijangka akan membuka nilai yang sangat besar.
