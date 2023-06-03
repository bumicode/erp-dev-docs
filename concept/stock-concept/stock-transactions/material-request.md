# Material Request

## Material Request

Material Request adalah permintaan bahan atau barang tertentu yang diajukan oleh departemen atau unit kerja di dalam sebuah organisasi kepada departemen gudang atau pergudangan. Pada aplikasi ERP, Material Request adalah dokumen yang digunakan untuk mengumpulkan permintaan bahan atau barang dari berbagai departemen atau unit kerja dalam organisasi secara terpusat dan mengelola permintaan tersebut secara efisien. Dokumen Material Request biasanya berisi informasi seperti jenis barang atau bahan yang diminta, kuantitas yang dibutuhkan, tanggal pengiriman yang diinginkan, dan informasi lain yang relevan.

### Logika

* **Material Request** milik [**Company**](../../core-concept/#company-perusahaan)
* **Material Request** memiliki 1 atau lebih [**Item**](../basic/item.md)
* **Material Request** mendapatkan id referensi dari ([**Sales Order**](../../selling-concept/sales-order.md), [**Request for Quotation**](../../buying-concept/request-for-quotation.md), [**Supplier Quotation**](../../buying-concept/supplier-quotation.md), [**Purchase Order**](../../buying-concept/purchase-order.md)). Contoh: ketika ada **Sales Order** tapi stock tidak mencukupi, maka dapat membuat **Material Request** yang kemudian **Material Request** dapat di konversi menjadi [**Purchase Order**](../../buying-concept/purchase-order.md)**.**

### Relasi

* **Material Request** belongs to a **Company**; **Company** has 0 to many **Material Request**.
* **Material Request** has many **Items; Item** belongs to many **Material Requests.**
* **Material Request** belongs to a **Sales Order; Sales Order** has one **Material Request.**
* **Material Request** has one **Purchase Order; Purchase Order** belongs to a **Material Request.**

### Table Structure

[https://dbdocs.io/mohamadsyalvasr/bumicode\_erp?table=material\_requests\&schema=stock\&view=table\_structure](https://dbdocs.io/mohamadsyalvasr/bumicode\_erp?table=material\_requests\&schema=stock\&view=table\_structure)
