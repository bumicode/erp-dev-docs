# Brand

## Brand

Brand mengacu pada merek produk yang dijual atau diproduksi oleh perusahaan.

Brand bisa dikategorikan ke dalam dua hal yaitu _selling_ dan _stock_.

Dalam hal _selling_, informasi tentang brand dapat digunakan untuk melacak penjualan produk dan memantau kinerja produk berdasarkan merek. Ini membantu perusahaan untuk menentukan apa yang menjadi _best seller_ dan memfokuskan strategi pemasaran pada produk dengan merek terbaik.

Dalam hal _stock_, informasi tentang brand juga penting untuk memantau stok produk. Ini membantu perusahaan untuk memastikan bahwa mereka memiliki stok yang tepat untuk memenuhi permintaan produk, dan membuat keputusan _restock_ berdasarkan permintaan produk berdasarkan merek.

### Logika

* **Brand** milik [**Company** ](../../core-concept.md#company-perusahaan)(secara sistem).
* **Brand** memiliki 0 atau lebih [**Item**](item.md)**.**

### Relasi

* **Brand** belongs to a **Company**; **Company** has 0 to many **Brands.**
* **Brand** has 0 to many **Items**; **Item** belongs to **Brand.**
