# CodeIgniter 4 Framework

## What is CodeIgniter?

CodeIgniter is a PHP full-stack web framework that is light, fast, flexible and secure.
More information can be found at the [official site](https://codeigniter.com).

This repository holds the distributable version of the framework.
It has been built from the
[development repository](https://github.com/codeigniter4/CodeIgniter4).

More information about the plans for version 4 can be found in [CodeIgniter 4](https://forum.codeigniter.com/forumdisplay.php?fid=28) on the forums.

The user guide corresponding to the latest version of the framework can be found
[here](https://codeigniter4.github.io/userguide/).

## Important Change with index.php

`index.php` is no longer in the root of the project! It has been moved inside the *public* folder,
for better security and separation of components.

This means that you should configure your web server to "point" to your project's *public* folder, and
not to the project root. A better practice would be to configure a virtual host to point there. A poor practice would be to point your web server to the project root and expect to enter *public/...*, as the rest of your logic and the
framework are exposed.

**Please** read the user guide for a better explanation of how CI4 works!

## Repository Management

We use GitHub issues, in our main repository, to track **BUGS** and to track approved **DEVELOPMENT** work packages.
We use our [forum](http://forum.codeigniter.com) to provide SUPPORT and to discuss
FEATURE REQUESTS.

This repository is a "distribution" one, built by our release preparation script.
Problems with it can be raised on our forum, or as issues in the main repository.

## Contributing

We welcome contributions from the community.

Please read the [*Contributing to CodeIgniter*](https://github.com/codeigniter4/CodeIgniter4/blob/develop/CONTRIBUTING.md) section in the development repository.

## Server Requirements

PHP version 7.4 or higher is required, with the following extensions installed:

- [intl](http://php.net/manual/en/intl.requirements.php)
- [mbstring](http://php.net/manual/en/mbstring.installation.php)

Additionally, make sure that the following extensions are enabled in your PHP:

- json (enabled by default - don't turn it off)
- [mysqlnd](http://php.net/manual/en/mysqlnd.install.php) if you plan to use MySQL
- [libcurl](http://php.net/manual/en/curl.requirements.php) if you plan to use the HTTP\CURLRequest library

## Tahapan Praktek

- Mengaktifkan Ekstentasi XAMPP
![image](https://github.com/ristof5/lab11_php_c4/assets/116700466/9a98b32c-29d9-475c-9119-16d6adbc402c)
teks ada disekitar line 900
bila sudah mendownload codeigniter, ekstrak file ke folder htdocs anda

- Menjalankan CLI
buka shell xampp lalu Arahkan lokasi direktori sesuai dengan direktori kerja project dibuat (xampp/htdocs/lab11_php_ci/ci4/)

lalu ketik "php spark"
![Screenshot (112)](https://github.com/ristof5/lab11_php_c4/assets/116700466/673da8dc-ebdf-4015-9d92-f37f6fe0be3b)

- Membuat routes baru
Tambahkan kode berikut di dalam Routes.php
$routes->get('/about', 'Page::about');
$routes->get('/contact', 'Page::contact');
$routes->get('/faqs', 'Page::faqs');

Untuk mengetahui route yang ditambahkan sudah benar, buka CLI dan jalankan perintah berikut.
php spark routes
![Screenshot (115)](https://github.com/ristof5/lab11_php_c4/assets/116700466/f20f042d-b834-4a5a-b745-99e53fa63330)

Untuk mencoba file lakukan ini di CLI terlebih dahulu "php spark serve"
![Screenshot (126)](https://github.com/ristof5/lab11_php_c4/assets/116700466/32175c72-e73e-4320-8281-62e54dc137c7)

lalu Selanjutnya coba akses route yang telah dibuat dengan mengakses alamat url
http://localhost:8080/about

- membuat view
membuat header lalu di lokasi app/view/template/header.php
![Screenshot (124)](https://github.com/ristof5/lab11_php_c4/assets/116700466/7d34448d-844e-4009-97fa-b4786dafd016)

membuat footer lalu di lokasi app/view/template/footer.php
![Screenshot (125)](https://github.com/ristof5/lab11_php_c4/assets/116700466/713caca8-50b7-4bf0-aeba-44f06b0b5443)

untuk cssnya simpan di direktori public
![image](https://github.com/ristof5/lab11_php_c4/assets/116700466/0dc4831e-dde8-4e93-a5fd-b2e67e76e99b)
hasilnya
![Screenshot (122)](https://github.com/ristof5/lab11_php_c4/assets/116700466/c37877c4-73e5-49fa-80fe-64d60ba9807a)
Terima kasih



