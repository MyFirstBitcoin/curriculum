# 9.3 Bagaimana Transaksi Berfungsi

Sekarang anda sudah memahami kunci awam dan kunci peribadi, serta peranan nod dan pelombong, berikut adalah cara transaksi Bitcoin berfungsi dari awal hingga akhir.

1. Adam ingin menghantar bitcoin kepada Ahmad. Dia mencipta satu transaksi dengan alamat Ahmad, jumlah yang ingin dihantar, dan yuran.
1. Adam menandatangani transaksi itu dengan kunci peribadinya untuk membuktikan pemilikan.
1. Dia menyiarkan transaksi itu ke rangkaian Bitcoin.
1. Nod menerima transaksi itu dan memeriksa sama ada ia mematuhi peraturan, termasuk mengesahkan tandatangan dan memastikan Adam mempunyai bitcoin yang mencukupi.
1. Jika sah, transaksi itu dikongsi ke seluruh rangkaian dan dimasukkan ke dalam mempool, di mana transaksi yang belum selesai menunggu.
1. Pelombong memilih transaksi dari mempool dan memasukkannya ke dalam blok yang mereka cuba lombong.
1. Apabila seorang pelombong berjaya melombong satu blok, ia dikongsi dengan rangkaian dan diperiksa oleh nod lain.
1. Jika sah, blok itu ditambah ke dalam rantaian blok. Ahmad menerima bitcoin tersebut.
1. Apabila lebih banyak blok ditambah, transaksi itu mendapat pengesahan, menjadikannya lebih selamat.

Setelah dimasukkan ke dalam satu blok, transaksi itu disahkan. Adam tidak boleh membelanjakan bitcoin itu lagi, dan Ahmad boleh membelanjakan apa yang diterimanya dalam transaksi baru.


> **Note**
>
> Transaksi & yuran dipilih → Ditandatangani oleh dompet dan dihantar → Diedarkan oleh nod → Pelombong menambah transaksi ke templat blok → Pelombong memenangi pertandingan Bukti-Kerja → Blok baharu disahkan → Blok baharu diedarkan oleh nod


###### Sumber


[▶ YouTube](https://www.youtube.com/watch?v=xc_TxlByxeY)
