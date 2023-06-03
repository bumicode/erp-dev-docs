# Purchase Order

## Purchase Order

**Purchase Order (PO)** adalah dokumen yang digunakan oleh perusahaan atau organisasi untuk melakukan pembelian barang atau jasa dari pemasok atau vendor. PO berisi detail lengkap tentang item yang dibeli, jumlahnya, harga per unit, dan instruksi lainnya yang diperlukan.

Dengan menggunakan PO, perusahaan atau organisasi dapat memastikan bahwa pesanan mereka kepada pemasok atau vendor spesifik telah tercatat secara resmi. PO juga membantu memastikan kesepakatan harga dan syarat-syarat lainnya telah disepakati sebelum pembelian dilakukan.

Biasanya, PO disiapkan oleh departemen pembelian atau pengadaan di perusahaan. Setelah PO selesai disusun, biasanya dikirimkan kepada pemasok atau vendor untuk dikonfirmasi sebelum pengiriman barang atau pemberian jasa dilakukan.

PO juga dapat digunakan sebagai alat untuk melacak pembelian dan mempermudah proses akuntansi. Setelah barang atau jasa diterima, pihak penerima akan membandingkan pesanan dengan barang yang diterima dan membuat catatan terkait. PO juga membantu dalam proses pembayaran, karena faktur yang diterima dari pemasok atau vendor dapat dibandingkan dengan PO untuk memastikan keakuratan dan memudahkan proses audit.

Dalam beberapa organisasi atau perusahaan, PO juga dapat memerlukan persetujuan dari pihak yang berwenang sebelum pembelian dapat dilakukan. Hal ini bertujuan untuk memastikan bahwa pembelian yang dilakukan sesuai dengan anggaran dan kebijakan yang telah ditetapkan.

Secara umum, **Purchase Order** adalah dokumen penting dalam proses pembelian yang membantu perusahaan atau organisasi dalam mengatur dan melacak pembelian mereka serta memastikan transaksi yang tepat dengan pemasok atau vendor.

## Logika dan Relasi

### Logika&#x20;

* **Purchase Order** milik [**Company**](../core-concept/#company-perusahaan)
* **Purchase Order** dapat dikaitkan dengan [**Material Request**](../stock-concept/stock-transactions/material-request.md)
* **Purchase Order** memiliki satu **Supplier**
* **Purchase Order** memiliki satu **Supplier Address**
* **Purchase Order** memiliki satu **Supplier Contact**
* **Purchase Order** memiliki satu **Shipping Address** ([**Address**](../crm-concept/address.md))
* **Purchase Order** memiliki 1 atau lebih [**Item**](../stock-concept/basic/item.md)
* **Purchase Order** memiliki 0 atau lebih **Tax**
* **Purchase Order** memiliki 0 atau lebih **Charge**
* **Purchase Order** memiliki satu **Terms**

### Relasi &#x20;

* **Purchase Order** belongs to a **Company**; **Company** has 0 to many **Sales Orders.**
* **Purchase Order** belongs to a **Material Request**; **Material Request** has one **Purchase Order.**&#x20;
* **Purchase Order** belongs to a **Supplier**; **Supplier** has 0 to many **Purchase Orders.**
* **Purchase Order** morph to many **Supplier Addresses**; **Address** morphed by Many **Purchase Orders. \***&#x20;
* **Purchase Order** morph to many **Supplier Contacts**; **Contact** morphed by Many **Purchase Orders. \***
* **Purchase Order** morph to many **Shipping Addresses**; **Address** morphed by Many **Purchase Orders. \***
* **Purchase Order** morph to many **Itemables**; **Itemables** morphed to Many **Sales Order.**
* **Purchase Order** morph to many **Taxable; Taxable** morphed to Many **Sales Order**&#x20;
* **Purchase Order** morph to many **Chargeable**; **Chargeable** morphed to Many **Sales Order**&#x20;
* **Purchase Order** has one **Terms**; **Terms** belongs to a **Purchase Order**&#x20;

### Table Structur
