# 🟢 Core Concept

## Company (Perusahaan)

**Company** adalah pemilik ERP ( tidak merepresentasikan sebagai individu ). **Company** berelasi dengan semua entitas yang ada pada ERP.

## User (Pengguna)

**User** adalah individu yang menggunakan ERP. **User** berelasi dengan semua entitas yang ada pada ERP.

## Role (Peran) & Permission (Izin)

### **Role**

**Role** adalah peran dari **User**. ERP akan mengimplementasikan Role secara dinamis, sehingga tidak akan ada batasan dalam pembuatan Role. Namun, ada beberapa Role yang memang sudah ditentukan diawal dan disesuaikan sesuai dengan modulnya masing-masing seperti berikut :&#x20;

#### Core

1. Super Administrator

#### Selling

1. Sales Partner
2. Sales Manager
3. Salesperson
4. POS Profile

#### Buying

1. Supplier

#### Accounting

1. Accountant

#### Warehouse

1. Warehouse Worker

### Permission (Izin)

**Permission** adalah izin apa saja yang dimiliki oleh **Role**. **Permission** akan disesuaikan dengan entitas yang ada dan setiap entitas minimal memiliki **Permission** berikut

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
Atau dapat menggunakan [**Login as Another User**](https://stackoverflow.com/questions/45705087/laravel-login-as-another-user) **** dengan menambahkan kondisi permission "can login as another user"
{% endhint %}

## [System Security (Keamanan Sistem)](../system-security/)

## [System Data Audit](../audit-record.md)
