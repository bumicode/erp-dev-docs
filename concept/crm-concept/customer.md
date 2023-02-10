---
description: Logika dan Relasi Lead Customer
---

# Customer

## Customer

**Customer** adalah pelanggan yang memiliki hubungan bisnis aktif dengan perusahaan dan membeli produk atau layanan dari perusahaan. Mereka memiliki riwayat pembelian dan memiliki potensi untuk membeli produk atau layanan lain dalam masa depan.

### Logika:

* **Customer** milik [**Company** ](../core-concept.md#company-perusahaan)(secara sistem).
* **Customer** milik [**Sales Partner**](../selling-concept/sales-partner.md) (individu / company (B2B)).
* **Customer** milik **Salesperson** (secara individu).
* **Customer** dapat dikaitkan dengan [**Lead**](lead.md).
* **Customer** dapat dikaitkan dengan [**Opportunity**](opportunity.md)**.**
* **Customer** memiliki satu atau lebih [**Address** ](address.md)**(Alamat)**.
* **Customer** memiliki satu atau lebih [**Contact** ](contact.md)**(Kontak)**.
* **Customer** memiliki 0 atau lebih [**Quotation**](../selling-concept/quotation.md)**.**
* **Customer** memiliki 0 atau lebih [**Sales Order**](../selling-concept/sales-order.md) **(Pesanan Penjualan)**.

### Relasi :

* **Customer** belongs to a **Company**; **Company** has 0 to many **Customers.**
* **Customer** belongs to a **Sales Partner**; **Sales Partner** has 0 to many **Customers.**
* **Customer** belongs to a **Salesperson**; **Salesperson** has 0 to many **Customers.**
* **Customer** belongs to a **Lead**; **Lead** has 0 to one **Customer.**
* **Customer** belongs to a **Opportunity**; **Opportunity** has 0 to one **Customer.**
* **Customer** morph to many **Addresses**; **Address** morphed by Many **Customers. \***
* **Customer** morph to many **Contacts**; **Contact** morphed by Many **Customers. \***
* **Customer** has 0 to one **Opportunity**; **Opportunity** belongs to a **Opportunity**.
* **Customer** has 0 to many **Quotations**; **Quotation** belongs to **Customer**.
* **Customer** has 0 to many **Sales Order**; **Sales Order** belongs to **Customer.**

{% hint style="info" %}
Setelah **Lead** menjadi **Customer** itu menandakan bahwa telah terjadinya transaksi antara **Pembeli** dan **Penjual** ditandai dengan telah terbuatnya **Sales Order.**

**Item** yang asalnya hanyalah **wish list**, berpindah ke data item yang ada di **Sales Order.**&#x20;
{% endhint %}
