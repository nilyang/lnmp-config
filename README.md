# debian 8 jessie lnmp env setup!

## 1.for php:

```
apt-get install \
    gcc build-essential autoconf curl webp libxml2 libxml2-dev \
    libzip-dev mcrypt libmcrypt-dev libpng12-dev libjpeg62-turbo-dev zlibc \
    libfreetype6 libfreetype6-dev openssl libcurl3-openssl-dev libicu-dev
```
## 2.for nginx:

```
apt-get install libpcre3 libpcre3-dev
```

## 3.all together

```
apt-get install \
    gcc build-essential autoconf curl webp libxml2 libxml2-dev \
    libzip-dev mcrypt libmcrypt-dev libpng12-dev libjpeg62-turbo-dev zlibc \
    libfreetype6 libfreetype6-dev openssl libcurl3-openssl-dev \
    libpcre3 libpcre3-dev \
    libicu-dev 
```

### ngxin rewrte libpcre3-dev
### php --enable-intl libicu-dev

## php configure options

```
./configure --prefix=/usr/local/php5.6.10 \
--with-libxml-dir \
--with-zlib \
--enable-bcmath \
--with-curl \
--with-jpeg-dir \
--with-png-dir \
--with-gd \
--with-zlib-dir \
--with-gettext \
--with-freetype-dir \
--enable-mbstring \
--enable-mysqlnd \
--with-mysql \
--with-mysqli \
--with-pdo-mysql \
--with-mcrypt \
--enable-sockets \
--enable-zip \
--with-pcre-dir \
--with-pear=/usr/local/pear \
--with-openssl \
--enable-opcache \
--enable-fpm \
--enable-pcntl \
--enable-intl \
--with-fpm-user=www-data \
--with-fpm-group=www-data

```
