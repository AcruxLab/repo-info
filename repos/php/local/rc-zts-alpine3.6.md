# `php:7.2.0RC5-zts-alpine3.6`

## Docker Metadata

- Image ID: `sha256:4abd23cf09ca442d61be1f58b9ef43ffadb12c47f2f616a943623de11bf98348`
- Created: `2017-11-04T10:11:15.136094276Z`
- Virtual Size: ~ 61.79 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["docker-php-entrypoint"]`
- Command: `["php","-a"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pcre-dev 		pkgconf 		re2c`
  - `PHP_INI_DIR=/usr/local/etc/php`
  - `PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts`
  - `PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2`
  - `PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2`
  - `PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie`
  - `GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F`
  - `PHP_VERSION=7.2.0RC5`
  - `PHP_URL=https://downloads.php.net/~pollita/php-7.2.0RC5.tar.xz`
  - `PHP_ASC_URL=https://downloads.php.net/~pollita/php-7.2.0RC5.tar.xz.asc`
  - `PHP_SHA256=92a745048912beb3f6c2a3c188ce695a51852c67201fdf9a21dafe59f51aecc1`
  - `PHP_MD5=`
