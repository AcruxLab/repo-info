<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:0.10.2`](#vault0102)
-	[`vault:latest`](#vaultlatest)

## `vault:0.10.2`

```console
$ docker pull vault@sha256:8314763be1368d2a3cca78888fdab02611027ba2edc9c0ecb99e110bd17cd650
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `vault:0.10.2` - linux; amd64

```console
$ docker pull vault@sha256:61f267f6dad8f94adb9a26605064b747673a4d3a72e8019641ac22d6683f8eaa
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.5 MB (24450883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e7759573ec8758972fa1c47c5c5fb57265a2e9cd7a624a0008244e2755f57fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Jan 2018 21:10:58 GMT
ADD file:093f0723fa46f6cdbd6f7bd146448bb70ecce54254c35701feeceb956414622f in / 
# Tue, 09 Jan 2018 21:10:58 GMT
CMD ["/bin/sh"]
# Thu, 07 Jun 2018 20:20:20 GMT
ENV VAULT_VERSION=0.10.2
# Thu, 07 Jun 2018 20:20:21 GMT
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 07 Jun 2018 20:20:35 GMT
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 07 Jun 2018 20:20:36 GMT
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 07 Jun 2018 20:20:36 GMT
VOLUME [/vault/logs]
# Thu, 07 Jun 2018 20:20:36 GMT
VOLUME [/vault/file]
# Thu, 07 Jun 2018 20:20:36 GMT
EXPOSE 8200/tcp
# Thu, 07 Jun 2018 20:20:36 GMT
COPY file:71f93573d5097ef42f7373b359230a67d5c04db40151c9f350d7d9c881341c67 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 07 Jun 2018 20:20:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Jun 2018 20:20:37 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:ff3a5c916c92643ff77519ffa742d3ec61b7f591b6b7504599d95a4a41134e28`  
		Last Modified: Tue, 09 Jan 2018 21:13:34 GMT  
		Size: 2.1 MB (2065537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb099864735c0ad478d8999dcc5d4b4a4e42edb69cc7421aa4cdf8fa8c7ccc90`  
		Last Modified: Thu, 07 Jun 2018 20:20:53 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6034c8b3202b7c221fffca1ce481a9c5ec60dd6a8c4be1113feb612ec4f2b47`  
		Last Modified: Thu, 07 Jun 2018 20:21:16 GMT  
		Size: 22.4 MB (22382144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45024412d2ef75a0c6c37e3b703075e64dc7f4b202da7477070ef9a7ea0013e7`  
		Last Modified: Thu, 07 Jun 2018 20:20:53 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426e4022c303dd8975658d575b611e071fa6552927710ab9a67c61a92f59141f`  
		Last Modified: Thu, 07 Jun 2018 20:20:53 GMT  
		Size: 1.8 KB (1794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:a2c8e82730e3d9703b3b76f31dd199253c56eea20fca12fcadb56037b5f33459
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:ba77730553ab0754305430a4f8f2d4ebbac5d0324577148160667c1bd54c76c2
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.1 MB (24135183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fe535ace00bc56ec2881b22fb29c4eb930476cceed0309ba84af6b749551963`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 09 Jan 2018 21:10:58 GMT
ADD file:093f0723fa46f6cdbd6f7bd146448bb70ecce54254c35701feeceb956414622f in / 
# Tue, 09 Jan 2018 21:10:58 GMT
CMD ["/bin/sh"]
# Fri, 27 Apr 2018 22:36:08 GMT
ENV VAULT_VERSION=0.10.1
# Fri, 27 Apr 2018 22:36:09 GMT
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 27 Apr 2018 22:36:19 GMT
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     gpg --keyserver hkp://pgp.mit.edu:80 --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 27 Apr 2018 22:36:20 GMT
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 27 Apr 2018 22:36:20 GMT
VOLUME [/vault/logs]
# Fri, 27 Apr 2018 22:36:20 GMT
VOLUME [/vault/file]
# Fri, 27 Apr 2018 22:36:21 GMT
EXPOSE 8200/tcp
# Fri, 27 Apr 2018 22:36:21 GMT
COPY file:71f93573d5097ef42f7373b359230a67d5c04db40151c9f350d7d9c881341c67 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 Apr 2018 22:36:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Apr 2018 22:36:22 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:ff3a5c916c92643ff77519ffa742d3ec61b7f591b6b7504599d95a4a41134e28`  
		Last Modified: Tue, 09 Jan 2018 21:13:34 GMT  
		Size: 2.1 MB (2065537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f9eface7fdbf13552f927bc90086e58ac2820069dcaccc9734a97e6985b36e`  
		Last Modified: Fri, 27 Apr 2018 22:39:45 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d800ad572feed4ac882ac10c1b4c79342a166d8ef6e3c2b66aadf6eeef9a7a`  
		Last Modified: Fri, 27 Apr 2018 22:39:49 GMT  
		Size: 22.1 MB (22066448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5889c13b9e5d8ec3d68357f4707ff7a78427ea571d7906f98e88f4d81f6ebce4`  
		Last Modified: Fri, 27 Apr 2018 22:39:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d24724ef698c1f39f13687d9dbe939c1e3c29a4023b6e490720bc3eeb7ea738`  
		Last Modified: Fri, 27 Apr 2018 22:39:46 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:2d94a025d4e6eeab42f37680a86e2c6b706ca35ddbc772dab493530dfb7739b3
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23447269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d46d38dec957152a13d02706b5f2271e3d2bd00b724ea62e00dce2d2e8bc05b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 01 Dec 2017 18:41:45 GMT
ADD file:966d84204dc4860e9281f7c93c792137c88298edb284f267def4b38a11b79a1f in / 
# Fri, 01 Dec 2017 18:41:45 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Fri, 01 Dec 2017 18:41:46 GMT
CMD ["/bin/sh"]
# Sat, 28 Apr 2018 07:49:23 GMT
ENV VAULT_VERSION=0.10.1
# Sat, 28 Apr 2018 07:49:28 GMT
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 28 Apr 2018 07:50:08 GMT
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     gpg --keyserver hkp://pgp.mit.edu:80 --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 28 Apr 2018 07:50:14 GMT
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 28 Apr 2018 07:50:14 GMT
VOLUME [/vault/logs]
# Sat, 28 Apr 2018 07:50:15 GMT
VOLUME [/vault/file]
# Sat, 28 Apr 2018 07:50:16 GMT
EXPOSE 8200/tcp
# Sat, 28 Apr 2018 07:50:17 GMT
COPY file:71f93573d5097ef42f7373b359230a67d5c04db40151c9f350d7d9c881341c67 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 28 Apr 2018 07:50:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Apr 2018 07:50:19 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:95d54dd4bdadebb53f9b91b25aa7dc5fcb83c534eb1d196eb0814aa1e16f3db2`  
		Last Modified: Fri, 01 Dec 2017 18:41:57 GMT  
		Size: 2.0 MB (2038298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bf7d76c39215a547858ef9260990b9b80c0e679bb2f6ceef942d7b6d0eeec3`  
		Last Modified: Fri, 01 Dec 2017 18:41:57 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d02d4e0da813e6a399d07d236c8c7610df7429a387ce76633608152c9512831`  
		Last Modified: Sat, 28 Apr 2018 07:50:29 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651cbc1c5e9d716dccd06f23cf5fa7bf1653d9b96ec4cfb3baf5a7b2b2ba9ffc`  
		Last Modified: Sat, 28 Apr 2018 07:50:56 GMT  
		Size: 21.4 MB (21405531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab25de9c5a1c2156a61224914a002d1a06806514437ee88f17a64cb5c2d8d20c`  
		Last Modified: Sat, 28 Apr 2018 07:50:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f9e3c31dd33052a9cc907d9d6207d9bf77d6f9187f233502cd2d64e7f4409e`  
		Last Modified: Sat, 28 Apr 2018 07:50:29 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:21e97023231e2c7d72ca82385e4ad24e1f3587bb1272de34c651a61bfdc62459
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.0 MB (22996614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b3a8647050cb60445aead2164a13249e58cd7ac46b73d7e2dc4b86be1266e4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 01 Dec 2017 18:42:42 GMT
ADD file:a6ef3cbbb1c0e5dfc6c3e41d70fd93e548594d9cb42c067e52df46d418c10a79 in / 
# Fri, 01 Dec 2017 18:42:42 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Fri, 01 Dec 2017 18:42:43 GMT
CMD ["/bin/sh"]
# Tue, 01 May 2018 03:25:23 GMT
ENV VAULT_VERSION=0.10.1
# Tue, 01 May 2018 03:25:27 GMT
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 01 May 2018 03:25:51 GMT
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     gpg --keyserver hkp://pgp.mit.edu:80 --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 01 May 2018 03:25:56 GMT
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 01 May 2018 03:25:58 GMT
VOLUME [/vault/logs]
# Tue, 01 May 2018 03:26:01 GMT
VOLUME [/vault/file]
# Tue, 01 May 2018 03:26:04 GMT
EXPOSE 8200/tcp
# Tue, 01 May 2018 03:26:07 GMT
COPY file:71f93573d5097ef42f7373b359230a67d5c04db40151c9f350d7d9c881341c67 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 01 May 2018 03:26:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 May 2018 03:26:13 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b78042c299ad99d1e646b18762d4bc22a84c4f88e5bb491ea6293a10f53ddf79`  
		Last Modified: Fri, 01 Dec 2017 18:43:42 GMT  
		Size: 2.0 MB (1988857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd45b97b6c2a3ac869ae5c99e087e97bc29714b165180e06f0c9116f400f2dd`  
		Last Modified: Fri, 01 Dec 2017 18:43:41 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21208efa6e1141e8e6fb015c3162423bc14cf8366108812469944646814a2d7`  
		Last Modified: Tue, 01 May 2018 03:26:36 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178037be4aebb19d9add50f935def85b95e68ca455f90a28459f92e48e0951bd`  
		Last Modified: Tue, 01 May 2018 03:26:45 GMT  
		Size: 21.0 MB (21004382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3772d7d74d37b7d7998bd11d1c98c7c23595e7a296af10878845d8d8150e583`  
		Last Modified: Tue, 01 May 2018 03:26:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25858b0519a711e091923b21797f059f44deccc122841757009b67f16004e1de`  
		Last Modified: Tue, 01 May 2018 03:26:36 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:90f3cd472451973b37687d3cc120c47bfab5ffb2b599f20201c7e49d2fdf5624
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23816970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f805b5d733aaa84b57e26af4676ea3a004bb52d973639031736c8bf9fe14916d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 01 Jun 2018 06:57:26 GMT
ADD file:614c07101e677db9a4118a71c852a2be45a337d94c5bedfb48ae8c4cad21d625 in / 
# Fri, 01 Jun 2018 06:57:26 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Fri, 01 Jun 2018 06:57:26 GMT
CMD ["/bin/sh"]
# Fri, 01 Jun 2018 09:20:39 GMT
ENV VAULT_VERSION=0.10.1
# Fri, 01 Jun 2018 09:20:39 GMT
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 01 Jun 2018 09:20:52 GMT
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     gpg --keyserver hkp://pgp.mit.edu:80 --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 01 Jun 2018 09:20:52 GMT
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 01 Jun 2018 09:20:53 GMT
VOLUME [/vault/logs]
# Fri, 01 Jun 2018 09:20:53 GMT
VOLUME [/vault/file]
# Fri, 01 Jun 2018 09:20:53 GMT
EXPOSE 8200/tcp
# Fri, 01 Jun 2018 09:20:53 GMT
COPY file:71f93573d5097ef42f7373b359230a67d5c04db40151c9f350d7d9c881341c67 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 01 Jun 2018 09:20:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Jun 2018 09:20:54 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:381c1d4107a4401d75b916e6dc4331efddc01adac41f49eeaa711ab898606a1a`  
		Last Modified: Fri, 01 Dec 2017 18:47:24 GMT  
		Size: 2.1 MB (2126217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061a9db3c9e4f3bc32618a5f1a7e2b8aefb20fcc48f8be709bc7f7eabe61d003`  
		Last Modified: Fri, 01 Jun 2018 06:57:51 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566e002235ea6763f22dd0841b602109e15ef6f8e6f936f74434705086368171`  
		Last Modified: Fri, 01 Jun 2018 09:21:05 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc7648759f43f44d05a2a66bb13dc86737b93ab7d4f3bf3ab3d1e70dff4e5a9`  
		Last Modified: Fri, 01 Jun 2018 09:21:16 GMT  
		Size: 21.7 MB (21687377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2170e1e93165b8679ff4c789fb165e9e79ff6fab2da21b1fd1a75e8f72bee3ca`  
		Last Modified: Fri, 01 Jun 2018 09:21:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee7732b1d78c17bf01ebc35c20fbb2893ab48e5b8c55bb5dac5f80b9eb75f4f`  
		Last Modified: Fri, 01 Jun 2018 09:21:07 GMT  
		Size: 1.8 KB (1793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
