## `wordpress:apache`

```console
$ docker pull wordpress@sha256:066e9c13f5ddb8b16eb47be5e6d3e76d4d5566a5ab097acb7605ae4505489de4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `wordpress:apache` - linux; amd64

```console
$ docker pull wordpress@sha256:303d6a4664d39adc86cb7aa8a02fa62b8d1959a2852e5fa2c59a470e811ea716
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.0 MB (171024076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f3ae7df08ed2ae48a499cb506b388d6d1894951d59ee745e8838de67f464eab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Mon, 09 Oct 2017 21:30:05 GMT
ADD file:55b071e2cfc3ea2f4bbf048d7d676e3c06a77a9a98d63f7af291f3decb495ec8 in / 
# Mon, 09 Oct 2017 21:30:05 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 01:12:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		libpcre3-dev 		make 		pkg-config 		re2c
# Tue, 10 Oct 2017 01:13:02 GMT
RUN apt-get update && apt-get install -y 		$PHPIZE_DEPS 		ca-certificates 		curl 		libedit2 		libsqlite3-0 		libxml2 		xz-utils 	--no-install-recommends && rm -r /var/lib/apt/lists/*
# Tue, 10 Oct 2017 01:13:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 10 Oct 2017 01:13:03 GMT
RUN mkdir -p $PHP_INI_DIR/conf.d
# Tue, 10 Oct 2017 01:22:10 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		apache2 	&& rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 01:22:12 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 10 Oct 2017 01:22:12 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 10 Oct 2017 01:22:13 GMT
RUN set -ex 		&& sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS" 		&& . "$APACHE_ENVVARS" 	&& for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 		/var/www/html 	; do 		rm -rvf "$dir" 		&& mkdir -p "$dir" 		&& chown -R "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 	done
# Tue, 10 Oct 2017 01:22:13 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 10 Oct 2017 01:22:14 GMT
RUN set -ex 	&& . "$APACHE_ENVVARS" 	&& ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log" 	&& ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log" 	&& ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"
# Tue, 10 Oct 2017 01:22:15 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 10 Oct 2017 01:22:15 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 10 Oct 2017 01:22:15 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2
# Tue, 10 Oct 2017 01:22:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Tue, 10 Oct 2017 01:22:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Tue, 10 Oct 2017 01:22:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Tue, 10 Oct 2017 02:14:51 GMT
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
# Mon, 30 Oct 2017 23:10:27 GMT
ENV PHP_VERSION=5.6.32
# Mon, 30 Oct 2017 23:10:27 GMT
ENV PHP_URL=https://secure.php.net/get/php-5.6.32.tar.xz/from/this/mirror PHP_ASC_URL=https://secure.php.net/get/php-5.6.32.tar.xz.asc/from/this/mirror
# Mon, 30 Oct 2017 23:10:27 GMT
ENV PHP_SHA256=8c2b4f721c7475fb9eabda2495209e91ea933082e6f34299d11cba88cd76e64b PHP_MD5=
# Mon, 30 Oct 2017 23:10:50 GMT
RUN set -xe; 		fetchDeps=' 		wget 	'; 	if ! command -v gpg > /dev/null; then 		fetchDeps="$fetchDeps 			dirmngr 			gnupg2 		"; 	fi; 	apt-get update; 	apt-get install -y --no-install-recommends $fetchDeps; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		wget -O php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		wget -O php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps
# Mon, 30 Oct 2017 23:10:51 GMT
COPY file:207c686e3fed4f71f8a7b245d8dcae9c9048d276a326d82b553c12a90af0c0ca in /usr/local/bin/ 
# Mon, 30 Oct 2017 23:13:19 GMT
RUN set -xe 	&& buildDeps=" 		$PHP_EXTRA_BUILD_DEPS 		libcurl4-openssl-dev 		libedit-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	" 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	&& docker-php-source extract 	&& cd /usr/src/php 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)" 	&& if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi 	&& ./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--disable-cgi 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pcre-regex=/usr 		--with-libdir="lib/$debMultiarch" 				$PHP_EXTRA_CONFIGURE_ARGS 	&& make -j "$(nproc)" 	&& make install 	&& { find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; } 	&& make clean 	&& cd / 	&& docker-php-source delete 		&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $buildDeps 		&& pecl update-channels 	&& rm -rf /tmp/pear ~/.pearrc
# Mon, 30 Oct 2017 23:16:19 GMT
COPY multi:dbabcc0b81566a75f49e7faa9ca5f96cd22a515b80ee7ea1e34fceceee3f9c2a in /usr/local/bin/ 
# Mon, 30 Oct 2017 23:16:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 30 Oct 2017 23:16:20 GMT
COPY file:24613ecbb1ce6a09f683b0753da9c26a1af07547326e8a02f6eec80ad6f2774a in /usr/local/bin/ 
# Mon, 30 Oct 2017 23:16:20 GMT
WORKDIR /var/www/html
# Mon, 30 Oct 2017 23:16:20 GMT
EXPOSE 80/tcp
# Mon, 30 Oct 2017 23:16:20 GMT
CMD ["apache2-foreground"]
# Tue, 31 Oct 2017 00:39:04 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y 		libjpeg-dev 		libpng-dev 	; 	rm -rf /var/lib/apt/lists/*; 		docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr; 	docker-php-ext-install gd mysqli opcache
# Tue, 31 Oct 2017 00:39:05 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 		echo 'opcache.enable_cli=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 31 Oct 2017 00:39:06 GMT
RUN a2enmod rewrite expires
# Tue, 31 Oct 2017 00:39:06 GMT
VOLUME [/var/www/html]
# Tue, 31 Oct 2017 23:04:00 GMT
ENV WORDPRESS_VERSION=4.8.3
# Tue, 31 Oct 2017 23:04:00 GMT
ENV WORDPRESS_SHA1=8efc0b9f6146e143ed419b5419d7bb8400a696fc
# Tue, 31 Oct 2017 23:04:02 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Tue, 31 Oct 2017 23:04:03 GMT
COPY file:db1f48c4963a4352b4c31c18f102b71fcc06a1266db6edd17f8f52458fe13130 in /usr/local/bin/ 
# Tue, 31 Oct 2017 23:04:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Oct 2017 23:04:03 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:85b1f47fba49da65256f07c8790542a3880e9216f9c491965040f35ce2c6ca7a`  
		Last Modified: Mon, 09 Oct 2017 21:36:40 GMT  
		Size: 52.6 MB (52595124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e22dddbf921907e82e3dbea870be475c0d58274774f04af85407e06ae4c6ba`  
		Last Modified: Tue, 10 Oct 2017 02:33:19 GMT  
		Size: 82.5 MB (82497677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0df491fd2e905203a9dd11b8efc67a152337cdea7168cbece4e430d13d05f6`  
		Last Modified: Tue, 10 Oct 2017 02:33:00 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:425226034711dd26e5829df0fb8971dfb8e5cfa13268ff67d1b8c23db0dd3274`  
		Last Modified: Tue, 10 Oct 2017 02:34:30 GMT  
		Size: 3.0 MB (3012916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba5c1815115971b0359b716d5638f959880a1b2a904ff0e048f76c66b7833e2`  
		Last Modified: Tue, 10 Oct 2017 02:34:29 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ab63dc099c167bdaff469cf4d01512f9b680b88a3f04c6188aa6f7a591fd34`  
		Last Modified: Tue, 10 Oct 2017 02:34:27 GMT  
		Size: 430.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389f9436e431e262b395b2348f6266933830cfd69cbe41775e6e022e9c828167`  
		Last Modified: Tue, 10 Oct 2017 02:34:27 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bc131d410eb84162eeea976435d25cd8b7ec8c75fbd2b77f5e872d23d42f5e`  
		Last Modified: Tue, 10 Oct 2017 02:34:27 GMT  
		Size: 484.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457ec74054f2550166055dc178a9ff024d2dc85e3a34f6fe1a86c9c56db96e29`  
		Last Modified: Tue, 31 Oct 2017 00:06:30 GMT  
		Size: 12.8 MB (12818709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff1a33a03f76ec6c718970b869d96b864ce1085cf94e2534c8bb1ec4dd161d1`  
		Last Modified: Tue, 31 Oct 2017 00:06:24 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6802925a83f8685b4aac0f57ac4b7e999655a97ec0978d8077551ed58546fe`  
		Last Modified: Tue, 31 Oct 2017 00:06:26 GMT  
		Size: 9.7 MB (9690983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b2639141e1d1c275bb30d7a412adeba434dca2e1d3b6d5b7e51c0e9e9b3c59`  
		Last Modified: Tue, 31 Oct 2017 00:06:24 GMT  
		Size: 2.2 KB (2181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b02b646409973384d5f734c65816e69af4f37e842d90025f79dc6a9fae21217`  
		Last Modified: Tue, 31 Oct 2017 00:06:24 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf2a146ddc0a6b103248b68d6f2e26d19497e7fa0fb795eb20d5e089ed766aa`  
		Last Modified: Tue, 31 Oct 2017 00:58:05 GMT  
		Size: 2.4 MB (2382129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cc7d14c1eda78646ec401ed7753f003539a838785070e91604077a9e02a44b`  
		Last Modified: Tue, 31 Oct 2017 00:58:06 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b2ef7e52181c4a001db89c55d05f6c7c4c7c434ee2c530a356755a8420250a`  
		Last Modified: Tue, 31 Oct 2017 00:58:04 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd6734484e20561fd803b9f87f4bff474f61153836a88e59e3ccaa7cd980ac0`  
		Last Modified: Tue, 31 Oct 2017 23:05:58 GMT  
		Size: 8.0 MB (8016452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725e747b6a5165a6cda70d50325a032d8a69912344453a3e83570e25cce1245f`  
		Last Modified: Tue, 31 Oct 2017 23:05:56 GMT  
		Size: 3.2 KB (3223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:apache` - linux; arm variant v5

```console
$ docker pull wordpress@sha256:ea61a3cf27126acc002fd00c9e97cb8876bde08bf4a1b5e9b6d9b1cc3878fbfc
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.6 MB (149579216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5032b3531736c9b0ae17a4ad0d71d03e7d2e7d2d65e083d7ff1179d864376b84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:07 GMT
ADD file:cfee2e008c8ea154a9e6408e017dd40cc1b53f7c31932cec7fa8e1dc14649764 in / 
# Mon, 09 Oct 2017 21:42:07 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:44:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		libpcre3-dev 		make 		pkg-config 		re2c
# Mon, 09 Oct 2017 22:45:58 GMT
RUN apt-get update && apt-get install -y 		$PHPIZE_DEPS 		ca-certificates 		curl 		libedit2 		libsqlite3-0 		libxml2 		xz-utils 	--no-install-recommends && rm -r /var/lib/apt/lists/*
# Mon, 09 Oct 2017 22:45:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 09 Oct 2017 22:46:00 GMT
RUN mkdir -p $PHP_INI_DIR/conf.d
# Mon, 09 Oct 2017 22:51:00 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		apache2 	&& rm -rf /var/lib/apt/lists/*
# Mon, 09 Oct 2017 22:51:01 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Mon, 09 Oct 2017 22:51:01 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Mon, 09 Oct 2017 22:51:02 GMT
RUN set -ex 		&& sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS" 		&& . "$APACHE_ENVVARS" 	&& for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 		/var/www/html 	; do 		rm -rvf "$dir" 		&& mkdir -p "$dir" 		&& chown -R "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 	done
# Mon, 09 Oct 2017 22:51:03 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Mon, 09 Oct 2017 22:51:04 GMT
RUN set -ex 	&& . "$APACHE_ENVVARS" 	&& ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log" 	&& ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log" 	&& ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"
# Mon, 09 Oct 2017 22:51:05 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Mon, 09 Oct 2017 22:51:05 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Mon, 09 Oct 2017 22:51:05 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2
# Mon, 09 Oct 2017 22:51:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Mon, 09 Oct 2017 22:51:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Mon, 09 Oct 2017 22:51:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Mon, 09 Oct 2017 23:25:43 GMT
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
# Tue, 31 Oct 2017 13:58:52 GMT
ENV PHP_VERSION=5.6.32
# Tue, 31 Oct 2017 13:58:53 GMT
ENV PHP_URL=https://secure.php.net/get/php-5.6.32.tar.xz/from/this/mirror PHP_ASC_URL=https://secure.php.net/get/php-5.6.32.tar.xz.asc/from/this/mirror
# Tue, 31 Oct 2017 13:58:53 GMT
ENV PHP_SHA256=8c2b4f721c7475fb9eabda2495209e91ea933082e6f34299d11cba88cd76e64b PHP_MD5=
# Fri, 03 Nov 2017 14:24:34 GMT
RUN set -xe; 		fetchDeps=' 		wget 	'; 	if ! command -v gpg > /dev/null; then 		fetchDeps="$fetchDeps 			dirmngr 			gnupg 		"; 	fi; 	apt-get update; 	apt-get install -y --no-install-recommends $fetchDeps; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		wget -O php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		wget -O php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps
# Fri, 03 Nov 2017 14:24:34 GMT
COPY file:207c686e3fed4f71f8a7b245d8dcae9c9048d276a326d82b553c12a90af0c0ca in /usr/local/bin/ 
# Fri, 03 Nov 2017 14:27:10 GMT
RUN set -xe 	&& buildDeps=" 		$PHP_EXTRA_BUILD_DEPS 		libcurl4-openssl-dev 		libedit-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	" 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	&& docker-php-source extract 	&& cd /usr/src/php 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)" 	&& if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi 	&& ./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--disable-cgi 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pcre-regex=/usr 		--with-libdir="lib/$debMultiarch" 				$PHP_EXTRA_CONFIGURE_ARGS 	&& make -j "$(nproc)" 	&& make install 	&& { find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; } 	&& make clean 	&& cd / 	&& docker-php-source delete 		&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $buildDeps 		&& pecl update-channels 	&& rm -rf /tmp/pear ~/.pearrc
# Fri, 03 Nov 2017 14:27:11 GMT
COPY multi:dbabcc0b81566a75f49e7faa9ca5f96cd22a515b80ee7ea1e34fceceee3f9c2a in /usr/local/bin/ 
# Fri, 03 Nov 2017 14:27:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Nov 2017 14:27:11 GMT
COPY file:24613ecbb1ce6a09f683b0753da9c26a1af07547326e8a02f6eec80ad6f2774a in /usr/local/bin/ 
# Fri, 03 Nov 2017 14:27:12 GMT
WORKDIR /var/www/html
# Fri, 03 Nov 2017 14:27:12 GMT
EXPOSE 80/tcp
# Fri, 03 Nov 2017 14:27:12 GMT
CMD ["apache2-foreground"]
# Fri, 03 Nov 2017 15:03:34 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y 		libjpeg-dev 		libpng-dev 	; 	rm -rf /var/lib/apt/lists/*; 		docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr; 	docker-php-ext-install gd mysqli opcache
# Fri, 03 Nov 2017 15:03:35 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 		echo 'opcache.enable_cli=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 03 Nov 2017 15:03:36 GMT
RUN a2enmod rewrite expires
# Fri, 03 Nov 2017 15:03:37 GMT
VOLUME [/var/www/html]
# Fri, 03 Nov 2017 15:03:37 GMT
ENV WORDPRESS_VERSION=4.8.3
# Fri, 03 Nov 2017 15:03:37 GMT
ENV WORDPRESS_SHA1=8efc0b9f6146e143ed419b5419d7bb8400a696fc
# Fri, 03 Nov 2017 15:03:41 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 03 Nov 2017 15:03:41 GMT
COPY file:db1f48c4963a4352b4c31c18f102b71fcc06a1266db6edd17f8f52458fe13130 in /usr/local/bin/ 
# Fri, 03 Nov 2017 15:03:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 15:03:42 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:29dee24d6376416a80f3fdb145082e8dd352694bfdcf639e49e26ddbf8d8cb52`  
		Last Modified: Mon, 09 Oct 2017 21:47:16 GMT  
		Size: 50.9 MB (50879894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad1ba133bf708efd9b75cf971201a4ed647286864942a66d5c9d86b126f9b92`  
		Last Modified: Mon, 09 Oct 2017 23:39:58 GMT  
		Size: 63.5 MB (63526955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa24f60e9c2ee1e5256863f0b528469123443a094ca2c8a19dfe9890a89b664a`  
		Last Modified: Mon, 09 Oct 2017 23:39:37 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2226c6d34b25989365cc4d9036799ca2fefec786911c54f67ef906f4b9bb76`  
		Last Modified: Mon, 09 Oct 2017 23:40:30 GMT  
		Size: 2.8 MB (2824242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589b717d3a226bfcde3047ef4cf6d796173d1f4a1ece0bc788271c06f29bba47`  
		Last Modified: Mon, 09 Oct 2017 23:40:29 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae277f94e125f9b12232fd0cb072c63090cad8a41f1c77e71b4c5374e5656946`  
		Last Modified: Mon, 09 Oct 2017 23:40:28 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11585a82e3a977c923548ce1364988534f529c5cb4b2555e3698a2f16cfd978f`  
		Last Modified: Mon, 09 Oct 2017 23:40:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e034a32b45a003b5387a7745c9c1e5ccc4fd3dc902b42894564087c846344889`  
		Last Modified: Mon, 09 Oct 2017 23:40:28 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dae074e268b2a7759e82ccc1e756158a26a1cbb4914b4288dc16d02fbd25356`  
		Last Modified: Fri, 03 Nov 2017 14:44:17 GMT  
		Size: 12.8 MB (12817005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abaa88b8add63c70b59297d4eb97ff0c9a0557f6d07eb873c6b6abd83cf1974`  
		Last Modified: Fri, 03 Nov 2017 14:44:15 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521c37ec6b75ab8bf3811477491d9d1ea027ed1da368411657a97966bc270839`  
		Last Modified: Fri, 03 Nov 2017 14:44:18 GMT  
		Size: 9.3 MB (9277756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c5e63483298b7dea1e5da5794d9c0d661728f55f82d9992992bb15cefa3aa2`  
		Last Modified: Fri, 03 Nov 2017 14:44:14 GMT  
		Size: 2.2 KB (2180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9863356fb78a785aed66d0a2ebfb81081d60d04d86946880ca763f00584961c`  
		Last Modified: Fri, 03 Nov 2017 14:44:15 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7326a80d644d6db87cc61b20af7cba249541e9073cde641cb3fa77b7bd65aa`  
		Last Modified: Fri, 03 Nov 2017 15:14:05 GMT  
		Size: 2.2 MB (2226674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0cafb7d9997b3a76f59ce0205b38e2c3c76c02d2785f5ecb36db2ba534ff50`  
		Last Modified: Fri, 03 Nov 2017 15:14:04 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec66e0dfc9a987360dad7b585aa6ba12a3cad95c743c564942bede11778c032`  
		Last Modified: Fri, 03 Nov 2017 15:14:04 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8acd37b194bca6d0087e74e2db665527d75e3d248d404da6c4920f8302a023`  
		Last Modified: Fri, 03 Nov 2017 15:14:07 GMT  
		Size: 8.0 MB (8016479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f3966718a59348e1a198eb215aca9c4089dc605f0ca636cfdeae8bff0f42fd`  
		Last Modified: Fri, 03 Nov 2017 15:14:04 GMT  
		Size: 3.2 KB (3224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:apache` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:ebc9c1d7def4711122957ab55052faff09e142b3d289d3a5c338d4cfa77d0160
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.0 MB (146987352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12cc2609df42e565691d3b602dc2852b2c00f39ad13c9e3203069c568e864163`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:19 GMT
ADD file:68eabcdf7d9c5518c34f691d547b77534be3929ad958c8835c5d4a54114c7ee4 in / 
# Mon, 09 Oct 2017 21:42:20 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 23:08:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		libpcre3-dev 		make 		pkg-config 		re2c
# Mon, 09 Oct 2017 23:10:02 GMT
RUN apt-get update && apt-get install -y 		$PHPIZE_DEPS 		ca-certificates 		curl 		libedit2 		libsqlite3-0 		libxml2 		xz-utils 	--no-install-recommends && rm -r /var/lib/apt/lists/*
# Mon, 09 Oct 2017 23:10:03 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 09 Oct 2017 23:10:04 GMT
RUN mkdir -p $PHP_INI_DIR/conf.d
# Mon, 09 Oct 2017 23:15:10 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		apache2 	&& rm -rf /var/lib/apt/lists/*
# Mon, 09 Oct 2017 23:15:10 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Mon, 09 Oct 2017 23:15:14 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Mon, 09 Oct 2017 23:15:16 GMT
RUN set -ex 		&& sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS" 		&& . "$APACHE_ENVVARS" 	&& for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 		/var/www/html 	; do 		rm -rvf "$dir" 		&& mkdir -p "$dir" 		&& chown -R "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 	done
# Mon, 09 Oct 2017 23:15:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Mon, 09 Oct 2017 23:15:19 GMT
RUN set -ex 	&& . "$APACHE_ENVVARS" 	&& ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log" 	&& ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log" 	&& ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"
# Mon, 09 Oct 2017 23:15:23 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Mon, 09 Oct 2017 23:15:27 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Mon, 09 Oct 2017 23:15:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2
# Mon, 09 Oct 2017 23:15:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Mon, 09 Oct 2017 23:15:31 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Mon, 09 Oct 2017 23:15:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Mon, 09 Oct 2017 23:49:05 GMT
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
# Tue, 31 Oct 2017 12:09:15 GMT
ENV PHP_VERSION=5.6.32
# Tue, 31 Oct 2017 12:09:15 GMT
ENV PHP_URL=https://secure.php.net/get/php-5.6.32.tar.xz/from/this/mirror PHP_ASC_URL=https://secure.php.net/get/php-5.6.32.tar.xz.asc/from/this/mirror
# Tue, 31 Oct 2017 12:09:15 GMT
ENV PHP_SHA256=8c2b4f721c7475fb9eabda2495209e91ea933082e6f34299d11cba88cd76e64b PHP_MD5=
# Fri, 03 Nov 2017 12:38:42 GMT
RUN set -xe; 		fetchDeps=' 		wget 	'; 	if ! command -v gpg > /dev/null; then 		fetchDeps="$fetchDeps 			dirmngr 			gnupg 		"; 	fi; 	apt-get update; 	apt-get install -y --no-install-recommends $fetchDeps; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		wget -O php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		wget -O php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps
# Fri, 03 Nov 2017 12:38:43 GMT
COPY file:207c686e3fed4f71f8a7b245d8dcae9c9048d276a326d82b553c12a90af0c0ca in /usr/local/bin/ 
# Fri, 03 Nov 2017 12:41:10 GMT
RUN set -xe 	&& buildDeps=" 		$PHP_EXTRA_BUILD_DEPS 		libcurl4-openssl-dev 		libedit-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	" 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	&& docker-php-source extract 	&& cd /usr/src/php 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)" 	&& if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi 	&& ./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--disable-cgi 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pcre-regex=/usr 		--with-libdir="lib/$debMultiarch" 				$PHP_EXTRA_CONFIGURE_ARGS 	&& make -j "$(nproc)" 	&& make install 	&& { find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; } 	&& make clean 	&& cd / 	&& docker-php-source delete 		&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $buildDeps 		&& pecl update-channels 	&& rm -rf /tmp/pear ~/.pearrc
# Fri, 03 Nov 2017 12:41:11 GMT
COPY multi:dbabcc0b81566a75f49e7faa9ca5f96cd22a515b80ee7ea1e34fceceee3f9c2a in /usr/local/bin/ 
# Fri, 03 Nov 2017 12:41:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Nov 2017 12:41:11 GMT
COPY file:24613ecbb1ce6a09f683b0753da9c26a1af07547326e8a02f6eec80ad6f2774a in /usr/local/bin/ 
# Fri, 03 Nov 2017 12:41:12 GMT
WORKDIR /var/www/html
# Fri, 03 Nov 2017 12:41:12 GMT
EXPOSE 80/tcp
# Fri, 03 Nov 2017 12:41:12 GMT
CMD ["apache2-foreground"]
# Fri, 03 Nov 2017 13:39:33 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y 		libjpeg-dev 		libpng-dev 	; 	rm -rf /var/lib/apt/lists/*; 		docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr; 	docker-php-ext-install gd mysqli opcache
# Fri, 03 Nov 2017 13:39:45 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 		echo 'opcache.enable_cli=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 03 Nov 2017 13:39:59 GMT
RUN a2enmod rewrite expires
# Fri, 03 Nov 2017 13:40:05 GMT
VOLUME [/var/www/html]
# Fri, 03 Nov 2017 13:40:12 GMT
ENV WORDPRESS_VERSION=4.8.3
# Fri, 03 Nov 2017 13:40:20 GMT
ENV WORDPRESS_SHA1=8efc0b9f6146e143ed419b5419d7bb8400a696fc
# Fri, 03 Nov 2017 13:40:30 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 03 Nov 2017 13:40:41 GMT
COPY file:db1f48c4963a4352b4c31c18f102b71fcc06a1266db6edd17f8f52458fe13130 in /usr/local/bin/ 
# Fri, 03 Nov 2017 13:40:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 13:40:48 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:e52c47bf5ccb0baf5e58ae2e958abbb260f942d8743078a07a367079102e162f`  
		Last Modified: Mon, 09 Oct 2017 21:48:44 GMT  
		Size: 48.7 MB (48686311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be530d54777d3b6901a69cebe98eb5b0bde4c6c3d6ab1447b9c76a1b7c86069d`  
		Last Modified: Tue, 10 Oct 2017 00:03:17 GMT  
		Size: 63.8 MB (63794787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4780c6a3912aa6ac660ed0fc0c12bba611f9ef448dfa9a5ba381e9f64e6c5e9`  
		Last Modified: Tue, 10 Oct 2017 00:02:59 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2b072a68b1ce966d087589a733ae3bcdae5bae86a87514685551381cba07f7`  
		Last Modified: Tue, 10 Oct 2017 00:03:59 GMT  
		Size: 2.7 MB (2679426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b5aa77f567a1f48fd4330791ccad8dfd3fc253242827b0bdb542f09ce6ea24`  
		Last Modified: Tue, 10 Oct 2017 00:03:59 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6631b21dd7133ce0dee7db390449eb7531c9172eec2f5013dd1a3932d54f885b`  
		Last Modified: Tue, 10 Oct 2017 00:03:58 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee4dfbed472dc58e234d5bdb206374277f6c6b3e3e684c15dd7ec6afd46e88e`  
		Last Modified: Tue, 10 Oct 2017 00:03:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d81fa28c2f426fba5560a1cda751278130e9becbcbcf17f06bc3a3832f45366`  
		Last Modified: Tue, 10 Oct 2017 00:03:58 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2447d20fd75821a18a601d71fbcefc0725ddc34e58085bf08aa67001ad1b8a91`  
		Last Modified: Fri, 03 Nov 2017 13:04:37 GMT  
		Size: 12.8 MB (12816969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a232e53b4fc48df3533a2ebee8831839564724e2e38b7aa1abd86abd183b501a`  
		Last Modified: Fri, 03 Nov 2017 13:04:35 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88c24f502bb2ee8c21e97b9a2da56d795b76daed858012533d49578e77cbd9e`  
		Last Modified: Fri, 03 Nov 2017 13:04:38 GMT  
		Size: 8.8 MB (8841318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385975715fd0e05b1d52f80d5afd3b0a3ee763a75a057496ac04d120f8e050df`  
		Last Modified: Fri, 03 Nov 2017 13:04:35 GMT  
		Size: 2.2 KB (2179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6de79fcfcb59b0451c7ea737bc2d82239cd01f753f26b7ce67f8b46d6203d1b`  
		Last Modified: Fri, 03 Nov 2017 13:04:35 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9983a77739c1e4d16532ea8908c030a910953d1b5808bbbffca4fd7fe575adf4`  
		Last Modified: Fri, 03 Nov 2017 13:52:27 GMT  
		Size: 2.1 MB (2141846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cfb3048492cf03517228061fa6d4775d5262b7726b6d175fb736a6b8c126a2`  
		Last Modified: Fri, 03 Nov 2017 13:52:26 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ec0de3da40ac91b753caf27078b5b84ebfc356df4ea6841e00e60a6df7cfd9`  
		Last Modified: Fri, 03 Nov 2017 13:52:25 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73347db3c699200e32af35c0d43a17edb79181f1d6c9b61ff593257628220d75`  
		Last Modified: Fri, 03 Nov 2017 13:52:30 GMT  
		Size: 8.0 MB (8016484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19179e6a759f9d53d4739952b22b16f49e5c5d7ac64696a89b472fb48e3fff44`  
		Last Modified: Fri, 03 Nov 2017 13:52:26 GMT  
		Size: 3.2 KB (3221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:apache` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:fd76def79ed5269594276cf9f5bce9d51e31a1e7508a827c20bad7f73f7818cc
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.6 MB (149558796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:703fd796f8d27d9e0f6183f0676f281e4acd871df36f7653edcb4f50a1627449`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Mon, 09 Oct 2017 21:43:13 GMT
ADD file:1661271485aa5a1ca074498b8ca025f41e547bf2b33335b108d9aaa06717b2a5 in / 
# Mon, 09 Oct 2017 21:43:14 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 03:01:07 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		libpcre3-dev 		make 		pkg-config 		re2c
# Tue, 10 Oct 2017 03:02:43 GMT
RUN apt-get update && apt-get install -y 		$PHPIZE_DEPS 		ca-certificates 		curl 		libedit2 		libsqlite3-0 		libxml2 		xz-utils 	--no-install-recommends && rm -r /var/lib/apt/lists/*
# Tue, 10 Oct 2017 03:02:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 10 Oct 2017 03:02:47 GMT
RUN mkdir -p $PHP_INI_DIR/conf.d
# Tue, 10 Oct 2017 03:12:18 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		apache2 	&& rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 03:12:19 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 10 Oct 2017 03:12:20 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 10 Oct 2017 03:12:21 GMT
RUN set -ex 		&& sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS" 		&& . "$APACHE_ENVVARS" 	&& for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 		/var/www/html 	; do 		rm -rvf "$dir" 		&& mkdir -p "$dir" 		&& chown -R "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 	done
# Tue, 10 Oct 2017 03:12:23 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 10 Oct 2017 03:12:25 GMT
RUN set -ex 	&& . "$APACHE_ENVVARS" 	&& ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log" 	&& ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log" 	&& ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"
# Tue, 10 Oct 2017 03:12:27 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 10 Oct 2017 03:12:27 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 10 Oct 2017 03:12:28 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2
# Tue, 10 Oct 2017 03:12:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Tue, 10 Oct 2017 03:12:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Tue, 10 Oct 2017 03:12:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Tue, 10 Oct 2017 04:17:26 GMT
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
# Tue, 31 Oct 2017 02:35:57 GMT
ENV PHP_VERSION=5.6.32
# Tue, 31 Oct 2017 02:35:58 GMT
ENV PHP_URL=https://secure.php.net/get/php-5.6.32.tar.xz/from/this/mirror PHP_ASC_URL=https://secure.php.net/get/php-5.6.32.tar.xz.asc/from/this/mirror
# Tue, 31 Oct 2017 02:35:59 GMT
ENV PHP_SHA256=8c2b4f721c7475fb9eabda2495209e91ea933082e6f34299d11cba88cd76e64b PHP_MD5=
# Fri, 03 Nov 2017 03:36:10 GMT
RUN set -xe; 		fetchDeps=' 		wget 	'; 	if ! command -v gpg > /dev/null; then 		fetchDeps="$fetchDeps 			dirmngr 			gnupg 		"; 	fi; 	apt-get update; 	apt-get install -y --no-install-recommends $fetchDeps; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		wget -O php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		wget -O php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps
# Fri, 03 Nov 2017 03:36:11 GMT
COPY file:207c686e3fed4f71f8a7b245d8dcae9c9048d276a326d82b553c12a90af0c0ca in /usr/local/bin/ 
# Fri, 03 Nov 2017 03:40:49 GMT
RUN set -xe 	&& buildDeps=" 		$PHP_EXTRA_BUILD_DEPS 		libcurl4-openssl-dev 		libedit-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	" 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	&& docker-php-source extract 	&& cd /usr/src/php 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)" 	&& if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi 	&& ./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--disable-cgi 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pcre-regex=/usr 		--with-libdir="lib/$debMultiarch" 				$PHP_EXTRA_CONFIGURE_ARGS 	&& make -j "$(nproc)" 	&& make install 	&& { find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; } 	&& make clean 	&& cd / 	&& docker-php-source delete 		&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $buildDeps 		&& pecl update-channels 	&& rm -rf /tmp/pear ~/.pearrc
# Fri, 03 Nov 2017 03:40:50 GMT
COPY multi:dbabcc0b81566a75f49e7faa9ca5f96cd22a515b80ee7ea1e34fceceee3f9c2a in /usr/local/bin/ 
# Fri, 03 Nov 2017 03:40:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Nov 2017 03:40:52 GMT
COPY file:24613ecbb1ce6a09f683b0753da9c26a1af07547326e8a02f6eec80ad6f2774a in /usr/local/bin/ 
# Fri, 03 Nov 2017 03:40:52 GMT
WORKDIR /var/www/html
# Fri, 03 Nov 2017 03:40:53 GMT
EXPOSE 80/tcp
# Fri, 03 Nov 2017 03:40:54 GMT
CMD ["apache2-foreground"]
# Sat, 04 Nov 2017 03:14:19 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y 		libjpeg-dev 		libpng-dev 	; 	rm -rf /var/lib/apt/lists/*; 		docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr; 	docker-php-ext-install gd mysqli opcache
# Sat, 04 Nov 2017 03:14:21 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 		echo 'opcache.enable_cli=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 04 Nov 2017 03:14:23 GMT
RUN a2enmod rewrite expires
# Sat, 04 Nov 2017 03:14:23 GMT
VOLUME [/var/www/html]
# Sat, 04 Nov 2017 03:14:24 GMT
ENV WORDPRESS_VERSION=4.8.3
# Sat, 04 Nov 2017 03:14:25 GMT
ENV WORDPRESS_SHA1=8efc0b9f6146e143ed419b5419d7bb8400a696fc
# Sat, 04 Nov 2017 03:14:30 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Sat, 04 Nov 2017 03:14:31 GMT
COPY file:db1f48c4963a4352b4c31c18f102b71fcc06a1266db6edd17f8f52458fe13130 in /usr/local/bin/ 
# Sat, 04 Nov 2017 03:14:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Nov 2017 03:14:32 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:abcff42ba939437677463734d9b81de5e60df7354c734ee3ddd879c0d3d5d595`  
		Last Modified: Mon, 09 Oct 2017 21:52:08 GMT  
		Size: 49.9 MB (49929310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566f7722328920229649e457c4c3f2ac00fbc51bf18e43b7e857a4bb929b14d3`  
		Last Modified: Tue, 10 Oct 2017 04:44:17 GMT  
		Size: 64.6 MB (64612700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336490976ea28a6a8a9bb6f3a9127ff718ef2f6b0ae5d00edc65504b2d61d00f`  
		Last Modified: Tue, 10 Oct 2017 04:43:16 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5dfd27021291ce354f213b19477dca9773fc1e56e213325ec2a820d746e2352`  
		Last Modified: Tue, 10 Oct 2017 04:46:10 GMT  
		Size: 2.8 MB (2788801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3ee4cd0d79dae5f32da9d943aa5e9c7f4d09d054780c65543e9af1cdd34eb5`  
		Last Modified: Tue, 10 Oct 2017 04:46:09 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5530aefb17865ebab2db37820b31434bde95050efc2d0c10281fc07567c70a`  
		Last Modified: Tue, 10 Oct 2017 04:46:06 GMT  
		Size: 430.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b640e2157bfabb87c7e4f4d15a7618d263128e48f2a7c5544050b30ba743f19b`  
		Last Modified: Tue, 10 Oct 2017 04:46:07 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfe762267100f0627688ec8a9bba8612e0e698fe064150f0a41b9310bd45a5e`  
		Last Modified: Tue, 10 Oct 2017 04:46:06 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a69c0a36dd12a11241fc1ac95d0b7a4cb83b7e7a7fc5384607aac0fe9d0e6e`  
		Last Modified: Sat, 04 Nov 2017 02:20:04 GMT  
		Size: 12.8 MB (12816360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967645f9b571d2d16214552e988c2da286a1a0544d2f97c8c2350f488bd746b4`  
		Last Modified: Sat, 04 Nov 2017 02:20:01 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7062b1fb1c0d21fd416d27d9885553dccfc6e87937e2991dbe99dcdb9800c326`  
		Last Modified: Sat, 04 Nov 2017 02:20:05 GMT  
		Size: 9.1 MB (9070615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a4de3ba5e7415fe01365afc926cadf40c9af6b84e9efa057a5178174a9acfe`  
		Last Modified: Sat, 04 Nov 2017 02:20:01 GMT  
		Size: 2.2 KB (2183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713a3bb5a8f6d0b97b92730c00754d5fa7840e29a695393f80a143027f332a53`  
		Last Modified: Sat, 04 Nov 2017 02:20:02 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644163c2b738e1d82a83b0f3f604df9668b9af60c37d4c1d462edcfc83dae182`  
		Last Modified: Sat, 04 Nov 2017 03:27:30 GMT  
		Size: 2.3 MB (2314454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7283be658dab498dd0aef530953b2afe2f1d0fccea8fb9f6bbed7f3f0aaee899`  
		Last Modified: Sat, 04 Nov 2017 03:27:28 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3352ab1132bc66d0e3c97f5951fe107ec8811e86b8c3526f6ba3b7d333c870`  
		Last Modified: Sat, 04 Nov 2017 03:27:28 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839236e95c4b8f6fc4de6c0bb25463ee677e88efc49c82003c32c538928db0b6`  
		Last Modified: Sat, 04 Nov 2017 03:27:32 GMT  
		Size: 8.0 MB (8016452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e912d601dc5111b0ad37a39f85ea27297608007e7350a26df2af649ce05e7b`  
		Last Modified: Sat, 04 Nov 2017 03:27:29 GMT  
		Size: 3.2 KB (3225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:apache` - linux; 386

```console
$ docker pull wordpress@sha256:46ee2ec02542c1a215bf541db2f3565657bfb527d910cb75b7cbf98044b3605b
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.0 MB (173013734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5251452d4d08dee7e593b2266b1e2a86e3b0046ac39d02794dc2f115c15e39e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:15 GMT
ADD file:69555c5f78a887c075ee9d9449d85a723324e07872867c7f577e7fa99f6d41c0 in / 
# Mon, 09 Oct 2017 21:42:15 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 00:46:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		libpcre3-dev 		make 		pkg-config 		re2c
# Tue, 10 Oct 2017 00:47:26 GMT
RUN apt-get update && apt-get install -y 		$PHPIZE_DEPS 		ca-certificates 		curl 		libedit2 		libsqlite3-0 		libxml2 		xz-utils 	--no-install-recommends && rm -r /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:47:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 10 Oct 2017 00:48:10 GMT
RUN mkdir -p $PHP_INI_DIR/conf.d
# Tue, 10 Oct 2017 00:57:55 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		apache2 	&& rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:57:55 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 10 Oct 2017 00:57:55 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 10 Oct 2017 00:57:56 GMT
RUN set -ex 		&& sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS" 		&& . "$APACHE_ENVVARS" 	&& for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 		/var/www/html 	; do 		rm -rvf "$dir" 		&& mkdir -p "$dir" 		&& chown -R "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 	done
# Tue, 10 Oct 2017 00:57:57 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 10 Oct 2017 00:57:58 GMT
RUN set -ex 	&& . "$APACHE_ENVVARS" 	&& ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log" 	&& ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log" 	&& ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"
# Tue, 10 Oct 2017 00:57:59 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 10 Oct 2017 00:57:59 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 10 Oct 2017 00:57:59 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2
# Tue, 10 Oct 2017 00:58:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Tue, 10 Oct 2017 00:58:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Tue, 10 Oct 2017 00:58:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Tue, 10 Oct 2017 01:52:09 GMT
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
# Tue, 31 Oct 2017 09:17:17 GMT
ENV PHP_VERSION=5.6.32
# Tue, 31 Oct 2017 09:17:17 GMT
ENV PHP_URL=https://secure.php.net/get/php-5.6.32.tar.xz/from/this/mirror PHP_ASC_URL=https://secure.php.net/get/php-5.6.32.tar.xz.asc/from/this/mirror
# Tue, 31 Oct 2017 09:17:17 GMT
ENV PHP_SHA256=8c2b4f721c7475fb9eabda2495209e91ea933082e6f34299d11cba88cd76e64b PHP_MD5=
# Fri, 03 Nov 2017 10:24:16 GMT
RUN set -xe; 		fetchDeps=' 		wget 	'; 	if ! command -v gpg > /dev/null; then 		fetchDeps="$fetchDeps 			dirmngr 			gnupg 		"; 	fi; 	apt-get update; 	apt-get install -y --no-install-recommends $fetchDeps; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		wget -O php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		wget -O php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps
# Fri, 03 Nov 2017 10:24:16 GMT
COPY file:207c686e3fed4f71f8a7b245d8dcae9c9048d276a326d82b553c12a90af0c0ca in /usr/local/bin/ 
# Fri, 03 Nov 2017 10:27:14 GMT
RUN set -xe 	&& buildDeps=" 		$PHP_EXTRA_BUILD_DEPS 		libcurl4-openssl-dev 		libedit-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	" 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	&& docker-php-source extract 	&& cd /usr/src/php 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)" 	&& if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi 	&& ./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--disable-cgi 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pcre-regex=/usr 		--with-libdir="lib/$debMultiarch" 				$PHP_EXTRA_CONFIGURE_ARGS 	&& make -j "$(nproc)" 	&& make install 	&& { find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; } 	&& make clean 	&& cd / 	&& docker-php-source delete 		&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $buildDeps 		&& pecl update-channels 	&& rm -rf /tmp/pear ~/.pearrc
# Fri, 03 Nov 2017 10:27:14 GMT
COPY multi:dbabcc0b81566a75f49e7faa9ca5f96cd22a515b80ee7ea1e34fceceee3f9c2a in /usr/local/bin/ 
# Fri, 03 Nov 2017 10:27:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Nov 2017 10:27:15 GMT
COPY file:24613ecbb1ce6a09f683b0753da9c26a1af07547326e8a02f6eec80ad6f2774a in /usr/local/bin/ 
# Fri, 03 Nov 2017 10:27:15 GMT
WORKDIR /var/www/html
# Fri, 03 Nov 2017 10:27:15 GMT
EXPOSE 80/tcp
# Fri, 03 Nov 2017 10:27:15 GMT
CMD ["apache2-foreground"]
# Fri, 03 Nov 2017 11:17:24 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y 		libjpeg-dev 		libpng-dev 	; 	rm -rf /var/lib/apt/lists/*; 		docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr; 	docker-php-ext-install gd mysqli opcache
# Fri, 03 Nov 2017 11:17:24 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 		echo 'opcache.enable_cli=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 03 Nov 2017 11:17:25 GMT
RUN a2enmod rewrite expires
# Fri, 03 Nov 2017 11:17:25 GMT
VOLUME [/var/www/html]
# Fri, 03 Nov 2017 11:17:26 GMT
ENV WORDPRESS_VERSION=4.8.3
# Fri, 03 Nov 2017 11:17:26 GMT
ENV WORDPRESS_SHA1=8efc0b9f6146e143ed419b5419d7bb8400a696fc
# Fri, 03 Nov 2017 11:17:27 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 03 Nov 2017 11:17:28 GMT
COPY file:db1f48c4963a4352b4c31c18f102b71fcc06a1266db6edd17f8f52458fe13130 in /usr/local/bin/ 
# Fri, 03 Nov 2017 11:17:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 11:17:28 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:e0f8ffe748163b60817bbe75e602fd998e062587f8802da580ccdb711e5d6b6e`  
		Last Modified: Mon, 09 Oct 2017 21:48:11 GMT  
		Size: 52.8 MB (52773848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671377a40e7b26497e7f12a7eac26f6af150ea739eebde2bbba9d79637b86551`  
		Last Modified: Tue, 10 Oct 2017 02:12:39 GMT  
		Size: 83.9 MB (83886879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f42450014c192b9a7782838f21339b652510d23b58558735a45cb0c723651b`  
		Last Modified: Tue, 10 Oct 2017 02:12:21 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a5c0800733c3b9785a87926d8034650a051c6a5a948cff91f66f1854bc4a1a`  
		Last Modified: Tue, 10 Oct 2017 02:13:37 GMT  
		Size: 3.1 MB (3118956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693c1c3f7bdaa4d80a14e4d22a1ee75c5fd791b9c6690f9579d6737e6b37f315`  
		Last Modified: Tue, 10 Oct 2017 02:13:36 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ff6ccd0fc5046c48d845d5b4107623c63a1b05af2d11c3d7971ddb9fcd9e26`  
		Last Modified: Tue, 10 Oct 2017 02:13:36 GMT  
		Size: 430.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9ef5b58b8f674d4c2db1d3da274fbf82e3b689a8fc0491cc05a216aa88e85d`  
		Last Modified: Tue, 10 Oct 2017 02:13:36 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f9c00c5ca9ae3f811cd5023870c28b20189436ac36328e950cfbe7c3a014b0`  
		Last Modified: Tue, 10 Oct 2017 02:13:36 GMT  
		Size: 486.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e74f92d037efb326805a55c6c57700be32ff99b4c2d4ceedaf0e9f4b7676b6`  
		Last Modified: Fri, 03 Nov 2017 10:58:03 GMT  
		Size: 12.8 MB (12818291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c8197f11f5287dd4634319b565d725cee7911b30af54b7112943a2fe55ed3b`  
		Last Modified: Fri, 03 Nov 2017 10:58:01 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ee9ef1010f892716438f40f3ca019d13d4d23743fd1223ca884f23b8546c36`  
		Last Modified: Fri, 03 Nov 2017 10:58:04 GMT  
		Size: 10.1 MB (10085789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050a7006a77b36ded44b3b6132be7cf32f69f9041db261f5b68685105c5bf0d8`  
		Last Modified: Fri, 03 Nov 2017 10:58:01 GMT  
		Size: 2.2 KB (2179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7f583fb2650f0429e055e968d63f764f9a6118fc86a1af16b888d51220b9b8`  
		Last Modified: Fri, 03 Nov 2017 10:58:02 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c934665c5c4fa6eeed8458f50041b1ce74b769a8ff41930e17f913d1def364`  
		Last Modified: Fri, 03 Nov 2017 11:45:29 GMT  
		Size: 2.3 MB (2303420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8240faad82ca6bf15ae99091ca0be5ae439b5db7b1e1ad93543dd03c59d56545`  
		Last Modified: Fri, 03 Nov 2017 11:45:28 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61614ce6ebb15b363e7712aace64c90d83e01bdce6aecbbf1bccc4470b3f80f4`  
		Last Modified: Fri, 03 Nov 2017 11:45:27 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5c7c74da17466b41eb2d725948349c074d18e46ee4c84c6e464a0458c622a5`  
		Last Modified: Fri, 03 Nov 2017 11:45:31 GMT  
		Size: 8.0 MB (8016464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb27c305e54c75b17e1e3a5ec37ed11f435281383ae630c1f2fb16eb650dc30`  
		Last Modified: Fri, 03 Nov 2017 11:45:27 GMT  
		Size: 3.2 KB (3221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:apache` - linux; ppc64le

```console
$ docker pull wordpress@sha256:e45d5018af1a958f7d2525341a18f706ab44bcbed95c98dc456323a784612836
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.5 MB (157522381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4ab458fee6385846fa51d68e19007398a0e41bca7255a31ae808a4b829947f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:51 GMT
ADD file:c62750f1e0dbf2b729abca09eb7927f2ee4fa8311dc40ae8066a53a4f1c85059 in / 
# Mon, 09 Oct 2017 21:42:53 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 04:59:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		libpcre3-dev 		make 		pkg-config 		re2c
# Tue, 10 Oct 2017 05:07:27 GMT
RUN apt-get update && apt-get install -y 		$PHPIZE_DEPS 		ca-certificates 		curl 		libedit2 		libsqlite3-0 		libxml2 		xz-utils 	--no-install-recommends && rm -r /var/lib/apt/lists/*
# Tue, 10 Oct 2017 05:07:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 10 Oct 2017 05:07:38 GMT
RUN mkdir -p $PHP_INI_DIR/conf.d
# Tue, 10 Oct 2017 05:15:32 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		apache2 	&& rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 05:15:35 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 10 Oct 2017 05:15:40 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 10 Oct 2017 05:15:47 GMT
RUN set -ex 		&& sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS" 		&& . "$APACHE_ENVVARS" 	&& for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 		/var/www/html 	; do 		rm -rvf "$dir" 		&& mkdir -p "$dir" 		&& chown -R "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 	done
# Tue, 10 Oct 2017 05:15:53 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 10 Oct 2017 05:15:59 GMT
RUN set -ex 	&& . "$APACHE_ENVVARS" 	&& ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log" 	&& ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log" 	&& ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"
# Tue, 10 Oct 2017 05:16:13 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 10 Oct 2017 05:16:15 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 10 Oct 2017 05:16:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2
# Tue, 10 Oct 2017 05:16:19 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Tue, 10 Oct 2017 05:16:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Tue, 10 Oct 2017 05:16:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Tue, 10 Oct 2017 06:15:04 GMT
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
# Tue, 31 Oct 2017 09:13:32 GMT
ENV PHP_VERSION=5.6.32
# Tue, 31 Oct 2017 09:13:33 GMT
ENV PHP_URL=https://secure.php.net/get/php-5.6.32.tar.xz/from/this/mirror PHP_ASC_URL=https://secure.php.net/get/php-5.6.32.tar.xz.asc/from/this/mirror
# Tue, 31 Oct 2017 09:13:35 GMT
ENV PHP_SHA256=8c2b4f721c7475fb9eabda2495209e91ea933082e6f34299d11cba88cd76e64b PHP_MD5=
# Fri, 03 Nov 2017 09:56:38 GMT
RUN set -xe; 		fetchDeps=' 		wget 	'; 	if ! command -v gpg > /dev/null; then 		fetchDeps="$fetchDeps 			dirmngr 			gnupg 		"; 	fi; 	apt-get update; 	apt-get install -y --no-install-recommends $fetchDeps; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		wget -O php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		wget -O php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps
# Fri, 03 Nov 2017 09:56:39 GMT
COPY file:207c686e3fed4f71f8a7b245d8dcae9c9048d276a326d82b553c12a90af0c0ca in /usr/local/bin/ 
# Fri, 03 Nov 2017 10:01:19 GMT
RUN set -xe 	&& buildDeps=" 		$PHP_EXTRA_BUILD_DEPS 		libcurl4-openssl-dev 		libedit-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	" 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	&& docker-php-source extract 	&& cd /usr/src/php 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)" 	&& if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi 	&& ./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--disable-cgi 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pcre-regex=/usr 		--with-libdir="lib/$debMultiarch" 				$PHP_EXTRA_CONFIGURE_ARGS 	&& make -j "$(nproc)" 	&& make install 	&& { find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; } 	&& make clean 	&& cd / 	&& docker-php-source delete 		&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $buildDeps 		&& pecl update-channels 	&& rm -rf /tmp/pear ~/.pearrc
# Fri, 03 Nov 2017 10:01:21 GMT
COPY multi:dbabcc0b81566a75f49e7faa9ca5f96cd22a515b80ee7ea1e34fceceee3f9c2a in /usr/local/bin/ 
# Fri, 03 Nov 2017 10:01:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Nov 2017 10:01:25 GMT
COPY file:24613ecbb1ce6a09f683b0753da9c26a1af07547326e8a02f6eec80ad6f2774a in /usr/local/bin/ 
# Fri, 03 Nov 2017 10:01:26 GMT
WORKDIR /var/www/html
# Fri, 03 Nov 2017 10:01:28 GMT
EXPOSE 80/tcp
# Fri, 03 Nov 2017 10:01:30 GMT
CMD ["apache2-foreground"]
# Fri, 03 Nov 2017 11:08:07 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y 		libjpeg-dev 		libpng-dev 	; 	rm -rf /var/lib/apt/lists/*; 		docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr; 	docker-php-ext-install gd mysqli opcache
# Fri, 03 Nov 2017 11:08:12 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 		echo 'opcache.enable_cli=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 03 Nov 2017 11:08:16 GMT
RUN a2enmod rewrite expires
# Fri, 03 Nov 2017 11:08:22 GMT
VOLUME [/var/www/html]
# Fri, 03 Nov 2017 11:08:24 GMT
ENV WORDPRESS_VERSION=4.8.3
# Fri, 03 Nov 2017 11:08:26 GMT
ENV WORDPRESS_SHA1=8efc0b9f6146e143ed419b5419d7bb8400a696fc
# Fri, 03 Nov 2017 11:08:34 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 03 Nov 2017 11:08:36 GMT
COPY file:db1f48c4963a4352b4c31c18f102b71fcc06a1266db6edd17f8f52458fe13130 in /usr/local/bin/ 
# Fri, 03 Nov 2017 11:08:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 11:08:40 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:0f531bde4b154605e2d6339e50b65d65d06568d747b8bef594269dd06602062f`  
		Last Modified: Mon, 09 Oct 2017 21:48:50 GMT  
		Size: 51.8 MB (51809739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc41d033d2921cba8c3fbd24aa09d8a180381ce21a996f56c5ba1b970a55b798`  
		Last Modified: Tue, 10 Oct 2017 06:45:18 GMT  
		Size: 70.0 MB (69979791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f923c00547c865a7523f58e49ceccbf4f04b88dc10b5cd3ee23729727731c2`  
		Last Modified: Tue, 10 Oct 2017 06:42:59 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc8808b95c3d4c76977c1f9665725fa3f91bcaef02d49caea930cf3f5a4156c`  
		Last Modified: Tue, 10 Oct 2017 06:46:09 GMT  
		Size: 2.9 MB (2908943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaffaa1bcc18483f24a5c0f3cb479470ce42a1117d8450ac961edfd9af260168`  
		Last Modified: Tue, 10 Oct 2017 06:46:06 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6796076a2938f2fb85232af9197067b3e1d07d0fb3e13904fc27df0f065873b`  
		Last Modified: Tue, 10 Oct 2017 06:46:04 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01602243d1dc9a2f49843681f0a849528e12248d5c70beceaa17f525d2d81a17`  
		Last Modified: Tue, 10 Oct 2017 06:46:04 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2c9272a190e9de8d0a48c07cdd5abe6ff1756f10961c7c1227a7d44eb44ab0`  
		Last Modified: Tue, 10 Oct 2017 06:46:03 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdfda5311146c8d6f4c7c42e2e6200ead403fcbb3cb56c434e34d5f1e32db6b`  
		Last Modified: Fri, 03 Nov 2017 10:25:40 GMT  
		Size: 12.8 MB (12817419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7168ca33ce9deb53b7947dfb2722aa0866abbd35ad09fda5f06a2c3f4215be25`  
		Last Modified: Fri, 03 Nov 2017 10:25:38 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a851a954c969a5a6c3f575b46d684f43b2ad5f1a13ff622899e525c88a05ab`  
		Last Modified: Fri, 03 Nov 2017 10:25:41 GMT  
		Size: 9.6 MB (9586529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da4e6f0c14ae574d1f5d8a9387fe6f997f62b931a4c365b912fdbe1ad17eccd`  
		Last Modified: Fri, 03 Nov 2017 10:25:38 GMT  
		Size: 2.2 KB (2181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:051bbdafbe7adbeac18c71904449e479f7c6d6ba373e94e53e0b3f5015172b85`  
		Last Modified: Fri, 03 Nov 2017 10:25:38 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116c2315887e85533c40454ef627230b6d52a6e8e40a92a4918339ffb7c4c578`  
		Last Modified: Fri, 03 Nov 2017 11:21:44 GMT  
		Size: 2.4 MB (2393244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8feb53e91708caf3451043b2a2c16ba41b426510c9fbef4b2f3186fca838a32c`  
		Last Modified: Fri, 03 Nov 2017 11:21:43 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1c22881f59655575c94b6fdeb6858ee2aa2749a0fd88c16bc297b38b292552`  
		Last Modified: Fri, 03 Nov 2017 11:21:44 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28014bbdb42e841e9b80281477bfd0b2a02d6f6de4a1facf93c5e6e8701e0962`  
		Last Modified: Fri, 03 Nov 2017 11:21:45 GMT  
		Size: 8.0 MB (8016486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc2c55be7dc5a6081a5d678dfca9ec4ce9dba656bb20681d91e05322a0f3c60`  
		Last Modified: Fri, 03 Nov 2017 11:21:44 GMT  
		Size: 3.2 KB (3222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:apache` - linux; s390x

```console
$ docker pull wordpress@sha256:e1b9f6cafc2bad64650ad6dbe6fb2a184b090564ceb5f89b8ec21f2b7cecd8ba
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.2 MB (153249951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb386c89f2c83d67a0de829019f9dc0cf378fa6be6d292a949f6243e55ff6bd3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:23 GMT
ADD file:1c306ad85a0adf89bf603a6f6a34a1059ddfa0811704a847df3e785c487ee58f in / 
# Mon, 09 Oct 2017 21:42:24 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:55:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		libpcre3-dev 		make 		pkg-config 		re2c
# Mon, 09 Oct 2017 22:55:37 GMT
RUN apt-get update && apt-get install -y 		$PHPIZE_DEPS 		ca-certificates 		curl 		libedit2 		libsqlite3-0 		libxml2 		xz-utils 	--no-install-recommends && rm -r /var/lib/apt/lists/*
# Mon, 09 Oct 2017 22:55:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 09 Oct 2017 22:55:39 GMT
RUN mkdir -p $PHP_INI_DIR/conf.d
# Mon, 09 Oct 2017 22:59:30 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		apache2 	&& rm -rf /var/lib/apt/lists/*
# Mon, 09 Oct 2017 22:59:31 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Mon, 09 Oct 2017 22:59:31 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Mon, 09 Oct 2017 22:59:31 GMT
RUN set -ex 		&& sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS" 		&& . "$APACHE_ENVVARS" 	&& for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 		/var/www/html 	; do 		rm -rvf "$dir" 		&& mkdir -p "$dir" 		&& chown -R "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 	done
# Mon, 09 Oct 2017 22:59:32 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Mon, 09 Oct 2017 22:59:33 GMT
RUN set -ex 	&& . "$APACHE_ENVVARS" 	&& ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log" 	&& ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log" 	&& ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"
# Mon, 09 Oct 2017 22:59:33 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Mon, 09 Oct 2017 22:59:33 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Mon, 09 Oct 2017 22:59:34 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2
# Mon, 09 Oct 2017 22:59:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Mon, 09 Oct 2017 22:59:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Mon, 09 Oct 2017 22:59:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Mon, 09 Oct 2017 23:26:32 GMT
ENV GPG_KEYS=0BD78B5F97500D450838F95DFE857D9A90D90EC1 6E4F6AB321FDC07F2C332E3AC2BF0BC433CFC8B3
# Tue, 31 Oct 2017 17:42:46 GMT
ENV PHP_VERSION=5.6.32
# Tue, 31 Oct 2017 17:42:46 GMT
ENV PHP_URL=https://secure.php.net/get/php-5.6.32.tar.xz/from/this/mirror PHP_ASC_URL=https://secure.php.net/get/php-5.6.32.tar.xz.asc/from/this/mirror
# Tue, 31 Oct 2017 17:42:46 GMT
ENV PHP_SHA256=8c2b4f721c7475fb9eabda2495209e91ea933082e6f34299d11cba88cd76e64b PHP_MD5=
# Thu, 02 Nov 2017 23:46:11 GMT
RUN set -xe; 		fetchDeps=' 		wget 	'; 	if ! command -v gpg > /dev/null; then 		fetchDeps="$fetchDeps 			dirmngr 			gnupg 		"; 	fi; 	apt-get update; 	apt-get install -y --no-install-recommends $fetchDeps; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		wget -O php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		wget -O php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps
# Thu, 02 Nov 2017 23:46:11 GMT
COPY file:207c686e3fed4f71f8a7b245d8dcae9c9048d276a326d82b553c12a90af0c0ca in /usr/local/bin/ 
# Thu, 02 Nov 2017 23:49:10 GMT
RUN set -xe 	&& buildDeps=" 		$PHP_EXTRA_BUILD_DEPS 		libcurl4-openssl-dev 		libedit-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	" 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	&& docker-php-source extract 	&& cd /usr/src/php 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)" 	&& if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi 	&& ./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--disable-cgi 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pcre-regex=/usr 		--with-libdir="lib/$debMultiarch" 				$PHP_EXTRA_CONFIGURE_ARGS 	&& make -j "$(nproc)" 	&& make install 	&& { find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; } 	&& make clean 	&& cd / 	&& docker-php-source delete 		&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $buildDeps 		&& pecl update-channels 	&& rm -rf /tmp/pear ~/.pearrc
# Thu, 02 Nov 2017 23:49:11 GMT
COPY multi:dbabcc0b81566a75f49e7faa9ca5f96cd22a515b80ee7ea1e34fceceee3f9c2a in /usr/local/bin/ 
# Thu, 02 Nov 2017 23:49:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 02 Nov 2017 23:49:11 GMT
COPY file:24613ecbb1ce6a09f683b0753da9c26a1af07547326e8a02f6eec80ad6f2774a in /usr/local/bin/ 
# Thu, 02 Nov 2017 23:49:11 GMT
WORKDIR /var/www/html
# Thu, 02 Nov 2017 23:49:12 GMT
EXPOSE 80/tcp
# Thu, 02 Nov 2017 23:49:12 GMT
CMD ["apache2-foreground"]
# Fri, 03 Nov 2017 00:53:47 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y 		libjpeg-dev 		libpng-dev 	; 	rm -rf /var/lib/apt/lists/*; 		docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr; 	docker-php-ext-install gd mysqli opcache
# Fri, 03 Nov 2017 00:53:48 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 		echo 'opcache.enable_cli=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 03 Nov 2017 00:53:49 GMT
RUN a2enmod rewrite expires
# Fri, 03 Nov 2017 00:53:49 GMT
VOLUME [/var/www/html]
# Fri, 03 Nov 2017 00:53:49 GMT
ENV WORDPRESS_VERSION=4.8.3
# Fri, 03 Nov 2017 00:53:50 GMT
ENV WORDPRESS_SHA1=8efc0b9f6146e143ed419b5419d7bb8400a696fc
# Fri, 03 Nov 2017 00:53:52 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 03 Nov 2017 00:53:53 GMT
COPY file:db1f48c4963a4352b4c31c18f102b71fcc06a1266db6edd17f8f52458fe13130 in /usr/local/bin/ 
# Fri, 03 Nov 2017 00:53:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 00:53:53 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:a0a92d62c165393786de44f21509e9a71868aa7c2765f0334d285aa2aa19a58f`  
		Last Modified: Mon, 09 Oct 2017 21:46:27 GMT  
		Size: 52.8 MB (52788868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fb66856860b5de241911f00d4159df363cf63a303d18ae7437e405aa3162e7`  
		Last Modified: Mon, 09 Oct 2017 23:36:47 GMT  
		Size: 64.0 MB (63980038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38a4e89ae8f8496f476f2092ceb43def00c3fc728237b0f3ced18375fcc3431`  
		Last Modified: Mon, 09 Oct 2017 23:36:16 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa08f5a322d716bc344e329f44d60ef75a976fd0ea5e530d59e527eeb8ecf40`  
		Last Modified: Mon, 09 Oct 2017 23:37:17 GMT  
		Size: 3.0 MB (3022574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf2af7622cabd637a262403d1aa90e8652eaf888035388a5660f2ef299f527e`  
		Last Modified: Mon, 09 Oct 2017 23:37:16 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dacb3b3a74e99a7a6559d4fe5b12de5023afcdc29fceda3e8efd5fd290a836a`  
		Last Modified: Mon, 09 Oct 2017 23:37:15 GMT  
		Size: 431.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b49a00cab668863e82ada97435faf0487a821fbddf62dfda16d67241390f3ba`  
		Last Modified: Mon, 09 Oct 2017 23:37:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0226e5908d56361a72c804c781675ed4f60c645aadda58418219637e6872196b`  
		Last Modified: Mon, 09 Oct 2017 23:37:15 GMT  
		Size: 486.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4747f0be820a2249f352303624752b069c1a6edfb514fb965dcf0a440c5602`  
		Last Modified: Fri, 03 Nov 2017 00:14:51 GMT  
		Size: 12.8 MB (12816115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa0c91ea082467d4591d5bb38b03dde3608e2ce83230695c1c137386e2aabfb`  
		Last Modified: Fri, 03 Nov 2017 00:14:49 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecabe806d92c61e5ab36ea2245ea3f947b36eefa4ab06dc18c032658b2871c41`  
		Last Modified: Fri, 03 Nov 2017 00:14:53 GMT  
		Size: 10.0 MB (9952948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d55f6a2617ff775e13cae3e199f04b4ae085c80cfcf5e710ba51552550f794c`  
		Last Modified: Fri, 03 Nov 2017 00:14:49 GMT  
		Size: 2.2 KB (2180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e6cfaadf87c92a53fc277c591f91664901d75437f7b2028a5da68272813583`  
		Last Modified: Fri, 03 Nov 2017 00:14:49 GMT  
		Size: 902.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9356af4b28f35915fbac34be9bb5f293c1393de34ce36ad105eba3bf030374`  
		Last Modified: Fri, 03 Nov 2017 00:59:45 GMT  
		Size: 2.7 MB (2662872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61aa2870c8c3f65f5b0ca150a9c296b06ea66776a3f2437cd01c9cdafbb0c40`  
		Last Modified: Fri, 03 Nov 2017 00:59:45 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6cf289ae6c8ce782492715014267f9dce4535ff9103b8a5806a933461f4ed7`  
		Last Modified: Fri, 03 Nov 2017 00:59:45 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031fa522e570377df8f82b447a093de3007db0b13d8fd0312143e3535005000e`  
		Last Modified: Fri, 03 Nov 2017 00:59:47 GMT  
		Size: 8.0 MB (8016452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6efd2441a4a0e155a26af81ac2eff93aa1e6078197ac361ab390ff5f6ed8e11`  
		Last Modified: Fri, 03 Nov 2017 00:59:45 GMT  
		Size: 3.2 KB (3223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
