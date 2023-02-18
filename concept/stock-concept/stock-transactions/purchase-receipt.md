# Purchase Receipt

## Purchase Receipt

**Purchase receipt** adalah bukti pembelian yang diberikan oleh penjual kepada pembeli sebagai tanda bahwa pembelian telah terjadi dan uang telah diterima oleh penjual.&#x20;

Purchase receipt berisi informasi tentang barang atau jasa yang dibeli, jumlah yang dibeli, harga per unit, total harga, tanggal dan waktu transaksi, serta informasi penting lainnya seperti nama dan alamat penjual dan pembeli. Purchase receipt biasanya digunakan oleh pembeli sebagai bukti pembelian jika nantinya terdapat masalah dengan produk yang dibeli, atau untuk keperluan akuntansi seperti pencatatan pengeluaran.

### Logika

* **Purchase Receipt** milik **Company**
* **Purchase Receipt** memiliki 1 atau lebih **Item**
* **Purchase Receipt** dapat dibuat setelah **Purchase Order** dan biasanya **Purchase Receipt** dibuat ketika **Item** dari **Supplier** diterima.

### Relasi

* **Purchase Receipt** belongs to a **Company; Company** has many **Purchase Receipts.**
* **Purchase Receipt** has 1 to many **Items; Item** belongs to many **Purchase Receipts.**
* **Purchase Receipt** belongs to a **Purchase Order; Purchase Order** has one **Purchase Receipt.**
