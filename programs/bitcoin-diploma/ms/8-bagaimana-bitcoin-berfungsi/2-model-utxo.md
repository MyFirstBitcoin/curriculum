# 8.2 Model UTXO

##### Apakah itu UTXO?

Jangan rasa terintimidasi dengan nama yang pelik ini. Anda boleh anggap UTXO sebagai kepingan bitcoin, sama seperti wang kertas dan syiling dalam dompet anda. Sebagai contoh, jika anda membayar barang bernilai RM6 dengan wang kertas RM10, anda akan menerima baki RM4. Bitcoin berfungsi dengan cara yang serupa.

Semua bitcoin yang anda miliki terdiri daripada pelbagai UTXO. Apabila anda menghantar bitcoin, dompet anda akan menggunakan satu atau lebih kepingan ini untuk membuat pembayaran.

Jika kepingan yang anda gunakan lebih besar daripada jumlah yang anda hantar, nilai selebihnya akan dikembalikan kepada anda sebagai baki dalam bentuk UTXO baharu. Pada masa yang sama, penerima akan menerima UTXO baharu yang mewakili bitcoin yang anda hantar.

Baki dompet anda hanyalah jumlah nilai semua UTXO yang anda kawal.


> **Callout – Privasi**
>
> Anda tidak sepatutnya memberitahu orang lain tentang UTXO anda kerana jika seseorang mengetahuinya, mereka boleh menjejak transaksi anda dan akhirnya tahu berapa banyak wang yang anda miliki.


###### Contoh

1. Aina ingin menghantar 5 BTC kepada Badrul.
1. Dompetnya menggunakan dua UTXO miliknya yang bernilai 6 BTC secara keseluruhan.
1. Transaksi itu menghantar **5 BTC kepada Badrul**, mencipta UTXO baharu dalam dompet Badrul.
1. Baki **0.99 BTC dikembalikan kepada Aina sebagai baki**, selepas membayar **yuran transaksi 0.01 BTC**.
1. Sebaik sahaja transaksi disahkan, ia akan ditambah ke lejar Bitcoin dan UTXO yang digunakan oleh Aina akan ditandakan sebagai telah digunakan, jadi ia tidak boleh digunakan lagi.

###### Sumber


[▶ Tonton “How Bitcoin Works under the Hood”](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
