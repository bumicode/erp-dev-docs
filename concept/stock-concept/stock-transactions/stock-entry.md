# Stock Entry

## Stock Entry

**Stock Entry** atau entri stok adalah proses mencatat atau memasukkan informasi tentang masuknya persediaan atau barang ke dalam inventaris perusahaan.

Proses stock entry biasanya dilakukan oleh bagian gudang atau bagian inventarisasi barang. Mereka akan mencatat informasi seperti nama barang, jumlah barang, nomor seri barang (jika diperlukan), dan tanggal masuknya barang. Informasi ini kemudian akan disimpan dalam sistem inventaris perusahaan untuk memudahkan pengelolaan dan pengawasan stok barang.

Stock entry merupakan salah satu bagian dari manajemen persediaan yang penting dalam bisnis karena dapat memengaruhi kelancaran operasional perusahaan. Dengan melakukan stock entry secara teratur dan akurat, perusahaan dapat memantau ketersediaan persediaan barang dan melakukan pengadaan barang dengan lebih efisien.

<details>

<summary>Material Receipt</summary>

**Material Receipt** adalah sebuah dokumen atau rekaman dalam sistem manajemen persediaan atau inventory management yang digunakan untuk mencatat penerimaan atau kedatangan material atau barang ke dalam gudang atau lokasi penyimpanan perusahaan.

**Material Receipt** biasanya dibuat setelah **Material Request**. Akan tetapi ada pengecualian jika **Material Receipt** dipakai sebagai **Opening Stock** ketika membuat **Item.**

### Logika

* **Material Receipt** milik **Company**
* **Material Receipt** milik **Material Request**
* **Material Receipt** memiliki 1 atau lebih **Item**
* **Material Receipt** dimiliki 2 **Account Transaction**

### Relasi

### Accounting

#### General Ledger

Ketika membuat **Material Receipt** maka akan dicatat pada **Buku Besar (General Ledger)** dengan pencatatan pada **Account** default untuk **Warehouse** dan juga **Account Beban Penjualan (Penyesuaian Stok)**

* **Debit** : Default Account Warehouse (contoh: 1141.001 - Persediaan Barang)
* **Credit** : 5110.000 - Beban Penjualan

#### Cash Flow

* **Cash Flow from Operations**
  * **Profit Tahun Yang Berjalan** : Persediaan Barang
  * **Perubahan Persediaan :** Beban Penjualan

</details>
