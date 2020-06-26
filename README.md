# ci4-rajaongkir
Cek Ongkos Kirim Dengan RajaOngkir CodeIgniter 4

> https://blog.cacan.id/cek-ongkos-kirim-dengan-rajaongkir-codeigniter-4

![000](https://user-images.githubusercontent.com/51890752/85823156-e30dad80-b7a6-11ea-885c-6d56b6ccef8c.jpg)

# Cara Penggunaan:

## Clone dari GitHub:
    git clone https://github.com/blogcacanid/slim3-rest-api-jwt.git

# Testing
Edit <b>KEY</b> dengan <i>Key</i> yang didapat dari RajaOngkir pada file-file berikut:
      
      app/Controllers/Ongkir.php
      app/Controllers/Kota.php

    "key: --ganti-dengan-api-key-anda--"

Masuk ke direktori project dan jalankan CodeIgniter 4 menggunakan perintah berikut:

    cd ci4-rajaongkir
    php spark serve


Untuk mengganti port anda bisa menggunakan perintah seperti berikut:
      
    php spark serve --port 9090


Kemudian buka browser dan ketikkan URL http://localhost:8080/ongkir

Selanjutnya silahkan coba untuk melakukan pengecekan ongkos kirim

![001](https://user-images.githubusercontent.com/51890752/85823193-fde02200-b7a6-11ea-95cb-ef54728da353.jpg)


# CodeIgniter 4 Framework

## What is CodeIgniter?

CodeIgniter is a PHP full-stack web framework that is light, fast, flexible, and secure. 
More information can be found at the [official site](http://codeigniter.com).

This repository holds the distributable version of the framework,
including the user guide. It has been built from the 
[development repository](https://github.com/codeigniter4/CodeIgniter4).

More information about the plans for version 4 can be found in [the announcement](http://forum.codeigniter.com/thread-62615.html) on the forums.

The user guide corresponding to this version of the framework can be found
[here](https://codeigniter4.github.io/userguide/). 


## Important Change with index.php

`index.php` is no longer in the root of the project! It has been moved inside the *public* folder,
for better security and separation of components.

This means that you should configure your web server to "point" to your project's *public* folder, and
not to the project root. A better practice would be to configure a virtual host to point there. A poor practice would be to point your web server to the project root and expect to enter *public/...*, as the rest of your logic and the
framework are exposed.

**Please** read the user guide for a better explanation of how CI4 works!
The user guide updating and deployment is a bit awkward at the moment, but we are working on it!

## Repository Management

We use Github issues, in our main repository, to track **BUGS** and to track approved **DEVELOPMENT** work packages.
We use our [forum](http://forum.codeigniter.com) to provide SUPPORT and to discuss
FEATURE REQUESTS.

This repository is a "distribution" one, built by our release preparation script. 
Problems with it can be raised on our forum, or as issues in the main repository.

## Contributing

We welcome contributions from the community.

Please read the [*Contributing to CodeIgniter*](https://github.com/codeigniter4/CodeIgniter4/blob/develop/contributing.md) section in the development repository.

## Server Requirements

PHP version 7.2 or higher is required, with the following extensions installed: 

- [intl](http://php.net/manual/en/intl.requirements.php)
- [libcurl](http://php.net/manual/en/curl.requirements.php) if you plan to use the HTTP\CURLRequest library

Additionally, make sure that the following extensions are enabled in your PHP:

- json (enabled by default - don't turn it off)
- [mbstring](http://php.net/manual/en/mbstring.installation.php)
- [mysqlnd](http://php.net/manual/en/mysqlnd.install.php)
- xml (enabled by default - don't turn it off)
