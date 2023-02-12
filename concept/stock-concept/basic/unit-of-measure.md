# Unit of Measure

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

* **UOM** milik [**Company** ](../../core-concept.md#company-perusahaan)(khusus untuk UOM yang dibuat sendiri dan bukan bawaan ERP)
* **UOM** memiliki dan dimiliki oleh 0 atau lebih [**Items**](item.md)**.**

### Relasi

* **UOM** belongs to a **Company**; **Company** has 0 to many **UOMs.**
* **UOM** many to many **Items;** **Item** many to many **UOMs.**
