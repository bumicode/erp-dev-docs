---
description: Logika dan Relasi Lead Address
---

# Address

## Address

**Address** merepresentasikan alamat dari individu atau sebagainya yang bisa memiliki alamat.

### **Logika**

* **Address** mili **Company** (secara sistem)
* **Address** dapat dikaitkan dengan [**Lead**](lead.md), [**Customer**](customer.md), **Supplier**, [**Sales Partner**](../selling-concept/sales-partner.md), atau [**Warehouse**](../stock-concept/basic/warehouse.md).

### Relasi

* **Address** belongs to a **Company**; **Company** has 0 to many **Addresses.**
* **Address** morphed by Many ([**Lead**](lead.md), [**Customer**](customer.md), **Supplier**, [**Sales Partner**](../selling-concept/sales-partner.md), [**Warehouse**](../stock-concept/basic/warehouse.md)); ([**Lead**](lead.md), [**Customer**](customer.md), **Supplier**, [**Sales Partner**](../selling-concept/sales-partner.md), [**Warehouse**](../stock-concept/basic/warehouse.md)) morph to many **Addresses.**
