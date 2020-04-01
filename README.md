[![CodeFactor](https://www.codefactor.io/repository/github/sergeevpasha/wordpress-docker-image/badge)](https://www.codefactor.io/repository/github/sergeevpasha/wordpress-docker-image)
![Docker Image CI](https://github.com/sergeevpasha/wordpress-docker-image/workflows/Docker%20Image%20CI/badge.svg)

# A docker image for Wordpress

Extended From wordpress:php7.4-fpm

Has support for postgreSQL

## PHP Modules

* bcmath
* Core
* ctype
* curl
* date
* dom
* exif
* fileinfo
* filter
* ftp
* gd
* hash
* iconv
* imagick
* json
* libxml
* mbstring
* mysqli
* mysqlnd
* openssl
* pcre
* PDO
* pdo_pgsql
* pdo_sqlite
* pgsql
* Phar
* posix
* readline
* Reflection
* session
* SimpleXML
* sodium
* SPL
* sqlite3
* standard
* tokenizer
* xml
* xmlreader
* xmlwriter
* Zend OPcache
* zip
* zlib

Example configuration for docker-compose.yml
```
app:
    image: sergeevpasha/wordpress:latest
    tty: true
    volumes:
        - ./:/var/www/html:consistent
    networks:
        - some-network
```