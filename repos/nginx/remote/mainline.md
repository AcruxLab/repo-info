## `nginx:mainline`

```console
$ docker pull nginx@sha256:3e2ffcf0edca2a4e9b24ca442d227baea7b7f0e33ad654ef1eb806fbd9bedcf0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `nginx:mainline` - linux; amd64

```console
$ docker pull nginx@sha256:1f9c00b4c95ef931afa097823d902e7602aebc3ec5532e907e066978075ca3e0
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44619165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd5239a0906a6ccf0562354852fae04bc5b52d72a2aff9a871ddb6bd57553569`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Sat, 28 Apr 2018 07:09:59 GMT
ADD file:ec5be7eec56a749752ca284359ece04f5eb0b981eac08b8855454c6b16e3893c in / 
# Sat, 28 Apr 2018 07:09:59 GMT
CMD ["bash"]
# Mon, 30 Apr 2018 13:55:06 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 05 Jun 2018 18:19:49 GMT
ENV NGINX_VERSION=1.15.0-1~stretch
# Tue, 05 Jun 2018 18:19:49 GMT
ENV NJS_VERSION=1.15.0.0.2.1-1~stretch
# Tue, 05 Jun 2018 18:20:13 GMT
RUN set -x 	&& apt-get update 	&& apt-get install --no-install-recommends --no-install-suggests -y gnupg1 apt-transport-https ca-certificates 	&& 	NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62; 	found=''; 	for server in 		ha.pool.sks-keyservers.net 		hkp://keyserver.ubuntu.com:80 		hkp://p80.pool.sks-keyservers.net:80 		pgp.mit.edu 	; do 		echo "Fetching GPG key $NGINX_GPGKEY from $server"; 		apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break; 	done; 	test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1; 	apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/* 	&& dpkgArch="$(dpkg --print-architecture)" 	&& nginxPackages=" 		nginx=${NGINX_VERSION} 		nginx-module-xslt=${NGINX_VERSION} 		nginx-module-geoip=${NGINX_VERSION} 		nginx-module-image-filter=${NGINX_VERSION} 		nginx-module-njs=${NJS_VERSION} 	" 	&& case "$dpkgArch" in 		amd64|i386) 			echo "deb https://nginx.org/packages/mainline/debian/ stretch nginx" >> /etc/apt/sources.list.d/nginx.list 			&& apt-get update 			;; 		*) 			echo "deb-src https://nginx.org/packages/mainline/debian/ stretch nginx" >> /etc/apt/sources.list.d/nginx.list 						&& tempDir="$(mktemp -d)" 			&& chmod 777 "$tempDir" 						&& savedAptMark="$(apt-mark showmanual)" 						&& apt-get update 			&& apt-get build-dep -y $nginxPackages 			&& ( 				cd "$tempDir" 				&& DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 					apt-get source --compile $nginxPackages 			) 						&& apt-mark showmanual | xargs apt-mark auto > /dev/null 			&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 						&& ls -lAFh "$tempDir" 			&& ( cd "$tempDir" && dpkg-scanpackages . > Packages ) 			&& grep '^Package: ' "$tempDir/Packages" 			&& echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list 			&& apt-get -o Acquire::GzipIndexes=false update 			;; 	esac 		&& apt-get install --no-install-recommends --no-install-suggests -y 						$nginxPackages 						gettext-base 	&& apt-get remove --purge --auto-remove -y apt-transport-https ca-certificates && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list 		&& if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove 		&& rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Tue, 05 Jun 2018 18:20:13 GMT
RUN ln -sf /dev/stdout /var/log/nginx/access.log 	&& ln -sf /dev/stderr /var/log/nginx/error.log
# Tue, 05 Jun 2018 18:20:14 GMT
EXPOSE 80/tcp
# Tue, 05 Jun 2018 18:20:14 GMT
STOPSIGNAL [SIGTERM]
# Tue, 05 Jun 2018 18:20:14 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:f2aa67a397c49232112953088506d02074a1fe577f65dc2052f158a3e5da52e8`  
		Last Modified: Sat, 28 Apr 2018 09:31:20 GMT  
		Size: 22.5 MB (22496029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd0975d4f456a5ab3196ae351a2a9d72077ee24da60b42004eb0c3e8d153aad`  
		Last Modified: Tue, 05 Jun 2018 20:05:17 GMT  
		Size: 22.1 MB (22122931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fd2d3be09a6d5bb4eee2e6c66e6929f9f9c71853dd250035a9bdb37fccce89`  
		Last Modified: Tue, 05 Jun 2018 20:05:12 GMT  
		Size: 205.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:mainline` - linux; arm variant v7

```console
$ docker pull nginx@sha256:eaeef53e922820316ff10f92ffdb586a6f1b6dea635dd95e4075b80062bf03c7
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (40048547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eecf376dc1a4164f3df4b9fc5ee9c1897068a8050abf993af0afd53953c1c94`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Sat, 28 Apr 2018 12:04:59 GMT
ADD file:f8bb9e9954bfe2f550e8a786c4be1dd5fca4a373b82b372b80c163e5640bd5a4 in / 
# Sat, 28 Apr 2018 12:05:00 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 13:32:21 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 06 Jun 2018 12:01:51 GMT
ENV NGINX_VERSION=1.15.0-1~stretch
# Wed, 06 Jun 2018 12:01:52 GMT
ENV NJS_VERSION=1.15.0.0.2.1-1~stretch
# Wed, 06 Jun 2018 12:06:06 GMT
RUN set -x 	&& apt-get update 	&& apt-get install --no-install-recommends --no-install-suggests -y gnupg1 apt-transport-https ca-certificates 	&& 	NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62; 	found=''; 	for server in 		ha.pool.sks-keyservers.net 		hkp://keyserver.ubuntu.com:80 		hkp://p80.pool.sks-keyservers.net:80 		pgp.mit.edu 	; do 		echo "Fetching GPG key $NGINX_GPGKEY from $server"; 		apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break; 	done; 	test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1; 	apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/* 	&& dpkgArch="$(dpkg --print-architecture)" 	&& nginxPackages=" 		nginx=${NGINX_VERSION} 		nginx-module-xslt=${NGINX_VERSION} 		nginx-module-geoip=${NGINX_VERSION} 		nginx-module-image-filter=${NGINX_VERSION} 		nginx-module-njs=${NJS_VERSION} 	" 	&& case "$dpkgArch" in 		amd64|i386) 			echo "deb https://nginx.org/packages/mainline/debian/ stretch nginx" >> /etc/apt/sources.list.d/nginx.list 			&& apt-get update 			;; 		*) 			echo "deb-src https://nginx.org/packages/mainline/debian/ stretch nginx" >> /etc/apt/sources.list.d/nginx.list 						&& tempDir="$(mktemp -d)" 			&& chmod 777 "$tempDir" 						&& savedAptMark="$(apt-mark showmanual)" 						&& apt-get update 			&& apt-get build-dep -y $nginxPackages 			&& ( 				cd "$tempDir" 				&& DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 					apt-get source --compile $nginxPackages 			) 						&& apt-mark showmanual | xargs apt-mark auto > /dev/null 			&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 						&& ls -lAFh "$tempDir" 			&& ( cd "$tempDir" && dpkg-scanpackages . > Packages ) 			&& grep '^Package: ' "$tempDir/Packages" 			&& echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list 			&& apt-get -o Acquire::GzipIndexes=false update 			;; 	esac 		&& apt-get install --no-install-recommends --no-install-suggests -y 						$nginxPackages 						gettext-base 	&& apt-get remove --purge --auto-remove -y apt-transport-https ca-certificates && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list 		&& if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove 		&& rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Wed, 06 Jun 2018 12:06:09 GMT
RUN ln -sf /dev/stdout /var/log/nginx/access.log 	&& ln -sf /dev/stderr /var/log/nginx/error.log
# Wed, 06 Jun 2018 12:06:09 GMT
EXPOSE 80/tcp
# Wed, 06 Jun 2018 12:06:09 GMT
STOPSIGNAL [SIGTERM]
# Wed, 06 Jun 2018 12:06:10 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:6c8a025e90b325dd5af06b0297cc1608120a47d4ab0e1cedb26c8cda811091d6`  
		Last Modified: Sat, 28 Apr 2018 12:16:08 GMT  
		Size: 19.3 MB (19286790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:082753991fa04f6b8d9b4213971f1bff60c58e0220da0fe193a68006167975cd`  
		Last Modified: Wed, 06 Jun 2018 12:11:53 GMT  
		Size: 20.8 MB (20761552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c382b469cbc9c58443f9d929556104f7a350eb31c8fa47bbdd2a8dd641b73400`  
		Last Modified: Wed, 06 Jun 2018 12:11:45 GMT  
		Size: 205.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:mainline` - linux; arm64 variant v8

```console
$ docker pull nginx@sha256:1b834ada36b03fae2d14bd72fe562a8c71a5503920b1519f89447e88670fbd48
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41821149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e0f046b6d6ef0c7c073277582d9aebc41ef6ca1b6da11edf293c3619b44124f`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Mon, 30 Apr 2018 23:33:18 GMT
ADD file:d423aa6d423df239af0602fe8134c14cb277778de23c8553d629d3b4b510f38b in / 
# Mon, 30 Apr 2018 23:33:20 GMT
CMD ["bash"]
# Tue, 01 May 2018 11:30:03 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 06 Jun 2018 08:39:51 GMT
ENV NGINX_VERSION=1.15.0-1~stretch
# Wed, 06 Jun 2018 08:39:52 GMT
ENV NJS_VERSION=1.15.0.0.2.1-1~stretch
# Wed, 06 Jun 2018 08:53:20 GMT
RUN set -x 	&& apt-get update 	&& apt-get install --no-install-recommends --no-install-suggests -y gnupg1 apt-transport-https ca-certificates 	&& 	NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62; 	found=''; 	for server in 		ha.pool.sks-keyservers.net 		hkp://keyserver.ubuntu.com:80 		hkp://p80.pool.sks-keyservers.net:80 		pgp.mit.edu 	; do 		echo "Fetching GPG key $NGINX_GPGKEY from $server"; 		apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break; 	done; 	test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1; 	apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/* 	&& dpkgArch="$(dpkg --print-architecture)" 	&& nginxPackages=" 		nginx=${NGINX_VERSION} 		nginx-module-xslt=${NGINX_VERSION} 		nginx-module-geoip=${NGINX_VERSION} 		nginx-module-image-filter=${NGINX_VERSION} 		nginx-module-njs=${NJS_VERSION} 	" 	&& case "$dpkgArch" in 		amd64|i386) 			echo "deb https://nginx.org/packages/mainline/debian/ stretch nginx" >> /etc/apt/sources.list.d/nginx.list 			&& apt-get update 			;; 		*) 			echo "deb-src https://nginx.org/packages/mainline/debian/ stretch nginx" >> /etc/apt/sources.list.d/nginx.list 						&& tempDir="$(mktemp -d)" 			&& chmod 777 "$tempDir" 						&& savedAptMark="$(apt-mark showmanual)" 						&& apt-get update 			&& apt-get build-dep -y $nginxPackages 			&& ( 				cd "$tempDir" 				&& DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 					apt-get source --compile $nginxPackages 			) 						&& apt-mark showmanual | xargs apt-mark auto > /dev/null 			&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 						&& ls -lAFh "$tempDir" 			&& ( cd "$tempDir" && dpkg-scanpackages . > Packages ) 			&& grep '^Package: ' "$tempDir/Packages" 			&& echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list 			&& apt-get -o Acquire::GzipIndexes=false update 			;; 	esac 		&& apt-get install --no-install-recommends --no-install-suggests -y 						$nginxPackages 						gettext-base 	&& apt-get remove --purge --auto-remove -y apt-transport-https ca-certificates && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list 		&& if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove 		&& rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Wed, 06 Jun 2018 08:53:22 GMT
RUN ln -sf /dev/stdout /var/log/nginx/access.log 	&& ln -sf /dev/stderr /var/log/nginx/error.log
# Wed, 06 Jun 2018 08:53:23 GMT
EXPOSE 80/tcp
# Wed, 06 Jun 2018 08:53:24 GMT
STOPSIGNAL [SIGTERM]
# Wed, 06 Jun 2018 08:53:26 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:18d6337cc9064ce5276eac2eb6da6c5fe3f204bc7f1392f5ad1ba468817c609e`  
		Last Modified: Mon, 30 Apr 2018 23:54:34 GMT  
		Size: 20.3 MB (20347907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f088c9a038b990b6c6739842a87ff5d4fc018f8618a5e827441ee0fef78d103a`  
		Last Modified: Wed, 06 Jun 2018 09:16:06 GMT  
		Size: 21.5 MB (21473037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac889d85841e7d43110c72775fa91881809fcd675b248160ec5e9276151aaacd`  
		Last Modified: Wed, 06 Jun 2018 09:16:00 GMT  
		Size: 205.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:mainline` - linux; 386

```console
$ docker pull nginx@sha256:a1eb298e6a54a02c9428ae23c4d3493c3b0dbfeb1842488ca819e1e1e624412f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45794624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bb138a88aef2cc6360f1107e1fad2d31e8d4d6ee918a2591c42755cdf2bbe06`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Sat, 28 Apr 2018 10:41:49 GMT
ADD file:9e45c98885c63b1f77e50324055758088ca38203260e2305cca24b13fbeb23cf in / 
# Sat, 28 Apr 2018 10:41:49 GMT
CMD ["bash"]
# Fri, 01 Jun 2018 09:48:29 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 06 Jun 2018 10:38:38 GMT
ENV NGINX_VERSION=1.15.0-1~stretch
# Wed, 06 Jun 2018 10:38:38 GMT
ENV NJS_VERSION=1.15.0.0.2.1-1~stretch
# Wed, 06 Jun 2018 10:39:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install --no-install-recommends --no-install-suggests -y gnupg1 apt-transport-https ca-certificates 	&& 	NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62; 	found=''; 	for server in 		ha.pool.sks-keyservers.net 		hkp://keyserver.ubuntu.com:80 		hkp://p80.pool.sks-keyservers.net:80 		pgp.mit.edu 	; do 		echo "Fetching GPG key $NGINX_GPGKEY from $server"; 		apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break; 	done; 	test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1; 	apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/* 	&& dpkgArch="$(dpkg --print-architecture)" 	&& nginxPackages=" 		nginx=${NGINX_VERSION} 		nginx-module-xslt=${NGINX_VERSION} 		nginx-module-geoip=${NGINX_VERSION} 		nginx-module-image-filter=${NGINX_VERSION} 		nginx-module-njs=${NJS_VERSION} 	" 	&& case "$dpkgArch" in 		amd64|i386) 			echo "deb https://nginx.org/packages/mainline/debian/ stretch nginx" >> /etc/apt/sources.list.d/nginx.list 			&& apt-get update 			;; 		*) 			echo "deb-src https://nginx.org/packages/mainline/debian/ stretch nginx" >> /etc/apt/sources.list.d/nginx.list 						&& tempDir="$(mktemp -d)" 			&& chmod 777 "$tempDir" 						&& savedAptMark="$(apt-mark showmanual)" 						&& apt-get update 			&& apt-get build-dep -y $nginxPackages 			&& ( 				cd "$tempDir" 				&& DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 					apt-get source --compile $nginxPackages 			) 						&& apt-mark showmanual | xargs apt-mark auto > /dev/null 			&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 						&& ls -lAFh "$tempDir" 			&& ( cd "$tempDir" && dpkg-scanpackages . > Packages ) 			&& grep '^Package: ' "$tempDir/Packages" 			&& echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list 			&& apt-get -o Acquire::GzipIndexes=false update 			;; 	esac 		&& apt-get install --no-install-recommends --no-install-suggests -y 						$nginxPackages 						gettext-base 	&& apt-get remove --purge --auto-remove -y apt-transport-https ca-certificates && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list 		&& if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove 		&& rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Wed, 06 Jun 2018 10:39:32 GMT
RUN ln -sf /dev/stdout /var/log/nginx/access.log 	&& ln -sf /dev/stderr /var/log/nginx/error.log
# Wed, 06 Jun 2018 10:39:32 GMT
EXPOSE 80/tcp
# Wed, 06 Jun 2018 10:39:32 GMT
STOPSIGNAL [SIGTERM]
# Wed, 06 Jun 2018 10:39:32 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:23510c5166fc980d20c6b002b2a7bbdde547dfc6195bbfcb7e0f2a39c590a210`  
		Last Modified: Sat, 28 Apr 2018 10:49:34 GMT  
		Size: 23.1 MB (23138515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5757f94b4544406080d71513280ff2be14d507bac6c7dd2482810939a38f885`  
		Last Modified: Wed, 06 Jun 2018 10:43:04 GMT  
		Size: 22.7 MB (22655904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f86eaa2d0f5f610a0cd5123cc50017fdaef84cc98ea4c5053593ce5b7a1a31c`  
		Last Modified: Wed, 06 Jun 2018 10:42:58 GMT  
		Size: 205.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:mainline` - linux; ppc64le

```console
$ docker pull nginx@sha256:35298308ca68e9b154ea6326080fcdae99935c0fbfc66811393542561e33293d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44798647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4839153708813bd6075c1f57538291397864f20756fa13baa0afbea3d516430a`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Sat, 28 Apr 2018 08:20:54 GMT
ADD file:c561a92d41ab01d60c88efa7b21fd9b48e6c0c96fb8d2552f4cebbed3df42bca in / 
# Sat, 28 Apr 2018 08:20:55 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 12:21:11 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 06 Jun 2018 08:16:48 GMT
ENV NGINX_VERSION=1.15.0-1~stretch
# Wed, 06 Jun 2018 08:16:51 GMT
ENV NJS_VERSION=1.15.0.0.2.1-1~stretch
# Wed, 06 Jun 2018 08:28:35 GMT
RUN set -x 	&& apt-get update 	&& apt-get install --no-install-recommends --no-install-suggests -y gnupg1 apt-transport-https ca-certificates 	&& 	NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62; 	found=''; 	for server in 		ha.pool.sks-keyservers.net 		hkp://keyserver.ubuntu.com:80 		hkp://p80.pool.sks-keyservers.net:80 		pgp.mit.edu 	; do 		echo "Fetching GPG key $NGINX_GPGKEY from $server"; 		apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break; 	done; 	test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1; 	apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/* 	&& dpkgArch="$(dpkg --print-architecture)" 	&& nginxPackages=" 		nginx=${NGINX_VERSION} 		nginx-module-xslt=${NGINX_VERSION} 		nginx-module-geoip=${NGINX_VERSION} 		nginx-module-image-filter=${NGINX_VERSION} 		nginx-module-njs=${NJS_VERSION} 	" 	&& case "$dpkgArch" in 		amd64|i386) 			echo "deb https://nginx.org/packages/mainline/debian/ stretch nginx" >> /etc/apt/sources.list.d/nginx.list 			&& apt-get update 			;; 		*) 			echo "deb-src https://nginx.org/packages/mainline/debian/ stretch nginx" >> /etc/apt/sources.list.d/nginx.list 						&& tempDir="$(mktemp -d)" 			&& chmod 777 "$tempDir" 						&& savedAptMark="$(apt-mark showmanual)" 						&& apt-get update 			&& apt-get build-dep -y $nginxPackages 			&& ( 				cd "$tempDir" 				&& DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 					apt-get source --compile $nginxPackages 			) 						&& apt-mark showmanual | xargs apt-mark auto > /dev/null 			&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 						&& ls -lAFh "$tempDir" 			&& ( cd "$tempDir" && dpkg-scanpackages . > Packages ) 			&& grep '^Package: ' "$tempDir/Packages" 			&& echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list 			&& apt-get -o Acquire::GzipIndexes=false update 			;; 	esac 		&& apt-get install --no-install-recommends --no-install-suggests -y 						$nginxPackages 						gettext-base 	&& apt-get remove --purge --auto-remove -y apt-transport-https ca-certificates && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list 		&& if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove 		&& rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Wed, 06 Jun 2018 08:28:43 GMT
RUN ln -sf /dev/stdout /var/log/nginx/access.log 	&& ln -sf /dev/stderr /var/log/nginx/error.log
# Wed, 06 Jun 2018 08:28:44 GMT
EXPOSE 80/tcp
# Wed, 06 Jun 2018 08:28:46 GMT
STOPSIGNAL [SIGTERM]
# Wed, 06 Jun 2018 08:28:48 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:39214b2a7dd7dd2d1069dd155ce8ab2206bb1fda22be8136b88451c8be20e82f`  
		Last Modified: Sat, 28 Apr 2018 08:30:28 GMT  
		Size: 22.8 MB (22753096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378eabc2a358f1a314a32e0a80b8dcc0a5ec7a1d69d9de9928dd0d4d0309028f`  
		Last Modified: Wed, 06 Jun 2018 08:52:53 GMT  
		Size: 22.0 MB (22045346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574feb67240fc359d4104fa46dfb53cb5c083cdb23052abb3d54440813f6f264`  
		Last Modified: Wed, 06 Jun 2018 08:52:47 GMT  
		Size: 205.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:mainline` - linux; s390x

```console
$ docker pull nginx@sha256:cdfad99b46875c1e4c6df98725e0b789fbc72f83279950120bd528c456e9923f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44545467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c430762fb87c1251bf5fc888f769ca2c758707eb60d5998d3bae0ff2102492f4`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Sat, 28 Apr 2018 11:45:29 GMT
ADD file:89223bc6886b09479a52e6d05479980ad8e46c8c707ac40cd81b664fe9827428 in / 
# Sat, 28 Apr 2018 11:45:29 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 15:01:25 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 06 Jun 2018 11:41:36 GMT
ENV NGINX_VERSION=1.15.0-1~stretch
# Wed, 06 Jun 2018 11:41:36 GMT
ENV NJS_VERSION=1.15.0.0.2.1-1~stretch
# Wed, 06 Jun 2018 11:45:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install --no-install-recommends --no-install-suggests -y gnupg1 apt-transport-https ca-certificates 	&& 	NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62; 	found=''; 	for server in 		ha.pool.sks-keyservers.net 		hkp://keyserver.ubuntu.com:80 		hkp://p80.pool.sks-keyservers.net:80 		pgp.mit.edu 	; do 		echo "Fetching GPG key $NGINX_GPGKEY from $server"; 		apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break; 	done; 	test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1; 	apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/* 	&& dpkgArch="$(dpkg --print-architecture)" 	&& nginxPackages=" 		nginx=${NGINX_VERSION} 		nginx-module-xslt=${NGINX_VERSION} 		nginx-module-geoip=${NGINX_VERSION} 		nginx-module-image-filter=${NGINX_VERSION} 		nginx-module-njs=${NJS_VERSION} 	" 	&& case "$dpkgArch" in 		amd64|i386) 			echo "deb https://nginx.org/packages/mainline/debian/ stretch nginx" >> /etc/apt/sources.list.d/nginx.list 			&& apt-get update 			;; 		*) 			echo "deb-src https://nginx.org/packages/mainline/debian/ stretch nginx" >> /etc/apt/sources.list.d/nginx.list 						&& tempDir="$(mktemp -d)" 			&& chmod 777 "$tempDir" 						&& savedAptMark="$(apt-mark showmanual)" 						&& apt-get update 			&& apt-get build-dep -y $nginxPackages 			&& ( 				cd "$tempDir" 				&& DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 					apt-get source --compile $nginxPackages 			) 						&& apt-mark showmanual | xargs apt-mark auto > /dev/null 			&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 						&& ls -lAFh "$tempDir" 			&& ( cd "$tempDir" && dpkg-scanpackages . > Packages ) 			&& grep '^Package: ' "$tempDir/Packages" 			&& echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list 			&& apt-get -o Acquire::GzipIndexes=false update 			;; 	esac 		&& apt-get install --no-install-recommends --no-install-suggests -y 						$nginxPackages 						gettext-base 	&& apt-get remove --purge --auto-remove -y apt-transport-https ca-certificates && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list 		&& if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove 		&& rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi
# Wed, 06 Jun 2018 11:45:25 GMT
RUN ln -sf /dev/stdout /var/log/nginx/access.log 	&& ln -sf /dev/stderr /var/log/nginx/error.log
# Wed, 06 Jun 2018 11:45:25 GMT
EXPOSE 80/tcp
# Wed, 06 Jun 2018 11:45:26 GMT
STOPSIGNAL [SIGTERM]
# Wed, 06 Jun 2018 11:45:26 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:39cbaa616b05fb96ca4be9aac8b4d99ba8bf573e07a754a8c43dbec7ff518bbb`  
		Last Modified: Sat, 28 Apr 2018 11:51:43 GMT  
		Size: 22.3 MB (22349898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3317396fd66cb3f16a918496ce62a399642c526b031adce9dd8579c59273c5d`  
		Last Modified: Wed, 06 Jun 2018 11:51:43 GMT  
		Size: 22.2 MB (22195365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59fdd745b29e84b77e899172fae22db662a5aa297b97086f3e168f67c4ea8efc`  
		Last Modified: Wed, 06 Jun 2018 11:51:39 GMT  
		Size: 204.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
