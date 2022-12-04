---
description: Tentang Logika dan Relasi Lead Opportunity
---

# Opportunity

## Opportunity

**Opportunity** adalah prospek yang diduga memiliki **kemungkinan tinggi** untuk menjadi pelanggan baru (**Customer**).&#x20;

### Logika :

* **Opportunity** milik **Company** (secara sistem).
* **Opportunity** milik **Sales Partner** (individu / company (B2B)).
* **Opportunity** milik **Sales Person** (secara individu).
* **Opportunity** dapat dimiliki **Lead**.
* **Opportunity** memiliki satu atau lebih **Address (Alamat)**.
* **Opportunity** memiliki satu atau lebih **Contact (Kontak)**.
* **Opportunity** dapat berubah menjadi **Customer**.
* **Opportunity** memiliki 0 atau lebih **Quotation.**
* **Opportunity** memiliki 0 atau lebih **Item**.&#x20;
* **Opportunity** memiliki 0 atau lebih **Sales Order (Pesanan Penjualan)**.

### Relasi

* **Opportunity** belongs to a **Company**; **Company** has 0 to many **Opportunities.**
* **Opportunity** belongs to a **Sales Partner**; **Sales Partner** has 0 to many **Opportunities.**
* **Lead** belongs to a **Sales Person**; **Sales Person** has 0 to many **Opportunities.**
* **Opportunity** morph to many **Addressess**; **Address** morphed by Many **Opportunities**.\*
* **Opportunity** morph to many **Contacts**; **Contact** morphed by Many **Opportunities**.\*
* **Opportunity** has 0 to one **Opportunity**; **Opportunity** belongs to a **Opportunity**.
* **Opportunity** has 0 to one **Customer**; **Customer** belongs to a **Opportunity**.
* **Opportunity** has 0 to many **Quotations**; **Quotation** belongs to **Opportunity**.
* **Opportunity** morph to many **Itemables**; **Itemables** morphed to Many **Opportunities**.
* **Opportunity** has 0 to many **Sales Order**; **Sales Order** belongs to **Opportunity.**
