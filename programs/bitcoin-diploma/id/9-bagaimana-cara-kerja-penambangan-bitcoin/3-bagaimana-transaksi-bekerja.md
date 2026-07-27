# 9.3 Bagaimana Transaksi Bekerja

Sekarang setelah Anda memahami kunci publik dan privat, serta peran node dan penambang, berikut adalah cara kerja transaksi Bitcoin dari awal hingga akhir.

1. Adam ingin mengirim bitcoin kepada Geri. Ia membuat transaksi dengan alamat Geri, jumlah yang akan dikirim, dan biaya transaksi.
1. Adam menandatangani transaksi tersebut dengan kunci privatnya untuk membuktikan kepemilikan.
1. Ia menyiarkan transaksi tersebut ke jaringan Bitcoin.
1. Node menerima transaksi itu dan memeriksa apakah sudah sesuai aturan, termasuk memverifikasi tanda tangan dan memastikan Adam memiliki cukup bitcoin.
1. Jika valid, transaksi tersebut dibagikan ke seluruh jaringan dan dimasukkan ke dalam mempool, tempat transaksi yang menunggu untuk diproses.
1. Penambang memilih transaksi dari mempool dan memasukkannya ke dalam blok yang mereka coba tambang.
1. Ketika seorang penambang berhasil menambang sebuah blok, blok tersebut dibagikan ke jaringan dan diperiksa oleh node lain.
1. Jika valid, blok tersebut ditambahkan ke blockchain. Geri menerima bitcoinnya.
1. Seiring bertambahnya blok, transaksi tersebut mendapatkan konfirmasi, sehingga menjadi lebih aman.

Setelah dimasukkan ke dalam blok, transaksi tersebut dikonfirmasi. Adam tidak dapat membelanjakan bitcoin itu lagi, dan Geri dapat membelanjakan yang ia terima dalam transaksi baru.


> **Light**
>
> Transaksi & biaya dipilih → Ditandatangani oleh dompet dan dikirim → Didistribusikan oleh node → Penambang menambahkan transaksi ke template blok → Penambang memenangkan kontes Proof-of-Work → Blok baru divalidasi → Blok baru didistribusikan oleh node


###### Sumber daya


[▶ Tonton video ini tentang Node Bitcoin](https://www.youtube.com/watch?v=xc_TxlByxeY)
