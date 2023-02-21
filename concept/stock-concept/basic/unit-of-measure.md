# Unit of Measure

## Unit of Measurement (UOM)&#x20;

Unit of Measurement (UOM) adalah cara mengukur jumlah suatu bahan baku atau produk. UOM digunakan dalam industri manufaktur dan perdagangan untuk memastikan bahwa jumlah yang diterima atau dikirimkan sesuai dengan spesifikasi.

Contoh UOM meliputi kilogram, liter, meter, unit, dan lain-lain. Dalam sistem informasi bisnis, seperti aplikasi ERP, UOM biasanya digunakan untuk memastikan bahwa perhitungan stok dan transaksi produk terjadi dengan benar.

Secara otomatis ERP akan menyediakan beberapa UOM yang umum digunakan seperti :&#x20;

* Unit (pcs, buah, item, dll.)
* Dus (dus, set, kotak, dll.)
* Gross (grs)
* Lusin (lns)
* Meter (m)
* Kilogram (kg)
* Liter (L)
* Pack (pck, paket, dll.)
* Buket (buket, tangkai, dll.)
* Ton (t)

Selain daftar di atas pengguna dapat menambahkan UOM sesuai dengan yang dibutuhkan oleh perusahaan.

### Logika

* **UOM** milik [**Company**](../../core-concept/#company-perusahaan)
* **UOM** memiliki dan dimiliki oleh 0 atau lebih [**Items**](item.md)**.**
* **UOM** memiliki 1 atau lebih **UOM Conversion Factors.**

### Relasi

* **UOM** belongs to a **Company**; **Company** has 0 to many **UOMs.**
* **UOM** many to many **Items;** **Item** many to many **UOMs.**
* **UOM** many to many **UOM Conversion Factors**. **UOM Conversion Factor** many to many **UOMs.**

## UOM Conversion Factor

UOM Conversion Factor adalah faktor konversi yang digunakan untuk mengubah satu unit pengukuran menjadi unit pengukuran lain.

Contohnya, jika Anda memiliki data berat bahan baku dalam kilogram, tetapi ingin mengonversinya ke pound, Anda dapat menggunakan faktor konversi 1 kilogram = 2,20462 pound. Dalam hal ini, faktor konversi 2,20462 adalah UOM Conversion Factor untuk mengonversikan kilogram ke pound.

Penggunaan UOM Conversion Factor sangat penting dalam aplikasi bisnis seperti manufaktur, logistik, dan perdagangan, di mana data berbagai jenis pengukuran harus dikonversikan dan dibandingkan.

### Logika

* **UOM Conversion Factor** milik [**Company**](../../core-concept/#company-perusahaan)
* **UOM Conversion Factor** milik dan memiliki **UOM.**

### Relasi

* **UOM Conversion Factor** belongs to a **Company**; **Company** has 0 to many **UOM Conversion Factors.**
* **UOM Conversion Factor** many to many **UOMs; UOM** many to many **UOM Conversion Factors.**
