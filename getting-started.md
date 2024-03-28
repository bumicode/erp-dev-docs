# 📍 Getting Started

## Prerequisites

* [Git](https://git-scm.com/)
* [PHP](https://php.net/) => ^8.1
* [Composer](https://getcomposer.org/) => ^2.5.4
* [PostgreSQL](https://www.postgresql.org/) => ^15.2
* [Redis](https://redis.io/) => ^7.0
* [Node.js](https://nodejs.org/en/download/)

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

```bash
cp .env.example .env
```

* Update isi dari **.env** pada pengaturan database menjadi

<pre class="language-bash" data-title=".env" data-overflow="wrap"><code class="lang-bash">...
<strong>DB_CONNECTION=pgsql
</strong>DB_HOST=127.0.0.1 
<strong>DB_PORT=5432
</strong>DB_DATABASE=laravel // Sesuaikan dengan database yang digunakan
DB_USERNAME=root // Sesuaikan dengan username database
DB_PASSWORD=     // Sesuaikan dengan password database
...
</code></pre>

* Install dependensi server, app key, migration database.

```bash
composer install
php artisan key:generate
php artisan migrate --seed
```

* Run Shiled (Roles and Permissions)

```bash
php artisan shield:generate
php artisan shield:super-admin
```

* Run Laravel

```bash
php artisan serve
```

\[Opsional] Vite.js

```bash
npm install
npm run dev
```
