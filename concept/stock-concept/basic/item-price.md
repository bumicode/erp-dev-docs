# Item Price

## Item Price

**Item Price** adalah harga suatu produk atau barang baik itu harga beli ataupun harga jual. Ini merupakan bagian penting dari informasi produk yang digunakan untuk mengelola, memantau, dan membuat laporan tentang aktivitas bisnis.

### Logika

* **Item Price** milik [**Company**](../../core-concept/#company-perusahaan)**.**
* **Item Price** milik [**Price Lists**](price-lists.md)**.**
* **Item Price** milik [**Item**](item.md)**.**
* **Item Price** milik **Customer / Supplier. \***

### Relasi

* **Item Price** belongs to a **Company**; **Company** has 0 to many **Item Price.**
* **Item Price** belongs to a **Price Lists; Price Lists** has 0 to many **Item Price.**
* **Item Price** belongs to a **Item; Item** has 1 to many **Item Price.**
* **Item Price** morph to one **Customers**; **Customer** morphed by one **Item Price. \***
* **Item Price** morph to one **Suppliers**; **Supplier** morphed by one **Item Price. \***

{% hint style="warning" %}
**Note:** \*

* **Priceable:** Polymorphic (Many To Many)
{% endhint %}
