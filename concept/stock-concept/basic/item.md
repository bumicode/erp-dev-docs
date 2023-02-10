# Item

**Item** adalah barang atau jasa yang dijual atau dibeli oleh perusahaan.&#x20;

### Logika

* **Item** milik [**Company** ](../../core-concept.md#company-perusahaan)(secara sistem).
* **Item** milik **Selling (**[**Quotation**](../../selling-concept/quotation.md), [**Sales Order**](../../selling-concept/sales-order.md), [**Sales Invoice**](../../selling-concept/sales-invoice.md), [**Blanked Order**](../../selling-concept/blanked-order.md)**).**
* **Item** milik **Buying (**[**Purchase Order**](../../buying-concept/purchase-order.md)**,** [**Purchase Invoice**](../../buying-concept/purchase-invoice.md)**,** [**Request for Quotation**](../../buying-concept/request-for-quotation.md)**,**[ **Supplier Quotation**](../../buying-concept/supplier-quotation.md)**).**
* **Item** milik **Stock Transactions (**[**Material Request**](../stock-transactions/material-request.md)**,** [**Stock Entry**](../stock-transactions/stock-entry.md)**,** [**Purchase Receipt**](../stock-transactions/purchase-receipt.md)**,** [**Delivery Note**](../stock-transactions/delivery-note.md)**,** [**Packing Slip**](../stock-transactions/packing-slip.md)**,** [**Shipment**](../stock-transactions/shipment.md)**,** [**Pick List**](../stock-transactions/pick-list.md)**)**
* **Item** memiliki 1 atau lebih [**UOM**](unit-of-measure.md).
* **Item** milik 1 [**Item Group**](item-group.md)**.**
* **Item** memiliki 1 atau lebih [**Item Price**](item-price.md)**.**
* **Item** memiliki 0 atau lebih [**Item Attribute**](../item-variants/item-attribute.md).
* **Item** memiliki 0 atau lebih [**Item Variants**](../item-variants/item-variants.md).
* **Item** milik 1 atau lebih [**Warehouse**](warehouse.md).
* **Item** memiliki 1 atau lebih **Common** (**Images, Attachments, Comments, Tags**).

### Relasi

* **Item** belongs to a **Company**; **Company** has 0 to many **Items.**
