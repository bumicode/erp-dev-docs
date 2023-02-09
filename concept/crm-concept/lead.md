---
description: Logika dan Relasi Lead
---

# Lead

## Lead

**Lead** adalah potensial calon pelanggan yang belum memenuhi kriteria sebagai pelanggan. **Lead** biasanya diperoleh melalui aktivitas pemasaran seperti pameran dagang, pendaftaran situs web, atau penawaran promosi. **Lead** harus dikonversi menjadi peluang sebelum dapat menjadi pelanggan. **Lead** dapat di teruskan atau di ubah ke entitas berikut :

* **Opportunity** (Peluang)
* **Customer** (Pelanggan)

### Logika :

* **Lead** milik [**Company** ](../core-concept.md#company-perusahaan)(secara sistem).
* **Lead** milik [**Sales Partner**](../selling-concept/sales-partner.md) **** (secara individu).&#x20;
* **Lead** milik **Salesperson** (secara individu).
* **Lead** memiliki satu atau lebih [**Address (Alamat)**](address.md).
* **Lead** memiliki satu atau lebih [**Contact (Kontak)**](contact.md).
* **Lead** dapat menjadi [**Opportunity**](opportunity.md).
* **Lead** dapat menjadi [**Customer**](customer.md).
* **Lead** memiliki 0 atau lebih [**Quotation**](../selling-concept/quotation.md)**.**
* **Lead** memiliki 0 atau lebih [**Item**](../stock-concept/basic/item.md).&#x20;

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

{% hint style="info" %}
**Item** yang ada disini adalah daftar keinginan (wishlist) dan belum masuk ke transaksi.
{% endhint %}

{% hint style="warning" %}
**Note:** \*

* **Addressable  :** Polymorphic ( Many To Many )
* **Contactable :** Polymorphic ( Many To Many )&#x20;
* **Itemable :** Polymorphic ( Many To Many )
{% endhint %}
