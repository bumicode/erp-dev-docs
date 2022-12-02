# CRM Concept

{% hint style="danger" %}
**Konsep belum final dan ada kemungkinan akan diubah sewaktu-waktu.**
{% endhint %}

Mengenal alur CRM dari Lead sampai Pembayaran (Sales)

## Lead

**Lead** bisa dibilang sebagai **Potential Customer**. Artinya, mereka adalah seseorang atau sekelompok yang tertarik terhadap sesuatu yang sudah di tawarkan, biasanya mereka sudah memberikan informasi data diri seperti nama, email, telepon dan sebagainya. Lead dapat di teruskan atau di ubah ke entitas berikut :

* Opportunity (Peluang)
* Customer (Pelanggan)\


### Logika :

* **Lead** milik **Company** (secara sistem) dan milik **Sales Partner** atau **Sales Person** (secara individu)
* **Lead** memiliki satu atau lebih **Address (Alamat)**.
* **Lead** memiliki satu atau lebih **Contact (Kontak)**.
* **Lead** dapat berubah menjadi **Opportunity**.
* **Lead** dapat berubah menjadi **Customer**.
* **Lead** memiliki satu atau lebih **Quotation**
* **Lead** memiliki satu atau lebih **Item**.&#x20;

{% hint style="success" %}
**Note**: Item disini adalah produk atau layanan yang membuat mereka tertarik.
{% endhint %}

### Relasi :

* **Lead** belongs to a **Company**; **Company** has 0 to many **Leads**
* **Lead** belongs to a **Sales Partner**; **Sales Partner** has 0 to many **Leads** or **Lead** belongs to a **Sales Person**; **Sales Person** has 0 to many **Leads**
* **Lead** morph to many **Addressess**; **Address** morphed by Many **Leads**.\*
* **Lead** morph to many **Contacts**; **Contact** morphed by Many **Leads**.\*
* **Lead** has 0 to one **Opportunity**; **Opportunity** belongs to a Lead
* **Lead** has 0 to one **Customer**; **Customer** belongs to a Lead
* **Lead** has 0 to many **Quotations**; **Quotation** belongs to Lead
* **Lead** morph to many **Itemables**; **Itemables** morphed to Many Leads

{% hint style="info" %}
**Lead** dapat berubah menjadi **Opportunity** / **Customer**. Bukan berarti hanya statusnya saja yang berubah tapi menyalin datanya juga ke entitas **Opportunity** atau **Customer** sehingga pada relasi diatas "has 0 to one" yang artinya **Opportunity** / **Customer** milik Lead.

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

* Quotation
* Sales Order

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
