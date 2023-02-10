---
description: Logika dan Relasi Lead Contact
---

# Contact

## Contact

**Contact** merepresentasikan individu atau seseorang

### **Logika**

* **Contact** milik **Company** (secara sistem)
* **Contact** dapat dikaitkan dengan [**Lead**](lead.md), [**Customer**](customer.md), **Supplier**, [**Sales Partner**](../selling-concept/sales-partner.md), atau [**User**](../core-concept.md#user-pengguna).

### Relasi

* **Contact** belongs to a **Company**; **Company** has 0 to many **Contacts.**
* **Contact** morphed by Many ([**Lead**](lead.md), [**Customer**](customer.md), **Supplier**, [**Sales Partner**](../selling-concept/sales-partner.md), [**User**](../core-concept.md#user-pengguna)). ; ([**Lead**](lead.md), [**Customer**](customer.md), **Supplier**, [**Sales Partner**](../selling-concept/sales-partner.md), [**User**](../core-concept.md#user-pengguna)) morph to many **Contacts**

### Table Structure

[https://dbdocs.io/mohamadsyalvasr/bumicode\_erp?table=contacts\&schema=common\&view=table\_structure](https://dbdocs.io/mohamadsyalvasr/bumicode\_erp?table=contacts\&schema=common\&view=table\_structure)

