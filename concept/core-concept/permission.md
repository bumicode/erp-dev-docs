# Permission

**Permission** adalah izin apa saja yang dimiliki oleh **Role**. **Permission** akan disesuaikan dengan model yang ada dan setiap model minimal memiliki **Permission** berikut

1. Dapat Membuat (Can Create)
2. Dapat Membaca (Can Read)
3. Dapat Memperbarui (Can Update)
4. Dapat Menghapus (Can Delete)

{% hint style="info" %}
**Permission** di atas adalah izin yang paling minimal. Lebih lanjut dapat menambahkan **Permission** berikut :&#x20;

1. Dapat Membuat Data Sebagai Orang Lain (can create data as others)
2. Dapat Memperbarui Data Milik Orang Lain (can update other people's data)&#x20;
3. Dapat Menghapus Data Milik Orang Lain (can delete other people's data)

\
Atau dapat menggunakan [**Login as Another User**](https://stackoverflow.com/questions/45705087/laravel-login-as-another-user) dengan menambahkan kondisi permission "can login as another user"
{% endhint %}
