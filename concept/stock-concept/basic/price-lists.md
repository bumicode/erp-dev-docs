# Price Lists

## Price Lists

**Price Lists** adalah pengelompokan [**Item Price**](item-price.md) baik itu Harga Jual, Harga Beli, ataupun keduanya.

ERP dapat menambahkan lebih dari satu [**Item Price**](item-price.md) tergantung situasi yang ada pada perusahaan misalnya harga barang tergantung dari [**Customer** ](../../crm-concept/customer.md)atau [**Sales Partner**](../../selling-concept/sales-partner.md) dan sebagainya. Dengan **Price Lists,** [**Item Price**](item-price.md) dapat di kelompokan sesuai dengan situasi tersebut.

### Logika

* **Price Lists** milik [**Company** ](../../core-concept.md#company-perusahaan)(secara sistem).
* **Price Lists** memiliki 0 atau lebih [**Item Price**](item-price.md)**.**
* **Price Lists** milik dan dimiliki oleh **Customer** (Selling Price)
* **Price Lists** milik dan dimiliki oleh **Sales Partner** (Buying Price)

### Relasi

* **Price Lists** belongs to a **Company**; **Company** has 0 to many **Price Lists.**
* **Price Lists** has 0 to many **Item Prices; Item Price** belongs to a **Price Lists.**
* **Price Lists** many to many **Customers; Customers** many to many **Price Lists.**
* **Price Lists** many to many **Sales Partners; Sales Partners** many to many **Price Lists.**
