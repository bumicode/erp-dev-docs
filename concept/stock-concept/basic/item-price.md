# Item Price

## Item Price

**Item Price** adalah harga suatu produk atau barang baik itu harga beli ataupun harga jual. Ini merupakan bagian penting dari informasi produk yang digunakan untuk mengelola, memantau, dan membuat laporan tentang aktivitas bisnis.

### Logika

* **Item Price** milik [**Company**](../../core-concept.md#company-perusahaan)**.**
* **Item Price** milik **Price Lists.**
* **Item Price** milik **Item.**

### Relasi

* **Item Price** belongs to a **Company**; **Company** has 0 to many **Item Price.**
* **Item Price** belongs to a **Price Lists; Price Lists** has 0 to many **Item Price.**
* **Item Price** belongs to a **Item; Item** has 1 to many **Item Price.**
