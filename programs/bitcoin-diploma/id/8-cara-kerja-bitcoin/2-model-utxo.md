# 8.2 Model UTXO

##### Apa itu UTXO?

Jangan takut dengan nama yang terdengar asing. Kamu bisa menganggap UTXO sebagai potongan bitcoin, mirip seperti uang kertas dan koin di dompetmu. Misalnya, jika kamu membayar barang seharga Rp60.000 dengan uang kertas Rp100.000, kamu akan menerima Rp40.000 sebagai kembalian. Bitcoin bekerja dengan cara yang serupa.

Semua bitcoin yang kamu miliki terdiri dari berbagai UTXO. Saat kamu mengirim bitcoin, dompetmu menggunakan satu atau lebih potongan ini untuk melakukan pembayaran.

Jika potongan yang kamu gunakan lebih besar dari jumlah yang kamu kirim, sisa nilainya akan kembali kepadamu sebagai kembalian dalam bentuk UTXO baru. Pada saat yang sama, penerima akan menerima UTXO baru yang mewakili bitcoin yang kamu kirimkan.

Saldo dompetmu hanyalah jumlah total dari semua UTXO yang kamu kendalikan.


> **Callout – Privasi**
>
> Kamu sebaiknya tidak memberitahukan UTXO-mu kepada orang lain karena jika seseorang mengetahuinya, mereka bisa melacak transaksimu dan pada akhirnya mengetahui berapa banyak uang yang kamu miliki.


###### Contoh

1. Andi ingin mengirim 5 BTC ke Budi.
1. Dompet Andi menggunakan dua UTXO miliknya yang jika digabungkan bernilai 6 BTC.
1. Transaksi tersebut mengirimkan **5 BTC ke Budi**, menciptakan UTXO baru di dompet Budi.
1. Sisa **0,99 BTC kembali ke Andi sebagai kembalian**, setelah membayar **biaya transaksi 0,01 BTC**.
1. Setelah transaksi dikonfirmasi, transaksi tersebut ditambahkan ke buku besar Bitcoin dan UTXO yang digunakan oleh Andi ditandai sebagai sudah digunakan, sehingga tidak bisa digunakan lagi.

###### Sumber daya


[▶ YouTube](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
