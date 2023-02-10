# Quotation

**Quotation** adalah surat penawaran yang diberikan kepada pelanggan setelah adanya permintaan (B2B).

### Logika&#x20;

* **Quotation** milik [**Company**](../core-concept.md#company-perusahaan)****
* **Quotation** milik [**Sales Partner**](sales-partner.md)****
* **Quotation** milik **Sales Person**
* **Quotation** dapat dikaitkan dengan [**Opportunity**](../crm-concept/opportunity.md)****
* **Quotation** dapat menjadi [**Sales Order**](sales-order.md)****
* **Quotation** memiliki 1 atau lebih [**Item**](../stock-concept/basic/item.md)****
* **Quotation** memiliki satu [**Address** ](../crm-concept/address.md)**(Alamat)**.
* **Quotation** memiliki satu [**Contact** ](../crm-concept/contact.md)**(Kontak)**.
* **Quotation** memiliki 0 atau lebih **Tax**
* **Quotation** memiliki 0 atau lebih **Charge**

### Relasi &#x20;

* **Quotation** belongs to a **Company**; **Company** has 0 to many **Quotations.**
* **Quotation** belongs to a **Sales Partner**; **Sales Partner** has 0 to many **Quotations.**&#x20;
* **Quotation** belongs to a **Sales Person**; **Sales Person** has 0 to many **Quotations.**
* **Quotation** morph to many **Addressess**; **Address** morphed by Many **Quotations**.\*
* **Quotation** morph to many **Contacts**; **Contact** morphed by Many **Quotations**.\*
* **Quotation** belongs to a **Opportunity**; **Opportunity** has 0 to many **Quotations.**
* **Quotation** morph to many **Itemables**; **Itemables** morphed to Many **Leads.**
* **Quotation** morph to many **Taxable; Taxable** morphed to Many **Quotations**
* **Quotation** morph to many **Chargeable**; **Chargeable** morphed to Many **Quotations**

### **Table Structure**

[https://dbdocs.io/mohamadsyalvasr/bumicode\_erp?table=quotations\&schema=selling\&view=table\_structure](https://dbdocs.io/mohamadsyalvasr/bumicode\_erp?table=quotations\&schema=selling\&view=table\_structure)
