# 📍 Getting Started

## Prerequisites

* [Git](https://git-scm.com/)
* [PHP](https://php.net/) => ^8.1
* [Composer](https://getcomposer.org/)
* [Laravel ](https://laravel.com/docs/10.x)=> ^10.x&#x20;
* [PostgreSQL](https://www.postgresql.org/)
* [Redis](https://redis.io/)

### PHP Extension Requirements

* Ctype PHP Extension
* cURL PHP Extension
* DOM PHP Extension
* Fileinfo PHP Extension
* Filter PHP Extension
* Hash PHP Extension
* Mbstring PHP Extension
* OpenSSL PHP Extension
* PCRE PHP Extension
* PDO PHP Extension
* Session PHP Extension
* Tokenizer PHP Extension
* XML PHP Extension

## Developing

* Clone repository resmi dari ERP

```bash
git clone https://github.com/bumicode/erp.git erp
```

* Copy **.env.example** menjadi **.env**
* Update isi dari **.env** pada pengaturan database menjadi

<pre class="language-bash" data-title=".env" data-overflow="wrap"><code class="lang-bash"><strong>...
</strong><strong>DB_CONNECTION=pgsql
</strong>DB_HOST=127.0.0.1 
DB_PORT=5432
DB_DATABASE=laravel // Sesuaikan dengan database yang digunakan
DB_USERNAME=root // Sesuaikan dengan username database
DB_PASSWORD=     // Sesuaikan dengan password database
...
</code></pre>

* Install dependensi server, app key, migration database

```bash
composer install
php artisan key:generate
php artisan migrate
```

* Run Laravel

```
php artisan serve
```