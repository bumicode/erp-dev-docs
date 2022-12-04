---
description: Logika dan Relasi Lead Customer
---

# Customer

## Customer

**Customer** atau dikenal juga sebagai **Klien** atau **Pembeli** adalah orang yang menerima barang, jasa atau produk dari penjual.

### Logika :

* **Customer** milik **Company** (secara sistem).
* **Customer** milik **Sales Partner** (individu / company (B2B)).
* **Customer** milik **Sales Person** (secara individu).
* **Customer** dapat dikaitkan dengan **Lead**.
* **Customer** dapat dikaitkan dengan **Opportunity.**
* **Customer** memiliki satu atau lebih **Address (Alamat)**.
* **Customer** memiliki satu atau lebih **Contact (Kontak)**.
* **Customer** memiliki 0 atau lebih [**Quotation**](../selling-concept/quotation.md)**.**
* **Customer** memiliki 0 atau lebih **Sales Order (Pesanan Penjualan)**.

### Relasi :

* **Customer** belongs to a **Company**; **Company** has 0 to many **Customers.**
* **Customer** belongs to a **Sales Partner**; **Sales Partner** has 0 to many **Customers.**
* **Customer** belongs to a **Sales Person**; **Sales Person** has 0 to many **Customers.**
* **Customer** belongs to a **Lead**; **Lead** has 0 to one **Customer.**
* **Customer** belongs to a **Opportunity**; **Opportunity** has 0 to one **Customer.**
* **Customer** morph to many **Addressess**; **Address** morphed by Many **Customers**.\*
* **Customer** morph to many **Contacts**; **Contact** morphed by Many **Customers**.\*
* **Customer** has 0 to one **Opportunity**; **Opportunity** belongs to a **Opportunity**.
* **Customer** has 0 to many **Quotations**; **Quotation** belongs to **Customer**.
* **Customer** has 0 to many **Sales Order**; **Sales Order** belongs to **Customer.**

{% hint style="info" %}
Setelah **Lead** menjadi **Customer** itu menandakan bahwa telah terjadinya transaksi antara **Pembeli** dan **Penjual** ditandai dengan telah terbuatnya **Sales Order.**

**Item** yang asalanya hanyalah **wishlist**, berpindah ke data item yang ada di **Sales Order.**&#x20;
{% endhint %}
