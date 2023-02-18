# Item Variants

## Item Variants

Item Variant adalah varian dari produk atau item yang memiliki karakteristik yang berbeda. Secara detail dan relasi, Item Variant sama dengan induknya yang bisa dilihat pada link dibawah ini.

{% content-ref url="../basic/item.md" %}
[item.md](../basic/item.md)
{% endcontent-ref %}

### Developer Tips

{% hint style="info" %}
**Cartesian product** adalah hasil dari operasi matematika yang menghasilkan himpunan semua pasangan terurut dari dua himpunan. Diberikan dua himpunan A dan B, maka Cartesian product A × B adalah himpunan semua pasangan terurut (a, b) di mana a berasal dari himpunan A dan b berasal dari himpunan B.

Contohnya, jika A = {1, 2} dan B = {a, b, c}, maka A × B adalah:

A × B = { (1, a), (1, b), (1, c), (2, a), (2, b), (2, c) }

Dalam matematika dan ilmu komputer, Cartesian product sering digunakan untuk membentuk himpunan semua kemungkinan kombinasi dari beberapa set atau untuk menjalankan perulangan berganda. Misalnya, dalam pemrograman, Cartesian product dapat digunakan untuk membuat loop yang berulang sebanyak kali berdasarkan pasangan nilai dari dua set atau lebih.
{% endhint %}

#### **Contoh JavaScript**

```javascript
let attributes = {
    warna: ['Merah', 'Biru', 'Hijau'],
    ukuran: ['22', '23', '24'],
    material: ['Logam', 'Metal']
};

let productCartesian = (arrays) => {
    if (arrays.length === 0) {
        return [[]];
    }
    let results = [];
    productCartesian(arrays.slice(1)).forEach((product) => {
        arrays[0].forEach((value) => {
            results.push([value].concat(product));
        });
    });
    return results;
};

let cartesianProduct = (attributes) => {
    let attributeNames = Object.keys(attributes);
    let attributeValues = attributeNames.map((name) => attributes[name]);
    return productCartesian(attributeValues).map((product) => {
        let obj = [];
        attributeNames.forEach((name, i) => {
            obj[name] = product[i];
        });
        return obj;
    });
};

let combinations = cartesianProduct(attributes);
console.log(combinations);
```
