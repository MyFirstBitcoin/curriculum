# 3.4 Hashcash

Hashcash telah dicipta oleh Adam Back, seorang lagi perintis awal dalam bidang ini. Adam sangat berminat terhadap pasaran bebas dan privasi di internet, dan menemui senarai mel Cypherpunks yang beliau sertai dan menjadi peserta aktif.

Beliau sangat berminat dengan wang digital, dan mencadangkan beberapa cara bagaimana kumpulan itu boleh bekerjasama dengan Chaum dalam DigiCash, tetapi cadangan-cadangan ini tidak ke mana. Kemudian, beliau memberi tumpuan kepada satu lagi masalah yang sedang muncul – spam emel. Beliau dan ahli Cypherpunks yang lain ingin mencari penyelesaian kepada masalah spam, di mana adalah terlalu mudah bagi spammer untuk mencipta dan menghantar ribuan emel yang menyumbat rangkaian. Penyelesaian inovatif beliau adalah berdasarkan hashing – keupayaan dalam kriptografi untuk menukar sebarang data kepada rentetan unik dan rawak dengan panjang tertentu, untuk mencipta 'setem' digital yang perlu ditambah pada emel supaya ia dianggap sah dan boleh dihantar melalui rangkaian. Kos yang kecil untuk emel sebenar, tetapi sangat membebankan bagi spammer.

Inovasi utama yang dicipta oleh Hashcash adalah mengaitkan sumber dunia sebenar – kuasa pengkomputeran – kepada rangkaian digital. Walaupun sumber digital sebelum ini boleh digandakan tanpa had, jumlah 'hashcash' yang dicipta dihadkan oleh berapa banyak tenaga yang sanggup dilaburkan oleh orang ramai.

Walaupun penyelesaian ini memenuhi beberapa kriteria yang Adam percaya diperlukan dalam sistem wang digital; ia adalah tanpa nama, tahan lasak dan tidak memerlukan kepercayaan, setiap hashcash tidak boleh digunakan semula dan tidak benar-benar terhad. Beliau mencadangkan cara lain untuk menangani isu-isu ini dengan menggunakan pihak ketiga luar.

##### BitGold

Nick Szabo membina konsep Hashcash dan bukti kerja untuk mencadangkan satu penyelesaian alternatif, yang beliau huraikan dalam satu senarai mel setahun selepas Hashcash diterbitkan, pada tahun 1998.

Walaupun semakin hampir kepada penyelesaian, cadangan ini masih mempunyai beberapa cabaran.

* Siapa yang akan mengendalikan Pendaftaran pemilikan hash dan bagaimana mereka boleh dipercayai?
* Hashing secara amnya akan menjadi lebih murah dari masa ke masa, satu cabaran untuk HashCash juga.

Oleh kerana hash yang dipautkan akan dicap masa, beliau mencadangkan satu bentuk penjejakan sejarah terhadap kesukaran hashing pada masa itu; hash yang lebih awal memerlukan lebih banyak kos pemprosesan berbanding yang kemudian kerana kos telah menurun. Malangnya, ini bermakna hash tidak akan 'boleh tukar ganti' iaitu mempunyai nilai yang sama, yang dianggap sebagai ciri utama wang digital. Untuk membantu menyelesaikan masalah ini, Nick mencadangkan satu bentuk 'perbankan bebas' yang berfungsi di atas BitGold yang boleh menggabungkan kumpulan hash yang berbeza supaya dinilai sama.

##### B-Money

Tidak lama selepas cadangan Bit Gold, Wei Dai mencadangkan penyelesaian yang serupa. Beliau telah pun membangunkan beberapa alat lain untuk Cypherpunks, dan mempunyai idea sendiri tentang wang digital.

Cadangan beliau menyerupai Bit Gold kerana ia menggunakan tandatangan digital untuk memindahkan wang, dan rekod transaksi akan disimpan dalam lejar, yang mengandungi kunci awam dan jumlah unit mata wang yang dikaitkan dengan setiap satu. Seperti Bit-Gold, pihak ketiga yang dipercayai dianggap sebagai kelemahan keselamatan, dan kepercayaan bahawa sistem wang elektronik tidak sepatutnya bergantung kepada satu entiti untuk menjejak baki, transaksi atau mengelakkan perbelanjaan berganda.

Wei Dai mencadangkan beberapa penyelesaian kepada isu-isu ini, salah satunya ialah daripada satu entiti pusat yang menyelenggara lejar, SEMUA nod akan menyimpan salinan. Jika semua pengguna menyemak lejar mereka sendiri dan kesahihan setiap transaksi, selagi semua nod sentiasa dikemas kini maka lejar akan kekal selaras di seluruh rangkaian. Sistem yang sangat teragih ini sukar untuk diganggu.

Wei Dai menyedari bahawa ini tidak menyelesaikan masalah jeneral Byzantine (1), kerana nod boleh dengan mudah kehilangan penyelarasan atau sekadar menipu. Beliau mencadangkan kaedah alternatif seperti mempunyai subset pelayan 'dipercayai' yang menyelenggara lejar, dan mewujudkan insentif kewangan untuk memastikan pelayan-pelayan ini jujur.

Untuk dasar kewangan, beliau mencadangkan kuasa beli B-Money dipautkan kepada satu bentuk indeks harga pengguna luaran. Beliau mahu jumlah B-Money yang sama boleh membeli bahagian yang sama dalam indeks itu dari masa ke masa, memberikan kestabilan harga. Jadi, sesiapa sahaja boleh menjana unit mata wang baru dengan menyediakan hash yang sah, tetapi kesukaran untuk menjana hash boleh berubah mengikut masa berdasarkan kos CPU dan indeks harga, supaya setiap unit akan menjadi 'tidak boleh diubah'.
