# Delivery Note

## Delivery Note

**Delivery Note (DN)** atau Surat Jalan adalah dokumen bisnis yang digunakan untuk mencatat dan mengonfirmasi pengiriman barang atau jasa dari penjual ke pembeli. Delivery Note mengandung informasi rinci tentang barang atau jasa yang dikirim, seperti jumlah, berat, dan deskripsi, serta alamat pengirim dan penerima. Selain itu, Delivery Note juga mencantumkan nomor pesanan, tanggal pengiriman, dan tanda tangan dari pihak pengirim dan penerima sebagai bukti penerimaan barang.

Pada dasarnya, Delivery Note adalah dokumen penting dalam logistik dan manajemen inventaris yang membantu memastikan bahwa barang atau jasa dikirimkan dan diterima dengan benar oleh penerima, dan memudahkan pengelolaan dan pengendalian inventaris oleh perusahaan.

### Logika

* **Delivery Note** milik **Company.**
* **Delivery Note** milik **Sales Order** sehingga semua data seperti **Item, Tax** dan biaya lainnya sama.

### Relasi

* **Delivery Note** belongs to a **Company; Company** has many **Delivery Notes.**
* **Delivery Note** belongs to a **Sales Order; Sales Order** has one **Delivery Note.**

### Akuntansi

Jika pembayaran dilakukan setelah pengiriman (kredit):

* **Debit:** Persediaan Barang Dagang (HPP)
* **Kredit:** Harga Pokok Penjualan (HPP)

Jika pembayaran dilakukan sebelum pengiriman (tunai): Tidak ada pencatatan akuntansi pada tahap ini karena transaksi sudah dicatat saat pembayaran diterima.
