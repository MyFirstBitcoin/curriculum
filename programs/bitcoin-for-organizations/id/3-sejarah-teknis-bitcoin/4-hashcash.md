# 3.4 Hashcash

Hashcash diciptakan oleh Adam Back, salah satu inovator awal di bidang ini. Adam sangat tertarik pada pasar bebas dan privasi di internet, dan menemukan milis Cypherpunks yang kemudian ia ikuti dan menjadi peserta aktif di dalamnya.

Ia sangat tertarik pada uang digital, dan memberikan beberapa saran tentang bagaimana kelompok tersebut bisa bekerja lebih dekat dengan Chaum di DigiCash, namun hal ini tidak berkembang. Ia kemudian mengalihkan perhatiannya ke masalah baru yang muncul – spam email. Ia dan para Cypherpunks lainnya ingin menemukan solusi untuk masalah spam, di mana sangat mudah bagi spammer untuk membuat dan mengirim ribuan email yang memenuhi jaringan. Solusi inovatifnya didasarkan pada hashing – kemampuan dalam kriptografi untuk mengubah data apa pun menjadi rangkaian unik dan acak dengan panjang tertentu, untuk menciptakan semacam ‘prangko’ digital yang harus ditambahkan ke email agar dianggap sah dan dapat dikirimkan melalui jaringan. Biaya yang sepele untuk email asli, namun sangat memberatkan bagi spammer.

Inovasi utama yang diciptakan Hashcash adalah mengaitkan sumber daya dunia nyata – kekuatan komputasi – ke jaringan digital. Sementara sumber daya digital hingga saat itu dapat direplikasi tanpa batas, jumlah ‘hashcash’ yang dibuat dibatasi oleh seberapa banyak energi yang bersedia diinvestasikan orang.

Meskipun solusi ini memenuhi beberapa kriteria yang menurut Adam dibutuhkan dalam sistem uang digital; anonim, tahan banting, dan tanpa kepercayaan, setiap hashcash tidak dapat digunakan kembali dan tidak benar-benar langka. Ia mengusulkan cara lain untuk mengatasi masalah ini dengan menggunakan pihak ketiga eksternal.

##### BitGold

Nick Szabo membangun konsep Hashcash dan proof of work untuk mengusulkan solusi alternatif, yang ia jelaskan di sebuah milis setahun setelah Hashcash diterbitkan, pada tahun 1998.

Meskipun semakin mendekati solusi, usulan ini masih memiliki beberapa tantangan.

* Siapa yang akan menjalankan Registri kepemilikan hash dan bagaimana mereka bisa dipercaya?
* Hashing umumnya akan menjadi lebih murah seiring waktu, tantangan juga bagi HashCash.

Karena hash yang terhubung akan diberi cap waktu, ia mengusulkan semacam pelacakan historis terhadap tingkat kesulitan hashing pada saat itu; hash yang lebih awal akan membutuhkan biaya pemrosesan lebih besar daripada yang lebih baru karena biaya telah turun. Sayangnya, ini berarti hash tidak akan ‘fungible’ yaitu bernilai sama, yang dianggap sebagai atribut kunci uang digital. Untuk membantu mengatasi hal ini, Nick mengusulkan semacam ‘free banking’ yang bekerja di atas BitGold yang dapat menggabungkan kelompok hash berbeda agar nilainya sama.

##### B-Money

Tak lama setelah proposal Bit Gold, Wei Dai mengusulkan solusi serupa. Ia sudah mengembangkan beberapa alat lain untuk para Cypherpunks, dan memiliki gagasan sendiri tentang uang digital.

Usulannya mirip dengan Bit Gold karena menggunakan tanda tangan digital untuk mentransfer uang, dan catatan transaksi akan disimpan di buku besar, berisi kunci publik dan jumlah unit mata uang yang dikaitkan dengan masing-masing. Seperti Bit-Gold, pihak ketiga yang dipercaya dianggap sebagai celah keamanan, dan diyakini bahwa sistem uang elektronik tidak boleh bergantung pada satu entitas untuk melacak saldo, transaksi, atau mencegah pengeluaran ganda.

Wei-Dai mengusulkan beberapa solusi untuk masalah ini, salah satunya adalah daripada entitas pusat yang memelihara buku besar, SEMUA node akan memelihara salinannya. Jika semua pengguna memeriksa buku besar mereka sendiri dan validitas setiap transaksi, selama semua node tetap terbarui maka buku besar akan tetap tersinkronisasi di seluruh jaringan. Sistem yang sangat terdistribusi ini akan sulit untuk disabotase.

Wei Dai menyadari bahwa ini tidak menyelesaikan masalah jenderal Bizantium (1), karena node bisa saja kehilangan sinkronisasi atau sekadar berbohong. Ia mengusulkan metode alternatif seperti memiliki sebagian server ‘tepercaya’ yang memelihara buku besar, dan menciptakan insentif finansial agar server-server ini tetap jujur.

Untuk kebijakan moneter, ia mengusulkan agar daya beli B-Money dipatok pada semacam indeks harga konsumen eksternal. Ia ingin jumlah B-Money yang sama dapat membeli bagian yang sama dari indeks tersebut dari waktu ke waktu, memberikan stabilitas harga. Jadi, siapa pun dapat menghasilkan unit mata uang baru dengan menyediakan hash yang valid, namun tingkat kesulitan menghasilkan hash dapat berubah seiring waktu berdasarkan biaya CPU dan indeks harga, sehingga setiap unit akan menjadi ‘tidak dapat diubah’.
