# Sales Invoice

**Sales Invoice atau faktur penjualan adalah dokumen yang diterbitkan oleh penjual kepada pembeli sebagai bukti transaksi jual beli.**

Sales Invoice juga berfungsi sebagai bukti pembayaran yang sah bagi pembeli sehingga pembeli dapat menggunakannya sebagai dasar untuk klaim atau pertanggungjawaban di kemudian hari. Dokumen ini juga berfungsi sebagai bukti keuangan untuk penjual, yang dapat digunakan untuk melacak penjualan dan pendapatan, serta untuk memperhitungkan pajak yang harus dibayarkan.

### Logika

### Relasi

### Akuntansi

#### Jika belum dibayar

* **Debit :** Piutang Lain-lain ( Total yang akan dibayar oleh Customer )
* **Credit :** Akun Default untuk Item ( Total harga Item yang dibeli oleh Customer )
* **Credit :** Akun sesuai dengan tipe transaksinya misalnya PPN masuk ke dalam Akun PPN.

**Jika sudah dibayar**

* **Debit :** Sesuai dengan payment method, contoh jika Cash maka masuk ke Akun Kas Kecil
* **Credit :** Piutang Lain-lain
