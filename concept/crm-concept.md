# CRM Concept

{% hint style="danger" %}
**Konsep belum final dan ada kemungkinan akan diubah sewaktu-waktu.**
{% endhint %}

Mengenal alur CRM dari Lead sampai Pembayaran (Sales)

## Lead

**Lead** bisa dibilang sebagai **Potential Customer**. Artinya, mereka adalah seseorang atau sekelompok yang tertarik terhadap sesuatu yang sudah di tawarkan, biasanya mereka sudah memberikan informasi data diri seperti nama, email, telepon dan sebagainya. Lead dapat di teruskan atau di ubah ke entitas berikut :

* Opportunity (Peluang)
* Customer (Pelanggan)

### Logika :

* **Lead** milik **Company** (secara sistem).
* **Lead** milik **Sales Partner** (secara individu).&#x20;
* **Lead** milik **Sales Person** (secara individu).
* **Lead** memiliki satu atau lebih **Address (Alamat)**.
* **Lead** memiliki satu atau lebih **Contact (Kontak)**.
* **Lead** dapat berubah menjadi **Opportunity**.
* **Lead** dapat berubah menjadi **Customer**.
* **Lead** memiliki 0 atau lebih **Quotation.**
* **Lead** memiliki 0 atau lebih **Item**.&#x20;

### Relasi :

* **Lead** belongs to a **Company**; **Company** has 0 to many **Leads.**
* **Lead** belongs to a **Sales Partner**; **Sales Partner** has 0 to many **Leads.**&#x20;
* **Lead** belongs to a **Sales Person**; **Sales Person** has 0 to many **Leads.**
* **Lead** morph to many **Addressess**; **Address** morphed by Many **Leads**.\*
* **Lead** morph to many **Contacts**; **Contact** morphed by Many **Leads**.\*
* **Lead** has 0 to one **Opportunity**; **Opportunity** belongs to a **Lead.**
* **Lead** has 0 to one **Customer**; **Customer** belongs to a **Lead.**
* **Lead** has 0 to many **Quotations**; **Quotation** belongs to **Lead.**
* **Lead** morph to many **Itemables**; **Itemables** morphed to Many **Leads.**

{% hint style="info" %}
**Lead** dapat berubah menjadi **Opportunity** / **Customer**. Bukan berarti hanya statusnya saja yang berubah tapi menyalin datanya juga ke entitas **Opportunity** atau **Customer** sehingga pada relasi diatas "has 0 to one" yang artinya **Opportunity** / **Customer** dapat dimiliki **Lead**.

Ini dilakukan untuk memudahkan dalam pelaporan.
{% endhint %}

{% hint style="warning" %}
**Note:** \*

* **Addressable  :** Polymorphic ( Many To Many )
* **Contactable :** Polymorphic ( Many To Many )&#x20;
* **Itemable :** Polymorphic ( Many To Many )
{% endhint %}

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

## Customer

* Opportunity
* Quotation
* Sales Order

## Quotation

* Sales Order

## Sales Order

* Delivery Note
  * Sales Invoice
    * Payment Entry
