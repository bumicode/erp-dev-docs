# Item Attribute

## Item Attribute

Item Attribute adalah karakteristik dari produk atau item yang diterapkan dalam sistem Enterprise Resource Planning (ERP). Ini adalah informasi tambahan yang digunakan untuk menjelaskan produk dan membantu dalam proses manajemen produk.

Contoh, produk "Sepatu" mungkin memiliki beberapa atribut seperti ukuran, warna, atau bahan.

### Logika

* **Item Attribute** milik **Company**
* **Item Attribute** bisa di tambahkan ke **Item**

### Relasi

* **Item Attribute** belongs to a **Company; Company** has 0 to many **Item Attributes.**

{% hint style="info" %}
**Item Attribute** hanyalah **Data** yang tidak berelasi dengan **Item** secara langsung
{% endhint %}

<pre class="language-json"><code class="lang-json">// Misalnya ada Item Attribute seperti berikut ini
    warna: ['RED', 'BLUE', 'GREEN']
    ukuran: ['22', '23', '24']
    
// Item hanya menambahkan data key saja seperti berikut
{  
    "item": {  
        "name":"Product A",      
        "attribute": {
<strong>            "warna": "",
</strong><strong>            "ukuran": ""
</strong>        }
    }  
} 

// Item Variant menambahkan data value seperti berikut
{  
    "item": {  
<strong>        "name":"Product A-RED-22",      
</strong>        "attribute": {
<strong>            "warna": "RED",
</strong><strong>            "ukuran": 22
</strong>        }
    }  
}  
</code></pre>
