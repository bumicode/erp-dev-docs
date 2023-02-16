# Material Request

## Material Request

Material Request adalah permintaan bahan atau barang tertentu yang diajukan oleh departemen atau unit kerja di dalam sebuah organisasi kepada departemen gudang atau pergudangan. Pada aplikasi ERP, Material Request adalah dokumen yang digunakan untuk mengumpulkan permintaan bahan atau barang dari berbagai departemen atau unit kerja dalam organisasi secara terpusat dan mengelola permintaan tersebut secara efisien. Dokumen Material Request biasanya berisi informasi seperti jenis barang atau bahan yang diminta, kuantitas yang dibutuhkan, tanggal pengiriman yang diinginkan, dan informasi lain yang relevan.

### Logika

* **Material Request** milik **Company**
* **Material Request** memiliki 1 atau lebih **Item**
* **Material Request** bisa menjadi referensi dari (**Sales Order**, **Request for Quotation**, **Supplier Quotation**, **Purchase Order**). Contoh: ketika ada **Sales Order** tapi stock tidak mencukupi, maka akan membuat **Material Request** yang kemudian **Material Request** dapat di konversi menjadi **Purchase Order.**

### Relasi

* **Material Request** belongs to a **Company**; **Company** has 0 to many **Material Request**.
* **Material Request** has many **Items; Item** belongs to many **Material Requests.**
* &#x20;

