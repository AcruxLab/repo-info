# `php:5.6.36-fpm-alpine3.7`

## Docker Metadata

- Image ID: `sha256:a5fc993f8159da451acd64e9a66b6f4270c9714bdd465d8c8d84e6acc6844e6a`
- Created: `2018-06-21T00:08:45.599345407Z`
- Virtual Size: ~ 57.05 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["docker-php-entrypoint"]`
- Command: `["php-fpm"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c`
  - `PHP_INI_DIR=/usr/local/etc/php`
  - `PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi`
  - `PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2`
  - `PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2`
  - `PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie`
  - `GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3`
  - `PHP_VERSION=5.6.36`
  - `PHP_URL=https://secure.php.net/get/php-5.6.36.tar.xz/from/this/mirror`
  - `PHP_ASC_URL=https://secure.php.net/get/php-5.6.36.tar.xz.asc/from/this/mirror`
  - `PHP_SHA256=18f536bf548e909b4e980379d0c4e56d024b2b1eb1c9768fd169360491f1d6dd`
  - `PHP_MD5=`
