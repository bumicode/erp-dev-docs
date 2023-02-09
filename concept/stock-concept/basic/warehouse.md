# Warehouse

## Warehouse

**Warehouse** adalah gudang yang digunakan untuk menyimpan barang atau produk. Warehouse dapat digunakan oleh perusahaan atau bisnis untuk menyimpan produk-produk yang akan dijual, barang-barang yang sudah diterima dari pemasok, atau bahan baku yang akan digunakan dalam produksi. Warehouse juga dapat digunakan sebagai tempat untuk menyimpan produk-produk yang sudah tidak dipakai atau sudah kedaluwarsa.

### Logika&#x20;

* **Warehouse** milik [**Company** ](../../core-concept.md#company-perusahaan)(secara sistem).
* **Warehouse** memiliki satu atau lebih [**Contact** ](../../crm-concept/contact.md)**(Kontak)**.
* **Warehouse** memiliki satu atau lebih [**Address** ](../../crm-concept/address.md)**(Alamat)**.
* **Warehouse** memiliki 0 atau lebih [**Item**](item.md)****

### Relasi

* **Warehouse** belongs to a **Company**; **Company** has 0 to many **Warehouse.**
* **Warehouse** morph to many **Addressess**; **Address** morphed by Many **Warehouse**.\*
* **Warehouse** morph to many **Contacts**; **Contact** morphed by Many **Warehouse**.\*
* **Warehouse** has 0 to many **Items**; **Item** belongs to **Warehouse**.

{% hint style="warning" %}
**Note:** \*

* **Addressable  :** Polymorphic ( Many To Many )
* **Contactable :** Polymorphic ( Many To Many )
{% endhint %}
