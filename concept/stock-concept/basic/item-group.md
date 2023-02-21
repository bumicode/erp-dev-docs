# Item Group

## **Item Group**

**Item Group** adalah konsep penggrupan item atau produk dalam sistem manajemen inventori atau manajemen barang. Dalam sistem ini, item atau produk dikelompokkan berdasarkan kategori atau jenis yang sama, seperti jenis barang, kegunaan, atau fitur tertentu. Tujuan dari penggrupan item ini adalah untuk mempermudah pengelolaan dan pengendalian stok, mempermudah pengambilan keputusan, dan mempermudah analisis data.

Dengan menggunakan **Item Group**, perusahaan dapat memantau dan mengendalikan stok dengan lebih efisien, memastikan bahwa item yang dibutuhkan tersedia dan dapat mengelola pembelian dengan lebih baik. Item Group juga dapat membantu perusahaan dalam memahami pola penjualan dan membuat keputusan yang lebih baik mengenai produk yang akan dipertahankan, produk yang akan ditinggalkan, dan produk baru yang akan dikembangkan.

### Logika

* **Item Group** milik [**Company** ](../../core-concept/#company-perusahaan)(secara sistem).
* **Item Group** memiliki 0 atau lebih [**Item**](item.md)**.**

### Relasi

* **Item Group** belongs to a **Company**; **Company** has 0 to many **Item Group.**
* **Item Group** has 0 to many **Items**; **Item** belongs to **Item Group**.
