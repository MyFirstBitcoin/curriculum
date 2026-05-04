# 2.7 Bitcoin sebenarnya tidak benar-benar terdesentralisasi

> Kerumitan kripto timbul daripada usaha untuk mendesentralisasikan—dengan mengagihkan kuasa dan tadbir urus dalam sistem, secara teorinya tidak perlu ada perantara yang dipercayai seperti institusi kewangan. Itulah premis kertas putih Bitcoin yang asal, yang menawarkan penyelesaian kriptografi bertujuan membolehkan pembayaran dihantar tanpa melibatkan mana-mana institusi kewangan atau perantara yang dipercayai. Namun, Bitcoin menjadi berpusat dengan sangat cepat dan kini bergantung kepada sekumpulan kecil pembangun perisian dan kolam perlombongan untuk berfungsi  
_Tabung Kewangan Antarabangsa_

Seperti yang ditunjukkan oleh petikan di atas daripada satu hantaran agak baru-baru ini oleh Tabung Kewangan Antarabangsa, industri kewangan arus perdana terus mendakwa bahawa Bitcoin tidak didesentralisasikan, serta mengelirukan Bitcoin dengan aset kripto lain.

##### Pengenalan

![Trilemma](https://cdn.sanity.io/images/vje9ehw2/staging/02eb7a58f46933df9b4daaa5cdcab6b9ba3b47d1-161x167.svg)

Desentralisasi adalah aspek kritikal bagi Bitcoin. Keupayaan untuk mengekalkan peraturan protokol seperti kekurangan dan pengagihan tanpa pihak berkuasa pusat memastikan ia boleh bertindak sebagai wang tanpa kebenaran untuk masyarakat global.

Seperti yang dinyatakan oleh Satoshi dalam surat-menyurat dalam taliannya, perkhidmatan terdesentralisasi seperti BitTorrent 'masih bertahan' terhadap tindakan keras Kerajaan, berbanding perkhidmatan yang mempunyai pemilik yang dikenalpasti dan pelayan terpusat. Beliau jelas bimbang tentang risiko potensi Kerajaan atau pihak berkepentingan lain menutup atau menjejaskan Bitcoin.

Dalam konteks ini, kita berminat dengan desentralisasi bagi:

* Pembangunan dan pengurusan kod yang menjalankan protokol; siapa yang dibenarkan mengubah peraturan?
* Fungsi perlombongan yang mencipta blok baharu mengikut peraturan dan mengesahkan terhadap perbelanjaan berganda
* Nod yang mengesahkan transaksi untuk kesahihan dan menyimpan salinan blockchain

##### Pembangun

Bitcoin ialah protokol sumber terbuka yang sesiapa sahaja bebas untuk melihat, memuat turun, menyalin atau mencadangkan perubahan. Ia tersedia dalam pustaka GitHub, kod sumbernya telah dilancarkan pada asalnya pada tahun 2009 oleh Satoshi Nakamoto. Sesiapa sahaja bebas memuat turun kod dan menjalankan nod, di mana majoritinya menjalankan perisian Bitcoin Core asal, yang telah dikemas kini dari semasa ke semasa.

![How Does an idea Make Its Way Into Bitcoin Core?](https://cdn.sanity.io/images/vje9ehw2/staging/49f70d059c9dbe19a6e4500e9abd8db66ca97bff-1300x1439.png)

_Sumber: https://river.com/learn/what-is-bitcoin-core/_

Pembangunan Bitcoin Core mengikuti amalan terbaik pembangunan sumber terbuka. Pada bila-bila masa, boleh ada mana-mana bilangan pembangun yang menulis atau menyemak perubahan kod. Mereka perlu mendengar kebimbangan pengendali nod dan pelombong, serta pengguna sebelum membuat sebarang perubahan kritikal pada kod, yang akan disemak dan dipersetujui seperti yang ditunjukkan dalam carta alir di atas sebelum dimasukkan ke dalam kod.

Peraturan Bitcoin kemudiannya dikodkan dalam perisian Bitcoin Core ini, yang dijalankan pada setiap nod. Sesiapa sahaja boleh mencadangkan perubahan pada peraturan – peraturan itu adalah kod, tetapi ia bukanlah_hanya_kod, ia adalah_kod yang dipersetujui_Jika diubah secara sepihak, kod baharu itu tidak lagi menjadi sebahagian daripada konsensus dan tidak lagi menjadi sebahagian daripada Bitcoin. Mengubah sesuatu dalam Bitcoin dan kekal dalam konsensus adalah rumit. Cadangan perubahan pada kod jatuh dalam salah satu daripada tiga kategori:

* Dalam peraturan sedia ada: Naik taraf kecil seperti kesilapan ejaan, antara muka pengguna yang lebih baik atau pengurusan data mungkin jatuh dalam kategori ini dan agak mudah untuk mendapat kelulusan.
* Menambah peraturan baharu yang menambah sekatan pada peraturan – seperti mengurangkan saiz blok. Ini dirujuk sebagai 'soft fork'. Nod yang memilih untuk tidak melaksanakan perubahan kod dan kekal pada keluaran lama masih boleh mengambil bahagian dalam rangkaian.
* Menambah peraturan baharu yang melanggar peraturan semasa, contohnya peningkatan saiz blok. Nod yang tidak menaik taraf kepada kod baharu akan menolak blok yang dicipta dengan saiz lebih besar sebagai tidak sah. Ini dirujuk sebagai 'hard fork' dan akan mewujudkan perpecahan rantaian antara nod yang menjalankan kod asal dan kod baharu serta mencipta syiling baharu. Ini pernah berlaku sebelum ini tetapi tidak membawa kejayaan jangka panjang untuk syiling baharu kerana majoriti nod memutuskan untuk kekal pada kod asal.

Oleh itu, satu pihak atau kumpulan orang tidak boleh mengubah kod Bitcoin secara sepihak tanpa mendapat persetujuan konsensus, atau mereka berisiko berlakunya perpecahan rantaian dan penciptaan syiling baharu yang mengikuti set peraturan berbeza.

##### Perlombongan

Fungsi perlombongan mengesahkan transaksi seperti mana-mana nod lain dalam rangkaian, tetapi ia kemudiannya akan menggunakan tenaga yang diperlukan untuk mencipta blok baharu yang memenuhi peraturan konsensus dalam kod. Kejayaan membolehkan pelombong memperoleh ganjaran dalam bentuk yuran transaksi dan ganjaran Bitcoin (pada masa penulisan 3.125 syiling setiap blok).

Perlombongan biasanya dijalankan oleh 'Pool' perlombongan di mana orang ramai menggabungkan kuasa perlombongan atau kadar hash bersama-sama untuk meningkatkan peluang melombong blok dengan berjaya dan berkongsi ganjaran. Terdapat bahaya bahawa satu atau lebih pool perlombongan ini boleh bergabung untuk mencapai dominasi 51% dalam perlombongan dan pada dasarnya menolak protokol pengesahan rangkaian memihak kepada mereka untuk membelanjakan syiling dua kali. Ini memerlukan sejumlah besar sumber untuk dicapai dengan kos yang tinggi, dan pelombong individu boleh dengan mudah berpindah ke pool perlombongan lain pada bila-bila masa. Serangan seperti ini juga mungkin menyebabkan nilai bitcoin jatuh, kerana jelas bahawa integriti rangkaian telah terjejas. Penyerang oleh itu perlu menukar mana-mana bitcoin yang diperoleh dengan cepat kepada fiat sebelum nilainya merosot. Ini menjadikannya lebih sukar untuk mengekalkan serangan dalam tempoh yang lama, dan oleh itu lebih menguntungkan bagi pelombong atau pengendali pool untuk mematuhi peraturan dan cuba melombong blok yang sah.

Taburan geografi fungsi perlombongan juga penting untuk mengelakkan kerajaan contohnya mengambil alih kapasiti perlombongan atau menutupnya. Sebagai contoh, larangan perlombongan baru-baru ini oleh China menunjukkan keupayaan Bitcoin untuk menyesuaikan diri dan bertahan daripada campur tangan kerajaan seperti itu, menyesuaikan diri dan pulih dengan cepat daripada kehilangan kuasa hash yang berlaku.

##### Nod

Tidak seperti perlombongan, yang memerlukan pelaburan kewangan yang besar untuk bersaing secara berkesan dalam perlumbaan melombong blok baharu, atau pembangunan kod yang memerlukan kepakaran pengekodan, menjalankan nod adalah sesuatu yang sesiapa sahaja yang berminat untuk membantu mengekalkan desentralisasi Bitcoin boleh lakukan.

Nod menjalankan perisian Bitcoin Core dan menguatkuasakan peraturan yang terkandung dalam kod untuk memastikan pelombong tidak menipu, contohnya dengan memberikan diri mereka ganjaran blok yang lebih besar daripada yang dibenarkan. Mereka juga menguatkuasakan had bekalan 21 juta, yang penting untuk mengekalkan kekurangan Bitcoin. Untuk mana-mana kerajaan atau pihak jahat menghentikan Bitcoin, mereka perlu memusnahkan setiap salinan blockchain, yang kini dijalankan di ribuan nod yang diedarkan di seluruh dunia, satu tugas yang hampir mustahil.

##### Orang

Satu lagi aspek potensi pemusatan ialah orang. Setiap 'alt-coin' lain mempunyai tokoh utama—seseorang yang boleh dipaksa untuk menyokong perubahan yang tidak memihak kepada Bitcoin. Satoshi Nakamoto kekal cukup lama untuk memastikan Bitcoin berada di landasan kejayaan sebelum menghilang untuk selama-lamanya, meninggalkannya di tangan orang lain untuk menambah baik dan menyesuaikan perisian.

Bagaimana pula dengan pemegang Bitcoin dalam jumlah besar? Pelabur awal, yang telah menyimpan syiling mereka dan tidak kehilangannya, akan menjadi sangat kaya pada ketika ini. Penting untuk diperhatikan bahawa ini mungkin benar, tetapi itu tidak memberi mereka lebih banyak pengaruh dalam sistem berbanding orang lain, tidak seperti syiling 'proof of stake' di mana pelopor yang sudah kaya dalam syiling itu mendapat kelebihan dalam membuat keputusan dan pengagihan syiling masa depan. Ini telah atau pasti akan membawa kepada pemusatan dari masa ke masa.

##### Kesimpulan

Apakah ancaman berpotensi yang boleh cuba dikurangkan oleh desentralisasi?

* Kerajaan menutup atau mengharamkan Bitcoin
* Perubahan kod yang tidak diingini yang memihak kepada satu pihak berkepentingan dalam Bitcoin, contohnya meningkatkan ganjaran blok
* Paksaan terhadap protokol oleh kerajaan atau pihak jahat untuk mempengaruhi hala tuju protokol
* Keupayaan sekumpulan pelombong untuk mengambil alih rangkaian dan 'double-spend' Bitcoin – serangan 51%

Seperti yang kita lihat, gabungan nod, pembangun kod dan pelombong, serta penggunaan mekanisme 'proof of work', mendesentralisasikan Bitcoin ke tahap yang mencukupi di mana ancaman berpotensi ini tidak dianggap sebagai kebimbangan besar. Komuniti perlu terus memantau keadaan untuk memastikan perkara ini kekal.
