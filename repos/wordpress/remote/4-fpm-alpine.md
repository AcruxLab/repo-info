## `wordpress:4-fpm-alpine`

```console
$ docker pull wordpress@sha256:ce13c11e93fcce45fab54ad761ff5348fd6f7fa02a8300e7bae06a822311abd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `wordpress:4-fpm-alpine` - linux; amd64

```console
$ docker pull wordpress@sha256:b2d7c64178f69df1e8213716dabf7d15d86be12aa11e5ce0f5bb28288c67389f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35563655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a87179c79d92f7db68e3d305c2ed41815cea96c3507d4e5559a27c764307bddd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 25 Oct 2017 23:20:59 GMT
ADD file:90342832e4e7931e42954849ed51216e77b3c974270ed83e9da5648918fb5e66 in / 
# Wed, 25 Oct 2017 23:20:59 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 02:09:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pcre-dev 		pkgconf 		re2c
# Thu, 26 Oct 2017 02:09:38 GMT
RUN apk add --no-cache --virtual .persistent-deps 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 26 Oct 2017 02:09:39 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Thu, 26 Oct 2017 02:09:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 26 Oct 2017 02:09:40 GMT
RUN mkdir -p $PHP_INI_DIR/conf.d
# Thu, 26 Oct 2017 02:18:33 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data
# Thu, 26 Oct 2017 02:18:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Thu, 26 Oct 2017 02:18:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Thu, 26 Oct 2017 02:18:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 26 Oct 2017 03:02:21 GMT
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
# Mon, 30 Oct 2017 23:33:05 GMT
ENV PHP_VERSION=5.6.32
# Mon, 30 Oct 2017 23:33:05 GMT
ENV PHP_URL=https://secure.php.net/get/php-5.6.32.tar.xz/from/this/mirror PHP_ASC_URL=https://secure.php.net/get/php-5.6.32.tar.xz.asc/from/this/mirror
# Mon, 30 Oct 2017 23:33:05 GMT
ENV PHP_SHA256=8c2b4f721c7475fb9eabda2495209e91ea933082e6f34299d11cba88cd76e64b PHP_MD5=
# Mon, 30 Oct 2017 23:33:37 GMT
RUN set -xe; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		mkdir -p /usr/src; 	cd /usr/src; 		wget -O php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		wget -O php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del .fetch-deps
# Mon, 30 Oct 2017 23:33:37 GMT
COPY file:207c686e3fed4f71f8a7b245d8dcae9c9048d276a326d82b553c12a90af0c0ca in /usr/local/bin/ 
# Mon, 30 Oct 2017 23:36:56 GMT
RUN set -xe 	&& apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		coreutils 		curl-dev 		libedit-dev 		openssl-dev 		libxml2-dev 		sqlite-dev 		&& export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	&& docker-php-source extract 	&& cd /usr/src/php 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--disable-cgi 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pcre-regex=/usr 				$PHP_EXTRA_CONFIGURE_ARGS 	&& make -j "$(nproc)" 	&& make install 	&& { find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; } 	&& make clean 	&& cd / 	&& docker-php-source delete 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .php-rundeps $runDeps 		&& apk del .build-deps 		&& pecl update-channels 	&& rm -rf /tmp/pear ~/.pearrc
# Mon, 30 Oct 2017 23:41:05 GMT
COPY multi:3a3ce8aa3891c64454909e9f8257446a1817abe660b49a7baaa26f28bfdc444d in /usr/local/bin/ 
# Mon, 30 Oct 2017 23:41:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 30 Oct 2017 23:41:05 GMT
WORKDIR /var/www/html
# Mon, 30 Oct 2017 23:41:06 GMT
RUN set -ex 	&& cd /usr/local/etc 	&& if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi 	&& { 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf 	&& { 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = [::]:9000'; 	} | tee php-fpm.d/zz-docker.conf
# Mon, 30 Oct 2017 23:41:06 GMT
EXPOSE 9000/tcp
# Mon, 30 Oct 2017 23:41:07 GMT
CMD ["php-fpm"]
# Tue, 31 Oct 2017 00:40:16 GMT
RUN apk add --no-cache 		bash 		sed
# Tue, 31 Oct 2017 00:40:50 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		libjpeg-turbo-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr; 	docker-php-ext-install gd mysqli opcache; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Tue, 31 Oct 2017 00:40:51 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 		echo 'opcache.enable_cli=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 31 Oct 2017 00:40:51 GMT
VOLUME [/var/www/html]
# Tue, 31 Oct 2017 23:04:22 GMT
ENV WORDPRESS_VERSION=4.8.3
# Tue, 31 Oct 2017 23:04:23 GMT
ENV WORDPRESS_SHA1=8efc0b9f6146e143ed419b5419d7bb8400a696fc
# Tue, 31 Oct 2017 23:04:25 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Tue, 31 Oct 2017 23:04:25 GMT
COPY file:db1f48c4963a4352b4c31c18f102b71fcc06a1266db6edd17f8f52458fe13130 in /usr/local/bin/ 
# Tue, 31 Oct 2017 23:04:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Oct 2017 23:04:25 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:49388a8c9c86a6f56d228954eede699c64fce6c671a989e3e21c391859694645`  
		Last Modified: Wed, 25 Oct 2017 23:22:36 GMT  
		Size: 2.4 MB (2385012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7714ce34247858cb9e07dddd918d6aab795389c9821e77e10edceaee78feee18`  
		Last Modified: Thu, 26 Oct 2017 03:16:37 GMT  
		Size: 1.3 MB (1308944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412dcd2f93dcaf9cff2500231b729aecf237c08f74a12e85aa150c43777c27e5`  
		Last Modified: Thu, 26 Oct 2017 03:16:38 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acafa3a5cc8368e875004fafd3ffd5077704b40f468dabdcc4849a17058a749`  
		Last Modified: Thu, 26 Oct 2017 03:16:34 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42f8caa901e0d2acfeda4906b39c5a9d65c939553c2ca494adeb7df3391de5e`  
		Last Modified: Tue, 31 Oct 2017 00:13:17 GMT  
		Size: 12.5 MB (12483428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f404894a431e22077a54e02844ba335e95286afe69a2eee133b57d9226f5bbd`  
		Last Modified: Tue, 31 Oct 2017 00:13:14 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dadb4c360092fd0f204ae0afe5ac7354d9aa8cfdab8962a605a01aad2128c8b`  
		Last Modified: Tue, 31 Oct 2017 00:13:18 GMT  
		Size: 10.0 MB (10008779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d594ce706e5377e502ea23555d3ee472f04bf28b1708b536e82de711ed07a9b`  
		Last Modified: Tue, 31 Oct 2017 00:13:14 GMT  
		Size: 2.2 KB (2163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7d1b0c19b6b0c52764d769d2a216b52c93e66a2a917f02bc487b5f6e528d7f`  
		Last Modified: Tue, 31 Oct 2017 00:13:15 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1640ec49421d235e73f822bfebcd2f6f8881ab9db1917c167c7b8caf348191cd`  
		Last Modified: Tue, 31 Oct 2017 00:13:14 GMT  
		Size: 7.6 KB (7604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e53b45df727cc91c0d6a893ad839e2713048c2d2e8b02f7fe3fea22f1c1a55`  
		Last Modified: Tue, 31 Oct 2017 01:07:19 GMT  
		Size: 611.8 KB (611802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377e83b204ca210c352945bdca78fa850ae05732190548634d72b387e86dc1c3`  
		Last Modified: Tue, 31 Oct 2017 01:07:19 GMT  
		Size: 733.1 KB (733075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c04d9aacb5b27d74afd0ffa6362e742b19f2e27c9ef0a677204348ef9e258e`  
		Last Modified: Tue, 31 Oct 2017 01:07:22 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22fa3dc75d1f3e4567b84c4c135b0e8e26247206dbdb19c6575fe2dabd7c01c1`  
		Last Modified: Tue, 31 Oct 2017 23:10:00 GMT  
		Size: 8.0 MB (8017227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529e73138d77959131686d4f91be15c7a38ab13a7080b7f69fbefa4648c22bbd`  
		Last Modified: Tue, 31 Oct 2017 23:09:59 GMT  
		Size: 3.2 KB (3216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
