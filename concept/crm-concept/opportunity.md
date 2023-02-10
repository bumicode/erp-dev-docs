---
description: Logika dan Relasi Lead Opportunity
---

# Opportunity

## Opportunity

**Opportunity** adalah prospek yang sudah dikenal dan memiliki potensi untuk menjadi pelanggan. **Opportunity** adalah langkah berikutnya setelah **Lead**, dan membutuhkan lebih banyak interaksi dan penjualan untuk memastikan bahwa mereka akan menjadi pelanggan aktif.

### Logika :

* **Opportunity** milik [**Company** ](../core-concept.md#company-perusahaan)(secara sistem).
* **Opportunity** milik [**Sales Partner**](../selling-concept/sales-partner.md) (individu / company (B2B)).
* **Opportunity** milik **Salesperson** (secara individu).
* **Opportunity** dapat dikaitkan dengan [**Lead**](lead.md).
* **Opportunity** memiliki satu atau lebih [**Address** ](address.md)**(Alamat)**.
* **Opportunity** memiliki satu atau lebih [**Contact** ](contact.md)**(Kontak)**.
* **Opportunity** dapat menjadi [**Customer**](customer.md).
* **Opportunity** memiliki 0 atau lebih [**Quotation**](../selling-concept/quotation.md)**.**
* **Opportunity** memiliki 0 atau lebih [**Sales Order**](../selling-concept/sales-order.md) **(Pesanan Penjualan)**.

### Relasi :

* **Opportunity** belongs to a **Company**; **Company** has 0 to many **Opportunities.**
* **Opportunity** belongs to a **Sales Partner**; **Sales Partner** has 0 to many **Opportunities.**
* **Opportunity** belongs to a **Salesperson**; **Salesperson** has 0 to many **Opportunities.**
* **Opportunity** belongs to a **Lead**; **Lead** has 0 to one **Opportunity.**
* **Opportunity** morph to many **Addresses**; **Address** morphed by Many **Opportunities. \***
* **Opportunity** morph to many **Contacts**; **Contact** morphed by Many **Opportunities**.\*
* **Opportunity** has 0 to one **Customer**; **Customer** belongs to a **Opportunity**.
* **Opportunity** has 0 to many **Quotations**; **Quotation** belongs to **Opportunity**.
* **Opportunity** has 0 to many **Sales Order**; **Sales Order** belongs to **Opportunity.**

{% hint style="info" %}
**Item** yang ada disini adalah daftar keinginan (wish list) dan belum masuk ke transaksi.
{% endhint %}

{% hint style="warning" %}
**Note:** \*

* **Addressable :** Polymorphic ( Many To Many )
* **Contactable :** Polymorphic ( Many To Many )&#x20;
{% endhint %}
