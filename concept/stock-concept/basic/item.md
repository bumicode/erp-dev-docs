# Item

**Item** adalah barang atau jasa yang dijual atau dibeli oleh perusahaan.&#x20;

### Logika

* **Item** milik [**Company** ](../../core-concept.md#company-perusahaan)(secara sistem).
* **Item** milik **Selling (Quotation**, **Sales Order**, **Sales Invoice**, **Blanked Order).**
* **Item** milik **Buying (Material Request, Purchase Order, Purchase Invoice, Request for Quotation, Supplier Quotation).**
* **Item** memiliki 1 atau lebih [**Item Price**](item-price.md)**.**

### Relasi

* **Item** belongs to a **Company**; **Company** has 0 to many **Items.**
