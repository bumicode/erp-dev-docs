# Item Attribute

## Item Attribute

Item Attribute adalah karakteristik dari produk atau item yang diterapkan dalam sistem Enterprise Resource Planning (ERP). Ini adalah informasi tambahan yang digunakan untuk menjelaskan produk dan membantu dalam proses manajemen produk.

Contoh, produk "Sepatu" mungkin memiliki beberapa atribut seperti ukuran, warna, atau bahan.

### Logika

* **Item Attribute** milik **Company**
* **Item Attribute** dimiliki 0 atau lebih **Item**

### Relasi

* **Item Attribute** belongs to a **Company; Company** has 0 to many **Item Attributes.**
* **Item Attribute** belongs to many **Items; Item** has 0 to many **Item Attributes.**
