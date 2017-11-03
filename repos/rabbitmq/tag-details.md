<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rabbitmq`

-	[`rabbitmq:3`](#rabbitmq3)
-	[`rabbitmq:3.6`](#rabbitmq36)
-	[`rabbitmq:3.6.12`](#rabbitmq3612)
-	[`rabbitmq:3.6.12-alpine`](#rabbitmq3612-alpine)
-	[`rabbitmq:3.6.12-management`](#rabbitmq3612-management)
-	[`rabbitmq:3.6.12-management-alpine`](#rabbitmq3612-management-alpine)
-	[`rabbitmq:3.6-alpine`](#rabbitmq36-alpine)
-	[`rabbitmq:3.6-management`](#rabbitmq36-management)
-	[`rabbitmq:3.6-management-alpine`](#rabbitmq36-management-alpine)
-	[`rabbitmq:3-alpine`](#rabbitmq3-alpine)
-	[`rabbitmq:3-management`](#rabbitmq3-management)
-	[`rabbitmq:3-management-alpine`](#rabbitmq3-management-alpine)
-	[`rabbitmq:alpine`](#rabbitmqalpine)
-	[`rabbitmq:latest`](#rabbitmqlatest)
-	[`rabbitmq:management`](#rabbitmqmanagement)
-	[`rabbitmq:management-alpine`](#rabbitmqmanagement-alpine)

## `rabbitmq:3`

```console
$ docker pull rabbitmq@sha256:2c3145ed1766d6eac4f224c990d02a2c2411e8b1dc02875a28b7cf8acc9fa985
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

### `rabbitmq:3` - linux; amd64

```console
$ docker pull rabbitmq@sha256:b99e238fa99bcd7ffcfd89a536fdf33bbd27e206cea118246874e3792ebfc2bc
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.9 MB (62852177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e186865bff877f181c4a4b4ffdb7235e91c0c988bdc0c926d1b68e5d8c81e45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:33:42 GMT
ADD file:45233d6b5c9b91e9437065d3e7c332d1c4eb4bce8e1079a4c1af342c450abe67 in / 
# Mon, 09 Oct 2017 21:33:43 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 02:41:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:41:43 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 02:41:43 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 02:42:10 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 02:42:40 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 02:42:41 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 02:42:42 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 02:43:16 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:43:16 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 02:43:17 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 02:43:17 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 02:43:18 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 02:43:19 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 13 Oct 2017 23:40:43 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 13 Oct 2017 23:40:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 13 Oct 2017 23:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2017 23:40:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 13 Oct 2017 23:40:45 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:bc95e04b23c06ba1b9bf092d07d1493177b218e0340bd2ed49dac351c1e34313`  
		Last Modified: Mon, 09 Oct 2017 21:42:28 GMT  
		Size: 22.5 MB (22492350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65f0b00e4cfb1535d0f4e7a63707172ae63483fb33140d777614f199afcb36`  
		Last Modified: Tue, 10 Oct 2017 02:43:59 GMT  
		Size: 4.5 MB (4498726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bd803179890909fcae186044c0e6ca1bc1d34e5fc05ef1ccea823e7be97540`  
		Last Modified: Tue, 10 Oct 2017 02:43:57 GMT  
		Size: 4.1 KB (4069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b05ca8302833edf783c50f03cd7ba0b8e12bc872b053eda3e3ae7e1f17e2b4b`  
		Last Modified: Tue, 10 Oct 2017 02:43:58 GMT  
		Size: 952.1 KB (952058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb5a4bbcce5a040eb83057f9e93d17663bb123f4e98168457444497f7d17b70`  
		Last Modified: Tue, 10 Oct 2017 02:44:03 GMT  
		Size: 27.7 MB (27703883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf840d8999f6fe46a162974c82378c38b3cf3dcccbbaff848c0fb199988aebe0`  
		Last Modified: Tue, 10 Oct 2017 02:44:00 GMT  
		Size: 7.2 MB (7194403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be339ca44883b1990e52771487402163d398a279755a501fdd8891ec71cf09d0`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce35cd9f9b5b917868095b3b074dd23d18e0e266f3ee68ff95e2c61467299812`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fe32a0a00d916ed4d632aae71d35d9d0baa5e5910d6bd179a24071c35bedb0`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77408ca9e94eb4bfeb346ab10c602857525802c2279e7c6995fcdbc90269444a`  
		Last Modified: Fri, 13 Oct 2017 23:41:26 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db03407a1aba1c0a89dffe960394aae639885702e3faa65271b918c36c7905cd`  
		Last Modified: Fri, 13 Oct 2017 23:41:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3` - linux; arm variant v5

```console
$ docker pull rabbitmq@sha256:53c2349355bbba2f2b1eeb11d5ed481cab005bba90148c0ed0c1aa44d33bcaff
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58432369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1107bbf7e8a883f25f4975b43d490503a84921e26ccb943e929596f9b418cf40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:44:48 GMT
ADD file:ff9945b48b1ac236dcec24eb9dfaf52b7c151a3b11c8502391f0866dfb4e3ac3 in / 
# Mon, 09 Oct 2017 21:44:48 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 00:18:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:18:11 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 00:18:11 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 00:18:29 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 00:18:58 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:18:58 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 00:18:58 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 00:19:26 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:19:26 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 00:19:27 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 00:19:28 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 00:19:29 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 00:19:30 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Sat, 14 Oct 2017 14:14:24 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Sat, 14 Oct 2017 14:14:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 14 Oct 2017 14:14:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 Oct 2017 14:14:25 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Sat, 14 Oct 2017 14:14:26 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:836d5b6056a9815be79c76480a90299267f60201bd1e3396817003e6c14819cc`  
		Last Modified: Mon, 09 Oct 2017 21:50:56 GMT  
		Size: 21.2 MB (21166251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb896fba83bd09a35c68457554b35289860c23c46f27a8c3ef42f13146ebba1`  
		Last Modified: Tue, 10 Oct 2017 00:20:01 GMT  
		Size: 4.2 MB (4231979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61827a16c114b9741d761aa4c60a972ffe1e0b60147794e86b05653d67822e91`  
		Last Modified: Tue, 10 Oct 2017 00:20:00 GMT  
		Size: 4.1 KB (4079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877cd9511def30e56a5ce354e145e8a2b1a93daaae7eaaa42dc4219838aa1743`  
		Last Modified: Tue, 10 Oct 2017 00:20:00 GMT  
		Size: 942.8 KB (942752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea9e378899e98c99e93ae2d0874bd5d89e24134bd14a19c285bdf39a0a42ade`  
		Last Modified: Tue, 10 Oct 2017 00:20:05 GMT  
		Size: 25.2 MB (25170810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc82a29314b16531aa2172ac523ba535e3678f85efdd699164fbb0241ab8b62`  
		Last Modified: Tue, 10 Oct 2017 00:20:01 GMT  
		Size: 6.9 MB (6909811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c44a3d016cf9de95021782180a42d3660e20fc7d8e92a7fe5ce9ede7928ca2`  
		Last Modified: Tue, 10 Oct 2017 00:19:59 GMT  
		Size: 2.3 KB (2261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abfdcdd98b40291ad91791bea09bf277e75c3669c6607c7891b09130101bfa3`  
		Last Modified: Tue, 10 Oct 2017 00:19:58 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a72811da4bf8ca8a2d06cdc182aa54116bb12133e8d82ef2b018a8de29ed74`  
		Last Modified: Tue, 10 Oct 2017 00:19:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147d8cf0897dea9b024bf5c6efb6873db3d86dec857fca062b146f88b7b5a735`  
		Last Modified: Sat, 14 Oct 2017 14:14:43 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f355fd0b70caedf30aa384298307b8e40d922e9e341492dd3fde71f119fd7d7`  
		Last Modified: Sat, 14 Oct 2017 14:14:44 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:c5a07be740a1d956343d5881d8827cb9e3d6dcceda2d8ce954cf187ab9be9abc
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55688150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c4235a850985eab3d39e30563f87f78348a6425ec30388363f9d372c082855e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:43 GMT
ADD file:b758c6c3ff989778bd740dde35c86b953fa09be913a7e02711b2881de6b8911d in / 
# Mon, 09 Oct 2017 21:45:44 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 13:07:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:07:42 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 13:07:42 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 13:07:58 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 13:08:17 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:08:17 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 13:08:17 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 13:08:39 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:08:39 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 13:08:40 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 13:08:41 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 13:08:42 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 13:08:43 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 13:08:43 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 13:08:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 13:08:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 13:08:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 13:08:45 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:59e81a3fde58ec8d4b8f2f58b98ef2f4d951d37dd9b99b016fd294a8e07d7796`  
		Last Modified: Mon, 09 Oct 2017 21:52:49 GMT  
		Size: 19.3 MB (19277135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2037b99f3c3dc51e8ace39aed9971155f34f325ac4f0a1e56a07c4d6c02f5ae6`  
		Last Modified: Fri, 03 Nov 2017 13:09:18 GMT  
		Size: 3.9 MB (3868347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f368172ea96bda944832762ad29b52dfe17ec5e6fae96eee37adc4e9d68674a5`  
		Last Modified: Fri, 03 Nov 2017 13:09:16 GMT  
		Size: 4.1 KB (4084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893cc1ae60f8bf72ac3020ccc60b22d9e0ad0cb0647e15bc4847d08c8985eee2`  
		Last Modified: Fri, 03 Nov 2017 13:09:16 GMT  
		Size: 926.1 KB (926097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13220cc1a683014bda9cfae7f7ee7015a26b28048f90f5aa3ed8b6a96f4b2813`  
		Last Modified: Fri, 03 Nov 2017 13:09:20 GMT  
		Size: 24.8 MB (24785610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269f4e069126132643c1c0be1faf600d55ff15e870066c527d03181904d99c5d`  
		Last Modified: Fri, 03 Nov 2017 13:09:17 GMT  
		Size: 6.8 MB (6820180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ae244f4f610a339fcbddf37612a15ec7b7f6674e3d888c3c4d36302283418e`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce7d85327b7bc7d59a7b54222a3e6babd7f8afd8eb080becb77fc52aed5a751`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dfa32e4b49700ed0130ebd563f40a2c381393983b571a9886435813102ad0c`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba15cd885dc21f438d366b40d0d9f595f2c25e063c60fa590ab4c0f6233ff94`  
		Last Modified: Fri, 03 Nov 2017 13:09:14 GMT  
		Size: 4.0 KB (4040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978a8434497fcb8e08cefc7484b515ac34fe23c281fb869d015f62b54673028c`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:3d9b2aee2786ff5328bb6b1195f2938e251fdfe7c183ffac1ead7ffe6f234d03
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57278372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa9e28302480b775a117eda9fd3d2e8897ee8a4ed19ceac66f0afaab1e5f8609`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:47:55 GMT
ADD file:3a528355cfc75437716aff3b517ef99ae602918d84d26dbafff0ed142248fb93 in / 
# Mon, 09 Oct 2017 21:47:56 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 04:57:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 04:57:04 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 04:57:05 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 04:57:37 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 04:58:35 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 04:58:36 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 04:58:37 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 04:58:37 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 04:58:38 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 04:58:39 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 04:58:39 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 05:00:22 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 05:00:23 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 05:00:25 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 05:00:26 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 05:00:28 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 05:00:31 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Sat, 14 Oct 2017 13:52:47 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Sat, 14 Oct 2017 13:52:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 14 Oct 2017 13:52:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 Oct 2017 13:52:51 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Sat, 14 Oct 2017 13:52:51 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:e907afd6e25615a4d3eb554d930cef57b87e79ec82413889c2eac38beb4eb8f7`  
		Last Modified: Mon, 09 Oct 2017 22:03:08 GMT  
		Size: 20.3 MB (20337143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5e6d35928560b933b85b5a3f2a8e96b4520fbb8df138b3e739e56d0c1f355`  
		Last Modified: Tue, 10 Oct 2017 05:01:18 GMT  
		Size: 4.1 MB (4073554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a862ab821b342790326492507ca5d70bfb7016bef765606193f1f7139f60c5ed`  
		Last Modified: Tue, 10 Oct 2017 05:01:14 GMT  
		Size: 4.1 KB (4072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92799a54920b79013733790e444f13d8c65faa29c79cbdaf1bc8af85f637a233`  
		Last Modified: Tue, 10 Oct 2017 05:01:14 GMT  
		Size: 919.5 KB (919487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b119999eef1bcadabedd3a5319b03c6b83ede91ba8535059851547d3433b205`  
		Last Modified: Tue, 10 Oct 2017 05:01:19 GMT  
		Size: 25.0 MB (25042572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62f8525a3a982a102aa37bb3313876195b15d8781cd253ed238dd2b9dff151`  
		Last Modified: Tue, 10 Oct 2017 05:01:15 GMT  
		Size: 6.9 MB (6894852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc028e70f04f6ea4365223a1cfe4e5c4384d5921acac419f3c170b148f7c7bf`  
		Last Modified: Tue, 10 Oct 2017 05:01:10 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e99faa03c2a8a272f56208c644c12b384b69dea50be6da9f6be400c14b945c`  
		Last Modified: Tue, 10 Oct 2017 05:01:12 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8fa260bcaa52d81ba20c11111f8d15bab954b17b48666724536c604220d94e`  
		Last Modified: Tue, 10 Oct 2017 05:01:11 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306840de948d03472918a306c089409429606802ec8cf841e96dec707a2f7178`  
		Last Modified: Sat, 14 Oct 2017 13:53:27 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a7a978032478b38adb1f0107466d187e53380f7037d058c62e4937cd07fc09`  
		Last Modified: Sat, 14 Oct 2017 13:53:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3` - linux; 386

```console
$ docker pull rabbitmq@sha256:900c25b037b878974bb75f9d056b5278794f96586c9d03f619af9905a6cf5229
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63902262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a993d7c3c104c0e9f2ed42d750b907890291a9a2693d23f166744b9fb8e9265d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:36 GMT
ADD file:6582536277127947668f7bfdc1471a4e36170915b91a4cb841e7e1bfa1de6535 in / 
# Mon, 09 Oct 2017 21:45:36 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 10:45:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:45:12 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 10:45:13 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 10:45:28 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 10:46:03 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 10:46:04 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 10:46:25 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:46:25 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 10:46:26 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 10:46:27 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 10:46:27 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 10:46:28 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 10:46:28 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 10:46:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 10:46:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 10:46:30 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 10:46:30 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:b2b52fe46b29fe5d0689f26449c2114e40f0731d4ce3eb8c3941397b74205432`  
		Last Modified: Mon, 09 Oct 2017 21:53:42 GMT  
		Size: 23.1 MB (23128678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d407b136da0731f5f38279001e9dd426217937443cad0f16e1f242366290773`  
		Last Modified: Fri, 03 Nov 2017 10:47:13 GMT  
		Size: 4.8 MB (4803637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c93817e78345b4b5070c81e5a37d02afc2b5fe347a1a4bf59e09f6084814fd2`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 4.1 KB (4057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97eae59c75f8f814ab781f5239ac2e132b7b65c77e75b35023c603c539ca54f`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 931.5 KB (931524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aed670dee19fde6946658d7129e13520c1a0747f8b80b6f92dac5f6d974ae52`  
		Last Modified: Fri, 03 Nov 2017 10:47:24 GMT  
		Size: 27.8 MB (27818690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b61d6d0b60ec18280aeba946a05d62817afbe030f277af85b5f434021e90c9`  
		Last Modified: Fri, 03 Nov 2017 10:47:16 GMT  
		Size: 7.2 MB (7208985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec7d4cc3b5497bbbd6b2d1e9574dbedb6c7ad11805cff4c287ea444ddc2e298`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 2.3 KB (2259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eec554591344f78e35e3976d002d617623a52d123fc71e65d33c4d533d2b2e7`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e433f73af1167eff0dee1984c095bf5be36593fcead5b8cc820e2cb829aaed0`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8d6e0dbdbb04b44f7a0972fce6b0b1b19262e4fc5416bd1589af560f16c99f`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 4.0 KB (4040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bab08cf9b00d8109139e1cb1cdec448b71fdae7d7f1260d4175771416a5f80`  
		Last Modified: Fri, 03 Nov 2017 10:47:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:63dcce5fe70ba7b07c27b3af47248ad1f0609ca79e98e01a2ea0cb4e5357cc55
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60384479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:929ca14b97313f42a819bb7e089422aea0fa6d6a7428046a573c11937059499d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:56 GMT
ADD file:7edf73437495be24244c16841b563be06c15452963f41ac940fb5e105ed96027 in / 
# Mon, 09 Oct 2017 21:45:58 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 07:12:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:12:51 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 07:12:53 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 07:13:49 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 07:15:26 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:15:28 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 07:15:29 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 07:15:31 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 07:15:33 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 07:15:34 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 07:15:35 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 07:16:54 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:16:55 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 07:17:00 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 07:17:01 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 07:17:06 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 07:17:11 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 07:17:13 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 07:17:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 07:17:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 07:17:21 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 07:17:23 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:c4860466fa1e6824151f4fa3a51ef0e9d7d3c3ba860e21d94e69988b65601260`  
		Last Modified: Mon, 09 Oct 2017 21:52:59 GMT  
		Size: 22.7 MB (22746217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebe4c87dcd1f7ef11d4d21752831bf4095ac42afe041706c35f1d7d4d0ca4f2`  
		Last Modified: Fri, 03 Nov 2017 07:18:05 GMT  
		Size: 4.4 MB (4360529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e5365525084de1c85fa29ef33d37c38b5f80621f5bcb26bb4882d71598c6f7`  
		Last Modified: Fri, 03 Nov 2017 07:18:03 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600c3853740b7f4cff9cc799ae478f669bd54277a8dd375479a34ed1bb47a803`  
		Last Modified: Fri, 03 Nov 2017 07:18:02 GMT  
		Size: 920.7 KB (920695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993868ec534130e348e45aa6d64b471fa46eafbf061836cc9d2a56edf73e9382`  
		Last Modified: Fri, 03 Nov 2017 07:18:06 GMT  
		Size: 25.5 MB (25492533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca1b92e212aaef163244d5fdd9e135fdb8be8c9dbbb626061ee2882d941a553`  
		Last Modified: Fri, 03 Nov 2017 07:18:03 GMT  
		Size: 6.9 MB (6853702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483f96d1f500f9f69170bc6927d599a7f0cd1550f96b6ee3f90eb4185a1bffb`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b433db63f40c7cab3080cf36bd7beabbdf7d9eece3f2dc16a65b900c61180`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93971551a2c911c34ca2e9af47495efb2f27e2922e567d93dd94dfb9b773bd3`  
		Last Modified: Fri, 03 Nov 2017 07:17:58 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5494bb8bcc45452a84c216edffedb3103a15c3e209aba0561dfbc70e4312192e`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 4.0 KB (4039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d56b2a4f9f8d7b11831a8f1952fe2c02613bcb014ab9d756b70b3b398b37269`  
		Last Modified: Fri, 03 Nov 2017 07:17:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3` - linux; s390x

```console
$ docker pull rabbitmq@sha256:c5e29e37ac52898d26c2d63c4e0506afbaf0fa3862456c04c425429dae26248a
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60364776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9b9f437096f93b98ba60e922a7e6c52ff1e8a75593833f81fa03b4a035a3f50`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:44:35 GMT
ADD file:ae4aaa6affe22f36ab5478771d5c84917f72de7a8dac16345a035709a1a5edf4 in / 
# Mon, 09 Oct 2017 21:44:36 GMT
CMD ["bash"]
# Thu, 02 Nov 2017 17:06:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 17:06:41 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Thu, 02 Nov 2017 17:06:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 02 Nov 2017 17:07:21 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Thu, 02 Nov 2017 17:07:43 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 02 Nov 2017 17:07:44 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 02 Nov 2017 17:07:45 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 17:07:48 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 17:07:48 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 17:07:49 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 17:07:50 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 17:07:52 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 17:07:53 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 17:07:54 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 17:07:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 17:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 17:07:57 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 17:07:57 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:671716cc49517eef5f430c695ce344d63e390cb65f58d30939f2ba615c953686`  
		Last Modified: Mon, 09 Oct 2017 21:49:09 GMT  
		Size: 22.3 MB (22339951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cae61f12be6f01ba06573d9393712e91821cd5496302310f550fe5842dea557`  
		Last Modified: Fri, 03 Nov 2017 17:08:41 GMT  
		Size: 4.5 MB (4529879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca307103ce923e7e89d35185be4df8e54c3c0b54d259b8880aa7bae107d4952`  
		Last Modified: Fri, 03 Nov 2017 17:08:39 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d16320f9fc35ea20ba7fb9b21f88e3f0f06c52d416682319f3b2a85a345a3d5`  
		Last Modified: Fri, 03 Nov 2017 17:08:39 GMT  
		Size: 938.0 KB (938019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801205b182b8d6f7acf36200b2ba07ed52ea224dfefe792b525224e4aacb4d4a`  
		Last Modified: Fri, 03 Nov 2017 17:08:48 GMT  
		Size: 25.6 MB (25619372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9cb605e6242f5ab505cbd229c7b2fdf2935a6254130070c12c4d8413616024`  
		Last Modified: Fri, 03 Nov 2017 17:08:40 GMT  
		Size: 6.9 MB (6926791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2799e1b1479136fbb3c3ba6df318d449990a3cf5fc3293a14142cde0d9f51980`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a6d5de3e6aaa1c06122a1b5cda3b4bcb98d54e5dc23f38896fc81e98cea769`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172fa2e52818dcedf69c727f6790f0f9744f8538da3f4222602aaa0ab9fa82c0`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c734f2707800c1189521a51409fed1508fb7e36c6e67eca5537d03c4b24ef0d`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 4.0 KB (4037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e7d712f1155d66243480cd441ec04e084a8e7e2d6a0653e27138b31b56d2ae`  
		Last Modified: Fri, 03 Nov 2017 17:08:38 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rabbitmq:3.6`

```console
$ docker pull rabbitmq@sha256:2c3145ed1766d6eac4f224c990d02a2c2411e8b1dc02875a28b7cf8acc9fa985
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

### `rabbitmq:3.6` - linux; amd64

```console
$ docker pull rabbitmq@sha256:b99e238fa99bcd7ffcfd89a536fdf33bbd27e206cea118246874e3792ebfc2bc
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.9 MB (62852177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e186865bff877f181c4a4b4ffdb7235e91c0c988bdc0c926d1b68e5d8c81e45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:33:42 GMT
ADD file:45233d6b5c9b91e9437065d3e7c332d1c4eb4bce8e1079a4c1af342c450abe67 in / 
# Mon, 09 Oct 2017 21:33:43 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 02:41:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:41:43 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 02:41:43 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 02:42:10 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 02:42:40 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 02:42:41 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 02:42:42 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 02:43:16 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:43:16 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 02:43:17 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 02:43:17 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 02:43:18 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 02:43:19 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 13 Oct 2017 23:40:43 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 13 Oct 2017 23:40:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 13 Oct 2017 23:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2017 23:40:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 13 Oct 2017 23:40:45 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:bc95e04b23c06ba1b9bf092d07d1493177b218e0340bd2ed49dac351c1e34313`  
		Last Modified: Mon, 09 Oct 2017 21:42:28 GMT  
		Size: 22.5 MB (22492350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65f0b00e4cfb1535d0f4e7a63707172ae63483fb33140d777614f199afcb36`  
		Last Modified: Tue, 10 Oct 2017 02:43:59 GMT  
		Size: 4.5 MB (4498726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bd803179890909fcae186044c0e6ca1bc1d34e5fc05ef1ccea823e7be97540`  
		Last Modified: Tue, 10 Oct 2017 02:43:57 GMT  
		Size: 4.1 KB (4069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b05ca8302833edf783c50f03cd7ba0b8e12bc872b053eda3e3ae7e1f17e2b4b`  
		Last Modified: Tue, 10 Oct 2017 02:43:58 GMT  
		Size: 952.1 KB (952058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb5a4bbcce5a040eb83057f9e93d17663bb123f4e98168457444497f7d17b70`  
		Last Modified: Tue, 10 Oct 2017 02:44:03 GMT  
		Size: 27.7 MB (27703883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf840d8999f6fe46a162974c82378c38b3cf3dcccbbaff848c0fb199988aebe0`  
		Last Modified: Tue, 10 Oct 2017 02:44:00 GMT  
		Size: 7.2 MB (7194403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be339ca44883b1990e52771487402163d398a279755a501fdd8891ec71cf09d0`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce35cd9f9b5b917868095b3b074dd23d18e0e266f3ee68ff95e2c61467299812`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fe32a0a00d916ed4d632aae71d35d9d0baa5e5910d6bd179a24071c35bedb0`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77408ca9e94eb4bfeb346ab10c602857525802c2279e7c6995fcdbc90269444a`  
		Last Modified: Fri, 13 Oct 2017 23:41:26 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db03407a1aba1c0a89dffe960394aae639885702e3faa65271b918c36c7905cd`  
		Last Modified: Fri, 13 Oct 2017 23:41:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6` - linux; arm variant v5

```console
$ docker pull rabbitmq@sha256:53c2349355bbba2f2b1eeb11d5ed481cab005bba90148c0ed0c1aa44d33bcaff
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58432369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1107bbf7e8a883f25f4975b43d490503a84921e26ccb943e929596f9b418cf40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:44:48 GMT
ADD file:ff9945b48b1ac236dcec24eb9dfaf52b7c151a3b11c8502391f0866dfb4e3ac3 in / 
# Mon, 09 Oct 2017 21:44:48 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 00:18:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:18:11 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 00:18:11 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 00:18:29 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 00:18:58 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:18:58 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 00:18:58 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 00:19:26 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:19:26 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 00:19:27 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 00:19:28 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 00:19:29 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 00:19:30 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Sat, 14 Oct 2017 14:14:24 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Sat, 14 Oct 2017 14:14:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 14 Oct 2017 14:14:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 Oct 2017 14:14:25 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Sat, 14 Oct 2017 14:14:26 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:836d5b6056a9815be79c76480a90299267f60201bd1e3396817003e6c14819cc`  
		Last Modified: Mon, 09 Oct 2017 21:50:56 GMT  
		Size: 21.2 MB (21166251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb896fba83bd09a35c68457554b35289860c23c46f27a8c3ef42f13146ebba1`  
		Last Modified: Tue, 10 Oct 2017 00:20:01 GMT  
		Size: 4.2 MB (4231979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61827a16c114b9741d761aa4c60a972ffe1e0b60147794e86b05653d67822e91`  
		Last Modified: Tue, 10 Oct 2017 00:20:00 GMT  
		Size: 4.1 KB (4079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877cd9511def30e56a5ce354e145e8a2b1a93daaae7eaaa42dc4219838aa1743`  
		Last Modified: Tue, 10 Oct 2017 00:20:00 GMT  
		Size: 942.8 KB (942752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea9e378899e98c99e93ae2d0874bd5d89e24134bd14a19c285bdf39a0a42ade`  
		Last Modified: Tue, 10 Oct 2017 00:20:05 GMT  
		Size: 25.2 MB (25170810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc82a29314b16531aa2172ac523ba535e3678f85efdd699164fbb0241ab8b62`  
		Last Modified: Tue, 10 Oct 2017 00:20:01 GMT  
		Size: 6.9 MB (6909811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c44a3d016cf9de95021782180a42d3660e20fc7d8e92a7fe5ce9ede7928ca2`  
		Last Modified: Tue, 10 Oct 2017 00:19:59 GMT  
		Size: 2.3 KB (2261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abfdcdd98b40291ad91791bea09bf277e75c3669c6607c7891b09130101bfa3`  
		Last Modified: Tue, 10 Oct 2017 00:19:58 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a72811da4bf8ca8a2d06cdc182aa54116bb12133e8d82ef2b018a8de29ed74`  
		Last Modified: Tue, 10 Oct 2017 00:19:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147d8cf0897dea9b024bf5c6efb6873db3d86dec857fca062b146f88b7b5a735`  
		Last Modified: Sat, 14 Oct 2017 14:14:43 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f355fd0b70caedf30aa384298307b8e40d922e9e341492dd3fde71f119fd7d7`  
		Last Modified: Sat, 14 Oct 2017 14:14:44 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:c5a07be740a1d956343d5881d8827cb9e3d6dcceda2d8ce954cf187ab9be9abc
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55688150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c4235a850985eab3d39e30563f87f78348a6425ec30388363f9d372c082855e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:43 GMT
ADD file:b758c6c3ff989778bd740dde35c86b953fa09be913a7e02711b2881de6b8911d in / 
# Mon, 09 Oct 2017 21:45:44 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 13:07:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:07:42 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 13:07:42 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 13:07:58 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 13:08:17 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:08:17 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 13:08:17 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 13:08:39 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:08:39 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 13:08:40 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 13:08:41 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 13:08:42 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 13:08:43 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 13:08:43 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 13:08:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 13:08:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 13:08:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 13:08:45 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:59e81a3fde58ec8d4b8f2f58b98ef2f4d951d37dd9b99b016fd294a8e07d7796`  
		Last Modified: Mon, 09 Oct 2017 21:52:49 GMT  
		Size: 19.3 MB (19277135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2037b99f3c3dc51e8ace39aed9971155f34f325ac4f0a1e56a07c4d6c02f5ae6`  
		Last Modified: Fri, 03 Nov 2017 13:09:18 GMT  
		Size: 3.9 MB (3868347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f368172ea96bda944832762ad29b52dfe17ec5e6fae96eee37adc4e9d68674a5`  
		Last Modified: Fri, 03 Nov 2017 13:09:16 GMT  
		Size: 4.1 KB (4084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893cc1ae60f8bf72ac3020ccc60b22d9e0ad0cb0647e15bc4847d08c8985eee2`  
		Last Modified: Fri, 03 Nov 2017 13:09:16 GMT  
		Size: 926.1 KB (926097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13220cc1a683014bda9cfae7f7ee7015a26b28048f90f5aa3ed8b6a96f4b2813`  
		Last Modified: Fri, 03 Nov 2017 13:09:20 GMT  
		Size: 24.8 MB (24785610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269f4e069126132643c1c0be1faf600d55ff15e870066c527d03181904d99c5d`  
		Last Modified: Fri, 03 Nov 2017 13:09:17 GMT  
		Size: 6.8 MB (6820180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ae244f4f610a339fcbddf37612a15ec7b7f6674e3d888c3c4d36302283418e`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce7d85327b7bc7d59a7b54222a3e6babd7f8afd8eb080becb77fc52aed5a751`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dfa32e4b49700ed0130ebd563f40a2c381393983b571a9886435813102ad0c`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba15cd885dc21f438d366b40d0d9f595f2c25e063c60fa590ab4c0f6233ff94`  
		Last Modified: Fri, 03 Nov 2017 13:09:14 GMT  
		Size: 4.0 KB (4040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978a8434497fcb8e08cefc7484b515ac34fe23c281fb869d015f62b54673028c`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:3d9b2aee2786ff5328bb6b1195f2938e251fdfe7c183ffac1ead7ffe6f234d03
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57278372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa9e28302480b775a117eda9fd3d2e8897ee8a4ed19ceac66f0afaab1e5f8609`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:47:55 GMT
ADD file:3a528355cfc75437716aff3b517ef99ae602918d84d26dbafff0ed142248fb93 in / 
# Mon, 09 Oct 2017 21:47:56 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 04:57:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 04:57:04 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 04:57:05 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 04:57:37 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 04:58:35 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 04:58:36 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 04:58:37 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 04:58:37 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 04:58:38 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 04:58:39 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 04:58:39 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 05:00:22 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 05:00:23 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 05:00:25 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 05:00:26 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 05:00:28 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 05:00:31 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Sat, 14 Oct 2017 13:52:47 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Sat, 14 Oct 2017 13:52:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 14 Oct 2017 13:52:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 Oct 2017 13:52:51 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Sat, 14 Oct 2017 13:52:51 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:e907afd6e25615a4d3eb554d930cef57b87e79ec82413889c2eac38beb4eb8f7`  
		Last Modified: Mon, 09 Oct 2017 22:03:08 GMT  
		Size: 20.3 MB (20337143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5e6d35928560b933b85b5a3f2a8e96b4520fbb8df138b3e739e56d0c1f355`  
		Last Modified: Tue, 10 Oct 2017 05:01:18 GMT  
		Size: 4.1 MB (4073554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a862ab821b342790326492507ca5d70bfb7016bef765606193f1f7139f60c5ed`  
		Last Modified: Tue, 10 Oct 2017 05:01:14 GMT  
		Size: 4.1 KB (4072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92799a54920b79013733790e444f13d8c65faa29c79cbdaf1bc8af85f637a233`  
		Last Modified: Tue, 10 Oct 2017 05:01:14 GMT  
		Size: 919.5 KB (919487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b119999eef1bcadabedd3a5319b03c6b83ede91ba8535059851547d3433b205`  
		Last Modified: Tue, 10 Oct 2017 05:01:19 GMT  
		Size: 25.0 MB (25042572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62f8525a3a982a102aa37bb3313876195b15d8781cd253ed238dd2b9dff151`  
		Last Modified: Tue, 10 Oct 2017 05:01:15 GMT  
		Size: 6.9 MB (6894852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc028e70f04f6ea4365223a1cfe4e5c4384d5921acac419f3c170b148f7c7bf`  
		Last Modified: Tue, 10 Oct 2017 05:01:10 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e99faa03c2a8a272f56208c644c12b384b69dea50be6da9f6be400c14b945c`  
		Last Modified: Tue, 10 Oct 2017 05:01:12 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8fa260bcaa52d81ba20c11111f8d15bab954b17b48666724536c604220d94e`  
		Last Modified: Tue, 10 Oct 2017 05:01:11 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306840de948d03472918a306c089409429606802ec8cf841e96dec707a2f7178`  
		Last Modified: Sat, 14 Oct 2017 13:53:27 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a7a978032478b38adb1f0107466d187e53380f7037d058c62e4937cd07fc09`  
		Last Modified: Sat, 14 Oct 2017 13:53:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6` - linux; 386

```console
$ docker pull rabbitmq@sha256:900c25b037b878974bb75f9d056b5278794f96586c9d03f619af9905a6cf5229
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63902262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a993d7c3c104c0e9f2ed42d750b907890291a9a2693d23f166744b9fb8e9265d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:36 GMT
ADD file:6582536277127947668f7bfdc1471a4e36170915b91a4cb841e7e1bfa1de6535 in / 
# Mon, 09 Oct 2017 21:45:36 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 10:45:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:45:12 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 10:45:13 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 10:45:28 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 10:46:03 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 10:46:04 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 10:46:25 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:46:25 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 10:46:26 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 10:46:27 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 10:46:27 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 10:46:28 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 10:46:28 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 10:46:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 10:46:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 10:46:30 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 10:46:30 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:b2b52fe46b29fe5d0689f26449c2114e40f0731d4ce3eb8c3941397b74205432`  
		Last Modified: Mon, 09 Oct 2017 21:53:42 GMT  
		Size: 23.1 MB (23128678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d407b136da0731f5f38279001e9dd426217937443cad0f16e1f242366290773`  
		Last Modified: Fri, 03 Nov 2017 10:47:13 GMT  
		Size: 4.8 MB (4803637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c93817e78345b4b5070c81e5a37d02afc2b5fe347a1a4bf59e09f6084814fd2`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 4.1 KB (4057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97eae59c75f8f814ab781f5239ac2e132b7b65c77e75b35023c603c539ca54f`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 931.5 KB (931524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aed670dee19fde6946658d7129e13520c1a0747f8b80b6f92dac5f6d974ae52`  
		Last Modified: Fri, 03 Nov 2017 10:47:24 GMT  
		Size: 27.8 MB (27818690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b61d6d0b60ec18280aeba946a05d62817afbe030f277af85b5f434021e90c9`  
		Last Modified: Fri, 03 Nov 2017 10:47:16 GMT  
		Size: 7.2 MB (7208985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec7d4cc3b5497bbbd6b2d1e9574dbedb6c7ad11805cff4c287ea444ddc2e298`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 2.3 KB (2259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eec554591344f78e35e3976d002d617623a52d123fc71e65d33c4d533d2b2e7`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e433f73af1167eff0dee1984c095bf5be36593fcead5b8cc820e2cb829aaed0`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8d6e0dbdbb04b44f7a0972fce6b0b1b19262e4fc5416bd1589af560f16c99f`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 4.0 KB (4040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bab08cf9b00d8109139e1cb1cdec448b71fdae7d7f1260d4175771416a5f80`  
		Last Modified: Fri, 03 Nov 2017 10:47:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:63dcce5fe70ba7b07c27b3af47248ad1f0609ca79e98e01a2ea0cb4e5357cc55
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60384479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:929ca14b97313f42a819bb7e089422aea0fa6d6a7428046a573c11937059499d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:56 GMT
ADD file:7edf73437495be24244c16841b563be06c15452963f41ac940fb5e105ed96027 in / 
# Mon, 09 Oct 2017 21:45:58 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 07:12:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:12:51 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 07:12:53 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 07:13:49 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 07:15:26 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:15:28 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 07:15:29 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 07:15:31 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 07:15:33 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 07:15:34 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 07:15:35 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 07:16:54 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:16:55 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 07:17:00 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 07:17:01 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 07:17:06 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 07:17:11 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 07:17:13 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 07:17:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 07:17:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 07:17:21 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 07:17:23 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:c4860466fa1e6824151f4fa3a51ef0e9d7d3c3ba860e21d94e69988b65601260`  
		Last Modified: Mon, 09 Oct 2017 21:52:59 GMT  
		Size: 22.7 MB (22746217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebe4c87dcd1f7ef11d4d21752831bf4095ac42afe041706c35f1d7d4d0ca4f2`  
		Last Modified: Fri, 03 Nov 2017 07:18:05 GMT  
		Size: 4.4 MB (4360529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e5365525084de1c85fa29ef33d37c38b5f80621f5bcb26bb4882d71598c6f7`  
		Last Modified: Fri, 03 Nov 2017 07:18:03 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600c3853740b7f4cff9cc799ae478f669bd54277a8dd375479a34ed1bb47a803`  
		Last Modified: Fri, 03 Nov 2017 07:18:02 GMT  
		Size: 920.7 KB (920695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993868ec534130e348e45aa6d64b471fa46eafbf061836cc9d2a56edf73e9382`  
		Last Modified: Fri, 03 Nov 2017 07:18:06 GMT  
		Size: 25.5 MB (25492533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca1b92e212aaef163244d5fdd9e135fdb8be8c9dbbb626061ee2882d941a553`  
		Last Modified: Fri, 03 Nov 2017 07:18:03 GMT  
		Size: 6.9 MB (6853702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483f96d1f500f9f69170bc6927d599a7f0cd1550f96b6ee3f90eb4185a1bffb`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b433db63f40c7cab3080cf36bd7beabbdf7d9eece3f2dc16a65b900c61180`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93971551a2c911c34ca2e9af47495efb2f27e2922e567d93dd94dfb9b773bd3`  
		Last Modified: Fri, 03 Nov 2017 07:17:58 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5494bb8bcc45452a84c216edffedb3103a15c3e209aba0561dfbc70e4312192e`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 4.0 KB (4039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d56b2a4f9f8d7b11831a8f1952fe2c02613bcb014ab9d756b70b3b398b37269`  
		Last Modified: Fri, 03 Nov 2017 07:17:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6` - linux; s390x

```console
$ docker pull rabbitmq@sha256:c5e29e37ac52898d26c2d63c4e0506afbaf0fa3862456c04c425429dae26248a
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60364776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9b9f437096f93b98ba60e922a7e6c52ff1e8a75593833f81fa03b4a035a3f50`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:44:35 GMT
ADD file:ae4aaa6affe22f36ab5478771d5c84917f72de7a8dac16345a035709a1a5edf4 in / 
# Mon, 09 Oct 2017 21:44:36 GMT
CMD ["bash"]
# Thu, 02 Nov 2017 17:06:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 17:06:41 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Thu, 02 Nov 2017 17:06:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 02 Nov 2017 17:07:21 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Thu, 02 Nov 2017 17:07:43 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 02 Nov 2017 17:07:44 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 02 Nov 2017 17:07:45 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 17:07:48 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 17:07:48 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 17:07:49 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 17:07:50 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 17:07:52 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 17:07:53 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 17:07:54 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 17:07:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 17:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 17:07:57 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 17:07:57 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:671716cc49517eef5f430c695ce344d63e390cb65f58d30939f2ba615c953686`  
		Last Modified: Mon, 09 Oct 2017 21:49:09 GMT  
		Size: 22.3 MB (22339951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cae61f12be6f01ba06573d9393712e91821cd5496302310f550fe5842dea557`  
		Last Modified: Fri, 03 Nov 2017 17:08:41 GMT  
		Size: 4.5 MB (4529879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca307103ce923e7e89d35185be4df8e54c3c0b54d259b8880aa7bae107d4952`  
		Last Modified: Fri, 03 Nov 2017 17:08:39 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d16320f9fc35ea20ba7fb9b21f88e3f0f06c52d416682319f3b2a85a345a3d5`  
		Last Modified: Fri, 03 Nov 2017 17:08:39 GMT  
		Size: 938.0 KB (938019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801205b182b8d6f7acf36200b2ba07ed52ea224dfefe792b525224e4aacb4d4a`  
		Last Modified: Fri, 03 Nov 2017 17:08:48 GMT  
		Size: 25.6 MB (25619372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9cb605e6242f5ab505cbd229c7b2fdf2935a6254130070c12c4d8413616024`  
		Last Modified: Fri, 03 Nov 2017 17:08:40 GMT  
		Size: 6.9 MB (6926791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2799e1b1479136fbb3c3ba6df318d449990a3cf5fc3293a14142cde0d9f51980`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a6d5de3e6aaa1c06122a1b5cda3b4bcb98d54e5dc23f38896fc81e98cea769`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172fa2e52818dcedf69c727f6790f0f9744f8538da3f4222602aaa0ab9fa82c0`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c734f2707800c1189521a51409fed1508fb7e36c6e67eca5537d03c4b24ef0d`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 4.0 KB (4037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e7d712f1155d66243480cd441ec04e084a8e7e2d6a0653e27138b31b56d2ae`  
		Last Modified: Fri, 03 Nov 2017 17:08:38 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rabbitmq:3.6.12`

```console
$ docker pull rabbitmq@sha256:2c3145ed1766d6eac4f224c990d02a2c2411e8b1dc02875a28b7cf8acc9fa985
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

### `rabbitmq:3.6.12` - linux; amd64

```console
$ docker pull rabbitmq@sha256:b99e238fa99bcd7ffcfd89a536fdf33bbd27e206cea118246874e3792ebfc2bc
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.9 MB (62852177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e186865bff877f181c4a4b4ffdb7235e91c0c988bdc0c926d1b68e5d8c81e45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:33:42 GMT
ADD file:45233d6b5c9b91e9437065d3e7c332d1c4eb4bce8e1079a4c1af342c450abe67 in / 
# Mon, 09 Oct 2017 21:33:43 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 02:41:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:41:43 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 02:41:43 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 02:42:10 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 02:42:40 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 02:42:41 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 02:42:42 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 02:43:16 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:43:16 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 02:43:17 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 02:43:17 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 02:43:18 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 02:43:19 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 13 Oct 2017 23:40:43 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 13 Oct 2017 23:40:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 13 Oct 2017 23:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2017 23:40:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 13 Oct 2017 23:40:45 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:bc95e04b23c06ba1b9bf092d07d1493177b218e0340bd2ed49dac351c1e34313`  
		Last Modified: Mon, 09 Oct 2017 21:42:28 GMT  
		Size: 22.5 MB (22492350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65f0b00e4cfb1535d0f4e7a63707172ae63483fb33140d777614f199afcb36`  
		Last Modified: Tue, 10 Oct 2017 02:43:59 GMT  
		Size: 4.5 MB (4498726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bd803179890909fcae186044c0e6ca1bc1d34e5fc05ef1ccea823e7be97540`  
		Last Modified: Tue, 10 Oct 2017 02:43:57 GMT  
		Size: 4.1 KB (4069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b05ca8302833edf783c50f03cd7ba0b8e12bc872b053eda3e3ae7e1f17e2b4b`  
		Last Modified: Tue, 10 Oct 2017 02:43:58 GMT  
		Size: 952.1 KB (952058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb5a4bbcce5a040eb83057f9e93d17663bb123f4e98168457444497f7d17b70`  
		Last Modified: Tue, 10 Oct 2017 02:44:03 GMT  
		Size: 27.7 MB (27703883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf840d8999f6fe46a162974c82378c38b3cf3dcccbbaff848c0fb199988aebe0`  
		Last Modified: Tue, 10 Oct 2017 02:44:00 GMT  
		Size: 7.2 MB (7194403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be339ca44883b1990e52771487402163d398a279755a501fdd8891ec71cf09d0`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce35cd9f9b5b917868095b3b074dd23d18e0e266f3ee68ff95e2c61467299812`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fe32a0a00d916ed4d632aae71d35d9d0baa5e5910d6bd179a24071c35bedb0`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77408ca9e94eb4bfeb346ab10c602857525802c2279e7c6995fcdbc90269444a`  
		Last Modified: Fri, 13 Oct 2017 23:41:26 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db03407a1aba1c0a89dffe960394aae639885702e3faa65271b918c36c7905cd`  
		Last Modified: Fri, 13 Oct 2017 23:41:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12` - linux; arm variant v5

```console
$ docker pull rabbitmq@sha256:53c2349355bbba2f2b1eeb11d5ed481cab005bba90148c0ed0c1aa44d33bcaff
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58432369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1107bbf7e8a883f25f4975b43d490503a84921e26ccb943e929596f9b418cf40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:44:48 GMT
ADD file:ff9945b48b1ac236dcec24eb9dfaf52b7c151a3b11c8502391f0866dfb4e3ac3 in / 
# Mon, 09 Oct 2017 21:44:48 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 00:18:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:18:11 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 00:18:11 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 00:18:29 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 00:18:58 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:18:58 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 00:18:58 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 00:19:26 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:19:26 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 00:19:27 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 00:19:28 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 00:19:29 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 00:19:30 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Sat, 14 Oct 2017 14:14:24 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Sat, 14 Oct 2017 14:14:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 14 Oct 2017 14:14:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 Oct 2017 14:14:25 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Sat, 14 Oct 2017 14:14:26 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:836d5b6056a9815be79c76480a90299267f60201bd1e3396817003e6c14819cc`  
		Last Modified: Mon, 09 Oct 2017 21:50:56 GMT  
		Size: 21.2 MB (21166251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb896fba83bd09a35c68457554b35289860c23c46f27a8c3ef42f13146ebba1`  
		Last Modified: Tue, 10 Oct 2017 00:20:01 GMT  
		Size: 4.2 MB (4231979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61827a16c114b9741d761aa4c60a972ffe1e0b60147794e86b05653d67822e91`  
		Last Modified: Tue, 10 Oct 2017 00:20:00 GMT  
		Size: 4.1 KB (4079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877cd9511def30e56a5ce354e145e8a2b1a93daaae7eaaa42dc4219838aa1743`  
		Last Modified: Tue, 10 Oct 2017 00:20:00 GMT  
		Size: 942.8 KB (942752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea9e378899e98c99e93ae2d0874bd5d89e24134bd14a19c285bdf39a0a42ade`  
		Last Modified: Tue, 10 Oct 2017 00:20:05 GMT  
		Size: 25.2 MB (25170810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc82a29314b16531aa2172ac523ba535e3678f85efdd699164fbb0241ab8b62`  
		Last Modified: Tue, 10 Oct 2017 00:20:01 GMT  
		Size: 6.9 MB (6909811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c44a3d016cf9de95021782180a42d3660e20fc7d8e92a7fe5ce9ede7928ca2`  
		Last Modified: Tue, 10 Oct 2017 00:19:59 GMT  
		Size: 2.3 KB (2261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abfdcdd98b40291ad91791bea09bf277e75c3669c6607c7891b09130101bfa3`  
		Last Modified: Tue, 10 Oct 2017 00:19:58 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a72811da4bf8ca8a2d06cdc182aa54116bb12133e8d82ef2b018a8de29ed74`  
		Last Modified: Tue, 10 Oct 2017 00:19:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147d8cf0897dea9b024bf5c6efb6873db3d86dec857fca062b146f88b7b5a735`  
		Last Modified: Sat, 14 Oct 2017 14:14:43 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f355fd0b70caedf30aa384298307b8e40d922e9e341492dd3fde71f119fd7d7`  
		Last Modified: Sat, 14 Oct 2017 14:14:44 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:c5a07be740a1d956343d5881d8827cb9e3d6dcceda2d8ce954cf187ab9be9abc
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55688150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c4235a850985eab3d39e30563f87f78348a6425ec30388363f9d372c082855e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:43 GMT
ADD file:b758c6c3ff989778bd740dde35c86b953fa09be913a7e02711b2881de6b8911d in / 
# Mon, 09 Oct 2017 21:45:44 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 13:07:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:07:42 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 13:07:42 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 13:07:58 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 13:08:17 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:08:17 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 13:08:17 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 13:08:39 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:08:39 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 13:08:40 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 13:08:41 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 13:08:42 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 13:08:43 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 13:08:43 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 13:08:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 13:08:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 13:08:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 13:08:45 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:59e81a3fde58ec8d4b8f2f58b98ef2f4d951d37dd9b99b016fd294a8e07d7796`  
		Last Modified: Mon, 09 Oct 2017 21:52:49 GMT  
		Size: 19.3 MB (19277135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2037b99f3c3dc51e8ace39aed9971155f34f325ac4f0a1e56a07c4d6c02f5ae6`  
		Last Modified: Fri, 03 Nov 2017 13:09:18 GMT  
		Size: 3.9 MB (3868347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f368172ea96bda944832762ad29b52dfe17ec5e6fae96eee37adc4e9d68674a5`  
		Last Modified: Fri, 03 Nov 2017 13:09:16 GMT  
		Size: 4.1 KB (4084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893cc1ae60f8bf72ac3020ccc60b22d9e0ad0cb0647e15bc4847d08c8985eee2`  
		Last Modified: Fri, 03 Nov 2017 13:09:16 GMT  
		Size: 926.1 KB (926097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13220cc1a683014bda9cfae7f7ee7015a26b28048f90f5aa3ed8b6a96f4b2813`  
		Last Modified: Fri, 03 Nov 2017 13:09:20 GMT  
		Size: 24.8 MB (24785610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269f4e069126132643c1c0be1faf600d55ff15e870066c527d03181904d99c5d`  
		Last Modified: Fri, 03 Nov 2017 13:09:17 GMT  
		Size: 6.8 MB (6820180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ae244f4f610a339fcbddf37612a15ec7b7f6674e3d888c3c4d36302283418e`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce7d85327b7bc7d59a7b54222a3e6babd7f8afd8eb080becb77fc52aed5a751`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dfa32e4b49700ed0130ebd563f40a2c381393983b571a9886435813102ad0c`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba15cd885dc21f438d366b40d0d9f595f2c25e063c60fa590ab4c0f6233ff94`  
		Last Modified: Fri, 03 Nov 2017 13:09:14 GMT  
		Size: 4.0 KB (4040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978a8434497fcb8e08cefc7484b515ac34fe23c281fb869d015f62b54673028c`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:3d9b2aee2786ff5328bb6b1195f2938e251fdfe7c183ffac1ead7ffe6f234d03
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57278372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa9e28302480b775a117eda9fd3d2e8897ee8a4ed19ceac66f0afaab1e5f8609`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:47:55 GMT
ADD file:3a528355cfc75437716aff3b517ef99ae602918d84d26dbafff0ed142248fb93 in / 
# Mon, 09 Oct 2017 21:47:56 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 04:57:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 04:57:04 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 04:57:05 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 04:57:37 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 04:58:35 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 04:58:36 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 04:58:37 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 04:58:37 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 04:58:38 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 04:58:39 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 04:58:39 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 05:00:22 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 05:00:23 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 05:00:25 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 05:00:26 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 05:00:28 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 05:00:31 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Sat, 14 Oct 2017 13:52:47 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Sat, 14 Oct 2017 13:52:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 14 Oct 2017 13:52:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 Oct 2017 13:52:51 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Sat, 14 Oct 2017 13:52:51 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:e907afd6e25615a4d3eb554d930cef57b87e79ec82413889c2eac38beb4eb8f7`  
		Last Modified: Mon, 09 Oct 2017 22:03:08 GMT  
		Size: 20.3 MB (20337143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5e6d35928560b933b85b5a3f2a8e96b4520fbb8df138b3e739e56d0c1f355`  
		Last Modified: Tue, 10 Oct 2017 05:01:18 GMT  
		Size: 4.1 MB (4073554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a862ab821b342790326492507ca5d70bfb7016bef765606193f1f7139f60c5ed`  
		Last Modified: Tue, 10 Oct 2017 05:01:14 GMT  
		Size: 4.1 KB (4072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92799a54920b79013733790e444f13d8c65faa29c79cbdaf1bc8af85f637a233`  
		Last Modified: Tue, 10 Oct 2017 05:01:14 GMT  
		Size: 919.5 KB (919487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b119999eef1bcadabedd3a5319b03c6b83ede91ba8535059851547d3433b205`  
		Last Modified: Tue, 10 Oct 2017 05:01:19 GMT  
		Size: 25.0 MB (25042572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62f8525a3a982a102aa37bb3313876195b15d8781cd253ed238dd2b9dff151`  
		Last Modified: Tue, 10 Oct 2017 05:01:15 GMT  
		Size: 6.9 MB (6894852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc028e70f04f6ea4365223a1cfe4e5c4384d5921acac419f3c170b148f7c7bf`  
		Last Modified: Tue, 10 Oct 2017 05:01:10 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e99faa03c2a8a272f56208c644c12b384b69dea50be6da9f6be400c14b945c`  
		Last Modified: Tue, 10 Oct 2017 05:01:12 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8fa260bcaa52d81ba20c11111f8d15bab954b17b48666724536c604220d94e`  
		Last Modified: Tue, 10 Oct 2017 05:01:11 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306840de948d03472918a306c089409429606802ec8cf841e96dec707a2f7178`  
		Last Modified: Sat, 14 Oct 2017 13:53:27 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a7a978032478b38adb1f0107466d187e53380f7037d058c62e4937cd07fc09`  
		Last Modified: Sat, 14 Oct 2017 13:53:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12` - linux; 386

```console
$ docker pull rabbitmq@sha256:900c25b037b878974bb75f9d056b5278794f96586c9d03f619af9905a6cf5229
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63902262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a993d7c3c104c0e9f2ed42d750b907890291a9a2693d23f166744b9fb8e9265d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:36 GMT
ADD file:6582536277127947668f7bfdc1471a4e36170915b91a4cb841e7e1bfa1de6535 in / 
# Mon, 09 Oct 2017 21:45:36 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 10:45:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:45:12 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 10:45:13 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 10:45:28 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 10:46:03 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 10:46:04 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 10:46:25 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:46:25 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 10:46:26 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 10:46:27 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 10:46:27 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 10:46:28 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 10:46:28 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 10:46:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 10:46:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 10:46:30 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 10:46:30 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:b2b52fe46b29fe5d0689f26449c2114e40f0731d4ce3eb8c3941397b74205432`  
		Last Modified: Mon, 09 Oct 2017 21:53:42 GMT  
		Size: 23.1 MB (23128678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d407b136da0731f5f38279001e9dd426217937443cad0f16e1f242366290773`  
		Last Modified: Fri, 03 Nov 2017 10:47:13 GMT  
		Size: 4.8 MB (4803637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c93817e78345b4b5070c81e5a37d02afc2b5fe347a1a4bf59e09f6084814fd2`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 4.1 KB (4057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97eae59c75f8f814ab781f5239ac2e132b7b65c77e75b35023c603c539ca54f`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 931.5 KB (931524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aed670dee19fde6946658d7129e13520c1a0747f8b80b6f92dac5f6d974ae52`  
		Last Modified: Fri, 03 Nov 2017 10:47:24 GMT  
		Size: 27.8 MB (27818690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b61d6d0b60ec18280aeba946a05d62817afbe030f277af85b5f434021e90c9`  
		Last Modified: Fri, 03 Nov 2017 10:47:16 GMT  
		Size: 7.2 MB (7208985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec7d4cc3b5497bbbd6b2d1e9574dbedb6c7ad11805cff4c287ea444ddc2e298`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 2.3 KB (2259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eec554591344f78e35e3976d002d617623a52d123fc71e65d33c4d533d2b2e7`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e433f73af1167eff0dee1984c095bf5be36593fcead5b8cc820e2cb829aaed0`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8d6e0dbdbb04b44f7a0972fce6b0b1b19262e4fc5416bd1589af560f16c99f`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 4.0 KB (4040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bab08cf9b00d8109139e1cb1cdec448b71fdae7d7f1260d4175771416a5f80`  
		Last Modified: Fri, 03 Nov 2017 10:47:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:63dcce5fe70ba7b07c27b3af47248ad1f0609ca79e98e01a2ea0cb4e5357cc55
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60384479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:929ca14b97313f42a819bb7e089422aea0fa6d6a7428046a573c11937059499d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:56 GMT
ADD file:7edf73437495be24244c16841b563be06c15452963f41ac940fb5e105ed96027 in / 
# Mon, 09 Oct 2017 21:45:58 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 07:12:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:12:51 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 07:12:53 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 07:13:49 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 07:15:26 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:15:28 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 07:15:29 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 07:15:31 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 07:15:33 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 07:15:34 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 07:15:35 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 07:16:54 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:16:55 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 07:17:00 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 07:17:01 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 07:17:06 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 07:17:11 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 07:17:13 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 07:17:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 07:17:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 07:17:21 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 07:17:23 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:c4860466fa1e6824151f4fa3a51ef0e9d7d3c3ba860e21d94e69988b65601260`  
		Last Modified: Mon, 09 Oct 2017 21:52:59 GMT  
		Size: 22.7 MB (22746217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebe4c87dcd1f7ef11d4d21752831bf4095ac42afe041706c35f1d7d4d0ca4f2`  
		Last Modified: Fri, 03 Nov 2017 07:18:05 GMT  
		Size: 4.4 MB (4360529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e5365525084de1c85fa29ef33d37c38b5f80621f5bcb26bb4882d71598c6f7`  
		Last Modified: Fri, 03 Nov 2017 07:18:03 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600c3853740b7f4cff9cc799ae478f669bd54277a8dd375479a34ed1bb47a803`  
		Last Modified: Fri, 03 Nov 2017 07:18:02 GMT  
		Size: 920.7 KB (920695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993868ec534130e348e45aa6d64b471fa46eafbf061836cc9d2a56edf73e9382`  
		Last Modified: Fri, 03 Nov 2017 07:18:06 GMT  
		Size: 25.5 MB (25492533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca1b92e212aaef163244d5fdd9e135fdb8be8c9dbbb626061ee2882d941a553`  
		Last Modified: Fri, 03 Nov 2017 07:18:03 GMT  
		Size: 6.9 MB (6853702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483f96d1f500f9f69170bc6927d599a7f0cd1550f96b6ee3f90eb4185a1bffb`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b433db63f40c7cab3080cf36bd7beabbdf7d9eece3f2dc16a65b900c61180`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93971551a2c911c34ca2e9af47495efb2f27e2922e567d93dd94dfb9b773bd3`  
		Last Modified: Fri, 03 Nov 2017 07:17:58 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5494bb8bcc45452a84c216edffedb3103a15c3e209aba0561dfbc70e4312192e`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 4.0 KB (4039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d56b2a4f9f8d7b11831a8f1952fe2c02613bcb014ab9d756b70b3b398b37269`  
		Last Modified: Fri, 03 Nov 2017 07:17:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12` - linux; s390x

```console
$ docker pull rabbitmq@sha256:c5e29e37ac52898d26c2d63c4e0506afbaf0fa3862456c04c425429dae26248a
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60364776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9b9f437096f93b98ba60e922a7e6c52ff1e8a75593833f81fa03b4a035a3f50`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:44:35 GMT
ADD file:ae4aaa6affe22f36ab5478771d5c84917f72de7a8dac16345a035709a1a5edf4 in / 
# Mon, 09 Oct 2017 21:44:36 GMT
CMD ["bash"]
# Thu, 02 Nov 2017 17:06:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 17:06:41 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Thu, 02 Nov 2017 17:06:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 02 Nov 2017 17:07:21 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Thu, 02 Nov 2017 17:07:43 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 02 Nov 2017 17:07:44 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 02 Nov 2017 17:07:45 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 17:07:48 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 17:07:48 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 17:07:49 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 17:07:50 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 17:07:52 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 17:07:53 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 17:07:54 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 17:07:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 17:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 17:07:57 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 17:07:57 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:671716cc49517eef5f430c695ce344d63e390cb65f58d30939f2ba615c953686`  
		Last Modified: Mon, 09 Oct 2017 21:49:09 GMT  
		Size: 22.3 MB (22339951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cae61f12be6f01ba06573d9393712e91821cd5496302310f550fe5842dea557`  
		Last Modified: Fri, 03 Nov 2017 17:08:41 GMT  
		Size: 4.5 MB (4529879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca307103ce923e7e89d35185be4df8e54c3c0b54d259b8880aa7bae107d4952`  
		Last Modified: Fri, 03 Nov 2017 17:08:39 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d16320f9fc35ea20ba7fb9b21f88e3f0f06c52d416682319f3b2a85a345a3d5`  
		Last Modified: Fri, 03 Nov 2017 17:08:39 GMT  
		Size: 938.0 KB (938019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801205b182b8d6f7acf36200b2ba07ed52ea224dfefe792b525224e4aacb4d4a`  
		Last Modified: Fri, 03 Nov 2017 17:08:48 GMT  
		Size: 25.6 MB (25619372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9cb605e6242f5ab505cbd229c7b2fdf2935a6254130070c12c4d8413616024`  
		Last Modified: Fri, 03 Nov 2017 17:08:40 GMT  
		Size: 6.9 MB (6926791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2799e1b1479136fbb3c3ba6df318d449990a3cf5fc3293a14142cde0d9f51980`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a6d5de3e6aaa1c06122a1b5cda3b4bcb98d54e5dc23f38896fc81e98cea769`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172fa2e52818dcedf69c727f6790f0f9744f8538da3f4222602aaa0ab9fa82c0`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c734f2707800c1189521a51409fed1508fb7e36c6e67eca5537d03c4b24ef0d`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 4.0 KB (4037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e7d712f1155d66243480cd441ec04e084a8e7e2d6a0653e27138b31b56d2ae`  
		Last Modified: Fri, 03 Nov 2017 17:08:38 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rabbitmq:3.6.12-alpine`

```console
$ docker pull rabbitmq@sha256:e49288ac5376cbd8699e6dd2d99410ce12ecd1a5f8885b9f8a1eebd863e3b4ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `rabbitmq:3.6.12-alpine` - linux; amd64

```console
$ docker pull rabbitmq@sha256:f8204cb30a089ec4fa99d41ed68f1b520670f5698bea479f6a6582d1926a5715
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23579666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:210310494165d259279503b1b25ecd975f73320e177d472300069bc8619908be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:19:51 GMT
ADD file:1e87ff33d1b6765b793888cd50e01b2bd0dfe152b7dbb4048008bfc2658faea7 in / 
# Wed, 25 Oct 2017 23:19:51 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 03:02:21 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 03:02:25 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 03:02:32 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 03:02:32 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 03:02:33 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 03:02:33 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 03:02:42 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 03:02:42 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 03:02:43 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 03:02:43 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 03:02:44 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 03:02:44 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 03:02:45 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 03:02:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 03:02:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 03:02:45 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:b56ae66c29370df48e7377c8f9baa744a3958058a766793f821dadcb144a4647`  
		Last Modified: Wed, 25 Oct 2017 23:21:25 GMT  
		Size: 2.0 MB (1991435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827e0bce86e3c8fa677ac91f0c55a7a4071cc45c729b171aecbe04d35ae160d7`  
		Last Modified: Thu, 26 Oct 2017 03:03:23 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe01d115cb92dc0ab37de6b6ffa2073ea20d30dfc49c537fbba569cd6a494b8`  
		Last Modified: Thu, 26 Oct 2017 03:03:23 GMT  
		Size: 8.2 KB (8176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bfc0dbbf8b1d2f532779c4873b4c7e0237d6ecc86161b1c6f28e3b6bd3149f`  
		Last Modified: Thu, 26 Oct 2017 03:03:26 GMT  
		Size: 16.6 MB (16561644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b24f4fd26b3494d310561a28e2d9aeb08e7baba442eaef2cd8697c7ebd9d9f1`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 5.0 MB (5012671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfb0f3b402f9674b21d7ed079f6576ec1be80f333f41c404e8ce3feb193b813`  
		Last Modified: Thu, 26 Oct 2017 03:03:22 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521b2b4b2311f153d53f0b9bde9a164f45df9dfd531512c36195ba2ccf5a4c76`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cedbb525e85f1b9257e8b20d04b4ad39f1004c9dfbc673086815dd887f380c3`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f35995cc5f5daa05334d17a87482ac8728aadfb0f10f9d62b3d70f5986e5cc`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:9bbc37dee4951514ff22f2fc83eed327e4fb935baedc146be69d4b7bd04b40b6
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23412846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d5e63a3df176d84fe8622b7515aa144197643b1a5ac6fc5b1578c6d78fb121c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:35 GMT
ADD file:009348222efb3c4ca2e53c387fb34c488679ca07db39525a6c5cc214e46abffd in / 
# Wed, 25 Oct 2017 23:28:36 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:36 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 05:25:53 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 05:25:55 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 05:26:10 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 05:26:10 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 05:26:10 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 05:26:11 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 05:26:19 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 05:26:19 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 05:26:20 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 05:26:20 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 05:26:21 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 05:26:22 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 05:26:22 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 05:26:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 05:26:22 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 05:26:23 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:0864efeeb5cb8dca4eb53e5d6fd38486daee80fa326fe36d1ad254f8fa6bb310`  
		Last Modified: Sun, 23 Jul 2017 20:21:42 GMT  
		Size: 2.0 MB (1965988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda69762aee1588fa82aeabf1af6d6ad24f737cce1451fab2e0199849b1e12e`  
		Last Modified: Wed, 25 Oct 2017 23:28:45 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62a8c5580cc1c2fbf2f9ce119bc0c06403a12ad18167bde2ec94420810916db`  
		Last Modified: Thu, 26 Oct 2017 05:26:38 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b096e39434b5aeddcb2ec167b7bf570cac7b8b16e68324d3f46c6f4d41b69c79`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 8.4 KB (8374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ad9273316fa6f22cd2e8cf88c92f34c3210325fa1be2041153a96f4124476f`  
		Last Modified: Thu, 26 Oct 2017 05:26:41 GMT  
		Size: 16.4 MB (16420180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed982c9e7d5644c85267595b470c0f21f25093a865603ab33304248efdb68b5d`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 5.0 MB (5012332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b76830a9cb5b5f898068945d6af6325c7d97b36d50e521a12097d3e908fd0`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a31f9ee2285379d9d5106926e707698e7a3283f707a4573fec9731e6ede58b5`  
		Last Modified: Thu, 26 Oct 2017 05:26:36 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff38544dc85623170156958b2d5d51604efd94b336b47a6479cde0417667838f`  
		Last Modified: Thu, 26 Oct 2017 05:26:36 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564bee8c5f497342e71777f1adc38d1578f7c95ddefe18efa16fc01b3e7e2a52`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:dcc95a027acff970a00636c77c269b7cc72e3176411c8aecc946eb6642b3906c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23318158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b316c629f8f17231a345cc527fcd76aa75a8b9e012eeae0d0497b3a92c014132`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:58 GMT
ADD file:45b5d3b8d5490ba7edfca2cf6f54cdcf49c772b0b3a2302ce69a7af061007aa4 in / 
# Wed, 25 Oct 2017 23:28:59 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:59 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 13:53:09 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 13:53:13 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 13:53:28 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 13:53:28 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 13:53:29 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 13:53:29 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 13:53:30 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 13:53:30 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 13:53:31 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 13:54:22 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 13:54:23 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 13:54:24 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 13:54:25 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 13:54:26 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 13:54:28 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 13:54:29 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 13:54:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 13:54:30 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 13:54:30 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:bb473f0ebc12fde1bd45c1bd3c46f2d3aab367b1b7739464771455b9972f7894`  
		Last Modified: Thu, 06 Jul 2017 09:54:42 GMT  
		Size: 1.9 MB (1914748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ff6b7ff3a208b8399e701e7ea1b7edbdc654c8c60d33c6f09a7803e2dda776`  
		Last Modified: Wed, 25 Oct 2017 23:29:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05834eac152e30997eb4f1aa4ffe8e952bd759c1a1009bd183dec80dca24cf86`  
		Last Modified: Thu, 26 Oct 2017 13:55:11 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd88a23486b40755f2e1192cb35d4fdaec20831c18ce83da31df3f8aa2f7b45c`  
		Last Modified: Thu, 26 Oct 2017 13:55:11 GMT  
		Size: 8.3 KB (8297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f9ba1206e6e4bfba21cef7f235482b41868ec966d5ebc44a4c4ac432a5fe03`  
		Last Modified: Thu, 26 Oct 2017 13:55:16 GMT  
		Size: 16.4 MB (16376872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5991837e23d785829d605fd052c61e10ed79a7cfb0dfee9dd40d6144bc9fad0f`  
		Last Modified: Thu, 26 Oct 2017 13:55:12 GMT  
		Size: 5.0 MB (5012322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf5663fa552ede671fc5ebf425b2ce3ff5257636b55df9564e556fe7ff85fce`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794d04d767a60fa6df4adb3af1f835701a3c2692e7f6b2d4a9db621a0bc8cd5f`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91155b0cb6bf92d1ab05fb7d13593e0a966eb79dd4e4173e3895d98dffe1c996`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969bbed547aa67091daaa801a46b062fd1c39f7835c81dd5052032056b6cf230`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:3355a334e7313d636e6b3d263a101f1ab926a88bcee118e357835788d527179a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23782989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b83bfaf99c5c91aa3c08ade40b04a3bc1b6bd3725fa905cd0a488133319eef9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:32:08 GMT
ADD file:4a952fc4b81d50b342e26a818dac48a148a4d5eddb878219650e579a5c9faeaa in / 
# Wed, 25 Oct 2017 23:32:08 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:32:08 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 10:44:24 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 10:44:28 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 10:44:50 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 10:44:50 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 10:44:51 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 10:44:51 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 10:45:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 10:45:05 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 10:45:06 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 10:45:06 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 10:45:07 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 10:45:07 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 10:45:08 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 10:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 10:45:08 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 10:45:08 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:ffe4428ef008913a7ec63449e4ad3aa536b26103943146a302591dfceb157d2f`  
		Last Modified: Sat, 17 Jun 2017 18:08:13 GMT  
		Size: 2.0 MB (2045593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4fe786260f2bd2710289e7c9487b423cb252a691fa501759b0768516122869`  
		Last Modified: Wed, 25 Oct 2017 23:32:27 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cf0f0a132c9bb882206147dffad08dc780f2bc82556cfbda9878a3218f1e7c`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00a9186496c6602ccd3efb4bb1780b42adb7028c8fa3cd3c1ff2f10bcfa33a3`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 8.3 KB (8305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc19938c3bf2e858347a9c7add1beac38af5a4f83b99d80ddc004aa4ad51e596`  
		Last Modified: Thu, 26 Oct 2017 10:45:30 GMT  
		Size: 16.7 MB (16710838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697b9a0ea77c953a543f168ba09045ae412f3b2bd0947b2bba8c18cd0cd2c70b`  
		Last Modified: Thu, 26 Oct 2017 10:45:30 GMT  
		Size: 5.0 MB (5012335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca279d1203917e8f98e0d5fe3f9de9bdde74bae202990b6388e1cc748caa726`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb3c81d25b2aa6fa5bf57aaf5f8ad6a5f27be02727e454818ff546e5a989c88`  
		Last Modified: Thu, 26 Oct 2017 10:45:29 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420233201c5d7a33d69bc90b4ac40d5db1285e61718701ffd97d4db8396a9508`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0b37b1c6d397d7b0daa633cac4b2d202e9656dd6340dc40496303190ed4a78`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:2a7e105872a021c9e0df106fd62ee50b80be17634c3b713596ca188b8ab3cf04
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23639927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01e565612a099b2324e2f273a6a14a62e8cab609839bdeb205adc72571cb62b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:47 GMT
ADD file:e0be8616517d68cb80a2f9b74eb967cda22b9937bbcbe8b75b6153815a6f7761 in / 
# Wed, 25 Oct 2017 23:28:48 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:50 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 07:12:01 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 07:12:12 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 07:12:36 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 07:12:37 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 07:12:39 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 07:12:41 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 07:12:42 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 07:12:44 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 07:12:45 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 07:13:07 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 07:13:09 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 07:13:13 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 07:13:15 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 07:13:19 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 07:13:23 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 07:13:25 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 07:13:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 07:13:28 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 07:13:30 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:1e52418956f7d2a8ea35e8e6e3318fd08e005b27457d77868c225e7433bbfa02`  
		Last Modified: Thu, 20 Jul 2017 15:12:59 GMT  
		Size: 2.0 MB (2008578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf472f4e5bb7956ac20bb343b304e1d3de1f79160c0d158cccbe25980022d50`  
		Last Modified: Wed, 25 Oct 2017 23:29:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48c95ed960185dbd69324a206614e723f0086f80b46bd3223f233e4f1e278bc`  
		Last Modified: Thu, 26 Oct 2017 07:14:01 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a8242358db9adbde1a17b0e2b320c02112fcefa90d397ecc028a9729efcf94`  
		Last Modified: Thu, 26 Oct 2017 07:14:01 GMT  
		Size: 9.1 KB (9059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6db9581873eb0cadddc4d474e33cb2ec978c0d68e3ea124ce4f07ab2731d79`  
		Last Modified: Thu, 26 Oct 2017 07:14:04 GMT  
		Size: 16.6 MB (16603134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a991ac52f27ddaf9fb4021acf59b12957c4fa6251ab4d74159bb54ac63878009`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 5.0 MB (5013168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d098ea301752e2203c7ad872d2a38cc3da3efa183b01e61fe5c2fcde29efceb8`  
		Last Modified: Thu, 26 Oct 2017 07:14:00 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8727c952955dcfc3ce7e96c808c78bc91d43e6033164a46a7faffd11dc22fb69`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fe10e7f312fce5a9bf6ca051d683f86b1cef271217890a7ea53164ef81c99d`  
		Last Modified: Thu, 26 Oct 2017 07:13:58 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcba876c6e465f99a2952b71be993ce0d4d82ef4f70f72a59e58200cf263252f`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:85a850d9b872c722bace7014c60c183a5746e338d9136a8319c91c3d2fb6a778
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23818845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45af14c4c176512dfc8deb7275c6c333b0f5933fff4eab2e34c6d8f888d40be2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:40 GMT
ADD file:6fbdff4b4c08600e192f5da9b67a02c58759237fb40525d70712104c80c34c48 in / 
# Wed, 25 Oct 2017 23:28:40 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:40 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 17:06:39 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 17:06:42 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 17:06:55 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 17:06:56 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 17:06:57 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 17:06:57 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 17:07:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 17:07:05 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 17:07:06 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 17:07:06 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 17:07:06 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 17:07:07 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 17:07:07 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 17:07:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 17:07:08 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 17:07:08 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:d45fd9d3c4f188ab1f3a4bf6a9f5202b3f1577dbb998f5f28e82d192e0c1f0e7`  
		Last Modified: Sat, 17 Jun 2017 20:41:42 GMT  
		Size: 2.1 MB (2065460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5978b6b34b3e943e0fd25dfb50991c0bad82a986cfdaa91c4de756431ba679`  
		Last Modified: Wed, 25 Oct 2017 23:28:59 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299a1fbc19bbea84dbf4d0b6e2e71fb847299b017209b1f9783faea14214c995`  
		Last Modified: Thu, 26 Oct 2017 17:07:31 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb76f2dd4162cae82233bc93ba436b63ca37e536d53c85a9f1d7343203e3c383`  
		Last Modified: Thu, 26 Oct 2017 17:07:31 GMT  
		Size: 8.6 KB (8604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac09bb55706d627cf6348c9d0bd891c2fe9a4155aee5d95264b92781371021db`  
		Last Modified: Thu, 26 Oct 2017 17:07:33 GMT  
		Size: 16.7 MB (16726549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e776aa2eebd7dc068e74be7736114ce80966ab2b25478d29763bc1ccf05c3e3`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 5.0 MB (5012317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57d3128b93c0f42a41ad6b2571d41e61c6096e070ee18ef58d34aeaf7318560`  
		Last Modified: Thu, 26 Oct 2017 17:07:29 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484c70be68b7dc1296d1199834238ebabbde1df9ce04ec3cf986a2096ad218b6`  
		Last Modified: Thu, 26 Oct 2017 17:07:29 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01611bf6acbe11966a7f1fe2e96d811430328e24513c20237576287afdd5079a`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f045868d086334dbd06f276dfb93c084fc32b243827527e36c2bc5a5d8583d`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rabbitmq:3.6.12-management`

```console
$ docker pull rabbitmq@sha256:90b467d41e6655bb52d7114802c028eb359e220a7ec87c98a23a294af2b81ad4
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

### `rabbitmq:3.6.12-management` - linux; amd64

```console
$ docker pull rabbitmq@sha256:40a956f5198d4d2050d1545dc48bf38b5e0342c33d10bcd04c9e0a7e7bc851af
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.9 MB (62852369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ac724eab06670229b033f2516a2e3af2cdfb453495a9bbb040fea13b398ab5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:33:42 GMT
ADD file:45233d6b5c9b91e9437065d3e7c332d1c4eb4bce8e1079a4c1af342c450abe67 in / 
# Mon, 09 Oct 2017 21:33:43 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 02:41:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:41:43 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 02:41:43 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 02:42:10 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 02:42:40 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 02:42:41 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 02:42:42 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 02:43:16 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:43:16 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 02:43:17 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 02:43:17 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 02:43:18 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 02:43:19 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 13 Oct 2017 23:40:43 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 13 Oct 2017 23:40:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 13 Oct 2017 23:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2017 23:40:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 13 Oct 2017 23:40:45 GMT
CMD ["rabbitmq-server"]
# Fri, 13 Oct 2017 23:40:56 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 13 Oct 2017 23:40:57 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:bc95e04b23c06ba1b9bf092d07d1493177b218e0340bd2ed49dac351c1e34313`  
		Last Modified: Mon, 09 Oct 2017 21:42:28 GMT  
		Size: 22.5 MB (22492350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65f0b00e4cfb1535d0f4e7a63707172ae63483fb33140d777614f199afcb36`  
		Last Modified: Tue, 10 Oct 2017 02:43:59 GMT  
		Size: 4.5 MB (4498726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bd803179890909fcae186044c0e6ca1bc1d34e5fc05ef1ccea823e7be97540`  
		Last Modified: Tue, 10 Oct 2017 02:43:57 GMT  
		Size: 4.1 KB (4069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b05ca8302833edf783c50f03cd7ba0b8e12bc872b053eda3e3ae7e1f17e2b4b`  
		Last Modified: Tue, 10 Oct 2017 02:43:58 GMT  
		Size: 952.1 KB (952058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb5a4bbcce5a040eb83057f9e93d17663bb123f4e98168457444497f7d17b70`  
		Last Modified: Tue, 10 Oct 2017 02:44:03 GMT  
		Size: 27.7 MB (27703883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf840d8999f6fe46a162974c82378c38b3cf3dcccbbaff848c0fb199988aebe0`  
		Last Modified: Tue, 10 Oct 2017 02:44:00 GMT  
		Size: 7.2 MB (7194403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be339ca44883b1990e52771487402163d398a279755a501fdd8891ec71cf09d0`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce35cd9f9b5b917868095b3b074dd23d18e0e266f3ee68ff95e2c61467299812`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fe32a0a00d916ed4d632aae71d35d9d0baa5e5910d6bd179a24071c35bedb0`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77408ca9e94eb4bfeb346ab10c602857525802c2279e7c6995fcdbc90269444a`  
		Last Modified: Fri, 13 Oct 2017 23:41:26 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db03407a1aba1c0a89dffe960394aae639885702e3faa65271b918c36c7905cd`  
		Last Modified: Fri, 13 Oct 2017 23:41:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b908f008ac2afe6632caccd124e3ee9bffd5ebcdb8ca5ca84ae7e014305e460f`  
		Last Modified: Fri, 13 Oct 2017 23:42:01 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12-management` - linux; arm variant v5

```console
$ docker pull rabbitmq@sha256:07150eac8a231b8c043f29aba9a9ba3d81aa4cdd16c8e3387621deb4d8fdf1f4
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58432562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00088686092d95f6db193285835d1af5662557d679f57a4c21d1d4ec648c0924`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:44:48 GMT
ADD file:ff9945b48b1ac236dcec24eb9dfaf52b7c151a3b11c8502391f0866dfb4e3ac3 in / 
# Mon, 09 Oct 2017 21:44:48 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 00:18:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:18:11 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 00:18:11 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 00:18:29 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 00:18:58 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:18:58 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 00:18:58 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 00:19:26 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:19:26 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 00:19:27 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 00:19:28 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 00:19:29 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 00:19:30 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Sat, 14 Oct 2017 14:14:24 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Sat, 14 Oct 2017 14:14:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 14 Oct 2017 14:14:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 Oct 2017 14:14:25 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Sat, 14 Oct 2017 14:14:26 GMT
CMD ["rabbitmq-server"]
# Sat, 14 Oct 2017 14:14:34 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Sat, 14 Oct 2017 14:14:34 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:836d5b6056a9815be79c76480a90299267f60201bd1e3396817003e6c14819cc`  
		Last Modified: Mon, 09 Oct 2017 21:50:56 GMT  
		Size: 21.2 MB (21166251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb896fba83bd09a35c68457554b35289860c23c46f27a8c3ef42f13146ebba1`  
		Last Modified: Tue, 10 Oct 2017 00:20:01 GMT  
		Size: 4.2 MB (4231979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61827a16c114b9741d761aa4c60a972ffe1e0b60147794e86b05653d67822e91`  
		Last Modified: Tue, 10 Oct 2017 00:20:00 GMT  
		Size: 4.1 KB (4079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877cd9511def30e56a5ce354e145e8a2b1a93daaae7eaaa42dc4219838aa1743`  
		Last Modified: Tue, 10 Oct 2017 00:20:00 GMT  
		Size: 942.8 KB (942752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea9e378899e98c99e93ae2d0874bd5d89e24134bd14a19c285bdf39a0a42ade`  
		Last Modified: Tue, 10 Oct 2017 00:20:05 GMT  
		Size: 25.2 MB (25170810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc82a29314b16531aa2172ac523ba535e3678f85efdd699164fbb0241ab8b62`  
		Last Modified: Tue, 10 Oct 2017 00:20:01 GMT  
		Size: 6.9 MB (6909811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c44a3d016cf9de95021782180a42d3660e20fc7d8e92a7fe5ce9ede7928ca2`  
		Last Modified: Tue, 10 Oct 2017 00:19:59 GMT  
		Size: 2.3 KB (2261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abfdcdd98b40291ad91791bea09bf277e75c3669c6607c7891b09130101bfa3`  
		Last Modified: Tue, 10 Oct 2017 00:19:58 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a72811da4bf8ca8a2d06cdc182aa54116bb12133e8d82ef2b018a8de29ed74`  
		Last Modified: Tue, 10 Oct 2017 00:19:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147d8cf0897dea9b024bf5c6efb6873db3d86dec857fca062b146f88b7b5a735`  
		Last Modified: Sat, 14 Oct 2017 14:14:43 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f355fd0b70caedf30aa384298307b8e40d922e9e341492dd3fde71f119fd7d7`  
		Last Modified: Sat, 14 Oct 2017 14:14:44 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77dcaa76990445223000f8a5eb10485f94e82d4817f74f142f106b0a4dd9ad0c`  
		Last Modified: Sat, 14 Oct 2017 14:15:02 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12-management` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:353fc3a4b10cc0fd93baf80287c8e7c779c49d7fd5421091aa004286b3bf559c
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55688342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd5c488f599ef650e2dc6824d489473db268160f94789b74f5ec312eef58600d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:43 GMT
ADD file:b758c6c3ff989778bd740dde35c86b953fa09be913a7e02711b2881de6b8911d in / 
# Mon, 09 Oct 2017 21:45:44 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 13:07:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:07:42 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 13:07:42 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 13:07:58 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 13:08:17 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:08:17 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 13:08:17 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 13:08:39 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:08:39 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 13:08:40 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 13:08:41 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 13:08:42 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 13:08:43 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 13:08:43 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 13:08:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 13:08:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 13:08:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 13:08:45 GMT
CMD ["rabbitmq-server"]
# Fri, 03 Nov 2017 13:09:01 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 03 Nov 2017 13:09:01 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:59e81a3fde58ec8d4b8f2f58b98ef2f4d951d37dd9b99b016fd294a8e07d7796`  
		Last Modified: Mon, 09 Oct 2017 21:52:49 GMT  
		Size: 19.3 MB (19277135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2037b99f3c3dc51e8ace39aed9971155f34f325ac4f0a1e56a07c4d6c02f5ae6`  
		Last Modified: Fri, 03 Nov 2017 13:09:18 GMT  
		Size: 3.9 MB (3868347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f368172ea96bda944832762ad29b52dfe17ec5e6fae96eee37adc4e9d68674a5`  
		Last Modified: Fri, 03 Nov 2017 13:09:16 GMT  
		Size: 4.1 KB (4084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893cc1ae60f8bf72ac3020ccc60b22d9e0ad0cb0647e15bc4847d08c8985eee2`  
		Last Modified: Fri, 03 Nov 2017 13:09:16 GMT  
		Size: 926.1 KB (926097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13220cc1a683014bda9cfae7f7ee7015a26b28048f90f5aa3ed8b6a96f4b2813`  
		Last Modified: Fri, 03 Nov 2017 13:09:20 GMT  
		Size: 24.8 MB (24785610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269f4e069126132643c1c0be1faf600d55ff15e870066c527d03181904d99c5d`  
		Last Modified: Fri, 03 Nov 2017 13:09:17 GMT  
		Size: 6.8 MB (6820180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ae244f4f610a339fcbddf37612a15ec7b7f6674e3d888c3c4d36302283418e`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce7d85327b7bc7d59a7b54222a3e6babd7f8afd8eb080becb77fc52aed5a751`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dfa32e4b49700ed0130ebd563f40a2c381393983b571a9886435813102ad0c`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba15cd885dc21f438d366b40d0d9f595f2c25e063c60fa590ab4c0f6233ff94`  
		Last Modified: Fri, 03 Nov 2017 13:09:14 GMT  
		Size: 4.0 KB (4040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978a8434497fcb8e08cefc7484b515ac34fe23c281fb869d015f62b54673028c`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34fa59eaf946f8e35134f1a0bf195874868c3ce1e2a025350fc57efe60ecbea`  
		Last Modified: Fri, 03 Nov 2017 13:09:54 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12-management` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:4ad104ab7b291ca9aea4bb42e18de213ae21ef6a655d909c3568e2b36f465074
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57278563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9356e7f3d3e445f04242803fb4b5afb70fad5f726388635b781f4814733c3af7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:47:55 GMT
ADD file:3a528355cfc75437716aff3b517ef99ae602918d84d26dbafff0ed142248fb93 in / 
# Mon, 09 Oct 2017 21:47:56 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 04:57:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 04:57:04 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 04:57:05 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 04:57:37 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 04:58:35 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 04:58:36 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 04:58:37 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 04:58:37 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 04:58:38 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 04:58:39 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 04:58:39 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 05:00:22 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 05:00:23 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 05:00:25 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 05:00:26 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 05:00:28 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 05:00:31 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Sat, 14 Oct 2017 13:52:47 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Sat, 14 Oct 2017 13:52:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 14 Oct 2017 13:52:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 Oct 2017 13:52:51 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Sat, 14 Oct 2017 13:52:51 GMT
CMD ["rabbitmq-server"]
# Sat, 14 Oct 2017 13:53:08 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Sat, 14 Oct 2017 13:53:09 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:e907afd6e25615a4d3eb554d930cef57b87e79ec82413889c2eac38beb4eb8f7`  
		Last Modified: Mon, 09 Oct 2017 22:03:08 GMT  
		Size: 20.3 MB (20337143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5e6d35928560b933b85b5a3f2a8e96b4520fbb8df138b3e739e56d0c1f355`  
		Last Modified: Tue, 10 Oct 2017 05:01:18 GMT  
		Size: 4.1 MB (4073554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a862ab821b342790326492507ca5d70bfb7016bef765606193f1f7139f60c5ed`  
		Last Modified: Tue, 10 Oct 2017 05:01:14 GMT  
		Size: 4.1 KB (4072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92799a54920b79013733790e444f13d8c65faa29c79cbdaf1bc8af85f637a233`  
		Last Modified: Tue, 10 Oct 2017 05:01:14 GMT  
		Size: 919.5 KB (919487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b119999eef1bcadabedd3a5319b03c6b83ede91ba8535059851547d3433b205`  
		Last Modified: Tue, 10 Oct 2017 05:01:19 GMT  
		Size: 25.0 MB (25042572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62f8525a3a982a102aa37bb3313876195b15d8781cd253ed238dd2b9dff151`  
		Last Modified: Tue, 10 Oct 2017 05:01:15 GMT  
		Size: 6.9 MB (6894852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc028e70f04f6ea4365223a1cfe4e5c4384d5921acac419f3c170b148f7c7bf`  
		Last Modified: Tue, 10 Oct 2017 05:01:10 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e99faa03c2a8a272f56208c644c12b384b69dea50be6da9f6be400c14b945c`  
		Last Modified: Tue, 10 Oct 2017 05:01:12 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8fa260bcaa52d81ba20c11111f8d15bab954b17b48666724536c604220d94e`  
		Last Modified: Tue, 10 Oct 2017 05:01:11 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306840de948d03472918a306c089409429606802ec8cf841e96dec707a2f7178`  
		Last Modified: Sat, 14 Oct 2017 13:53:27 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a7a978032478b38adb1f0107466d187e53380f7037d058c62e4937cd07fc09`  
		Last Modified: Sat, 14 Oct 2017 13:53:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3facaa930064fd14fbd9a077b63e5f3261d1e63bd15c3d1426575c6c4f8eca`  
		Last Modified: Sat, 14 Oct 2017 13:54:17 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12-management` - linux; 386

```console
$ docker pull rabbitmq@sha256:16ab1fd6ebf60e7fe32149ac86bf79cd5a2e2d573dec3267fd0d7d646514384c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63902453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a8039a2961a84491da6ac62bad7d9b065b333750e66543f8e7cf931c13ed028`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:36 GMT
ADD file:6582536277127947668f7bfdc1471a4e36170915b91a4cb841e7e1bfa1de6535 in / 
# Mon, 09 Oct 2017 21:45:36 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 10:45:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:45:12 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 10:45:13 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 10:45:28 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 10:46:03 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 10:46:04 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 10:46:25 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:46:25 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 10:46:26 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 10:46:27 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 10:46:27 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 10:46:28 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 10:46:28 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 10:46:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 10:46:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 10:46:30 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 10:46:30 GMT
CMD ["rabbitmq-server"]
# Fri, 03 Nov 2017 10:46:58 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 03 Nov 2017 10:46:58 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:b2b52fe46b29fe5d0689f26449c2114e40f0731d4ce3eb8c3941397b74205432`  
		Last Modified: Mon, 09 Oct 2017 21:53:42 GMT  
		Size: 23.1 MB (23128678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d407b136da0731f5f38279001e9dd426217937443cad0f16e1f242366290773`  
		Last Modified: Fri, 03 Nov 2017 10:47:13 GMT  
		Size: 4.8 MB (4803637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c93817e78345b4b5070c81e5a37d02afc2b5fe347a1a4bf59e09f6084814fd2`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 4.1 KB (4057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97eae59c75f8f814ab781f5239ac2e132b7b65c77e75b35023c603c539ca54f`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 931.5 KB (931524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aed670dee19fde6946658d7129e13520c1a0747f8b80b6f92dac5f6d974ae52`  
		Last Modified: Fri, 03 Nov 2017 10:47:24 GMT  
		Size: 27.8 MB (27818690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b61d6d0b60ec18280aeba946a05d62817afbe030f277af85b5f434021e90c9`  
		Last Modified: Fri, 03 Nov 2017 10:47:16 GMT  
		Size: 7.2 MB (7208985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec7d4cc3b5497bbbd6b2d1e9574dbedb6c7ad11805cff4c287ea444ddc2e298`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 2.3 KB (2259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eec554591344f78e35e3976d002d617623a52d123fc71e65d33c4d533d2b2e7`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e433f73af1167eff0dee1984c095bf5be36593fcead5b8cc820e2cb829aaed0`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8d6e0dbdbb04b44f7a0972fce6b0b1b19262e4fc5416bd1589af560f16c99f`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 4.0 KB (4040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bab08cf9b00d8109139e1cb1cdec448b71fdae7d7f1260d4175771416a5f80`  
		Last Modified: Fri, 03 Nov 2017 10:47:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2aad62bc4e7f6b9b68a5196e492b29083b8ab4e68dfea4a93b469cb79aae29`  
		Last Modified: Fri, 03 Nov 2017 10:48:04 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12-management` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:47fb5bf4afd56afb9e9ab383f1449cee19c3ab7a7e653d0b04037cf839cfab52
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60384672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c4dbfbbd301b5dbb171ca49da8419b76567c7aa2d00978e12759ced95ca846`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:56 GMT
ADD file:7edf73437495be24244c16841b563be06c15452963f41ac940fb5e105ed96027 in / 
# Mon, 09 Oct 2017 21:45:58 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 07:12:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:12:51 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 07:12:53 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 07:13:49 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 07:15:26 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:15:28 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 07:15:29 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 07:15:31 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 07:15:33 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 07:15:34 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 07:15:35 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 07:16:54 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:16:55 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 07:17:00 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 07:17:01 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 07:17:06 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 07:17:11 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 07:17:13 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 07:17:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 07:17:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 07:17:21 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 07:17:23 GMT
CMD ["rabbitmq-server"]
# Fri, 03 Nov 2017 07:17:36 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 03 Nov 2017 07:17:39 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:c4860466fa1e6824151f4fa3a51ef0e9d7d3c3ba860e21d94e69988b65601260`  
		Last Modified: Mon, 09 Oct 2017 21:52:59 GMT  
		Size: 22.7 MB (22746217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebe4c87dcd1f7ef11d4d21752831bf4095ac42afe041706c35f1d7d4d0ca4f2`  
		Last Modified: Fri, 03 Nov 2017 07:18:05 GMT  
		Size: 4.4 MB (4360529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e5365525084de1c85fa29ef33d37c38b5f80621f5bcb26bb4882d71598c6f7`  
		Last Modified: Fri, 03 Nov 2017 07:18:03 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600c3853740b7f4cff9cc799ae478f669bd54277a8dd375479a34ed1bb47a803`  
		Last Modified: Fri, 03 Nov 2017 07:18:02 GMT  
		Size: 920.7 KB (920695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993868ec534130e348e45aa6d64b471fa46eafbf061836cc9d2a56edf73e9382`  
		Last Modified: Fri, 03 Nov 2017 07:18:06 GMT  
		Size: 25.5 MB (25492533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca1b92e212aaef163244d5fdd9e135fdb8be8c9dbbb626061ee2882d941a553`  
		Last Modified: Fri, 03 Nov 2017 07:18:03 GMT  
		Size: 6.9 MB (6853702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483f96d1f500f9f69170bc6927d599a7f0cd1550f96b6ee3f90eb4185a1bffb`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b433db63f40c7cab3080cf36bd7beabbdf7d9eece3f2dc16a65b900c61180`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93971551a2c911c34ca2e9af47495efb2f27e2922e567d93dd94dfb9b773bd3`  
		Last Modified: Fri, 03 Nov 2017 07:17:58 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5494bb8bcc45452a84c216edffedb3103a15c3e209aba0561dfbc70e4312192e`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 4.0 KB (4039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d56b2a4f9f8d7b11831a8f1952fe2c02613bcb014ab9d756b70b3b398b37269`  
		Last Modified: Fri, 03 Nov 2017 07:17:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e2264063017ef705c9dcc066695ab771b32f19f38ba34c158531e7d3f4c9fc`  
		Last Modified: Fri, 03 Nov 2017 07:18:40 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12-management` - linux; s390x

```console
$ docker pull rabbitmq@sha256:35d9ecb54b432f7591ecfe0cb1ee71d152199b0ae07ecdd8c9b21cd6a87b0a51
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60364970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a628fac494ad4d163ad91471c151b4ed5bcfbe2f318bc677224413d944cf4ce8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:44:35 GMT
ADD file:ae4aaa6affe22f36ab5478771d5c84917f72de7a8dac16345a035709a1a5edf4 in / 
# Mon, 09 Oct 2017 21:44:36 GMT
CMD ["bash"]
# Thu, 02 Nov 2017 17:06:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 17:06:41 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Thu, 02 Nov 2017 17:06:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 02 Nov 2017 17:07:21 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Thu, 02 Nov 2017 17:07:43 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 02 Nov 2017 17:07:44 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 02 Nov 2017 17:07:45 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 17:07:48 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 17:07:48 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 17:07:49 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 17:07:50 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 17:07:52 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 17:07:53 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 17:07:54 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 17:07:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 17:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 17:07:57 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 17:07:57 GMT
CMD ["rabbitmq-server"]
# Fri, 03 Nov 2017 17:08:14 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 03 Nov 2017 17:08:15 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:671716cc49517eef5f430c695ce344d63e390cb65f58d30939f2ba615c953686`  
		Last Modified: Mon, 09 Oct 2017 21:49:09 GMT  
		Size: 22.3 MB (22339951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cae61f12be6f01ba06573d9393712e91821cd5496302310f550fe5842dea557`  
		Last Modified: Fri, 03 Nov 2017 17:08:41 GMT  
		Size: 4.5 MB (4529879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca307103ce923e7e89d35185be4df8e54c3c0b54d259b8880aa7bae107d4952`  
		Last Modified: Fri, 03 Nov 2017 17:08:39 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d16320f9fc35ea20ba7fb9b21f88e3f0f06c52d416682319f3b2a85a345a3d5`  
		Last Modified: Fri, 03 Nov 2017 17:08:39 GMT  
		Size: 938.0 KB (938019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801205b182b8d6f7acf36200b2ba07ed52ea224dfefe792b525224e4aacb4d4a`  
		Last Modified: Fri, 03 Nov 2017 17:08:48 GMT  
		Size: 25.6 MB (25619372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9cb605e6242f5ab505cbd229c7b2fdf2935a6254130070c12c4d8413616024`  
		Last Modified: Fri, 03 Nov 2017 17:08:40 GMT  
		Size: 6.9 MB (6926791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2799e1b1479136fbb3c3ba6df318d449990a3cf5fc3293a14142cde0d9f51980`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a6d5de3e6aaa1c06122a1b5cda3b4bcb98d54e5dc23f38896fc81e98cea769`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172fa2e52818dcedf69c727f6790f0f9744f8538da3f4222602aaa0ab9fa82c0`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c734f2707800c1189521a51409fed1508fb7e36c6e67eca5537d03c4b24ef0d`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 4.0 KB (4037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e7d712f1155d66243480cd441ec04e084a8e7e2d6a0653e27138b31b56d2ae`  
		Last Modified: Fri, 03 Nov 2017 17:08:38 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9489f6c1d1f9d4090b7d9220b20aac5cc7e9588c9ddf66d0357f1eb8226071`  
		Last Modified: Fri, 03 Nov 2017 17:09:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rabbitmq:3.6.12-management-alpine`

```console
$ docker pull rabbitmq@sha256:cc6bb38a4167c70483b6f174d43bf43032a23b1d9c661530cfda228bf60e3f87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `rabbitmq:3.6.12-management-alpine` - linux; amd64

```console
$ docker pull rabbitmq@sha256:ef2b9b2cbfbe00330d8cfaaf8acef1127996756ee66bad0ac832aba8e63ae67f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23579858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4927e0fd02a40ab3ffc333a1326f9a21be7aec9059d82c2dfdc37580847a76f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:19:51 GMT
ADD file:1e87ff33d1b6765b793888cd50e01b2bd0dfe152b7dbb4048008bfc2658faea7 in / 
# Wed, 25 Oct 2017 23:19:51 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 03:02:21 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 03:02:25 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 03:02:32 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 03:02:32 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 03:02:33 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 03:02:33 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 03:02:42 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 03:02:42 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 03:02:43 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 03:02:43 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 03:02:44 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 03:02:44 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 03:02:45 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 03:02:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 03:02:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 03:02:45 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 03:02:59 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 03:02:59 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:b56ae66c29370df48e7377c8f9baa744a3958058a766793f821dadcb144a4647`  
		Last Modified: Wed, 25 Oct 2017 23:21:25 GMT  
		Size: 2.0 MB (1991435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827e0bce86e3c8fa677ac91f0c55a7a4071cc45c729b171aecbe04d35ae160d7`  
		Last Modified: Thu, 26 Oct 2017 03:03:23 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe01d115cb92dc0ab37de6b6ffa2073ea20d30dfc49c537fbba569cd6a494b8`  
		Last Modified: Thu, 26 Oct 2017 03:03:23 GMT  
		Size: 8.2 KB (8176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bfc0dbbf8b1d2f532779c4873b4c7e0237d6ecc86161b1c6f28e3b6bd3149f`  
		Last Modified: Thu, 26 Oct 2017 03:03:26 GMT  
		Size: 16.6 MB (16561644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b24f4fd26b3494d310561a28e2d9aeb08e7baba442eaef2cd8697c7ebd9d9f1`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 5.0 MB (5012671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfb0f3b402f9674b21d7ed079f6576ec1be80f333f41c404e8ce3feb193b813`  
		Last Modified: Thu, 26 Oct 2017 03:03:22 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521b2b4b2311f153d53f0b9bde9a164f45df9dfd531512c36195ba2ccf5a4c76`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cedbb525e85f1b9257e8b20d04b4ad39f1004c9dfbc673086815dd887f380c3`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f35995cc5f5daa05334d17a87482ac8728aadfb0f10f9d62b3d70f5986e5cc`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f1f0f842cbbd9046d7b95afc926b8e22e4befd18e38ed5d4514e14105d2be`  
		Last Modified: Thu, 26 Oct 2017 03:04:25 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12-management-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:e8e0295fdf1734258af64b4f82784721e845b6a68146965bd1592c0e15c58d1a
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23413037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1379abcce7a4a22ec254dfd3fe56547de4c89c0b12cfaf5e044ea05c4205dfb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:35 GMT
ADD file:009348222efb3c4ca2e53c387fb34c488679ca07db39525a6c5cc214e46abffd in / 
# Wed, 25 Oct 2017 23:28:36 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:36 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 05:25:53 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 05:25:55 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 05:26:10 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 05:26:10 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 05:26:10 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 05:26:11 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 05:26:19 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 05:26:19 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 05:26:20 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 05:26:20 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 05:26:21 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 05:26:22 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 05:26:22 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 05:26:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 05:26:22 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 05:26:23 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 05:26:30 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 05:26:30 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:0864efeeb5cb8dca4eb53e5d6fd38486daee80fa326fe36d1ad254f8fa6bb310`  
		Last Modified: Sun, 23 Jul 2017 20:21:42 GMT  
		Size: 2.0 MB (1965988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda69762aee1588fa82aeabf1af6d6ad24f737cce1451fab2e0199849b1e12e`  
		Last Modified: Wed, 25 Oct 2017 23:28:45 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62a8c5580cc1c2fbf2f9ce119bc0c06403a12ad18167bde2ec94420810916db`  
		Last Modified: Thu, 26 Oct 2017 05:26:38 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b096e39434b5aeddcb2ec167b7bf570cac7b8b16e68324d3f46c6f4d41b69c79`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 8.4 KB (8374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ad9273316fa6f22cd2e8cf88c92f34c3210325fa1be2041153a96f4124476f`  
		Last Modified: Thu, 26 Oct 2017 05:26:41 GMT  
		Size: 16.4 MB (16420180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed982c9e7d5644c85267595b470c0f21f25093a865603ab33304248efdb68b5d`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 5.0 MB (5012332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b76830a9cb5b5f898068945d6af6325c7d97b36d50e521a12097d3e908fd0`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a31f9ee2285379d9d5106926e707698e7a3283f707a4573fec9731e6ede58b5`  
		Last Modified: Thu, 26 Oct 2017 05:26:36 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff38544dc85623170156958b2d5d51604efd94b336b47a6479cde0417667838f`  
		Last Modified: Thu, 26 Oct 2017 05:26:36 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564bee8c5f497342e71777f1adc38d1578f7c95ddefe18efa16fc01b3e7e2a52`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fe4d4545d22113e1fa0e2fbc7ae69364213b6ca264274a71ad66ac045835d1`  
		Last Modified: Thu, 26 Oct 2017 05:26:49 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12-management-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:bf020d55089aa6f03eb3e259eefa2014a2191041616b46f4c7e56fd10fd09b76
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23318349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67e8f6bc203146953e13d3ce7086f40a6796ae711f8d8231aac5693d99175f9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:58 GMT
ADD file:45b5d3b8d5490ba7edfca2cf6f54cdcf49c772b0b3a2302ce69a7af061007aa4 in / 
# Wed, 25 Oct 2017 23:28:59 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:59 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 13:53:09 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 13:53:13 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 13:53:28 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 13:53:28 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 13:53:29 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 13:53:29 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 13:53:30 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 13:53:30 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 13:53:31 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 13:54:22 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 13:54:23 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 13:54:24 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 13:54:25 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 13:54:26 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 13:54:28 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 13:54:29 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 13:54:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 13:54:30 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 13:54:30 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 13:54:47 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 13:54:47 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:bb473f0ebc12fde1bd45c1bd3c46f2d3aab367b1b7739464771455b9972f7894`  
		Last Modified: Thu, 06 Jul 2017 09:54:42 GMT  
		Size: 1.9 MB (1914748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ff6b7ff3a208b8399e701e7ea1b7edbdc654c8c60d33c6f09a7803e2dda776`  
		Last Modified: Wed, 25 Oct 2017 23:29:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05834eac152e30997eb4f1aa4ffe8e952bd759c1a1009bd183dec80dca24cf86`  
		Last Modified: Thu, 26 Oct 2017 13:55:11 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd88a23486b40755f2e1192cb35d4fdaec20831c18ce83da31df3f8aa2f7b45c`  
		Last Modified: Thu, 26 Oct 2017 13:55:11 GMT  
		Size: 8.3 KB (8297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f9ba1206e6e4bfba21cef7f235482b41868ec966d5ebc44a4c4ac432a5fe03`  
		Last Modified: Thu, 26 Oct 2017 13:55:16 GMT  
		Size: 16.4 MB (16376872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5991837e23d785829d605fd052c61e10ed79a7cfb0dfee9dd40d6144bc9fad0f`  
		Last Modified: Thu, 26 Oct 2017 13:55:12 GMT  
		Size: 5.0 MB (5012322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf5663fa552ede671fc5ebf425b2ce3ff5257636b55df9564e556fe7ff85fce`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794d04d767a60fa6df4adb3af1f835701a3c2692e7f6b2d4a9db621a0bc8cd5f`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91155b0cb6bf92d1ab05fb7d13593e0a966eb79dd4e4173e3895d98dffe1c996`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969bbed547aa67091daaa801a46b062fd1c39f7835c81dd5052032056b6cf230`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1643075e82e89fd6745e0baa4b9fd436da4f959fffedec9f0d149f84a7c16f8f`  
		Last Modified: Thu, 26 Oct 2017 13:56:10 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12-management-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:775482d2d2f81b04a7f91840ed0a169b185315f4dc226d515adaacb675e6f6dc
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23783181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:845026f49dc450aaf8e569e45ba76c8b1bf506da17e742b0a54fbddaf5bcf9f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:32:08 GMT
ADD file:4a952fc4b81d50b342e26a818dac48a148a4d5eddb878219650e579a5c9faeaa in / 
# Wed, 25 Oct 2017 23:32:08 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:32:08 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 10:44:24 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 10:44:28 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 10:44:50 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 10:44:50 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 10:44:51 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 10:44:51 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 10:45:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 10:45:05 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 10:45:06 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 10:45:06 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 10:45:07 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 10:45:07 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 10:45:08 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 10:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 10:45:08 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 10:45:08 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 10:45:16 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 10:45:16 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:ffe4428ef008913a7ec63449e4ad3aa536b26103943146a302591dfceb157d2f`  
		Last Modified: Sat, 17 Jun 2017 18:08:13 GMT  
		Size: 2.0 MB (2045593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4fe786260f2bd2710289e7c9487b423cb252a691fa501759b0768516122869`  
		Last Modified: Wed, 25 Oct 2017 23:32:27 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cf0f0a132c9bb882206147dffad08dc780f2bc82556cfbda9878a3218f1e7c`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00a9186496c6602ccd3efb4bb1780b42adb7028c8fa3cd3c1ff2f10bcfa33a3`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 8.3 KB (8305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc19938c3bf2e858347a9c7add1beac38af5a4f83b99d80ddc004aa4ad51e596`  
		Last Modified: Thu, 26 Oct 2017 10:45:30 GMT  
		Size: 16.7 MB (16710838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697b9a0ea77c953a543f168ba09045ae412f3b2bd0947b2bba8c18cd0cd2c70b`  
		Last Modified: Thu, 26 Oct 2017 10:45:30 GMT  
		Size: 5.0 MB (5012335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca279d1203917e8f98e0d5fe3f9de9bdde74bae202990b6388e1cc748caa726`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb3c81d25b2aa6fa5bf57aaf5f8ad6a5f27be02727e454818ff546e5a989c88`  
		Last Modified: Thu, 26 Oct 2017 10:45:29 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420233201c5d7a33d69bc90b4ac40d5db1285e61718701ffd97d4db8396a9508`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0b37b1c6d397d7b0daa633cac4b2d202e9656dd6340dc40496303190ed4a78`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b719c08f02439306e8baee89f388d47a99542fc0eec294aaf615c425ec5253de`  
		Last Modified: Thu, 26 Oct 2017 10:45:59 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12-management-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:1f2ed16a80e1b71fd652fe7520fa1ba2ac5c9b5a207199bc7aaec39c61d5a38e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23640124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0244f72e17b275644966d172a75c7023650024e2761d2541020cbb3592bd01f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:47 GMT
ADD file:e0be8616517d68cb80a2f9b74eb967cda22b9937bbcbe8b75b6153815a6f7761 in / 
# Wed, 25 Oct 2017 23:28:48 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:50 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 07:12:01 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 07:12:12 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 07:12:36 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 07:12:37 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 07:12:39 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 07:12:41 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 07:12:42 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 07:12:44 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 07:12:45 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 07:13:07 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 07:13:09 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 07:13:13 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 07:13:15 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 07:13:19 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 07:13:23 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 07:13:25 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 07:13:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 07:13:28 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 07:13:30 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 07:13:42 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 07:13:44 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:1e52418956f7d2a8ea35e8e6e3318fd08e005b27457d77868c225e7433bbfa02`  
		Last Modified: Thu, 20 Jul 2017 15:12:59 GMT  
		Size: 2.0 MB (2008578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf472f4e5bb7956ac20bb343b304e1d3de1f79160c0d158cccbe25980022d50`  
		Last Modified: Wed, 25 Oct 2017 23:29:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48c95ed960185dbd69324a206614e723f0086f80b46bd3223f233e4f1e278bc`  
		Last Modified: Thu, 26 Oct 2017 07:14:01 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a8242358db9adbde1a17b0e2b320c02112fcefa90d397ecc028a9729efcf94`  
		Last Modified: Thu, 26 Oct 2017 07:14:01 GMT  
		Size: 9.1 KB (9059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6db9581873eb0cadddc4d474e33cb2ec978c0d68e3ea124ce4f07ab2731d79`  
		Last Modified: Thu, 26 Oct 2017 07:14:04 GMT  
		Size: 16.6 MB (16603134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a991ac52f27ddaf9fb4021acf59b12957c4fa6251ab4d74159bb54ac63878009`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 5.0 MB (5013168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d098ea301752e2203c7ad872d2a38cc3da3efa183b01e61fe5c2fcde29efceb8`  
		Last Modified: Thu, 26 Oct 2017 07:14:00 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8727c952955dcfc3ce7e96c808c78bc91d43e6033164a46a7faffd11dc22fb69`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fe10e7f312fce5a9bf6ca051d683f86b1cef271217890a7ea53164ef81c99d`  
		Last Modified: Thu, 26 Oct 2017 07:13:58 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcba876c6e465f99a2952b71be993ce0d4d82ef4f70f72a59e58200cf263252f`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d8f64c426c0a1bf9de5b158513294037721b7e6c1c4fbc5e75f84a63743aae`  
		Last Modified: Thu, 26 Oct 2017 07:14:31 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6.12-management-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:4af0a8312682b92651de05ff83aac54b00b55118b9babda060c043b4fdf9609b
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23819037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b62c33cd033388e2676822a15081284e991d3078ed4b51ebab5b72b7cb5a983`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:40 GMT
ADD file:6fbdff4b4c08600e192f5da9b67a02c58759237fb40525d70712104c80c34c48 in / 
# Wed, 25 Oct 2017 23:28:40 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:40 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 17:06:39 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 17:06:42 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 17:06:55 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 17:06:56 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 17:06:57 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 17:06:57 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 17:07:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 17:07:05 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 17:07:06 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 17:07:06 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 17:07:06 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 17:07:07 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 17:07:07 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 17:07:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 17:07:08 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 17:07:08 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 17:07:19 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 17:07:19 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:d45fd9d3c4f188ab1f3a4bf6a9f5202b3f1577dbb998f5f28e82d192e0c1f0e7`  
		Last Modified: Sat, 17 Jun 2017 20:41:42 GMT  
		Size: 2.1 MB (2065460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5978b6b34b3e943e0fd25dfb50991c0bad82a986cfdaa91c4de756431ba679`  
		Last Modified: Wed, 25 Oct 2017 23:28:59 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299a1fbc19bbea84dbf4d0b6e2e71fb847299b017209b1f9783faea14214c995`  
		Last Modified: Thu, 26 Oct 2017 17:07:31 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb76f2dd4162cae82233bc93ba436b63ca37e536d53c85a9f1d7343203e3c383`  
		Last Modified: Thu, 26 Oct 2017 17:07:31 GMT  
		Size: 8.6 KB (8604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac09bb55706d627cf6348c9d0bd891c2fe9a4155aee5d95264b92781371021db`  
		Last Modified: Thu, 26 Oct 2017 17:07:33 GMT  
		Size: 16.7 MB (16726549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e776aa2eebd7dc068e74be7736114ce80966ab2b25478d29763bc1ccf05c3e3`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 5.0 MB (5012317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57d3128b93c0f42a41ad6b2571d41e61c6096e070ee18ef58d34aeaf7318560`  
		Last Modified: Thu, 26 Oct 2017 17:07:29 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484c70be68b7dc1296d1199834238ebabbde1df9ce04ec3cf986a2096ad218b6`  
		Last Modified: Thu, 26 Oct 2017 17:07:29 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01611bf6acbe11966a7f1fe2e96d811430328e24513c20237576287afdd5079a`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f045868d086334dbd06f276dfb93c084fc32b243827527e36c2bc5a5d8583d`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed30107b153ffda65732449b2eea0bdac7dbd4327b3a82ef0fcd5553b0ca55fc`  
		Last Modified: Thu, 26 Oct 2017 17:07:50 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rabbitmq:3.6-alpine`

```console
$ docker pull rabbitmq@sha256:e49288ac5376cbd8699e6dd2d99410ce12ecd1a5f8885b9f8a1eebd863e3b4ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `rabbitmq:3.6-alpine` - linux; amd64

```console
$ docker pull rabbitmq@sha256:f8204cb30a089ec4fa99d41ed68f1b520670f5698bea479f6a6582d1926a5715
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23579666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:210310494165d259279503b1b25ecd975f73320e177d472300069bc8619908be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:19:51 GMT
ADD file:1e87ff33d1b6765b793888cd50e01b2bd0dfe152b7dbb4048008bfc2658faea7 in / 
# Wed, 25 Oct 2017 23:19:51 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 03:02:21 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 03:02:25 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 03:02:32 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 03:02:32 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 03:02:33 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 03:02:33 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 03:02:42 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 03:02:42 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 03:02:43 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 03:02:43 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 03:02:44 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 03:02:44 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 03:02:45 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 03:02:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 03:02:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 03:02:45 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:b56ae66c29370df48e7377c8f9baa744a3958058a766793f821dadcb144a4647`  
		Last Modified: Wed, 25 Oct 2017 23:21:25 GMT  
		Size: 2.0 MB (1991435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827e0bce86e3c8fa677ac91f0c55a7a4071cc45c729b171aecbe04d35ae160d7`  
		Last Modified: Thu, 26 Oct 2017 03:03:23 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe01d115cb92dc0ab37de6b6ffa2073ea20d30dfc49c537fbba569cd6a494b8`  
		Last Modified: Thu, 26 Oct 2017 03:03:23 GMT  
		Size: 8.2 KB (8176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bfc0dbbf8b1d2f532779c4873b4c7e0237d6ecc86161b1c6f28e3b6bd3149f`  
		Last Modified: Thu, 26 Oct 2017 03:03:26 GMT  
		Size: 16.6 MB (16561644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b24f4fd26b3494d310561a28e2d9aeb08e7baba442eaef2cd8697c7ebd9d9f1`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 5.0 MB (5012671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfb0f3b402f9674b21d7ed079f6576ec1be80f333f41c404e8ce3feb193b813`  
		Last Modified: Thu, 26 Oct 2017 03:03:22 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521b2b4b2311f153d53f0b9bde9a164f45df9dfd531512c36195ba2ccf5a4c76`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cedbb525e85f1b9257e8b20d04b4ad39f1004c9dfbc673086815dd887f380c3`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f35995cc5f5daa05334d17a87482ac8728aadfb0f10f9d62b3d70f5986e5cc`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:9bbc37dee4951514ff22f2fc83eed327e4fb935baedc146be69d4b7bd04b40b6
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23412846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d5e63a3df176d84fe8622b7515aa144197643b1a5ac6fc5b1578c6d78fb121c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:35 GMT
ADD file:009348222efb3c4ca2e53c387fb34c488679ca07db39525a6c5cc214e46abffd in / 
# Wed, 25 Oct 2017 23:28:36 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:36 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 05:25:53 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 05:25:55 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 05:26:10 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 05:26:10 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 05:26:10 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 05:26:11 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 05:26:19 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 05:26:19 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 05:26:20 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 05:26:20 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 05:26:21 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 05:26:22 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 05:26:22 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 05:26:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 05:26:22 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 05:26:23 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:0864efeeb5cb8dca4eb53e5d6fd38486daee80fa326fe36d1ad254f8fa6bb310`  
		Last Modified: Sun, 23 Jul 2017 20:21:42 GMT  
		Size: 2.0 MB (1965988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda69762aee1588fa82aeabf1af6d6ad24f737cce1451fab2e0199849b1e12e`  
		Last Modified: Wed, 25 Oct 2017 23:28:45 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62a8c5580cc1c2fbf2f9ce119bc0c06403a12ad18167bde2ec94420810916db`  
		Last Modified: Thu, 26 Oct 2017 05:26:38 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b096e39434b5aeddcb2ec167b7bf570cac7b8b16e68324d3f46c6f4d41b69c79`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 8.4 KB (8374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ad9273316fa6f22cd2e8cf88c92f34c3210325fa1be2041153a96f4124476f`  
		Last Modified: Thu, 26 Oct 2017 05:26:41 GMT  
		Size: 16.4 MB (16420180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed982c9e7d5644c85267595b470c0f21f25093a865603ab33304248efdb68b5d`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 5.0 MB (5012332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b76830a9cb5b5f898068945d6af6325c7d97b36d50e521a12097d3e908fd0`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a31f9ee2285379d9d5106926e707698e7a3283f707a4573fec9731e6ede58b5`  
		Last Modified: Thu, 26 Oct 2017 05:26:36 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff38544dc85623170156958b2d5d51604efd94b336b47a6479cde0417667838f`  
		Last Modified: Thu, 26 Oct 2017 05:26:36 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564bee8c5f497342e71777f1adc38d1578f7c95ddefe18efa16fc01b3e7e2a52`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:dcc95a027acff970a00636c77c269b7cc72e3176411c8aecc946eb6642b3906c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23318158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b316c629f8f17231a345cc527fcd76aa75a8b9e012eeae0d0497b3a92c014132`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:58 GMT
ADD file:45b5d3b8d5490ba7edfca2cf6f54cdcf49c772b0b3a2302ce69a7af061007aa4 in / 
# Wed, 25 Oct 2017 23:28:59 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:59 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 13:53:09 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 13:53:13 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 13:53:28 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 13:53:28 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 13:53:29 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 13:53:29 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 13:53:30 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 13:53:30 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 13:53:31 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 13:54:22 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 13:54:23 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 13:54:24 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 13:54:25 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 13:54:26 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 13:54:28 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 13:54:29 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 13:54:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 13:54:30 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 13:54:30 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:bb473f0ebc12fde1bd45c1bd3c46f2d3aab367b1b7739464771455b9972f7894`  
		Last Modified: Thu, 06 Jul 2017 09:54:42 GMT  
		Size: 1.9 MB (1914748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ff6b7ff3a208b8399e701e7ea1b7edbdc654c8c60d33c6f09a7803e2dda776`  
		Last Modified: Wed, 25 Oct 2017 23:29:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05834eac152e30997eb4f1aa4ffe8e952bd759c1a1009bd183dec80dca24cf86`  
		Last Modified: Thu, 26 Oct 2017 13:55:11 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd88a23486b40755f2e1192cb35d4fdaec20831c18ce83da31df3f8aa2f7b45c`  
		Last Modified: Thu, 26 Oct 2017 13:55:11 GMT  
		Size: 8.3 KB (8297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f9ba1206e6e4bfba21cef7f235482b41868ec966d5ebc44a4c4ac432a5fe03`  
		Last Modified: Thu, 26 Oct 2017 13:55:16 GMT  
		Size: 16.4 MB (16376872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5991837e23d785829d605fd052c61e10ed79a7cfb0dfee9dd40d6144bc9fad0f`  
		Last Modified: Thu, 26 Oct 2017 13:55:12 GMT  
		Size: 5.0 MB (5012322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf5663fa552ede671fc5ebf425b2ce3ff5257636b55df9564e556fe7ff85fce`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794d04d767a60fa6df4adb3af1f835701a3c2692e7f6b2d4a9db621a0bc8cd5f`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91155b0cb6bf92d1ab05fb7d13593e0a966eb79dd4e4173e3895d98dffe1c996`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969bbed547aa67091daaa801a46b062fd1c39f7835c81dd5052032056b6cf230`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:3355a334e7313d636e6b3d263a101f1ab926a88bcee118e357835788d527179a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23782989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b83bfaf99c5c91aa3c08ade40b04a3bc1b6bd3725fa905cd0a488133319eef9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:32:08 GMT
ADD file:4a952fc4b81d50b342e26a818dac48a148a4d5eddb878219650e579a5c9faeaa in / 
# Wed, 25 Oct 2017 23:32:08 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:32:08 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 10:44:24 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 10:44:28 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 10:44:50 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 10:44:50 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 10:44:51 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 10:44:51 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 10:45:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 10:45:05 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 10:45:06 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 10:45:06 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 10:45:07 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 10:45:07 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 10:45:08 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 10:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 10:45:08 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 10:45:08 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:ffe4428ef008913a7ec63449e4ad3aa536b26103943146a302591dfceb157d2f`  
		Last Modified: Sat, 17 Jun 2017 18:08:13 GMT  
		Size: 2.0 MB (2045593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4fe786260f2bd2710289e7c9487b423cb252a691fa501759b0768516122869`  
		Last Modified: Wed, 25 Oct 2017 23:32:27 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cf0f0a132c9bb882206147dffad08dc780f2bc82556cfbda9878a3218f1e7c`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00a9186496c6602ccd3efb4bb1780b42adb7028c8fa3cd3c1ff2f10bcfa33a3`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 8.3 KB (8305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc19938c3bf2e858347a9c7add1beac38af5a4f83b99d80ddc004aa4ad51e596`  
		Last Modified: Thu, 26 Oct 2017 10:45:30 GMT  
		Size: 16.7 MB (16710838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697b9a0ea77c953a543f168ba09045ae412f3b2bd0947b2bba8c18cd0cd2c70b`  
		Last Modified: Thu, 26 Oct 2017 10:45:30 GMT  
		Size: 5.0 MB (5012335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca279d1203917e8f98e0d5fe3f9de9bdde74bae202990b6388e1cc748caa726`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb3c81d25b2aa6fa5bf57aaf5f8ad6a5f27be02727e454818ff546e5a989c88`  
		Last Modified: Thu, 26 Oct 2017 10:45:29 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420233201c5d7a33d69bc90b4ac40d5db1285e61718701ffd97d4db8396a9508`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0b37b1c6d397d7b0daa633cac4b2d202e9656dd6340dc40496303190ed4a78`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:2a7e105872a021c9e0df106fd62ee50b80be17634c3b713596ca188b8ab3cf04
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23639927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01e565612a099b2324e2f273a6a14a62e8cab609839bdeb205adc72571cb62b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:47 GMT
ADD file:e0be8616517d68cb80a2f9b74eb967cda22b9937bbcbe8b75b6153815a6f7761 in / 
# Wed, 25 Oct 2017 23:28:48 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:50 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 07:12:01 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 07:12:12 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 07:12:36 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 07:12:37 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 07:12:39 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 07:12:41 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 07:12:42 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 07:12:44 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 07:12:45 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 07:13:07 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 07:13:09 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 07:13:13 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 07:13:15 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 07:13:19 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 07:13:23 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 07:13:25 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 07:13:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 07:13:28 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 07:13:30 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:1e52418956f7d2a8ea35e8e6e3318fd08e005b27457d77868c225e7433bbfa02`  
		Last Modified: Thu, 20 Jul 2017 15:12:59 GMT  
		Size: 2.0 MB (2008578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf472f4e5bb7956ac20bb343b304e1d3de1f79160c0d158cccbe25980022d50`  
		Last Modified: Wed, 25 Oct 2017 23:29:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48c95ed960185dbd69324a206614e723f0086f80b46bd3223f233e4f1e278bc`  
		Last Modified: Thu, 26 Oct 2017 07:14:01 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a8242358db9adbde1a17b0e2b320c02112fcefa90d397ecc028a9729efcf94`  
		Last Modified: Thu, 26 Oct 2017 07:14:01 GMT  
		Size: 9.1 KB (9059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6db9581873eb0cadddc4d474e33cb2ec978c0d68e3ea124ce4f07ab2731d79`  
		Last Modified: Thu, 26 Oct 2017 07:14:04 GMT  
		Size: 16.6 MB (16603134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a991ac52f27ddaf9fb4021acf59b12957c4fa6251ab4d74159bb54ac63878009`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 5.0 MB (5013168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d098ea301752e2203c7ad872d2a38cc3da3efa183b01e61fe5c2fcde29efceb8`  
		Last Modified: Thu, 26 Oct 2017 07:14:00 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8727c952955dcfc3ce7e96c808c78bc91d43e6033164a46a7faffd11dc22fb69`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fe10e7f312fce5a9bf6ca051d683f86b1cef271217890a7ea53164ef81c99d`  
		Last Modified: Thu, 26 Oct 2017 07:13:58 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcba876c6e465f99a2952b71be993ce0d4d82ef4f70f72a59e58200cf263252f`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:85a850d9b872c722bace7014c60c183a5746e338d9136a8319c91c3d2fb6a778
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23818845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45af14c4c176512dfc8deb7275c6c333b0f5933fff4eab2e34c6d8f888d40be2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:40 GMT
ADD file:6fbdff4b4c08600e192f5da9b67a02c58759237fb40525d70712104c80c34c48 in / 
# Wed, 25 Oct 2017 23:28:40 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:40 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 17:06:39 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 17:06:42 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 17:06:55 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 17:06:56 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 17:06:57 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 17:06:57 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 17:07:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 17:07:05 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 17:07:06 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 17:07:06 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 17:07:06 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 17:07:07 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 17:07:07 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 17:07:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 17:07:08 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 17:07:08 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:d45fd9d3c4f188ab1f3a4bf6a9f5202b3f1577dbb998f5f28e82d192e0c1f0e7`  
		Last Modified: Sat, 17 Jun 2017 20:41:42 GMT  
		Size: 2.1 MB (2065460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5978b6b34b3e943e0fd25dfb50991c0bad82a986cfdaa91c4de756431ba679`  
		Last Modified: Wed, 25 Oct 2017 23:28:59 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299a1fbc19bbea84dbf4d0b6e2e71fb847299b017209b1f9783faea14214c995`  
		Last Modified: Thu, 26 Oct 2017 17:07:31 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb76f2dd4162cae82233bc93ba436b63ca37e536d53c85a9f1d7343203e3c383`  
		Last Modified: Thu, 26 Oct 2017 17:07:31 GMT  
		Size: 8.6 KB (8604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac09bb55706d627cf6348c9d0bd891c2fe9a4155aee5d95264b92781371021db`  
		Last Modified: Thu, 26 Oct 2017 17:07:33 GMT  
		Size: 16.7 MB (16726549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e776aa2eebd7dc068e74be7736114ce80966ab2b25478d29763bc1ccf05c3e3`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 5.0 MB (5012317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57d3128b93c0f42a41ad6b2571d41e61c6096e070ee18ef58d34aeaf7318560`  
		Last Modified: Thu, 26 Oct 2017 17:07:29 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484c70be68b7dc1296d1199834238ebabbde1df9ce04ec3cf986a2096ad218b6`  
		Last Modified: Thu, 26 Oct 2017 17:07:29 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01611bf6acbe11966a7f1fe2e96d811430328e24513c20237576287afdd5079a`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f045868d086334dbd06f276dfb93c084fc32b243827527e36c2bc5a5d8583d`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rabbitmq:3.6-management`

```console
$ docker pull rabbitmq@sha256:90b467d41e6655bb52d7114802c028eb359e220a7ec87c98a23a294af2b81ad4
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

### `rabbitmq:3.6-management` - linux; amd64

```console
$ docker pull rabbitmq@sha256:40a956f5198d4d2050d1545dc48bf38b5e0342c33d10bcd04c9e0a7e7bc851af
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.9 MB (62852369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ac724eab06670229b033f2516a2e3af2cdfb453495a9bbb040fea13b398ab5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:33:42 GMT
ADD file:45233d6b5c9b91e9437065d3e7c332d1c4eb4bce8e1079a4c1af342c450abe67 in / 
# Mon, 09 Oct 2017 21:33:43 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 02:41:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:41:43 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 02:41:43 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 02:42:10 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 02:42:40 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 02:42:41 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 02:42:42 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 02:43:16 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:43:16 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 02:43:17 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 02:43:17 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 02:43:18 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 02:43:19 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 13 Oct 2017 23:40:43 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 13 Oct 2017 23:40:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 13 Oct 2017 23:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2017 23:40:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 13 Oct 2017 23:40:45 GMT
CMD ["rabbitmq-server"]
# Fri, 13 Oct 2017 23:40:56 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 13 Oct 2017 23:40:57 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:bc95e04b23c06ba1b9bf092d07d1493177b218e0340bd2ed49dac351c1e34313`  
		Last Modified: Mon, 09 Oct 2017 21:42:28 GMT  
		Size: 22.5 MB (22492350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65f0b00e4cfb1535d0f4e7a63707172ae63483fb33140d777614f199afcb36`  
		Last Modified: Tue, 10 Oct 2017 02:43:59 GMT  
		Size: 4.5 MB (4498726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bd803179890909fcae186044c0e6ca1bc1d34e5fc05ef1ccea823e7be97540`  
		Last Modified: Tue, 10 Oct 2017 02:43:57 GMT  
		Size: 4.1 KB (4069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b05ca8302833edf783c50f03cd7ba0b8e12bc872b053eda3e3ae7e1f17e2b4b`  
		Last Modified: Tue, 10 Oct 2017 02:43:58 GMT  
		Size: 952.1 KB (952058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb5a4bbcce5a040eb83057f9e93d17663bb123f4e98168457444497f7d17b70`  
		Last Modified: Tue, 10 Oct 2017 02:44:03 GMT  
		Size: 27.7 MB (27703883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf840d8999f6fe46a162974c82378c38b3cf3dcccbbaff848c0fb199988aebe0`  
		Last Modified: Tue, 10 Oct 2017 02:44:00 GMT  
		Size: 7.2 MB (7194403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be339ca44883b1990e52771487402163d398a279755a501fdd8891ec71cf09d0`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce35cd9f9b5b917868095b3b074dd23d18e0e266f3ee68ff95e2c61467299812`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fe32a0a00d916ed4d632aae71d35d9d0baa5e5910d6bd179a24071c35bedb0`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77408ca9e94eb4bfeb346ab10c602857525802c2279e7c6995fcdbc90269444a`  
		Last Modified: Fri, 13 Oct 2017 23:41:26 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db03407a1aba1c0a89dffe960394aae639885702e3faa65271b918c36c7905cd`  
		Last Modified: Fri, 13 Oct 2017 23:41:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b908f008ac2afe6632caccd124e3ee9bffd5ebcdb8ca5ca84ae7e014305e460f`  
		Last Modified: Fri, 13 Oct 2017 23:42:01 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6-management` - linux; arm variant v5

```console
$ docker pull rabbitmq@sha256:07150eac8a231b8c043f29aba9a9ba3d81aa4cdd16c8e3387621deb4d8fdf1f4
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58432562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00088686092d95f6db193285835d1af5662557d679f57a4c21d1d4ec648c0924`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:44:48 GMT
ADD file:ff9945b48b1ac236dcec24eb9dfaf52b7c151a3b11c8502391f0866dfb4e3ac3 in / 
# Mon, 09 Oct 2017 21:44:48 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 00:18:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:18:11 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 00:18:11 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 00:18:29 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 00:18:58 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:18:58 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 00:18:58 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 00:19:26 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:19:26 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 00:19:27 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 00:19:28 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 00:19:29 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 00:19:30 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Sat, 14 Oct 2017 14:14:24 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Sat, 14 Oct 2017 14:14:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 14 Oct 2017 14:14:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 Oct 2017 14:14:25 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Sat, 14 Oct 2017 14:14:26 GMT
CMD ["rabbitmq-server"]
# Sat, 14 Oct 2017 14:14:34 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Sat, 14 Oct 2017 14:14:34 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:836d5b6056a9815be79c76480a90299267f60201bd1e3396817003e6c14819cc`  
		Last Modified: Mon, 09 Oct 2017 21:50:56 GMT  
		Size: 21.2 MB (21166251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb896fba83bd09a35c68457554b35289860c23c46f27a8c3ef42f13146ebba1`  
		Last Modified: Tue, 10 Oct 2017 00:20:01 GMT  
		Size: 4.2 MB (4231979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61827a16c114b9741d761aa4c60a972ffe1e0b60147794e86b05653d67822e91`  
		Last Modified: Tue, 10 Oct 2017 00:20:00 GMT  
		Size: 4.1 KB (4079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877cd9511def30e56a5ce354e145e8a2b1a93daaae7eaaa42dc4219838aa1743`  
		Last Modified: Tue, 10 Oct 2017 00:20:00 GMT  
		Size: 942.8 KB (942752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea9e378899e98c99e93ae2d0874bd5d89e24134bd14a19c285bdf39a0a42ade`  
		Last Modified: Tue, 10 Oct 2017 00:20:05 GMT  
		Size: 25.2 MB (25170810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc82a29314b16531aa2172ac523ba535e3678f85efdd699164fbb0241ab8b62`  
		Last Modified: Tue, 10 Oct 2017 00:20:01 GMT  
		Size: 6.9 MB (6909811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c44a3d016cf9de95021782180a42d3660e20fc7d8e92a7fe5ce9ede7928ca2`  
		Last Modified: Tue, 10 Oct 2017 00:19:59 GMT  
		Size: 2.3 KB (2261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abfdcdd98b40291ad91791bea09bf277e75c3669c6607c7891b09130101bfa3`  
		Last Modified: Tue, 10 Oct 2017 00:19:58 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a72811da4bf8ca8a2d06cdc182aa54116bb12133e8d82ef2b018a8de29ed74`  
		Last Modified: Tue, 10 Oct 2017 00:19:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147d8cf0897dea9b024bf5c6efb6873db3d86dec857fca062b146f88b7b5a735`  
		Last Modified: Sat, 14 Oct 2017 14:14:43 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f355fd0b70caedf30aa384298307b8e40d922e9e341492dd3fde71f119fd7d7`  
		Last Modified: Sat, 14 Oct 2017 14:14:44 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77dcaa76990445223000f8a5eb10485f94e82d4817f74f142f106b0a4dd9ad0c`  
		Last Modified: Sat, 14 Oct 2017 14:15:02 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6-management` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:353fc3a4b10cc0fd93baf80287c8e7c779c49d7fd5421091aa004286b3bf559c
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55688342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd5c488f599ef650e2dc6824d489473db268160f94789b74f5ec312eef58600d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:43 GMT
ADD file:b758c6c3ff989778bd740dde35c86b953fa09be913a7e02711b2881de6b8911d in / 
# Mon, 09 Oct 2017 21:45:44 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 13:07:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:07:42 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 13:07:42 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 13:07:58 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 13:08:17 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:08:17 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 13:08:17 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 13:08:39 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:08:39 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 13:08:40 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 13:08:41 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 13:08:42 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 13:08:43 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 13:08:43 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 13:08:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 13:08:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 13:08:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 13:08:45 GMT
CMD ["rabbitmq-server"]
# Fri, 03 Nov 2017 13:09:01 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 03 Nov 2017 13:09:01 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:59e81a3fde58ec8d4b8f2f58b98ef2f4d951d37dd9b99b016fd294a8e07d7796`  
		Last Modified: Mon, 09 Oct 2017 21:52:49 GMT  
		Size: 19.3 MB (19277135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2037b99f3c3dc51e8ace39aed9971155f34f325ac4f0a1e56a07c4d6c02f5ae6`  
		Last Modified: Fri, 03 Nov 2017 13:09:18 GMT  
		Size: 3.9 MB (3868347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f368172ea96bda944832762ad29b52dfe17ec5e6fae96eee37adc4e9d68674a5`  
		Last Modified: Fri, 03 Nov 2017 13:09:16 GMT  
		Size: 4.1 KB (4084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893cc1ae60f8bf72ac3020ccc60b22d9e0ad0cb0647e15bc4847d08c8985eee2`  
		Last Modified: Fri, 03 Nov 2017 13:09:16 GMT  
		Size: 926.1 KB (926097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13220cc1a683014bda9cfae7f7ee7015a26b28048f90f5aa3ed8b6a96f4b2813`  
		Last Modified: Fri, 03 Nov 2017 13:09:20 GMT  
		Size: 24.8 MB (24785610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269f4e069126132643c1c0be1faf600d55ff15e870066c527d03181904d99c5d`  
		Last Modified: Fri, 03 Nov 2017 13:09:17 GMT  
		Size: 6.8 MB (6820180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ae244f4f610a339fcbddf37612a15ec7b7f6674e3d888c3c4d36302283418e`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce7d85327b7bc7d59a7b54222a3e6babd7f8afd8eb080becb77fc52aed5a751`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dfa32e4b49700ed0130ebd563f40a2c381393983b571a9886435813102ad0c`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba15cd885dc21f438d366b40d0d9f595f2c25e063c60fa590ab4c0f6233ff94`  
		Last Modified: Fri, 03 Nov 2017 13:09:14 GMT  
		Size: 4.0 KB (4040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978a8434497fcb8e08cefc7484b515ac34fe23c281fb869d015f62b54673028c`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34fa59eaf946f8e35134f1a0bf195874868c3ce1e2a025350fc57efe60ecbea`  
		Last Modified: Fri, 03 Nov 2017 13:09:54 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6-management` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:4ad104ab7b291ca9aea4bb42e18de213ae21ef6a655d909c3568e2b36f465074
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57278563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9356e7f3d3e445f04242803fb4b5afb70fad5f726388635b781f4814733c3af7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:47:55 GMT
ADD file:3a528355cfc75437716aff3b517ef99ae602918d84d26dbafff0ed142248fb93 in / 
# Mon, 09 Oct 2017 21:47:56 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 04:57:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 04:57:04 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 04:57:05 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 04:57:37 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 04:58:35 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 04:58:36 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 04:58:37 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 04:58:37 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 04:58:38 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 04:58:39 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 04:58:39 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 05:00:22 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 05:00:23 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 05:00:25 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 05:00:26 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 05:00:28 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 05:00:31 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Sat, 14 Oct 2017 13:52:47 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Sat, 14 Oct 2017 13:52:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 14 Oct 2017 13:52:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 Oct 2017 13:52:51 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Sat, 14 Oct 2017 13:52:51 GMT
CMD ["rabbitmq-server"]
# Sat, 14 Oct 2017 13:53:08 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Sat, 14 Oct 2017 13:53:09 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:e907afd6e25615a4d3eb554d930cef57b87e79ec82413889c2eac38beb4eb8f7`  
		Last Modified: Mon, 09 Oct 2017 22:03:08 GMT  
		Size: 20.3 MB (20337143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5e6d35928560b933b85b5a3f2a8e96b4520fbb8df138b3e739e56d0c1f355`  
		Last Modified: Tue, 10 Oct 2017 05:01:18 GMT  
		Size: 4.1 MB (4073554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a862ab821b342790326492507ca5d70bfb7016bef765606193f1f7139f60c5ed`  
		Last Modified: Tue, 10 Oct 2017 05:01:14 GMT  
		Size: 4.1 KB (4072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92799a54920b79013733790e444f13d8c65faa29c79cbdaf1bc8af85f637a233`  
		Last Modified: Tue, 10 Oct 2017 05:01:14 GMT  
		Size: 919.5 KB (919487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b119999eef1bcadabedd3a5319b03c6b83ede91ba8535059851547d3433b205`  
		Last Modified: Tue, 10 Oct 2017 05:01:19 GMT  
		Size: 25.0 MB (25042572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62f8525a3a982a102aa37bb3313876195b15d8781cd253ed238dd2b9dff151`  
		Last Modified: Tue, 10 Oct 2017 05:01:15 GMT  
		Size: 6.9 MB (6894852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc028e70f04f6ea4365223a1cfe4e5c4384d5921acac419f3c170b148f7c7bf`  
		Last Modified: Tue, 10 Oct 2017 05:01:10 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e99faa03c2a8a272f56208c644c12b384b69dea50be6da9f6be400c14b945c`  
		Last Modified: Tue, 10 Oct 2017 05:01:12 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8fa260bcaa52d81ba20c11111f8d15bab954b17b48666724536c604220d94e`  
		Last Modified: Tue, 10 Oct 2017 05:01:11 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306840de948d03472918a306c089409429606802ec8cf841e96dec707a2f7178`  
		Last Modified: Sat, 14 Oct 2017 13:53:27 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a7a978032478b38adb1f0107466d187e53380f7037d058c62e4937cd07fc09`  
		Last Modified: Sat, 14 Oct 2017 13:53:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3facaa930064fd14fbd9a077b63e5f3261d1e63bd15c3d1426575c6c4f8eca`  
		Last Modified: Sat, 14 Oct 2017 13:54:17 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6-management` - linux; 386

```console
$ docker pull rabbitmq@sha256:16ab1fd6ebf60e7fe32149ac86bf79cd5a2e2d573dec3267fd0d7d646514384c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63902453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a8039a2961a84491da6ac62bad7d9b065b333750e66543f8e7cf931c13ed028`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:36 GMT
ADD file:6582536277127947668f7bfdc1471a4e36170915b91a4cb841e7e1bfa1de6535 in / 
# Mon, 09 Oct 2017 21:45:36 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 10:45:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:45:12 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 10:45:13 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 10:45:28 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 10:46:03 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 10:46:04 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 10:46:25 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:46:25 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 10:46:26 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 10:46:27 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 10:46:27 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 10:46:28 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 10:46:28 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 10:46:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 10:46:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 10:46:30 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 10:46:30 GMT
CMD ["rabbitmq-server"]
# Fri, 03 Nov 2017 10:46:58 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 03 Nov 2017 10:46:58 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:b2b52fe46b29fe5d0689f26449c2114e40f0731d4ce3eb8c3941397b74205432`  
		Last Modified: Mon, 09 Oct 2017 21:53:42 GMT  
		Size: 23.1 MB (23128678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d407b136da0731f5f38279001e9dd426217937443cad0f16e1f242366290773`  
		Last Modified: Fri, 03 Nov 2017 10:47:13 GMT  
		Size: 4.8 MB (4803637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c93817e78345b4b5070c81e5a37d02afc2b5fe347a1a4bf59e09f6084814fd2`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 4.1 KB (4057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97eae59c75f8f814ab781f5239ac2e132b7b65c77e75b35023c603c539ca54f`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 931.5 KB (931524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aed670dee19fde6946658d7129e13520c1a0747f8b80b6f92dac5f6d974ae52`  
		Last Modified: Fri, 03 Nov 2017 10:47:24 GMT  
		Size: 27.8 MB (27818690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b61d6d0b60ec18280aeba946a05d62817afbe030f277af85b5f434021e90c9`  
		Last Modified: Fri, 03 Nov 2017 10:47:16 GMT  
		Size: 7.2 MB (7208985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec7d4cc3b5497bbbd6b2d1e9574dbedb6c7ad11805cff4c287ea444ddc2e298`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 2.3 KB (2259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eec554591344f78e35e3976d002d617623a52d123fc71e65d33c4d533d2b2e7`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e433f73af1167eff0dee1984c095bf5be36593fcead5b8cc820e2cb829aaed0`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8d6e0dbdbb04b44f7a0972fce6b0b1b19262e4fc5416bd1589af560f16c99f`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 4.0 KB (4040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bab08cf9b00d8109139e1cb1cdec448b71fdae7d7f1260d4175771416a5f80`  
		Last Modified: Fri, 03 Nov 2017 10:47:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2aad62bc4e7f6b9b68a5196e492b29083b8ab4e68dfea4a93b469cb79aae29`  
		Last Modified: Fri, 03 Nov 2017 10:48:04 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6-management` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:47fb5bf4afd56afb9e9ab383f1449cee19c3ab7a7e653d0b04037cf839cfab52
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60384672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c4dbfbbd301b5dbb171ca49da8419b76567c7aa2d00978e12759ced95ca846`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:56 GMT
ADD file:7edf73437495be24244c16841b563be06c15452963f41ac940fb5e105ed96027 in / 
# Mon, 09 Oct 2017 21:45:58 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 07:12:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:12:51 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 07:12:53 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 07:13:49 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 07:15:26 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:15:28 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 07:15:29 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 07:15:31 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 07:15:33 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 07:15:34 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 07:15:35 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 07:16:54 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:16:55 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 07:17:00 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 07:17:01 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 07:17:06 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 07:17:11 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 07:17:13 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 07:17:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 07:17:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 07:17:21 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 07:17:23 GMT
CMD ["rabbitmq-server"]
# Fri, 03 Nov 2017 07:17:36 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 03 Nov 2017 07:17:39 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:c4860466fa1e6824151f4fa3a51ef0e9d7d3c3ba860e21d94e69988b65601260`  
		Last Modified: Mon, 09 Oct 2017 21:52:59 GMT  
		Size: 22.7 MB (22746217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebe4c87dcd1f7ef11d4d21752831bf4095ac42afe041706c35f1d7d4d0ca4f2`  
		Last Modified: Fri, 03 Nov 2017 07:18:05 GMT  
		Size: 4.4 MB (4360529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e5365525084de1c85fa29ef33d37c38b5f80621f5bcb26bb4882d71598c6f7`  
		Last Modified: Fri, 03 Nov 2017 07:18:03 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600c3853740b7f4cff9cc799ae478f669bd54277a8dd375479a34ed1bb47a803`  
		Last Modified: Fri, 03 Nov 2017 07:18:02 GMT  
		Size: 920.7 KB (920695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993868ec534130e348e45aa6d64b471fa46eafbf061836cc9d2a56edf73e9382`  
		Last Modified: Fri, 03 Nov 2017 07:18:06 GMT  
		Size: 25.5 MB (25492533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca1b92e212aaef163244d5fdd9e135fdb8be8c9dbbb626061ee2882d941a553`  
		Last Modified: Fri, 03 Nov 2017 07:18:03 GMT  
		Size: 6.9 MB (6853702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483f96d1f500f9f69170bc6927d599a7f0cd1550f96b6ee3f90eb4185a1bffb`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b433db63f40c7cab3080cf36bd7beabbdf7d9eece3f2dc16a65b900c61180`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93971551a2c911c34ca2e9af47495efb2f27e2922e567d93dd94dfb9b773bd3`  
		Last Modified: Fri, 03 Nov 2017 07:17:58 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5494bb8bcc45452a84c216edffedb3103a15c3e209aba0561dfbc70e4312192e`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 4.0 KB (4039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d56b2a4f9f8d7b11831a8f1952fe2c02613bcb014ab9d756b70b3b398b37269`  
		Last Modified: Fri, 03 Nov 2017 07:17:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e2264063017ef705c9dcc066695ab771b32f19f38ba34c158531e7d3f4c9fc`  
		Last Modified: Fri, 03 Nov 2017 07:18:40 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6-management` - linux; s390x

```console
$ docker pull rabbitmq@sha256:35d9ecb54b432f7591ecfe0cb1ee71d152199b0ae07ecdd8c9b21cd6a87b0a51
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60364970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a628fac494ad4d163ad91471c151b4ed5bcfbe2f318bc677224413d944cf4ce8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:44:35 GMT
ADD file:ae4aaa6affe22f36ab5478771d5c84917f72de7a8dac16345a035709a1a5edf4 in / 
# Mon, 09 Oct 2017 21:44:36 GMT
CMD ["bash"]
# Thu, 02 Nov 2017 17:06:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 17:06:41 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Thu, 02 Nov 2017 17:06:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 02 Nov 2017 17:07:21 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Thu, 02 Nov 2017 17:07:43 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 02 Nov 2017 17:07:44 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 02 Nov 2017 17:07:45 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 17:07:48 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 17:07:48 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 17:07:49 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 17:07:50 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 17:07:52 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 17:07:53 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 17:07:54 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 17:07:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 17:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 17:07:57 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 17:07:57 GMT
CMD ["rabbitmq-server"]
# Fri, 03 Nov 2017 17:08:14 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 03 Nov 2017 17:08:15 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:671716cc49517eef5f430c695ce344d63e390cb65f58d30939f2ba615c953686`  
		Last Modified: Mon, 09 Oct 2017 21:49:09 GMT  
		Size: 22.3 MB (22339951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cae61f12be6f01ba06573d9393712e91821cd5496302310f550fe5842dea557`  
		Last Modified: Fri, 03 Nov 2017 17:08:41 GMT  
		Size: 4.5 MB (4529879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca307103ce923e7e89d35185be4df8e54c3c0b54d259b8880aa7bae107d4952`  
		Last Modified: Fri, 03 Nov 2017 17:08:39 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d16320f9fc35ea20ba7fb9b21f88e3f0f06c52d416682319f3b2a85a345a3d5`  
		Last Modified: Fri, 03 Nov 2017 17:08:39 GMT  
		Size: 938.0 KB (938019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801205b182b8d6f7acf36200b2ba07ed52ea224dfefe792b525224e4aacb4d4a`  
		Last Modified: Fri, 03 Nov 2017 17:08:48 GMT  
		Size: 25.6 MB (25619372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9cb605e6242f5ab505cbd229c7b2fdf2935a6254130070c12c4d8413616024`  
		Last Modified: Fri, 03 Nov 2017 17:08:40 GMT  
		Size: 6.9 MB (6926791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2799e1b1479136fbb3c3ba6df318d449990a3cf5fc3293a14142cde0d9f51980`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a6d5de3e6aaa1c06122a1b5cda3b4bcb98d54e5dc23f38896fc81e98cea769`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172fa2e52818dcedf69c727f6790f0f9744f8538da3f4222602aaa0ab9fa82c0`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c734f2707800c1189521a51409fed1508fb7e36c6e67eca5537d03c4b24ef0d`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 4.0 KB (4037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e7d712f1155d66243480cd441ec04e084a8e7e2d6a0653e27138b31b56d2ae`  
		Last Modified: Fri, 03 Nov 2017 17:08:38 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9489f6c1d1f9d4090b7d9220b20aac5cc7e9588c9ddf66d0357f1eb8226071`  
		Last Modified: Fri, 03 Nov 2017 17:09:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rabbitmq:3.6-management-alpine`

```console
$ docker pull rabbitmq@sha256:cc6bb38a4167c70483b6f174d43bf43032a23b1d9c661530cfda228bf60e3f87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `rabbitmq:3.6-management-alpine` - linux; amd64

```console
$ docker pull rabbitmq@sha256:ef2b9b2cbfbe00330d8cfaaf8acef1127996756ee66bad0ac832aba8e63ae67f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23579858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4927e0fd02a40ab3ffc333a1326f9a21be7aec9059d82c2dfdc37580847a76f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:19:51 GMT
ADD file:1e87ff33d1b6765b793888cd50e01b2bd0dfe152b7dbb4048008bfc2658faea7 in / 
# Wed, 25 Oct 2017 23:19:51 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 03:02:21 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 03:02:25 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 03:02:32 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 03:02:32 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 03:02:33 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 03:02:33 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 03:02:42 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 03:02:42 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 03:02:43 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 03:02:43 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 03:02:44 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 03:02:44 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 03:02:45 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 03:02:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 03:02:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 03:02:45 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 03:02:59 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 03:02:59 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:b56ae66c29370df48e7377c8f9baa744a3958058a766793f821dadcb144a4647`  
		Last Modified: Wed, 25 Oct 2017 23:21:25 GMT  
		Size: 2.0 MB (1991435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827e0bce86e3c8fa677ac91f0c55a7a4071cc45c729b171aecbe04d35ae160d7`  
		Last Modified: Thu, 26 Oct 2017 03:03:23 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe01d115cb92dc0ab37de6b6ffa2073ea20d30dfc49c537fbba569cd6a494b8`  
		Last Modified: Thu, 26 Oct 2017 03:03:23 GMT  
		Size: 8.2 KB (8176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bfc0dbbf8b1d2f532779c4873b4c7e0237d6ecc86161b1c6f28e3b6bd3149f`  
		Last Modified: Thu, 26 Oct 2017 03:03:26 GMT  
		Size: 16.6 MB (16561644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b24f4fd26b3494d310561a28e2d9aeb08e7baba442eaef2cd8697c7ebd9d9f1`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 5.0 MB (5012671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfb0f3b402f9674b21d7ed079f6576ec1be80f333f41c404e8ce3feb193b813`  
		Last Modified: Thu, 26 Oct 2017 03:03:22 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521b2b4b2311f153d53f0b9bde9a164f45df9dfd531512c36195ba2ccf5a4c76`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cedbb525e85f1b9257e8b20d04b4ad39f1004c9dfbc673086815dd887f380c3`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f35995cc5f5daa05334d17a87482ac8728aadfb0f10f9d62b3d70f5986e5cc`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f1f0f842cbbd9046d7b95afc926b8e22e4befd18e38ed5d4514e14105d2be`  
		Last Modified: Thu, 26 Oct 2017 03:04:25 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6-management-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:e8e0295fdf1734258af64b4f82784721e845b6a68146965bd1592c0e15c58d1a
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23413037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1379abcce7a4a22ec254dfd3fe56547de4c89c0b12cfaf5e044ea05c4205dfb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:35 GMT
ADD file:009348222efb3c4ca2e53c387fb34c488679ca07db39525a6c5cc214e46abffd in / 
# Wed, 25 Oct 2017 23:28:36 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:36 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 05:25:53 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 05:25:55 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 05:26:10 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 05:26:10 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 05:26:10 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 05:26:11 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 05:26:19 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 05:26:19 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 05:26:20 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 05:26:20 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 05:26:21 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 05:26:22 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 05:26:22 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 05:26:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 05:26:22 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 05:26:23 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 05:26:30 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 05:26:30 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:0864efeeb5cb8dca4eb53e5d6fd38486daee80fa326fe36d1ad254f8fa6bb310`  
		Last Modified: Sun, 23 Jul 2017 20:21:42 GMT  
		Size: 2.0 MB (1965988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda69762aee1588fa82aeabf1af6d6ad24f737cce1451fab2e0199849b1e12e`  
		Last Modified: Wed, 25 Oct 2017 23:28:45 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62a8c5580cc1c2fbf2f9ce119bc0c06403a12ad18167bde2ec94420810916db`  
		Last Modified: Thu, 26 Oct 2017 05:26:38 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b096e39434b5aeddcb2ec167b7bf570cac7b8b16e68324d3f46c6f4d41b69c79`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 8.4 KB (8374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ad9273316fa6f22cd2e8cf88c92f34c3210325fa1be2041153a96f4124476f`  
		Last Modified: Thu, 26 Oct 2017 05:26:41 GMT  
		Size: 16.4 MB (16420180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed982c9e7d5644c85267595b470c0f21f25093a865603ab33304248efdb68b5d`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 5.0 MB (5012332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b76830a9cb5b5f898068945d6af6325c7d97b36d50e521a12097d3e908fd0`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a31f9ee2285379d9d5106926e707698e7a3283f707a4573fec9731e6ede58b5`  
		Last Modified: Thu, 26 Oct 2017 05:26:36 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff38544dc85623170156958b2d5d51604efd94b336b47a6479cde0417667838f`  
		Last Modified: Thu, 26 Oct 2017 05:26:36 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564bee8c5f497342e71777f1adc38d1578f7c95ddefe18efa16fc01b3e7e2a52`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fe4d4545d22113e1fa0e2fbc7ae69364213b6ca264274a71ad66ac045835d1`  
		Last Modified: Thu, 26 Oct 2017 05:26:49 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6-management-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:bf020d55089aa6f03eb3e259eefa2014a2191041616b46f4c7e56fd10fd09b76
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23318349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67e8f6bc203146953e13d3ce7086f40a6796ae711f8d8231aac5693d99175f9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:58 GMT
ADD file:45b5d3b8d5490ba7edfca2cf6f54cdcf49c772b0b3a2302ce69a7af061007aa4 in / 
# Wed, 25 Oct 2017 23:28:59 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:59 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 13:53:09 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 13:53:13 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 13:53:28 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 13:53:28 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 13:53:29 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 13:53:29 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 13:53:30 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 13:53:30 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 13:53:31 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 13:54:22 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 13:54:23 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 13:54:24 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 13:54:25 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 13:54:26 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 13:54:28 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 13:54:29 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 13:54:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 13:54:30 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 13:54:30 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 13:54:47 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 13:54:47 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:bb473f0ebc12fde1bd45c1bd3c46f2d3aab367b1b7739464771455b9972f7894`  
		Last Modified: Thu, 06 Jul 2017 09:54:42 GMT  
		Size: 1.9 MB (1914748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ff6b7ff3a208b8399e701e7ea1b7edbdc654c8c60d33c6f09a7803e2dda776`  
		Last Modified: Wed, 25 Oct 2017 23:29:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05834eac152e30997eb4f1aa4ffe8e952bd759c1a1009bd183dec80dca24cf86`  
		Last Modified: Thu, 26 Oct 2017 13:55:11 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd88a23486b40755f2e1192cb35d4fdaec20831c18ce83da31df3f8aa2f7b45c`  
		Last Modified: Thu, 26 Oct 2017 13:55:11 GMT  
		Size: 8.3 KB (8297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f9ba1206e6e4bfba21cef7f235482b41868ec966d5ebc44a4c4ac432a5fe03`  
		Last Modified: Thu, 26 Oct 2017 13:55:16 GMT  
		Size: 16.4 MB (16376872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5991837e23d785829d605fd052c61e10ed79a7cfb0dfee9dd40d6144bc9fad0f`  
		Last Modified: Thu, 26 Oct 2017 13:55:12 GMT  
		Size: 5.0 MB (5012322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf5663fa552ede671fc5ebf425b2ce3ff5257636b55df9564e556fe7ff85fce`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794d04d767a60fa6df4adb3af1f835701a3c2692e7f6b2d4a9db621a0bc8cd5f`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91155b0cb6bf92d1ab05fb7d13593e0a966eb79dd4e4173e3895d98dffe1c996`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969bbed547aa67091daaa801a46b062fd1c39f7835c81dd5052032056b6cf230`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1643075e82e89fd6745e0baa4b9fd436da4f959fffedec9f0d149f84a7c16f8f`  
		Last Modified: Thu, 26 Oct 2017 13:56:10 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6-management-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:775482d2d2f81b04a7f91840ed0a169b185315f4dc226d515adaacb675e6f6dc
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23783181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:845026f49dc450aaf8e569e45ba76c8b1bf506da17e742b0a54fbddaf5bcf9f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:32:08 GMT
ADD file:4a952fc4b81d50b342e26a818dac48a148a4d5eddb878219650e579a5c9faeaa in / 
# Wed, 25 Oct 2017 23:32:08 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:32:08 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 10:44:24 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 10:44:28 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 10:44:50 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 10:44:50 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 10:44:51 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 10:44:51 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 10:45:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 10:45:05 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 10:45:06 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 10:45:06 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 10:45:07 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 10:45:07 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 10:45:08 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 10:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 10:45:08 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 10:45:08 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 10:45:16 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 10:45:16 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:ffe4428ef008913a7ec63449e4ad3aa536b26103943146a302591dfceb157d2f`  
		Last Modified: Sat, 17 Jun 2017 18:08:13 GMT  
		Size: 2.0 MB (2045593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4fe786260f2bd2710289e7c9487b423cb252a691fa501759b0768516122869`  
		Last Modified: Wed, 25 Oct 2017 23:32:27 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cf0f0a132c9bb882206147dffad08dc780f2bc82556cfbda9878a3218f1e7c`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00a9186496c6602ccd3efb4bb1780b42adb7028c8fa3cd3c1ff2f10bcfa33a3`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 8.3 KB (8305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc19938c3bf2e858347a9c7add1beac38af5a4f83b99d80ddc004aa4ad51e596`  
		Last Modified: Thu, 26 Oct 2017 10:45:30 GMT  
		Size: 16.7 MB (16710838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697b9a0ea77c953a543f168ba09045ae412f3b2bd0947b2bba8c18cd0cd2c70b`  
		Last Modified: Thu, 26 Oct 2017 10:45:30 GMT  
		Size: 5.0 MB (5012335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca279d1203917e8f98e0d5fe3f9de9bdde74bae202990b6388e1cc748caa726`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb3c81d25b2aa6fa5bf57aaf5f8ad6a5f27be02727e454818ff546e5a989c88`  
		Last Modified: Thu, 26 Oct 2017 10:45:29 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420233201c5d7a33d69bc90b4ac40d5db1285e61718701ffd97d4db8396a9508`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0b37b1c6d397d7b0daa633cac4b2d202e9656dd6340dc40496303190ed4a78`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b719c08f02439306e8baee89f388d47a99542fc0eec294aaf615c425ec5253de`  
		Last Modified: Thu, 26 Oct 2017 10:45:59 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6-management-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:1f2ed16a80e1b71fd652fe7520fa1ba2ac5c9b5a207199bc7aaec39c61d5a38e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23640124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0244f72e17b275644966d172a75c7023650024e2761d2541020cbb3592bd01f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:47 GMT
ADD file:e0be8616517d68cb80a2f9b74eb967cda22b9937bbcbe8b75b6153815a6f7761 in / 
# Wed, 25 Oct 2017 23:28:48 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:50 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 07:12:01 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 07:12:12 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 07:12:36 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 07:12:37 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 07:12:39 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 07:12:41 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 07:12:42 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 07:12:44 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 07:12:45 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 07:13:07 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 07:13:09 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 07:13:13 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 07:13:15 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 07:13:19 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 07:13:23 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 07:13:25 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 07:13:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 07:13:28 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 07:13:30 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 07:13:42 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 07:13:44 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:1e52418956f7d2a8ea35e8e6e3318fd08e005b27457d77868c225e7433bbfa02`  
		Last Modified: Thu, 20 Jul 2017 15:12:59 GMT  
		Size: 2.0 MB (2008578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf472f4e5bb7956ac20bb343b304e1d3de1f79160c0d158cccbe25980022d50`  
		Last Modified: Wed, 25 Oct 2017 23:29:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48c95ed960185dbd69324a206614e723f0086f80b46bd3223f233e4f1e278bc`  
		Last Modified: Thu, 26 Oct 2017 07:14:01 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a8242358db9adbde1a17b0e2b320c02112fcefa90d397ecc028a9729efcf94`  
		Last Modified: Thu, 26 Oct 2017 07:14:01 GMT  
		Size: 9.1 KB (9059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6db9581873eb0cadddc4d474e33cb2ec978c0d68e3ea124ce4f07ab2731d79`  
		Last Modified: Thu, 26 Oct 2017 07:14:04 GMT  
		Size: 16.6 MB (16603134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a991ac52f27ddaf9fb4021acf59b12957c4fa6251ab4d74159bb54ac63878009`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 5.0 MB (5013168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d098ea301752e2203c7ad872d2a38cc3da3efa183b01e61fe5c2fcde29efceb8`  
		Last Modified: Thu, 26 Oct 2017 07:14:00 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8727c952955dcfc3ce7e96c808c78bc91d43e6033164a46a7faffd11dc22fb69`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fe10e7f312fce5a9bf6ca051d683f86b1cef271217890a7ea53164ef81c99d`  
		Last Modified: Thu, 26 Oct 2017 07:13:58 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcba876c6e465f99a2952b71be993ce0d4d82ef4f70f72a59e58200cf263252f`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d8f64c426c0a1bf9de5b158513294037721b7e6c1c4fbc5e75f84a63743aae`  
		Last Modified: Thu, 26 Oct 2017 07:14:31 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3.6-management-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:4af0a8312682b92651de05ff83aac54b00b55118b9babda060c043b4fdf9609b
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23819037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b62c33cd033388e2676822a15081284e991d3078ed4b51ebab5b72b7cb5a983`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:40 GMT
ADD file:6fbdff4b4c08600e192f5da9b67a02c58759237fb40525d70712104c80c34c48 in / 
# Wed, 25 Oct 2017 23:28:40 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:40 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 17:06:39 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 17:06:42 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 17:06:55 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 17:06:56 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 17:06:57 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 17:06:57 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 17:07:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 17:07:05 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 17:07:06 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 17:07:06 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 17:07:06 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 17:07:07 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 17:07:07 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 17:07:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 17:07:08 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 17:07:08 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 17:07:19 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 17:07:19 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:d45fd9d3c4f188ab1f3a4bf6a9f5202b3f1577dbb998f5f28e82d192e0c1f0e7`  
		Last Modified: Sat, 17 Jun 2017 20:41:42 GMT  
		Size: 2.1 MB (2065460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5978b6b34b3e943e0fd25dfb50991c0bad82a986cfdaa91c4de756431ba679`  
		Last Modified: Wed, 25 Oct 2017 23:28:59 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299a1fbc19bbea84dbf4d0b6e2e71fb847299b017209b1f9783faea14214c995`  
		Last Modified: Thu, 26 Oct 2017 17:07:31 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb76f2dd4162cae82233bc93ba436b63ca37e536d53c85a9f1d7343203e3c383`  
		Last Modified: Thu, 26 Oct 2017 17:07:31 GMT  
		Size: 8.6 KB (8604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac09bb55706d627cf6348c9d0bd891c2fe9a4155aee5d95264b92781371021db`  
		Last Modified: Thu, 26 Oct 2017 17:07:33 GMT  
		Size: 16.7 MB (16726549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e776aa2eebd7dc068e74be7736114ce80966ab2b25478d29763bc1ccf05c3e3`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 5.0 MB (5012317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57d3128b93c0f42a41ad6b2571d41e61c6096e070ee18ef58d34aeaf7318560`  
		Last Modified: Thu, 26 Oct 2017 17:07:29 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484c70be68b7dc1296d1199834238ebabbde1df9ce04ec3cf986a2096ad218b6`  
		Last Modified: Thu, 26 Oct 2017 17:07:29 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01611bf6acbe11966a7f1fe2e96d811430328e24513c20237576287afdd5079a`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f045868d086334dbd06f276dfb93c084fc32b243827527e36c2bc5a5d8583d`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed30107b153ffda65732449b2eea0bdac7dbd4327b3a82ef0fcd5553b0ca55fc`  
		Last Modified: Thu, 26 Oct 2017 17:07:50 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rabbitmq:3-alpine`

```console
$ docker pull rabbitmq@sha256:e49288ac5376cbd8699e6dd2d99410ce12ecd1a5f8885b9f8a1eebd863e3b4ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `rabbitmq:3-alpine` - linux; amd64

```console
$ docker pull rabbitmq@sha256:f8204cb30a089ec4fa99d41ed68f1b520670f5698bea479f6a6582d1926a5715
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23579666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:210310494165d259279503b1b25ecd975f73320e177d472300069bc8619908be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:19:51 GMT
ADD file:1e87ff33d1b6765b793888cd50e01b2bd0dfe152b7dbb4048008bfc2658faea7 in / 
# Wed, 25 Oct 2017 23:19:51 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 03:02:21 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 03:02:25 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 03:02:32 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 03:02:32 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 03:02:33 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 03:02:33 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 03:02:42 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 03:02:42 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 03:02:43 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 03:02:43 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 03:02:44 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 03:02:44 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 03:02:45 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 03:02:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 03:02:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 03:02:45 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:b56ae66c29370df48e7377c8f9baa744a3958058a766793f821dadcb144a4647`  
		Last Modified: Wed, 25 Oct 2017 23:21:25 GMT  
		Size: 2.0 MB (1991435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827e0bce86e3c8fa677ac91f0c55a7a4071cc45c729b171aecbe04d35ae160d7`  
		Last Modified: Thu, 26 Oct 2017 03:03:23 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe01d115cb92dc0ab37de6b6ffa2073ea20d30dfc49c537fbba569cd6a494b8`  
		Last Modified: Thu, 26 Oct 2017 03:03:23 GMT  
		Size: 8.2 KB (8176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bfc0dbbf8b1d2f532779c4873b4c7e0237d6ecc86161b1c6f28e3b6bd3149f`  
		Last Modified: Thu, 26 Oct 2017 03:03:26 GMT  
		Size: 16.6 MB (16561644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b24f4fd26b3494d310561a28e2d9aeb08e7baba442eaef2cd8697c7ebd9d9f1`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 5.0 MB (5012671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfb0f3b402f9674b21d7ed079f6576ec1be80f333f41c404e8ce3feb193b813`  
		Last Modified: Thu, 26 Oct 2017 03:03:22 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521b2b4b2311f153d53f0b9bde9a164f45df9dfd531512c36195ba2ccf5a4c76`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cedbb525e85f1b9257e8b20d04b4ad39f1004c9dfbc673086815dd887f380c3`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f35995cc5f5daa05334d17a87482ac8728aadfb0f10f9d62b3d70f5986e5cc`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:9bbc37dee4951514ff22f2fc83eed327e4fb935baedc146be69d4b7bd04b40b6
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23412846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d5e63a3df176d84fe8622b7515aa144197643b1a5ac6fc5b1578c6d78fb121c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:35 GMT
ADD file:009348222efb3c4ca2e53c387fb34c488679ca07db39525a6c5cc214e46abffd in / 
# Wed, 25 Oct 2017 23:28:36 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:36 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 05:25:53 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 05:25:55 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 05:26:10 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 05:26:10 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 05:26:10 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 05:26:11 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 05:26:19 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 05:26:19 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 05:26:20 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 05:26:20 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 05:26:21 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 05:26:22 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 05:26:22 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 05:26:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 05:26:22 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 05:26:23 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:0864efeeb5cb8dca4eb53e5d6fd38486daee80fa326fe36d1ad254f8fa6bb310`  
		Last Modified: Sun, 23 Jul 2017 20:21:42 GMT  
		Size: 2.0 MB (1965988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda69762aee1588fa82aeabf1af6d6ad24f737cce1451fab2e0199849b1e12e`  
		Last Modified: Wed, 25 Oct 2017 23:28:45 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62a8c5580cc1c2fbf2f9ce119bc0c06403a12ad18167bde2ec94420810916db`  
		Last Modified: Thu, 26 Oct 2017 05:26:38 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b096e39434b5aeddcb2ec167b7bf570cac7b8b16e68324d3f46c6f4d41b69c79`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 8.4 KB (8374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ad9273316fa6f22cd2e8cf88c92f34c3210325fa1be2041153a96f4124476f`  
		Last Modified: Thu, 26 Oct 2017 05:26:41 GMT  
		Size: 16.4 MB (16420180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed982c9e7d5644c85267595b470c0f21f25093a865603ab33304248efdb68b5d`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 5.0 MB (5012332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b76830a9cb5b5f898068945d6af6325c7d97b36d50e521a12097d3e908fd0`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a31f9ee2285379d9d5106926e707698e7a3283f707a4573fec9731e6ede58b5`  
		Last Modified: Thu, 26 Oct 2017 05:26:36 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff38544dc85623170156958b2d5d51604efd94b336b47a6479cde0417667838f`  
		Last Modified: Thu, 26 Oct 2017 05:26:36 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564bee8c5f497342e71777f1adc38d1578f7c95ddefe18efa16fc01b3e7e2a52`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:dcc95a027acff970a00636c77c269b7cc72e3176411c8aecc946eb6642b3906c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23318158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b316c629f8f17231a345cc527fcd76aa75a8b9e012eeae0d0497b3a92c014132`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:58 GMT
ADD file:45b5d3b8d5490ba7edfca2cf6f54cdcf49c772b0b3a2302ce69a7af061007aa4 in / 
# Wed, 25 Oct 2017 23:28:59 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:59 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 13:53:09 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 13:53:13 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 13:53:28 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 13:53:28 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 13:53:29 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 13:53:29 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 13:53:30 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 13:53:30 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 13:53:31 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 13:54:22 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 13:54:23 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 13:54:24 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 13:54:25 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 13:54:26 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 13:54:28 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 13:54:29 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 13:54:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 13:54:30 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 13:54:30 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:bb473f0ebc12fde1bd45c1bd3c46f2d3aab367b1b7739464771455b9972f7894`  
		Last Modified: Thu, 06 Jul 2017 09:54:42 GMT  
		Size: 1.9 MB (1914748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ff6b7ff3a208b8399e701e7ea1b7edbdc654c8c60d33c6f09a7803e2dda776`  
		Last Modified: Wed, 25 Oct 2017 23:29:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05834eac152e30997eb4f1aa4ffe8e952bd759c1a1009bd183dec80dca24cf86`  
		Last Modified: Thu, 26 Oct 2017 13:55:11 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd88a23486b40755f2e1192cb35d4fdaec20831c18ce83da31df3f8aa2f7b45c`  
		Last Modified: Thu, 26 Oct 2017 13:55:11 GMT  
		Size: 8.3 KB (8297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f9ba1206e6e4bfba21cef7f235482b41868ec966d5ebc44a4c4ac432a5fe03`  
		Last Modified: Thu, 26 Oct 2017 13:55:16 GMT  
		Size: 16.4 MB (16376872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5991837e23d785829d605fd052c61e10ed79a7cfb0dfee9dd40d6144bc9fad0f`  
		Last Modified: Thu, 26 Oct 2017 13:55:12 GMT  
		Size: 5.0 MB (5012322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf5663fa552ede671fc5ebf425b2ce3ff5257636b55df9564e556fe7ff85fce`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794d04d767a60fa6df4adb3af1f835701a3c2692e7f6b2d4a9db621a0bc8cd5f`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91155b0cb6bf92d1ab05fb7d13593e0a966eb79dd4e4173e3895d98dffe1c996`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969bbed547aa67091daaa801a46b062fd1c39f7835c81dd5052032056b6cf230`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:3355a334e7313d636e6b3d263a101f1ab926a88bcee118e357835788d527179a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23782989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b83bfaf99c5c91aa3c08ade40b04a3bc1b6bd3725fa905cd0a488133319eef9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:32:08 GMT
ADD file:4a952fc4b81d50b342e26a818dac48a148a4d5eddb878219650e579a5c9faeaa in / 
# Wed, 25 Oct 2017 23:32:08 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:32:08 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 10:44:24 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 10:44:28 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 10:44:50 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 10:44:50 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 10:44:51 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 10:44:51 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 10:45:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 10:45:05 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 10:45:06 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 10:45:06 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 10:45:07 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 10:45:07 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 10:45:08 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 10:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 10:45:08 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 10:45:08 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:ffe4428ef008913a7ec63449e4ad3aa536b26103943146a302591dfceb157d2f`  
		Last Modified: Sat, 17 Jun 2017 18:08:13 GMT  
		Size: 2.0 MB (2045593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4fe786260f2bd2710289e7c9487b423cb252a691fa501759b0768516122869`  
		Last Modified: Wed, 25 Oct 2017 23:32:27 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cf0f0a132c9bb882206147dffad08dc780f2bc82556cfbda9878a3218f1e7c`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00a9186496c6602ccd3efb4bb1780b42adb7028c8fa3cd3c1ff2f10bcfa33a3`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 8.3 KB (8305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc19938c3bf2e858347a9c7add1beac38af5a4f83b99d80ddc004aa4ad51e596`  
		Last Modified: Thu, 26 Oct 2017 10:45:30 GMT  
		Size: 16.7 MB (16710838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697b9a0ea77c953a543f168ba09045ae412f3b2bd0947b2bba8c18cd0cd2c70b`  
		Last Modified: Thu, 26 Oct 2017 10:45:30 GMT  
		Size: 5.0 MB (5012335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca279d1203917e8f98e0d5fe3f9de9bdde74bae202990b6388e1cc748caa726`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb3c81d25b2aa6fa5bf57aaf5f8ad6a5f27be02727e454818ff546e5a989c88`  
		Last Modified: Thu, 26 Oct 2017 10:45:29 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420233201c5d7a33d69bc90b4ac40d5db1285e61718701ffd97d4db8396a9508`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0b37b1c6d397d7b0daa633cac4b2d202e9656dd6340dc40496303190ed4a78`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:2a7e105872a021c9e0df106fd62ee50b80be17634c3b713596ca188b8ab3cf04
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23639927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01e565612a099b2324e2f273a6a14a62e8cab609839bdeb205adc72571cb62b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:47 GMT
ADD file:e0be8616517d68cb80a2f9b74eb967cda22b9937bbcbe8b75b6153815a6f7761 in / 
# Wed, 25 Oct 2017 23:28:48 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:50 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 07:12:01 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 07:12:12 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 07:12:36 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 07:12:37 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 07:12:39 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 07:12:41 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 07:12:42 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 07:12:44 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 07:12:45 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 07:13:07 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 07:13:09 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 07:13:13 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 07:13:15 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 07:13:19 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 07:13:23 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 07:13:25 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 07:13:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 07:13:28 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 07:13:30 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:1e52418956f7d2a8ea35e8e6e3318fd08e005b27457d77868c225e7433bbfa02`  
		Last Modified: Thu, 20 Jul 2017 15:12:59 GMT  
		Size: 2.0 MB (2008578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf472f4e5bb7956ac20bb343b304e1d3de1f79160c0d158cccbe25980022d50`  
		Last Modified: Wed, 25 Oct 2017 23:29:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48c95ed960185dbd69324a206614e723f0086f80b46bd3223f233e4f1e278bc`  
		Last Modified: Thu, 26 Oct 2017 07:14:01 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a8242358db9adbde1a17b0e2b320c02112fcefa90d397ecc028a9729efcf94`  
		Last Modified: Thu, 26 Oct 2017 07:14:01 GMT  
		Size: 9.1 KB (9059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6db9581873eb0cadddc4d474e33cb2ec978c0d68e3ea124ce4f07ab2731d79`  
		Last Modified: Thu, 26 Oct 2017 07:14:04 GMT  
		Size: 16.6 MB (16603134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a991ac52f27ddaf9fb4021acf59b12957c4fa6251ab4d74159bb54ac63878009`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 5.0 MB (5013168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d098ea301752e2203c7ad872d2a38cc3da3efa183b01e61fe5c2fcde29efceb8`  
		Last Modified: Thu, 26 Oct 2017 07:14:00 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8727c952955dcfc3ce7e96c808c78bc91d43e6033164a46a7faffd11dc22fb69`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fe10e7f312fce5a9bf6ca051d683f86b1cef271217890a7ea53164ef81c99d`  
		Last Modified: Thu, 26 Oct 2017 07:13:58 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcba876c6e465f99a2952b71be993ce0d4d82ef4f70f72a59e58200cf263252f`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:85a850d9b872c722bace7014c60c183a5746e338d9136a8319c91c3d2fb6a778
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23818845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45af14c4c176512dfc8deb7275c6c333b0f5933fff4eab2e34c6d8f888d40be2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:40 GMT
ADD file:6fbdff4b4c08600e192f5da9b67a02c58759237fb40525d70712104c80c34c48 in / 
# Wed, 25 Oct 2017 23:28:40 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:40 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 17:06:39 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 17:06:42 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 17:06:55 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 17:06:56 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 17:06:57 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 17:06:57 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 17:07:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 17:07:05 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 17:07:06 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 17:07:06 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 17:07:06 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 17:07:07 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 17:07:07 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 17:07:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 17:07:08 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 17:07:08 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:d45fd9d3c4f188ab1f3a4bf6a9f5202b3f1577dbb998f5f28e82d192e0c1f0e7`  
		Last Modified: Sat, 17 Jun 2017 20:41:42 GMT  
		Size: 2.1 MB (2065460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5978b6b34b3e943e0fd25dfb50991c0bad82a986cfdaa91c4de756431ba679`  
		Last Modified: Wed, 25 Oct 2017 23:28:59 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299a1fbc19bbea84dbf4d0b6e2e71fb847299b017209b1f9783faea14214c995`  
		Last Modified: Thu, 26 Oct 2017 17:07:31 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb76f2dd4162cae82233bc93ba436b63ca37e536d53c85a9f1d7343203e3c383`  
		Last Modified: Thu, 26 Oct 2017 17:07:31 GMT  
		Size: 8.6 KB (8604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac09bb55706d627cf6348c9d0bd891c2fe9a4155aee5d95264b92781371021db`  
		Last Modified: Thu, 26 Oct 2017 17:07:33 GMT  
		Size: 16.7 MB (16726549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e776aa2eebd7dc068e74be7736114ce80966ab2b25478d29763bc1ccf05c3e3`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 5.0 MB (5012317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57d3128b93c0f42a41ad6b2571d41e61c6096e070ee18ef58d34aeaf7318560`  
		Last Modified: Thu, 26 Oct 2017 17:07:29 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484c70be68b7dc1296d1199834238ebabbde1df9ce04ec3cf986a2096ad218b6`  
		Last Modified: Thu, 26 Oct 2017 17:07:29 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01611bf6acbe11966a7f1fe2e96d811430328e24513c20237576287afdd5079a`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f045868d086334dbd06f276dfb93c084fc32b243827527e36c2bc5a5d8583d`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rabbitmq:3-management`

```console
$ docker pull rabbitmq@sha256:90b467d41e6655bb52d7114802c028eb359e220a7ec87c98a23a294af2b81ad4
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

### `rabbitmq:3-management` - linux; amd64

```console
$ docker pull rabbitmq@sha256:40a956f5198d4d2050d1545dc48bf38b5e0342c33d10bcd04c9e0a7e7bc851af
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.9 MB (62852369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ac724eab06670229b033f2516a2e3af2cdfb453495a9bbb040fea13b398ab5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:33:42 GMT
ADD file:45233d6b5c9b91e9437065d3e7c332d1c4eb4bce8e1079a4c1af342c450abe67 in / 
# Mon, 09 Oct 2017 21:33:43 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 02:41:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:41:43 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 02:41:43 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 02:42:10 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 02:42:40 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 02:42:41 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 02:42:42 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 02:43:16 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:43:16 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 02:43:17 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 02:43:17 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 02:43:18 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 02:43:19 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 13 Oct 2017 23:40:43 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 13 Oct 2017 23:40:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 13 Oct 2017 23:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2017 23:40:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 13 Oct 2017 23:40:45 GMT
CMD ["rabbitmq-server"]
# Fri, 13 Oct 2017 23:40:56 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 13 Oct 2017 23:40:57 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:bc95e04b23c06ba1b9bf092d07d1493177b218e0340bd2ed49dac351c1e34313`  
		Last Modified: Mon, 09 Oct 2017 21:42:28 GMT  
		Size: 22.5 MB (22492350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65f0b00e4cfb1535d0f4e7a63707172ae63483fb33140d777614f199afcb36`  
		Last Modified: Tue, 10 Oct 2017 02:43:59 GMT  
		Size: 4.5 MB (4498726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bd803179890909fcae186044c0e6ca1bc1d34e5fc05ef1ccea823e7be97540`  
		Last Modified: Tue, 10 Oct 2017 02:43:57 GMT  
		Size: 4.1 KB (4069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b05ca8302833edf783c50f03cd7ba0b8e12bc872b053eda3e3ae7e1f17e2b4b`  
		Last Modified: Tue, 10 Oct 2017 02:43:58 GMT  
		Size: 952.1 KB (952058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb5a4bbcce5a040eb83057f9e93d17663bb123f4e98168457444497f7d17b70`  
		Last Modified: Tue, 10 Oct 2017 02:44:03 GMT  
		Size: 27.7 MB (27703883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf840d8999f6fe46a162974c82378c38b3cf3dcccbbaff848c0fb199988aebe0`  
		Last Modified: Tue, 10 Oct 2017 02:44:00 GMT  
		Size: 7.2 MB (7194403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be339ca44883b1990e52771487402163d398a279755a501fdd8891ec71cf09d0`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce35cd9f9b5b917868095b3b074dd23d18e0e266f3ee68ff95e2c61467299812`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fe32a0a00d916ed4d632aae71d35d9d0baa5e5910d6bd179a24071c35bedb0`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77408ca9e94eb4bfeb346ab10c602857525802c2279e7c6995fcdbc90269444a`  
		Last Modified: Fri, 13 Oct 2017 23:41:26 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db03407a1aba1c0a89dffe960394aae639885702e3faa65271b918c36c7905cd`  
		Last Modified: Fri, 13 Oct 2017 23:41:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b908f008ac2afe6632caccd124e3ee9bffd5ebcdb8ca5ca84ae7e014305e460f`  
		Last Modified: Fri, 13 Oct 2017 23:42:01 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management` - linux; arm variant v5

```console
$ docker pull rabbitmq@sha256:07150eac8a231b8c043f29aba9a9ba3d81aa4cdd16c8e3387621deb4d8fdf1f4
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58432562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00088686092d95f6db193285835d1af5662557d679f57a4c21d1d4ec648c0924`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:44:48 GMT
ADD file:ff9945b48b1ac236dcec24eb9dfaf52b7c151a3b11c8502391f0866dfb4e3ac3 in / 
# Mon, 09 Oct 2017 21:44:48 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 00:18:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:18:11 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 00:18:11 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 00:18:29 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 00:18:58 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:18:58 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 00:18:58 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 00:19:26 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:19:26 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 00:19:27 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 00:19:28 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 00:19:29 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 00:19:30 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Sat, 14 Oct 2017 14:14:24 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Sat, 14 Oct 2017 14:14:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 14 Oct 2017 14:14:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 Oct 2017 14:14:25 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Sat, 14 Oct 2017 14:14:26 GMT
CMD ["rabbitmq-server"]
# Sat, 14 Oct 2017 14:14:34 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Sat, 14 Oct 2017 14:14:34 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:836d5b6056a9815be79c76480a90299267f60201bd1e3396817003e6c14819cc`  
		Last Modified: Mon, 09 Oct 2017 21:50:56 GMT  
		Size: 21.2 MB (21166251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb896fba83bd09a35c68457554b35289860c23c46f27a8c3ef42f13146ebba1`  
		Last Modified: Tue, 10 Oct 2017 00:20:01 GMT  
		Size: 4.2 MB (4231979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61827a16c114b9741d761aa4c60a972ffe1e0b60147794e86b05653d67822e91`  
		Last Modified: Tue, 10 Oct 2017 00:20:00 GMT  
		Size: 4.1 KB (4079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877cd9511def30e56a5ce354e145e8a2b1a93daaae7eaaa42dc4219838aa1743`  
		Last Modified: Tue, 10 Oct 2017 00:20:00 GMT  
		Size: 942.8 KB (942752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea9e378899e98c99e93ae2d0874bd5d89e24134bd14a19c285bdf39a0a42ade`  
		Last Modified: Tue, 10 Oct 2017 00:20:05 GMT  
		Size: 25.2 MB (25170810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc82a29314b16531aa2172ac523ba535e3678f85efdd699164fbb0241ab8b62`  
		Last Modified: Tue, 10 Oct 2017 00:20:01 GMT  
		Size: 6.9 MB (6909811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c44a3d016cf9de95021782180a42d3660e20fc7d8e92a7fe5ce9ede7928ca2`  
		Last Modified: Tue, 10 Oct 2017 00:19:59 GMT  
		Size: 2.3 KB (2261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abfdcdd98b40291ad91791bea09bf277e75c3669c6607c7891b09130101bfa3`  
		Last Modified: Tue, 10 Oct 2017 00:19:58 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a72811da4bf8ca8a2d06cdc182aa54116bb12133e8d82ef2b018a8de29ed74`  
		Last Modified: Tue, 10 Oct 2017 00:19:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147d8cf0897dea9b024bf5c6efb6873db3d86dec857fca062b146f88b7b5a735`  
		Last Modified: Sat, 14 Oct 2017 14:14:43 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f355fd0b70caedf30aa384298307b8e40d922e9e341492dd3fde71f119fd7d7`  
		Last Modified: Sat, 14 Oct 2017 14:14:44 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77dcaa76990445223000f8a5eb10485f94e82d4817f74f142f106b0a4dd9ad0c`  
		Last Modified: Sat, 14 Oct 2017 14:15:02 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:353fc3a4b10cc0fd93baf80287c8e7c779c49d7fd5421091aa004286b3bf559c
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55688342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd5c488f599ef650e2dc6824d489473db268160f94789b74f5ec312eef58600d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:43 GMT
ADD file:b758c6c3ff989778bd740dde35c86b953fa09be913a7e02711b2881de6b8911d in / 
# Mon, 09 Oct 2017 21:45:44 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 13:07:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:07:42 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 13:07:42 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 13:07:58 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 13:08:17 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:08:17 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 13:08:17 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 13:08:39 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:08:39 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 13:08:40 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 13:08:41 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 13:08:42 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 13:08:43 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 13:08:43 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 13:08:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 13:08:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 13:08:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 13:08:45 GMT
CMD ["rabbitmq-server"]
# Fri, 03 Nov 2017 13:09:01 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 03 Nov 2017 13:09:01 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:59e81a3fde58ec8d4b8f2f58b98ef2f4d951d37dd9b99b016fd294a8e07d7796`  
		Last Modified: Mon, 09 Oct 2017 21:52:49 GMT  
		Size: 19.3 MB (19277135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2037b99f3c3dc51e8ace39aed9971155f34f325ac4f0a1e56a07c4d6c02f5ae6`  
		Last Modified: Fri, 03 Nov 2017 13:09:18 GMT  
		Size: 3.9 MB (3868347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f368172ea96bda944832762ad29b52dfe17ec5e6fae96eee37adc4e9d68674a5`  
		Last Modified: Fri, 03 Nov 2017 13:09:16 GMT  
		Size: 4.1 KB (4084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893cc1ae60f8bf72ac3020ccc60b22d9e0ad0cb0647e15bc4847d08c8985eee2`  
		Last Modified: Fri, 03 Nov 2017 13:09:16 GMT  
		Size: 926.1 KB (926097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13220cc1a683014bda9cfae7f7ee7015a26b28048f90f5aa3ed8b6a96f4b2813`  
		Last Modified: Fri, 03 Nov 2017 13:09:20 GMT  
		Size: 24.8 MB (24785610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269f4e069126132643c1c0be1faf600d55ff15e870066c527d03181904d99c5d`  
		Last Modified: Fri, 03 Nov 2017 13:09:17 GMT  
		Size: 6.8 MB (6820180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ae244f4f610a339fcbddf37612a15ec7b7f6674e3d888c3c4d36302283418e`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce7d85327b7bc7d59a7b54222a3e6babd7f8afd8eb080becb77fc52aed5a751`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dfa32e4b49700ed0130ebd563f40a2c381393983b571a9886435813102ad0c`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba15cd885dc21f438d366b40d0d9f595f2c25e063c60fa590ab4c0f6233ff94`  
		Last Modified: Fri, 03 Nov 2017 13:09:14 GMT  
		Size: 4.0 KB (4040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978a8434497fcb8e08cefc7484b515ac34fe23c281fb869d015f62b54673028c`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34fa59eaf946f8e35134f1a0bf195874868c3ce1e2a025350fc57efe60ecbea`  
		Last Modified: Fri, 03 Nov 2017 13:09:54 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:4ad104ab7b291ca9aea4bb42e18de213ae21ef6a655d909c3568e2b36f465074
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57278563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9356e7f3d3e445f04242803fb4b5afb70fad5f726388635b781f4814733c3af7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:47:55 GMT
ADD file:3a528355cfc75437716aff3b517ef99ae602918d84d26dbafff0ed142248fb93 in / 
# Mon, 09 Oct 2017 21:47:56 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 04:57:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 04:57:04 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 04:57:05 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 04:57:37 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 04:58:35 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 04:58:36 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 04:58:37 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 04:58:37 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 04:58:38 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 04:58:39 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 04:58:39 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 05:00:22 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 05:00:23 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 05:00:25 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 05:00:26 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 05:00:28 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 05:00:31 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Sat, 14 Oct 2017 13:52:47 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Sat, 14 Oct 2017 13:52:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 14 Oct 2017 13:52:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 Oct 2017 13:52:51 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Sat, 14 Oct 2017 13:52:51 GMT
CMD ["rabbitmq-server"]
# Sat, 14 Oct 2017 13:53:08 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Sat, 14 Oct 2017 13:53:09 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:e907afd6e25615a4d3eb554d930cef57b87e79ec82413889c2eac38beb4eb8f7`  
		Last Modified: Mon, 09 Oct 2017 22:03:08 GMT  
		Size: 20.3 MB (20337143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5e6d35928560b933b85b5a3f2a8e96b4520fbb8df138b3e739e56d0c1f355`  
		Last Modified: Tue, 10 Oct 2017 05:01:18 GMT  
		Size: 4.1 MB (4073554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a862ab821b342790326492507ca5d70bfb7016bef765606193f1f7139f60c5ed`  
		Last Modified: Tue, 10 Oct 2017 05:01:14 GMT  
		Size: 4.1 KB (4072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92799a54920b79013733790e444f13d8c65faa29c79cbdaf1bc8af85f637a233`  
		Last Modified: Tue, 10 Oct 2017 05:01:14 GMT  
		Size: 919.5 KB (919487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b119999eef1bcadabedd3a5319b03c6b83ede91ba8535059851547d3433b205`  
		Last Modified: Tue, 10 Oct 2017 05:01:19 GMT  
		Size: 25.0 MB (25042572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62f8525a3a982a102aa37bb3313876195b15d8781cd253ed238dd2b9dff151`  
		Last Modified: Tue, 10 Oct 2017 05:01:15 GMT  
		Size: 6.9 MB (6894852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc028e70f04f6ea4365223a1cfe4e5c4384d5921acac419f3c170b148f7c7bf`  
		Last Modified: Tue, 10 Oct 2017 05:01:10 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e99faa03c2a8a272f56208c644c12b384b69dea50be6da9f6be400c14b945c`  
		Last Modified: Tue, 10 Oct 2017 05:01:12 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8fa260bcaa52d81ba20c11111f8d15bab954b17b48666724536c604220d94e`  
		Last Modified: Tue, 10 Oct 2017 05:01:11 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306840de948d03472918a306c089409429606802ec8cf841e96dec707a2f7178`  
		Last Modified: Sat, 14 Oct 2017 13:53:27 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a7a978032478b38adb1f0107466d187e53380f7037d058c62e4937cd07fc09`  
		Last Modified: Sat, 14 Oct 2017 13:53:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3facaa930064fd14fbd9a077b63e5f3261d1e63bd15c3d1426575c6c4f8eca`  
		Last Modified: Sat, 14 Oct 2017 13:54:17 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management` - linux; 386

```console
$ docker pull rabbitmq@sha256:16ab1fd6ebf60e7fe32149ac86bf79cd5a2e2d573dec3267fd0d7d646514384c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63902453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a8039a2961a84491da6ac62bad7d9b065b333750e66543f8e7cf931c13ed028`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:36 GMT
ADD file:6582536277127947668f7bfdc1471a4e36170915b91a4cb841e7e1bfa1de6535 in / 
# Mon, 09 Oct 2017 21:45:36 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 10:45:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:45:12 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 10:45:13 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 10:45:28 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 10:46:03 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 10:46:04 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 10:46:25 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:46:25 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 10:46:26 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 10:46:27 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 10:46:27 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 10:46:28 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 10:46:28 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 10:46:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 10:46:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 10:46:30 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 10:46:30 GMT
CMD ["rabbitmq-server"]
# Fri, 03 Nov 2017 10:46:58 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 03 Nov 2017 10:46:58 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:b2b52fe46b29fe5d0689f26449c2114e40f0731d4ce3eb8c3941397b74205432`  
		Last Modified: Mon, 09 Oct 2017 21:53:42 GMT  
		Size: 23.1 MB (23128678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d407b136da0731f5f38279001e9dd426217937443cad0f16e1f242366290773`  
		Last Modified: Fri, 03 Nov 2017 10:47:13 GMT  
		Size: 4.8 MB (4803637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c93817e78345b4b5070c81e5a37d02afc2b5fe347a1a4bf59e09f6084814fd2`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 4.1 KB (4057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97eae59c75f8f814ab781f5239ac2e132b7b65c77e75b35023c603c539ca54f`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 931.5 KB (931524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aed670dee19fde6946658d7129e13520c1a0747f8b80b6f92dac5f6d974ae52`  
		Last Modified: Fri, 03 Nov 2017 10:47:24 GMT  
		Size: 27.8 MB (27818690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b61d6d0b60ec18280aeba946a05d62817afbe030f277af85b5f434021e90c9`  
		Last Modified: Fri, 03 Nov 2017 10:47:16 GMT  
		Size: 7.2 MB (7208985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec7d4cc3b5497bbbd6b2d1e9574dbedb6c7ad11805cff4c287ea444ddc2e298`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 2.3 KB (2259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eec554591344f78e35e3976d002d617623a52d123fc71e65d33c4d533d2b2e7`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e433f73af1167eff0dee1984c095bf5be36593fcead5b8cc820e2cb829aaed0`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8d6e0dbdbb04b44f7a0972fce6b0b1b19262e4fc5416bd1589af560f16c99f`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 4.0 KB (4040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bab08cf9b00d8109139e1cb1cdec448b71fdae7d7f1260d4175771416a5f80`  
		Last Modified: Fri, 03 Nov 2017 10:47:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2aad62bc4e7f6b9b68a5196e492b29083b8ab4e68dfea4a93b469cb79aae29`  
		Last Modified: Fri, 03 Nov 2017 10:48:04 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:47fb5bf4afd56afb9e9ab383f1449cee19c3ab7a7e653d0b04037cf839cfab52
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60384672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c4dbfbbd301b5dbb171ca49da8419b76567c7aa2d00978e12759ced95ca846`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:56 GMT
ADD file:7edf73437495be24244c16841b563be06c15452963f41ac940fb5e105ed96027 in / 
# Mon, 09 Oct 2017 21:45:58 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 07:12:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:12:51 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 07:12:53 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 07:13:49 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 07:15:26 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:15:28 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 07:15:29 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 07:15:31 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 07:15:33 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 07:15:34 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 07:15:35 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 07:16:54 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:16:55 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 07:17:00 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 07:17:01 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 07:17:06 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 07:17:11 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 07:17:13 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 07:17:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 07:17:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 07:17:21 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 07:17:23 GMT
CMD ["rabbitmq-server"]
# Fri, 03 Nov 2017 07:17:36 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 03 Nov 2017 07:17:39 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:c4860466fa1e6824151f4fa3a51ef0e9d7d3c3ba860e21d94e69988b65601260`  
		Last Modified: Mon, 09 Oct 2017 21:52:59 GMT  
		Size: 22.7 MB (22746217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebe4c87dcd1f7ef11d4d21752831bf4095ac42afe041706c35f1d7d4d0ca4f2`  
		Last Modified: Fri, 03 Nov 2017 07:18:05 GMT  
		Size: 4.4 MB (4360529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e5365525084de1c85fa29ef33d37c38b5f80621f5bcb26bb4882d71598c6f7`  
		Last Modified: Fri, 03 Nov 2017 07:18:03 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600c3853740b7f4cff9cc799ae478f669bd54277a8dd375479a34ed1bb47a803`  
		Last Modified: Fri, 03 Nov 2017 07:18:02 GMT  
		Size: 920.7 KB (920695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993868ec534130e348e45aa6d64b471fa46eafbf061836cc9d2a56edf73e9382`  
		Last Modified: Fri, 03 Nov 2017 07:18:06 GMT  
		Size: 25.5 MB (25492533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca1b92e212aaef163244d5fdd9e135fdb8be8c9dbbb626061ee2882d941a553`  
		Last Modified: Fri, 03 Nov 2017 07:18:03 GMT  
		Size: 6.9 MB (6853702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483f96d1f500f9f69170bc6927d599a7f0cd1550f96b6ee3f90eb4185a1bffb`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b433db63f40c7cab3080cf36bd7beabbdf7d9eece3f2dc16a65b900c61180`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93971551a2c911c34ca2e9af47495efb2f27e2922e567d93dd94dfb9b773bd3`  
		Last Modified: Fri, 03 Nov 2017 07:17:58 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5494bb8bcc45452a84c216edffedb3103a15c3e209aba0561dfbc70e4312192e`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 4.0 KB (4039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d56b2a4f9f8d7b11831a8f1952fe2c02613bcb014ab9d756b70b3b398b37269`  
		Last Modified: Fri, 03 Nov 2017 07:17:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e2264063017ef705c9dcc066695ab771b32f19f38ba34c158531e7d3f4c9fc`  
		Last Modified: Fri, 03 Nov 2017 07:18:40 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management` - linux; s390x

```console
$ docker pull rabbitmq@sha256:35d9ecb54b432f7591ecfe0cb1ee71d152199b0ae07ecdd8c9b21cd6a87b0a51
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60364970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a628fac494ad4d163ad91471c151b4ed5bcfbe2f318bc677224413d944cf4ce8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:44:35 GMT
ADD file:ae4aaa6affe22f36ab5478771d5c84917f72de7a8dac16345a035709a1a5edf4 in / 
# Mon, 09 Oct 2017 21:44:36 GMT
CMD ["bash"]
# Thu, 02 Nov 2017 17:06:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 17:06:41 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Thu, 02 Nov 2017 17:06:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 02 Nov 2017 17:07:21 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Thu, 02 Nov 2017 17:07:43 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 02 Nov 2017 17:07:44 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 02 Nov 2017 17:07:45 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 17:07:48 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 17:07:48 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 17:07:49 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 17:07:50 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 17:07:52 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 17:07:53 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 17:07:54 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 17:07:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 17:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 17:07:57 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 17:07:57 GMT
CMD ["rabbitmq-server"]
# Fri, 03 Nov 2017 17:08:14 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 03 Nov 2017 17:08:15 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:671716cc49517eef5f430c695ce344d63e390cb65f58d30939f2ba615c953686`  
		Last Modified: Mon, 09 Oct 2017 21:49:09 GMT  
		Size: 22.3 MB (22339951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cae61f12be6f01ba06573d9393712e91821cd5496302310f550fe5842dea557`  
		Last Modified: Fri, 03 Nov 2017 17:08:41 GMT  
		Size: 4.5 MB (4529879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca307103ce923e7e89d35185be4df8e54c3c0b54d259b8880aa7bae107d4952`  
		Last Modified: Fri, 03 Nov 2017 17:08:39 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d16320f9fc35ea20ba7fb9b21f88e3f0f06c52d416682319f3b2a85a345a3d5`  
		Last Modified: Fri, 03 Nov 2017 17:08:39 GMT  
		Size: 938.0 KB (938019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801205b182b8d6f7acf36200b2ba07ed52ea224dfefe792b525224e4aacb4d4a`  
		Last Modified: Fri, 03 Nov 2017 17:08:48 GMT  
		Size: 25.6 MB (25619372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9cb605e6242f5ab505cbd229c7b2fdf2935a6254130070c12c4d8413616024`  
		Last Modified: Fri, 03 Nov 2017 17:08:40 GMT  
		Size: 6.9 MB (6926791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2799e1b1479136fbb3c3ba6df318d449990a3cf5fc3293a14142cde0d9f51980`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a6d5de3e6aaa1c06122a1b5cda3b4bcb98d54e5dc23f38896fc81e98cea769`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172fa2e52818dcedf69c727f6790f0f9744f8538da3f4222602aaa0ab9fa82c0`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c734f2707800c1189521a51409fed1508fb7e36c6e67eca5537d03c4b24ef0d`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 4.0 KB (4037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e7d712f1155d66243480cd441ec04e084a8e7e2d6a0653e27138b31b56d2ae`  
		Last Modified: Fri, 03 Nov 2017 17:08:38 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9489f6c1d1f9d4090b7d9220b20aac5cc7e9588c9ddf66d0357f1eb8226071`  
		Last Modified: Fri, 03 Nov 2017 17:09:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rabbitmq:3-management-alpine`

```console
$ docker pull rabbitmq@sha256:cc6bb38a4167c70483b6f174d43bf43032a23b1d9c661530cfda228bf60e3f87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `rabbitmq:3-management-alpine` - linux; amd64

```console
$ docker pull rabbitmq@sha256:ef2b9b2cbfbe00330d8cfaaf8acef1127996756ee66bad0ac832aba8e63ae67f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23579858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4927e0fd02a40ab3ffc333a1326f9a21be7aec9059d82c2dfdc37580847a76f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:19:51 GMT
ADD file:1e87ff33d1b6765b793888cd50e01b2bd0dfe152b7dbb4048008bfc2658faea7 in / 
# Wed, 25 Oct 2017 23:19:51 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 03:02:21 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 03:02:25 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 03:02:32 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 03:02:32 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 03:02:33 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 03:02:33 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 03:02:42 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 03:02:42 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 03:02:43 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 03:02:43 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 03:02:44 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 03:02:44 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 03:02:45 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 03:02:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 03:02:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 03:02:45 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 03:02:59 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 03:02:59 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:b56ae66c29370df48e7377c8f9baa744a3958058a766793f821dadcb144a4647`  
		Last Modified: Wed, 25 Oct 2017 23:21:25 GMT  
		Size: 2.0 MB (1991435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827e0bce86e3c8fa677ac91f0c55a7a4071cc45c729b171aecbe04d35ae160d7`  
		Last Modified: Thu, 26 Oct 2017 03:03:23 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe01d115cb92dc0ab37de6b6ffa2073ea20d30dfc49c537fbba569cd6a494b8`  
		Last Modified: Thu, 26 Oct 2017 03:03:23 GMT  
		Size: 8.2 KB (8176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bfc0dbbf8b1d2f532779c4873b4c7e0237d6ecc86161b1c6f28e3b6bd3149f`  
		Last Modified: Thu, 26 Oct 2017 03:03:26 GMT  
		Size: 16.6 MB (16561644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b24f4fd26b3494d310561a28e2d9aeb08e7baba442eaef2cd8697c7ebd9d9f1`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 5.0 MB (5012671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfb0f3b402f9674b21d7ed079f6576ec1be80f333f41c404e8ce3feb193b813`  
		Last Modified: Thu, 26 Oct 2017 03:03:22 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521b2b4b2311f153d53f0b9bde9a164f45df9dfd531512c36195ba2ccf5a4c76`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cedbb525e85f1b9257e8b20d04b4ad39f1004c9dfbc673086815dd887f380c3`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f35995cc5f5daa05334d17a87482ac8728aadfb0f10f9d62b3d70f5986e5cc`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f1f0f842cbbd9046d7b95afc926b8e22e4befd18e38ed5d4514e14105d2be`  
		Last Modified: Thu, 26 Oct 2017 03:04:25 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:e8e0295fdf1734258af64b4f82784721e845b6a68146965bd1592c0e15c58d1a
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23413037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1379abcce7a4a22ec254dfd3fe56547de4c89c0b12cfaf5e044ea05c4205dfb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:35 GMT
ADD file:009348222efb3c4ca2e53c387fb34c488679ca07db39525a6c5cc214e46abffd in / 
# Wed, 25 Oct 2017 23:28:36 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:36 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 05:25:53 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 05:25:55 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 05:26:10 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 05:26:10 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 05:26:10 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 05:26:11 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 05:26:19 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 05:26:19 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 05:26:20 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 05:26:20 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 05:26:21 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 05:26:22 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 05:26:22 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 05:26:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 05:26:22 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 05:26:23 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 05:26:30 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 05:26:30 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:0864efeeb5cb8dca4eb53e5d6fd38486daee80fa326fe36d1ad254f8fa6bb310`  
		Last Modified: Sun, 23 Jul 2017 20:21:42 GMT  
		Size: 2.0 MB (1965988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda69762aee1588fa82aeabf1af6d6ad24f737cce1451fab2e0199849b1e12e`  
		Last Modified: Wed, 25 Oct 2017 23:28:45 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62a8c5580cc1c2fbf2f9ce119bc0c06403a12ad18167bde2ec94420810916db`  
		Last Modified: Thu, 26 Oct 2017 05:26:38 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b096e39434b5aeddcb2ec167b7bf570cac7b8b16e68324d3f46c6f4d41b69c79`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 8.4 KB (8374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ad9273316fa6f22cd2e8cf88c92f34c3210325fa1be2041153a96f4124476f`  
		Last Modified: Thu, 26 Oct 2017 05:26:41 GMT  
		Size: 16.4 MB (16420180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed982c9e7d5644c85267595b470c0f21f25093a865603ab33304248efdb68b5d`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 5.0 MB (5012332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b76830a9cb5b5f898068945d6af6325c7d97b36d50e521a12097d3e908fd0`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a31f9ee2285379d9d5106926e707698e7a3283f707a4573fec9731e6ede58b5`  
		Last Modified: Thu, 26 Oct 2017 05:26:36 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff38544dc85623170156958b2d5d51604efd94b336b47a6479cde0417667838f`  
		Last Modified: Thu, 26 Oct 2017 05:26:36 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564bee8c5f497342e71777f1adc38d1578f7c95ddefe18efa16fc01b3e7e2a52`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fe4d4545d22113e1fa0e2fbc7ae69364213b6ca264274a71ad66ac045835d1`  
		Last Modified: Thu, 26 Oct 2017 05:26:49 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:bf020d55089aa6f03eb3e259eefa2014a2191041616b46f4c7e56fd10fd09b76
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23318349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67e8f6bc203146953e13d3ce7086f40a6796ae711f8d8231aac5693d99175f9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:58 GMT
ADD file:45b5d3b8d5490ba7edfca2cf6f54cdcf49c772b0b3a2302ce69a7af061007aa4 in / 
# Wed, 25 Oct 2017 23:28:59 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:59 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 13:53:09 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 13:53:13 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 13:53:28 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 13:53:28 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 13:53:29 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 13:53:29 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 13:53:30 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 13:53:30 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 13:53:31 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 13:54:22 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 13:54:23 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 13:54:24 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 13:54:25 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 13:54:26 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 13:54:28 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 13:54:29 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 13:54:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 13:54:30 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 13:54:30 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 13:54:47 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 13:54:47 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:bb473f0ebc12fde1bd45c1bd3c46f2d3aab367b1b7739464771455b9972f7894`  
		Last Modified: Thu, 06 Jul 2017 09:54:42 GMT  
		Size: 1.9 MB (1914748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ff6b7ff3a208b8399e701e7ea1b7edbdc654c8c60d33c6f09a7803e2dda776`  
		Last Modified: Wed, 25 Oct 2017 23:29:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05834eac152e30997eb4f1aa4ffe8e952bd759c1a1009bd183dec80dca24cf86`  
		Last Modified: Thu, 26 Oct 2017 13:55:11 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd88a23486b40755f2e1192cb35d4fdaec20831c18ce83da31df3f8aa2f7b45c`  
		Last Modified: Thu, 26 Oct 2017 13:55:11 GMT  
		Size: 8.3 KB (8297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f9ba1206e6e4bfba21cef7f235482b41868ec966d5ebc44a4c4ac432a5fe03`  
		Last Modified: Thu, 26 Oct 2017 13:55:16 GMT  
		Size: 16.4 MB (16376872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5991837e23d785829d605fd052c61e10ed79a7cfb0dfee9dd40d6144bc9fad0f`  
		Last Modified: Thu, 26 Oct 2017 13:55:12 GMT  
		Size: 5.0 MB (5012322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf5663fa552ede671fc5ebf425b2ce3ff5257636b55df9564e556fe7ff85fce`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794d04d767a60fa6df4adb3af1f835701a3c2692e7f6b2d4a9db621a0bc8cd5f`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91155b0cb6bf92d1ab05fb7d13593e0a966eb79dd4e4173e3895d98dffe1c996`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969bbed547aa67091daaa801a46b062fd1c39f7835c81dd5052032056b6cf230`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1643075e82e89fd6745e0baa4b9fd436da4f959fffedec9f0d149f84a7c16f8f`  
		Last Modified: Thu, 26 Oct 2017 13:56:10 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:775482d2d2f81b04a7f91840ed0a169b185315f4dc226d515adaacb675e6f6dc
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23783181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:845026f49dc450aaf8e569e45ba76c8b1bf506da17e742b0a54fbddaf5bcf9f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:32:08 GMT
ADD file:4a952fc4b81d50b342e26a818dac48a148a4d5eddb878219650e579a5c9faeaa in / 
# Wed, 25 Oct 2017 23:32:08 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:32:08 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 10:44:24 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 10:44:28 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 10:44:50 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 10:44:50 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 10:44:51 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 10:44:51 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 10:45:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 10:45:05 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 10:45:06 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 10:45:06 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 10:45:07 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 10:45:07 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 10:45:08 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 10:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 10:45:08 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 10:45:08 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 10:45:16 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 10:45:16 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:ffe4428ef008913a7ec63449e4ad3aa536b26103943146a302591dfceb157d2f`  
		Last Modified: Sat, 17 Jun 2017 18:08:13 GMT  
		Size: 2.0 MB (2045593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4fe786260f2bd2710289e7c9487b423cb252a691fa501759b0768516122869`  
		Last Modified: Wed, 25 Oct 2017 23:32:27 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cf0f0a132c9bb882206147dffad08dc780f2bc82556cfbda9878a3218f1e7c`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00a9186496c6602ccd3efb4bb1780b42adb7028c8fa3cd3c1ff2f10bcfa33a3`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 8.3 KB (8305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc19938c3bf2e858347a9c7add1beac38af5a4f83b99d80ddc004aa4ad51e596`  
		Last Modified: Thu, 26 Oct 2017 10:45:30 GMT  
		Size: 16.7 MB (16710838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697b9a0ea77c953a543f168ba09045ae412f3b2bd0947b2bba8c18cd0cd2c70b`  
		Last Modified: Thu, 26 Oct 2017 10:45:30 GMT  
		Size: 5.0 MB (5012335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca279d1203917e8f98e0d5fe3f9de9bdde74bae202990b6388e1cc748caa726`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb3c81d25b2aa6fa5bf57aaf5f8ad6a5f27be02727e454818ff546e5a989c88`  
		Last Modified: Thu, 26 Oct 2017 10:45:29 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420233201c5d7a33d69bc90b4ac40d5db1285e61718701ffd97d4db8396a9508`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0b37b1c6d397d7b0daa633cac4b2d202e9656dd6340dc40496303190ed4a78`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b719c08f02439306e8baee89f388d47a99542fc0eec294aaf615c425ec5253de`  
		Last Modified: Thu, 26 Oct 2017 10:45:59 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:1f2ed16a80e1b71fd652fe7520fa1ba2ac5c9b5a207199bc7aaec39c61d5a38e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23640124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0244f72e17b275644966d172a75c7023650024e2761d2541020cbb3592bd01f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:47 GMT
ADD file:e0be8616517d68cb80a2f9b74eb967cda22b9937bbcbe8b75b6153815a6f7761 in / 
# Wed, 25 Oct 2017 23:28:48 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:50 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 07:12:01 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 07:12:12 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 07:12:36 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 07:12:37 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 07:12:39 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 07:12:41 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 07:12:42 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 07:12:44 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 07:12:45 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 07:13:07 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 07:13:09 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 07:13:13 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 07:13:15 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 07:13:19 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 07:13:23 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 07:13:25 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 07:13:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 07:13:28 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 07:13:30 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 07:13:42 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 07:13:44 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:1e52418956f7d2a8ea35e8e6e3318fd08e005b27457d77868c225e7433bbfa02`  
		Last Modified: Thu, 20 Jul 2017 15:12:59 GMT  
		Size: 2.0 MB (2008578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf472f4e5bb7956ac20bb343b304e1d3de1f79160c0d158cccbe25980022d50`  
		Last Modified: Wed, 25 Oct 2017 23:29:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48c95ed960185dbd69324a206614e723f0086f80b46bd3223f233e4f1e278bc`  
		Last Modified: Thu, 26 Oct 2017 07:14:01 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a8242358db9adbde1a17b0e2b320c02112fcefa90d397ecc028a9729efcf94`  
		Last Modified: Thu, 26 Oct 2017 07:14:01 GMT  
		Size: 9.1 KB (9059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6db9581873eb0cadddc4d474e33cb2ec978c0d68e3ea124ce4f07ab2731d79`  
		Last Modified: Thu, 26 Oct 2017 07:14:04 GMT  
		Size: 16.6 MB (16603134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a991ac52f27ddaf9fb4021acf59b12957c4fa6251ab4d74159bb54ac63878009`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 5.0 MB (5013168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d098ea301752e2203c7ad872d2a38cc3da3efa183b01e61fe5c2fcde29efceb8`  
		Last Modified: Thu, 26 Oct 2017 07:14:00 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8727c952955dcfc3ce7e96c808c78bc91d43e6033164a46a7faffd11dc22fb69`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fe10e7f312fce5a9bf6ca051d683f86b1cef271217890a7ea53164ef81c99d`  
		Last Modified: Thu, 26 Oct 2017 07:13:58 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcba876c6e465f99a2952b71be993ce0d4d82ef4f70f72a59e58200cf263252f`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d8f64c426c0a1bf9de5b158513294037721b7e6c1c4fbc5e75f84a63743aae`  
		Last Modified: Thu, 26 Oct 2017 07:14:31 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:3-management-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:4af0a8312682b92651de05ff83aac54b00b55118b9babda060c043b4fdf9609b
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23819037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b62c33cd033388e2676822a15081284e991d3078ed4b51ebab5b72b7cb5a983`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:40 GMT
ADD file:6fbdff4b4c08600e192f5da9b67a02c58759237fb40525d70712104c80c34c48 in / 
# Wed, 25 Oct 2017 23:28:40 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:40 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 17:06:39 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 17:06:42 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 17:06:55 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 17:06:56 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 17:06:57 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 17:06:57 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 17:07:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 17:07:05 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 17:07:06 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 17:07:06 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 17:07:06 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 17:07:07 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 17:07:07 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 17:07:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 17:07:08 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 17:07:08 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 17:07:19 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 17:07:19 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:d45fd9d3c4f188ab1f3a4bf6a9f5202b3f1577dbb998f5f28e82d192e0c1f0e7`  
		Last Modified: Sat, 17 Jun 2017 20:41:42 GMT  
		Size: 2.1 MB (2065460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5978b6b34b3e943e0fd25dfb50991c0bad82a986cfdaa91c4de756431ba679`  
		Last Modified: Wed, 25 Oct 2017 23:28:59 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299a1fbc19bbea84dbf4d0b6e2e71fb847299b017209b1f9783faea14214c995`  
		Last Modified: Thu, 26 Oct 2017 17:07:31 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb76f2dd4162cae82233bc93ba436b63ca37e536d53c85a9f1d7343203e3c383`  
		Last Modified: Thu, 26 Oct 2017 17:07:31 GMT  
		Size: 8.6 KB (8604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac09bb55706d627cf6348c9d0bd891c2fe9a4155aee5d95264b92781371021db`  
		Last Modified: Thu, 26 Oct 2017 17:07:33 GMT  
		Size: 16.7 MB (16726549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e776aa2eebd7dc068e74be7736114ce80966ab2b25478d29763bc1ccf05c3e3`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 5.0 MB (5012317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57d3128b93c0f42a41ad6b2571d41e61c6096e070ee18ef58d34aeaf7318560`  
		Last Modified: Thu, 26 Oct 2017 17:07:29 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484c70be68b7dc1296d1199834238ebabbde1df9ce04ec3cf986a2096ad218b6`  
		Last Modified: Thu, 26 Oct 2017 17:07:29 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01611bf6acbe11966a7f1fe2e96d811430328e24513c20237576287afdd5079a`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f045868d086334dbd06f276dfb93c084fc32b243827527e36c2bc5a5d8583d`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed30107b153ffda65732449b2eea0bdac7dbd4327b3a82ef0fcd5553b0ca55fc`  
		Last Modified: Thu, 26 Oct 2017 17:07:50 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rabbitmq:alpine`

```console
$ docker pull rabbitmq@sha256:e49288ac5376cbd8699e6dd2d99410ce12ecd1a5f8885b9f8a1eebd863e3b4ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `rabbitmq:alpine` - linux; amd64

```console
$ docker pull rabbitmq@sha256:f8204cb30a089ec4fa99d41ed68f1b520670f5698bea479f6a6582d1926a5715
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23579666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:210310494165d259279503b1b25ecd975f73320e177d472300069bc8619908be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:19:51 GMT
ADD file:1e87ff33d1b6765b793888cd50e01b2bd0dfe152b7dbb4048008bfc2658faea7 in / 
# Wed, 25 Oct 2017 23:19:51 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 03:02:21 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 03:02:25 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 03:02:32 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 03:02:32 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 03:02:33 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 03:02:33 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 03:02:42 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 03:02:42 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 03:02:43 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 03:02:43 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 03:02:44 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 03:02:44 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 03:02:45 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 03:02:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 03:02:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 03:02:45 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:b56ae66c29370df48e7377c8f9baa744a3958058a766793f821dadcb144a4647`  
		Last Modified: Wed, 25 Oct 2017 23:21:25 GMT  
		Size: 2.0 MB (1991435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827e0bce86e3c8fa677ac91f0c55a7a4071cc45c729b171aecbe04d35ae160d7`  
		Last Modified: Thu, 26 Oct 2017 03:03:23 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe01d115cb92dc0ab37de6b6ffa2073ea20d30dfc49c537fbba569cd6a494b8`  
		Last Modified: Thu, 26 Oct 2017 03:03:23 GMT  
		Size: 8.2 KB (8176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bfc0dbbf8b1d2f532779c4873b4c7e0237d6ecc86161b1c6f28e3b6bd3149f`  
		Last Modified: Thu, 26 Oct 2017 03:03:26 GMT  
		Size: 16.6 MB (16561644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b24f4fd26b3494d310561a28e2d9aeb08e7baba442eaef2cd8697c7ebd9d9f1`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 5.0 MB (5012671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfb0f3b402f9674b21d7ed079f6576ec1be80f333f41c404e8ce3feb193b813`  
		Last Modified: Thu, 26 Oct 2017 03:03:22 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521b2b4b2311f153d53f0b9bde9a164f45df9dfd531512c36195ba2ccf5a4c76`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cedbb525e85f1b9257e8b20d04b4ad39f1004c9dfbc673086815dd887f380c3`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f35995cc5f5daa05334d17a87482ac8728aadfb0f10f9d62b3d70f5986e5cc`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:9bbc37dee4951514ff22f2fc83eed327e4fb935baedc146be69d4b7bd04b40b6
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23412846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d5e63a3df176d84fe8622b7515aa144197643b1a5ac6fc5b1578c6d78fb121c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:35 GMT
ADD file:009348222efb3c4ca2e53c387fb34c488679ca07db39525a6c5cc214e46abffd in / 
# Wed, 25 Oct 2017 23:28:36 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:36 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 05:25:53 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 05:25:55 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 05:26:10 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 05:26:10 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 05:26:10 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 05:26:11 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 05:26:19 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 05:26:19 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 05:26:20 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 05:26:20 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 05:26:21 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 05:26:22 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 05:26:22 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 05:26:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 05:26:22 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 05:26:23 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:0864efeeb5cb8dca4eb53e5d6fd38486daee80fa326fe36d1ad254f8fa6bb310`  
		Last Modified: Sun, 23 Jul 2017 20:21:42 GMT  
		Size: 2.0 MB (1965988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda69762aee1588fa82aeabf1af6d6ad24f737cce1451fab2e0199849b1e12e`  
		Last Modified: Wed, 25 Oct 2017 23:28:45 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62a8c5580cc1c2fbf2f9ce119bc0c06403a12ad18167bde2ec94420810916db`  
		Last Modified: Thu, 26 Oct 2017 05:26:38 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b096e39434b5aeddcb2ec167b7bf570cac7b8b16e68324d3f46c6f4d41b69c79`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 8.4 KB (8374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ad9273316fa6f22cd2e8cf88c92f34c3210325fa1be2041153a96f4124476f`  
		Last Modified: Thu, 26 Oct 2017 05:26:41 GMT  
		Size: 16.4 MB (16420180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed982c9e7d5644c85267595b470c0f21f25093a865603ab33304248efdb68b5d`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 5.0 MB (5012332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b76830a9cb5b5f898068945d6af6325c7d97b36d50e521a12097d3e908fd0`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a31f9ee2285379d9d5106926e707698e7a3283f707a4573fec9731e6ede58b5`  
		Last Modified: Thu, 26 Oct 2017 05:26:36 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff38544dc85623170156958b2d5d51604efd94b336b47a6479cde0417667838f`  
		Last Modified: Thu, 26 Oct 2017 05:26:36 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564bee8c5f497342e71777f1adc38d1578f7c95ddefe18efa16fc01b3e7e2a52`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:dcc95a027acff970a00636c77c269b7cc72e3176411c8aecc946eb6642b3906c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23318158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b316c629f8f17231a345cc527fcd76aa75a8b9e012eeae0d0497b3a92c014132`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:58 GMT
ADD file:45b5d3b8d5490ba7edfca2cf6f54cdcf49c772b0b3a2302ce69a7af061007aa4 in / 
# Wed, 25 Oct 2017 23:28:59 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:59 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 13:53:09 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 13:53:13 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 13:53:28 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 13:53:28 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 13:53:29 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 13:53:29 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 13:53:30 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 13:53:30 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 13:53:31 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 13:54:22 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 13:54:23 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 13:54:24 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 13:54:25 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 13:54:26 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 13:54:28 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 13:54:29 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 13:54:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 13:54:30 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 13:54:30 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:bb473f0ebc12fde1bd45c1bd3c46f2d3aab367b1b7739464771455b9972f7894`  
		Last Modified: Thu, 06 Jul 2017 09:54:42 GMT  
		Size: 1.9 MB (1914748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ff6b7ff3a208b8399e701e7ea1b7edbdc654c8c60d33c6f09a7803e2dda776`  
		Last Modified: Wed, 25 Oct 2017 23:29:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05834eac152e30997eb4f1aa4ffe8e952bd759c1a1009bd183dec80dca24cf86`  
		Last Modified: Thu, 26 Oct 2017 13:55:11 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd88a23486b40755f2e1192cb35d4fdaec20831c18ce83da31df3f8aa2f7b45c`  
		Last Modified: Thu, 26 Oct 2017 13:55:11 GMT  
		Size: 8.3 KB (8297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f9ba1206e6e4bfba21cef7f235482b41868ec966d5ebc44a4c4ac432a5fe03`  
		Last Modified: Thu, 26 Oct 2017 13:55:16 GMT  
		Size: 16.4 MB (16376872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5991837e23d785829d605fd052c61e10ed79a7cfb0dfee9dd40d6144bc9fad0f`  
		Last Modified: Thu, 26 Oct 2017 13:55:12 GMT  
		Size: 5.0 MB (5012322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf5663fa552ede671fc5ebf425b2ce3ff5257636b55df9564e556fe7ff85fce`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794d04d767a60fa6df4adb3af1f835701a3c2692e7f6b2d4a9db621a0bc8cd5f`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91155b0cb6bf92d1ab05fb7d13593e0a966eb79dd4e4173e3895d98dffe1c996`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969bbed547aa67091daaa801a46b062fd1c39f7835c81dd5052032056b6cf230`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:3355a334e7313d636e6b3d263a101f1ab926a88bcee118e357835788d527179a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23782989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b83bfaf99c5c91aa3c08ade40b04a3bc1b6bd3725fa905cd0a488133319eef9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:32:08 GMT
ADD file:4a952fc4b81d50b342e26a818dac48a148a4d5eddb878219650e579a5c9faeaa in / 
# Wed, 25 Oct 2017 23:32:08 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:32:08 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 10:44:24 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 10:44:28 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 10:44:50 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 10:44:50 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 10:44:51 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 10:44:51 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 10:45:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 10:45:05 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 10:45:06 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 10:45:06 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 10:45:07 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 10:45:07 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 10:45:08 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 10:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 10:45:08 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 10:45:08 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:ffe4428ef008913a7ec63449e4ad3aa536b26103943146a302591dfceb157d2f`  
		Last Modified: Sat, 17 Jun 2017 18:08:13 GMT  
		Size: 2.0 MB (2045593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4fe786260f2bd2710289e7c9487b423cb252a691fa501759b0768516122869`  
		Last Modified: Wed, 25 Oct 2017 23:32:27 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cf0f0a132c9bb882206147dffad08dc780f2bc82556cfbda9878a3218f1e7c`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00a9186496c6602ccd3efb4bb1780b42adb7028c8fa3cd3c1ff2f10bcfa33a3`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 8.3 KB (8305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc19938c3bf2e858347a9c7add1beac38af5a4f83b99d80ddc004aa4ad51e596`  
		Last Modified: Thu, 26 Oct 2017 10:45:30 GMT  
		Size: 16.7 MB (16710838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697b9a0ea77c953a543f168ba09045ae412f3b2bd0947b2bba8c18cd0cd2c70b`  
		Last Modified: Thu, 26 Oct 2017 10:45:30 GMT  
		Size: 5.0 MB (5012335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca279d1203917e8f98e0d5fe3f9de9bdde74bae202990b6388e1cc748caa726`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb3c81d25b2aa6fa5bf57aaf5f8ad6a5f27be02727e454818ff546e5a989c88`  
		Last Modified: Thu, 26 Oct 2017 10:45:29 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420233201c5d7a33d69bc90b4ac40d5db1285e61718701ffd97d4db8396a9508`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0b37b1c6d397d7b0daa633cac4b2d202e9656dd6340dc40496303190ed4a78`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:2a7e105872a021c9e0df106fd62ee50b80be17634c3b713596ca188b8ab3cf04
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23639927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01e565612a099b2324e2f273a6a14a62e8cab609839bdeb205adc72571cb62b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:47 GMT
ADD file:e0be8616517d68cb80a2f9b74eb967cda22b9937bbcbe8b75b6153815a6f7761 in / 
# Wed, 25 Oct 2017 23:28:48 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:50 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 07:12:01 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 07:12:12 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 07:12:36 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 07:12:37 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 07:12:39 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 07:12:41 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 07:12:42 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 07:12:44 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 07:12:45 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 07:13:07 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 07:13:09 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 07:13:13 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 07:13:15 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 07:13:19 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 07:13:23 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 07:13:25 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 07:13:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 07:13:28 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 07:13:30 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:1e52418956f7d2a8ea35e8e6e3318fd08e005b27457d77868c225e7433bbfa02`  
		Last Modified: Thu, 20 Jul 2017 15:12:59 GMT  
		Size: 2.0 MB (2008578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf472f4e5bb7956ac20bb343b304e1d3de1f79160c0d158cccbe25980022d50`  
		Last Modified: Wed, 25 Oct 2017 23:29:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48c95ed960185dbd69324a206614e723f0086f80b46bd3223f233e4f1e278bc`  
		Last Modified: Thu, 26 Oct 2017 07:14:01 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a8242358db9adbde1a17b0e2b320c02112fcefa90d397ecc028a9729efcf94`  
		Last Modified: Thu, 26 Oct 2017 07:14:01 GMT  
		Size: 9.1 KB (9059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6db9581873eb0cadddc4d474e33cb2ec978c0d68e3ea124ce4f07ab2731d79`  
		Last Modified: Thu, 26 Oct 2017 07:14:04 GMT  
		Size: 16.6 MB (16603134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a991ac52f27ddaf9fb4021acf59b12957c4fa6251ab4d74159bb54ac63878009`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 5.0 MB (5013168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d098ea301752e2203c7ad872d2a38cc3da3efa183b01e61fe5c2fcde29efceb8`  
		Last Modified: Thu, 26 Oct 2017 07:14:00 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8727c952955dcfc3ce7e96c808c78bc91d43e6033164a46a7faffd11dc22fb69`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fe10e7f312fce5a9bf6ca051d683f86b1cef271217890a7ea53164ef81c99d`  
		Last Modified: Thu, 26 Oct 2017 07:13:58 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcba876c6e465f99a2952b71be993ce0d4d82ef4f70f72a59e58200cf263252f`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:85a850d9b872c722bace7014c60c183a5746e338d9136a8319c91c3d2fb6a778
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23818845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45af14c4c176512dfc8deb7275c6c333b0f5933fff4eab2e34c6d8f888d40be2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:40 GMT
ADD file:6fbdff4b4c08600e192f5da9b67a02c58759237fb40525d70712104c80c34c48 in / 
# Wed, 25 Oct 2017 23:28:40 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:40 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 17:06:39 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 17:06:42 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 17:06:55 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 17:06:56 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 17:06:57 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 17:06:57 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 17:07:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 17:07:05 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 17:07:06 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 17:07:06 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 17:07:06 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 17:07:07 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 17:07:07 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 17:07:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 17:07:08 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 17:07:08 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:d45fd9d3c4f188ab1f3a4bf6a9f5202b3f1577dbb998f5f28e82d192e0c1f0e7`  
		Last Modified: Sat, 17 Jun 2017 20:41:42 GMT  
		Size: 2.1 MB (2065460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5978b6b34b3e943e0fd25dfb50991c0bad82a986cfdaa91c4de756431ba679`  
		Last Modified: Wed, 25 Oct 2017 23:28:59 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299a1fbc19bbea84dbf4d0b6e2e71fb847299b017209b1f9783faea14214c995`  
		Last Modified: Thu, 26 Oct 2017 17:07:31 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb76f2dd4162cae82233bc93ba436b63ca37e536d53c85a9f1d7343203e3c383`  
		Last Modified: Thu, 26 Oct 2017 17:07:31 GMT  
		Size: 8.6 KB (8604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac09bb55706d627cf6348c9d0bd891c2fe9a4155aee5d95264b92781371021db`  
		Last Modified: Thu, 26 Oct 2017 17:07:33 GMT  
		Size: 16.7 MB (16726549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e776aa2eebd7dc068e74be7736114ce80966ab2b25478d29763bc1ccf05c3e3`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 5.0 MB (5012317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57d3128b93c0f42a41ad6b2571d41e61c6096e070ee18ef58d34aeaf7318560`  
		Last Modified: Thu, 26 Oct 2017 17:07:29 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484c70be68b7dc1296d1199834238ebabbde1df9ce04ec3cf986a2096ad218b6`  
		Last Modified: Thu, 26 Oct 2017 17:07:29 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01611bf6acbe11966a7f1fe2e96d811430328e24513c20237576287afdd5079a`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f045868d086334dbd06f276dfb93c084fc32b243827527e36c2bc5a5d8583d`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rabbitmq:latest`

```console
$ docker pull rabbitmq@sha256:2c3145ed1766d6eac4f224c990d02a2c2411e8b1dc02875a28b7cf8acc9fa985
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

### `rabbitmq:latest` - linux; amd64

```console
$ docker pull rabbitmq@sha256:b99e238fa99bcd7ffcfd89a536fdf33bbd27e206cea118246874e3792ebfc2bc
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.9 MB (62852177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e186865bff877f181c4a4b4ffdb7235e91c0c988bdc0c926d1b68e5d8c81e45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:33:42 GMT
ADD file:45233d6b5c9b91e9437065d3e7c332d1c4eb4bce8e1079a4c1af342c450abe67 in / 
# Mon, 09 Oct 2017 21:33:43 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 02:41:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:41:43 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 02:41:43 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 02:42:10 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 02:42:40 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 02:42:41 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 02:42:42 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 02:43:16 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:43:16 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 02:43:17 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 02:43:17 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 02:43:18 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 02:43:19 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 13 Oct 2017 23:40:43 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 13 Oct 2017 23:40:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 13 Oct 2017 23:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2017 23:40:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 13 Oct 2017 23:40:45 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:bc95e04b23c06ba1b9bf092d07d1493177b218e0340bd2ed49dac351c1e34313`  
		Last Modified: Mon, 09 Oct 2017 21:42:28 GMT  
		Size: 22.5 MB (22492350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65f0b00e4cfb1535d0f4e7a63707172ae63483fb33140d777614f199afcb36`  
		Last Modified: Tue, 10 Oct 2017 02:43:59 GMT  
		Size: 4.5 MB (4498726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bd803179890909fcae186044c0e6ca1bc1d34e5fc05ef1ccea823e7be97540`  
		Last Modified: Tue, 10 Oct 2017 02:43:57 GMT  
		Size: 4.1 KB (4069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b05ca8302833edf783c50f03cd7ba0b8e12bc872b053eda3e3ae7e1f17e2b4b`  
		Last Modified: Tue, 10 Oct 2017 02:43:58 GMT  
		Size: 952.1 KB (952058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb5a4bbcce5a040eb83057f9e93d17663bb123f4e98168457444497f7d17b70`  
		Last Modified: Tue, 10 Oct 2017 02:44:03 GMT  
		Size: 27.7 MB (27703883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf840d8999f6fe46a162974c82378c38b3cf3dcccbbaff848c0fb199988aebe0`  
		Last Modified: Tue, 10 Oct 2017 02:44:00 GMT  
		Size: 7.2 MB (7194403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be339ca44883b1990e52771487402163d398a279755a501fdd8891ec71cf09d0`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce35cd9f9b5b917868095b3b074dd23d18e0e266f3ee68ff95e2c61467299812`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fe32a0a00d916ed4d632aae71d35d9d0baa5e5910d6bd179a24071c35bedb0`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77408ca9e94eb4bfeb346ab10c602857525802c2279e7c6995fcdbc90269444a`  
		Last Modified: Fri, 13 Oct 2017 23:41:26 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db03407a1aba1c0a89dffe960394aae639885702e3faa65271b918c36c7905cd`  
		Last Modified: Fri, 13 Oct 2017 23:41:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; arm variant v5

```console
$ docker pull rabbitmq@sha256:53c2349355bbba2f2b1eeb11d5ed481cab005bba90148c0ed0c1aa44d33bcaff
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58432369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1107bbf7e8a883f25f4975b43d490503a84921e26ccb943e929596f9b418cf40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:44:48 GMT
ADD file:ff9945b48b1ac236dcec24eb9dfaf52b7c151a3b11c8502391f0866dfb4e3ac3 in / 
# Mon, 09 Oct 2017 21:44:48 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 00:18:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:18:11 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 00:18:11 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 00:18:29 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 00:18:58 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:18:58 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 00:18:58 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 00:19:26 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:19:26 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 00:19:27 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 00:19:28 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 00:19:29 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 00:19:30 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Sat, 14 Oct 2017 14:14:24 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Sat, 14 Oct 2017 14:14:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 14 Oct 2017 14:14:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 Oct 2017 14:14:25 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Sat, 14 Oct 2017 14:14:26 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:836d5b6056a9815be79c76480a90299267f60201bd1e3396817003e6c14819cc`  
		Last Modified: Mon, 09 Oct 2017 21:50:56 GMT  
		Size: 21.2 MB (21166251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb896fba83bd09a35c68457554b35289860c23c46f27a8c3ef42f13146ebba1`  
		Last Modified: Tue, 10 Oct 2017 00:20:01 GMT  
		Size: 4.2 MB (4231979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61827a16c114b9741d761aa4c60a972ffe1e0b60147794e86b05653d67822e91`  
		Last Modified: Tue, 10 Oct 2017 00:20:00 GMT  
		Size: 4.1 KB (4079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877cd9511def30e56a5ce354e145e8a2b1a93daaae7eaaa42dc4219838aa1743`  
		Last Modified: Tue, 10 Oct 2017 00:20:00 GMT  
		Size: 942.8 KB (942752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea9e378899e98c99e93ae2d0874bd5d89e24134bd14a19c285bdf39a0a42ade`  
		Last Modified: Tue, 10 Oct 2017 00:20:05 GMT  
		Size: 25.2 MB (25170810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc82a29314b16531aa2172ac523ba535e3678f85efdd699164fbb0241ab8b62`  
		Last Modified: Tue, 10 Oct 2017 00:20:01 GMT  
		Size: 6.9 MB (6909811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c44a3d016cf9de95021782180a42d3660e20fc7d8e92a7fe5ce9ede7928ca2`  
		Last Modified: Tue, 10 Oct 2017 00:19:59 GMT  
		Size: 2.3 KB (2261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abfdcdd98b40291ad91791bea09bf277e75c3669c6607c7891b09130101bfa3`  
		Last Modified: Tue, 10 Oct 2017 00:19:58 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a72811da4bf8ca8a2d06cdc182aa54116bb12133e8d82ef2b018a8de29ed74`  
		Last Modified: Tue, 10 Oct 2017 00:19:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147d8cf0897dea9b024bf5c6efb6873db3d86dec857fca062b146f88b7b5a735`  
		Last Modified: Sat, 14 Oct 2017 14:14:43 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f355fd0b70caedf30aa384298307b8e40d922e9e341492dd3fde71f119fd7d7`  
		Last Modified: Sat, 14 Oct 2017 14:14:44 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:c5a07be740a1d956343d5881d8827cb9e3d6dcceda2d8ce954cf187ab9be9abc
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55688150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c4235a850985eab3d39e30563f87f78348a6425ec30388363f9d372c082855e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:43 GMT
ADD file:b758c6c3ff989778bd740dde35c86b953fa09be913a7e02711b2881de6b8911d in / 
# Mon, 09 Oct 2017 21:45:44 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 13:07:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:07:42 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 13:07:42 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 13:07:58 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 13:08:17 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:08:17 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 13:08:17 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 13:08:39 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:08:39 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 13:08:40 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 13:08:41 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 13:08:42 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 13:08:43 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 13:08:43 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 13:08:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 13:08:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 13:08:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 13:08:45 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:59e81a3fde58ec8d4b8f2f58b98ef2f4d951d37dd9b99b016fd294a8e07d7796`  
		Last Modified: Mon, 09 Oct 2017 21:52:49 GMT  
		Size: 19.3 MB (19277135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2037b99f3c3dc51e8ace39aed9971155f34f325ac4f0a1e56a07c4d6c02f5ae6`  
		Last Modified: Fri, 03 Nov 2017 13:09:18 GMT  
		Size: 3.9 MB (3868347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f368172ea96bda944832762ad29b52dfe17ec5e6fae96eee37adc4e9d68674a5`  
		Last Modified: Fri, 03 Nov 2017 13:09:16 GMT  
		Size: 4.1 KB (4084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893cc1ae60f8bf72ac3020ccc60b22d9e0ad0cb0647e15bc4847d08c8985eee2`  
		Last Modified: Fri, 03 Nov 2017 13:09:16 GMT  
		Size: 926.1 KB (926097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13220cc1a683014bda9cfae7f7ee7015a26b28048f90f5aa3ed8b6a96f4b2813`  
		Last Modified: Fri, 03 Nov 2017 13:09:20 GMT  
		Size: 24.8 MB (24785610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269f4e069126132643c1c0be1faf600d55ff15e870066c527d03181904d99c5d`  
		Last Modified: Fri, 03 Nov 2017 13:09:17 GMT  
		Size: 6.8 MB (6820180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ae244f4f610a339fcbddf37612a15ec7b7f6674e3d888c3c4d36302283418e`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce7d85327b7bc7d59a7b54222a3e6babd7f8afd8eb080becb77fc52aed5a751`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dfa32e4b49700ed0130ebd563f40a2c381393983b571a9886435813102ad0c`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba15cd885dc21f438d366b40d0d9f595f2c25e063c60fa590ab4c0f6233ff94`  
		Last Modified: Fri, 03 Nov 2017 13:09:14 GMT  
		Size: 4.0 KB (4040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978a8434497fcb8e08cefc7484b515ac34fe23c281fb869d015f62b54673028c`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:3d9b2aee2786ff5328bb6b1195f2938e251fdfe7c183ffac1ead7ffe6f234d03
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57278372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa9e28302480b775a117eda9fd3d2e8897ee8a4ed19ceac66f0afaab1e5f8609`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:47:55 GMT
ADD file:3a528355cfc75437716aff3b517ef99ae602918d84d26dbafff0ed142248fb93 in / 
# Mon, 09 Oct 2017 21:47:56 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 04:57:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 04:57:04 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 04:57:05 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 04:57:37 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 04:58:35 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 04:58:36 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 04:58:37 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 04:58:37 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 04:58:38 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 04:58:39 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 04:58:39 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 05:00:22 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 05:00:23 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 05:00:25 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 05:00:26 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 05:00:28 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 05:00:31 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Sat, 14 Oct 2017 13:52:47 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Sat, 14 Oct 2017 13:52:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 14 Oct 2017 13:52:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 Oct 2017 13:52:51 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Sat, 14 Oct 2017 13:52:51 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:e907afd6e25615a4d3eb554d930cef57b87e79ec82413889c2eac38beb4eb8f7`  
		Last Modified: Mon, 09 Oct 2017 22:03:08 GMT  
		Size: 20.3 MB (20337143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5e6d35928560b933b85b5a3f2a8e96b4520fbb8df138b3e739e56d0c1f355`  
		Last Modified: Tue, 10 Oct 2017 05:01:18 GMT  
		Size: 4.1 MB (4073554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a862ab821b342790326492507ca5d70bfb7016bef765606193f1f7139f60c5ed`  
		Last Modified: Tue, 10 Oct 2017 05:01:14 GMT  
		Size: 4.1 KB (4072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92799a54920b79013733790e444f13d8c65faa29c79cbdaf1bc8af85f637a233`  
		Last Modified: Tue, 10 Oct 2017 05:01:14 GMT  
		Size: 919.5 KB (919487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b119999eef1bcadabedd3a5319b03c6b83ede91ba8535059851547d3433b205`  
		Last Modified: Tue, 10 Oct 2017 05:01:19 GMT  
		Size: 25.0 MB (25042572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62f8525a3a982a102aa37bb3313876195b15d8781cd253ed238dd2b9dff151`  
		Last Modified: Tue, 10 Oct 2017 05:01:15 GMT  
		Size: 6.9 MB (6894852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc028e70f04f6ea4365223a1cfe4e5c4384d5921acac419f3c170b148f7c7bf`  
		Last Modified: Tue, 10 Oct 2017 05:01:10 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e99faa03c2a8a272f56208c644c12b384b69dea50be6da9f6be400c14b945c`  
		Last Modified: Tue, 10 Oct 2017 05:01:12 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8fa260bcaa52d81ba20c11111f8d15bab954b17b48666724536c604220d94e`  
		Last Modified: Tue, 10 Oct 2017 05:01:11 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306840de948d03472918a306c089409429606802ec8cf841e96dec707a2f7178`  
		Last Modified: Sat, 14 Oct 2017 13:53:27 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a7a978032478b38adb1f0107466d187e53380f7037d058c62e4937cd07fc09`  
		Last Modified: Sat, 14 Oct 2017 13:53:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; 386

```console
$ docker pull rabbitmq@sha256:900c25b037b878974bb75f9d056b5278794f96586c9d03f619af9905a6cf5229
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63902262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a993d7c3c104c0e9f2ed42d750b907890291a9a2693d23f166744b9fb8e9265d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:36 GMT
ADD file:6582536277127947668f7bfdc1471a4e36170915b91a4cb841e7e1bfa1de6535 in / 
# Mon, 09 Oct 2017 21:45:36 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 10:45:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:45:12 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 10:45:13 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 10:45:28 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 10:46:03 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 10:46:04 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 10:46:25 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:46:25 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 10:46:26 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 10:46:27 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 10:46:27 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 10:46:28 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 10:46:28 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 10:46:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 10:46:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 10:46:30 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 10:46:30 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:b2b52fe46b29fe5d0689f26449c2114e40f0731d4ce3eb8c3941397b74205432`  
		Last Modified: Mon, 09 Oct 2017 21:53:42 GMT  
		Size: 23.1 MB (23128678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d407b136da0731f5f38279001e9dd426217937443cad0f16e1f242366290773`  
		Last Modified: Fri, 03 Nov 2017 10:47:13 GMT  
		Size: 4.8 MB (4803637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c93817e78345b4b5070c81e5a37d02afc2b5fe347a1a4bf59e09f6084814fd2`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 4.1 KB (4057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97eae59c75f8f814ab781f5239ac2e132b7b65c77e75b35023c603c539ca54f`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 931.5 KB (931524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aed670dee19fde6946658d7129e13520c1a0747f8b80b6f92dac5f6d974ae52`  
		Last Modified: Fri, 03 Nov 2017 10:47:24 GMT  
		Size: 27.8 MB (27818690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b61d6d0b60ec18280aeba946a05d62817afbe030f277af85b5f434021e90c9`  
		Last Modified: Fri, 03 Nov 2017 10:47:16 GMT  
		Size: 7.2 MB (7208985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec7d4cc3b5497bbbd6b2d1e9574dbedb6c7ad11805cff4c287ea444ddc2e298`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 2.3 KB (2259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eec554591344f78e35e3976d002d617623a52d123fc71e65d33c4d533d2b2e7`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e433f73af1167eff0dee1984c095bf5be36593fcead5b8cc820e2cb829aaed0`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8d6e0dbdbb04b44f7a0972fce6b0b1b19262e4fc5416bd1589af560f16c99f`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 4.0 KB (4040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bab08cf9b00d8109139e1cb1cdec448b71fdae7d7f1260d4175771416a5f80`  
		Last Modified: Fri, 03 Nov 2017 10:47:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:63dcce5fe70ba7b07c27b3af47248ad1f0609ca79e98e01a2ea0cb4e5357cc55
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60384479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:929ca14b97313f42a819bb7e089422aea0fa6d6a7428046a573c11937059499d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:56 GMT
ADD file:7edf73437495be24244c16841b563be06c15452963f41ac940fb5e105ed96027 in / 
# Mon, 09 Oct 2017 21:45:58 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 07:12:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:12:51 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 07:12:53 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 07:13:49 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 07:15:26 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:15:28 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 07:15:29 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 07:15:31 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 07:15:33 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 07:15:34 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 07:15:35 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 07:16:54 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:16:55 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 07:17:00 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 07:17:01 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 07:17:06 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 07:17:11 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 07:17:13 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 07:17:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 07:17:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 07:17:21 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 07:17:23 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:c4860466fa1e6824151f4fa3a51ef0e9d7d3c3ba860e21d94e69988b65601260`  
		Last Modified: Mon, 09 Oct 2017 21:52:59 GMT  
		Size: 22.7 MB (22746217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebe4c87dcd1f7ef11d4d21752831bf4095ac42afe041706c35f1d7d4d0ca4f2`  
		Last Modified: Fri, 03 Nov 2017 07:18:05 GMT  
		Size: 4.4 MB (4360529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e5365525084de1c85fa29ef33d37c38b5f80621f5bcb26bb4882d71598c6f7`  
		Last Modified: Fri, 03 Nov 2017 07:18:03 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600c3853740b7f4cff9cc799ae478f669bd54277a8dd375479a34ed1bb47a803`  
		Last Modified: Fri, 03 Nov 2017 07:18:02 GMT  
		Size: 920.7 KB (920695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993868ec534130e348e45aa6d64b471fa46eafbf061836cc9d2a56edf73e9382`  
		Last Modified: Fri, 03 Nov 2017 07:18:06 GMT  
		Size: 25.5 MB (25492533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca1b92e212aaef163244d5fdd9e135fdb8be8c9dbbb626061ee2882d941a553`  
		Last Modified: Fri, 03 Nov 2017 07:18:03 GMT  
		Size: 6.9 MB (6853702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483f96d1f500f9f69170bc6927d599a7f0cd1550f96b6ee3f90eb4185a1bffb`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b433db63f40c7cab3080cf36bd7beabbdf7d9eece3f2dc16a65b900c61180`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93971551a2c911c34ca2e9af47495efb2f27e2922e567d93dd94dfb9b773bd3`  
		Last Modified: Fri, 03 Nov 2017 07:17:58 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5494bb8bcc45452a84c216edffedb3103a15c3e209aba0561dfbc70e4312192e`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 4.0 KB (4039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d56b2a4f9f8d7b11831a8f1952fe2c02613bcb014ab9d756b70b3b398b37269`  
		Last Modified: Fri, 03 Nov 2017 07:17:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:latest` - linux; s390x

```console
$ docker pull rabbitmq@sha256:c5e29e37ac52898d26c2d63c4e0506afbaf0fa3862456c04c425429dae26248a
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60364776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9b9f437096f93b98ba60e922a7e6c52ff1e8a75593833f81fa03b4a035a3f50`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:44:35 GMT
ADD file:ae4aaa6affe22f36ab5478771d5c84917f72de7a8dac16345a035709a1a5edf4 in / 
# Mon, 09 Oct 2017 21:44:36 GMT
CMD ["bash"]
# Thu, 02 Nov 2017 17:06:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 17:06:41 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Thu, 02 Nov 2017 17:06:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 02 Nov 2017 17:07:21 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Thu, 02 Nov 2017 17:07:43 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 02 Nov 2017 17:07:44 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 02 Nov 2017 17:07:45 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 17:07:48 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 17:07:48 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 17:07:49 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 17:07:50 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 17:07:52 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 17:07:53 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 17:07:54 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 17:07:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 17:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 17:07:57 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 17:07:57 GMT
CMD ["rabbitmq-server"]
```

-	Layers:
	-	`sha256:671716cc49517eef5f430c695ce344d63e390cb65f58d30939f2ba615c953686`  
		Last Modified: Mon, 09 Oct 2017 21:49:09 GMT  
		Size: 22.3 MB (22339951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cae61f12be6f01ba06573d9393712e91821cd5496302310f550fe5842dea557`  
		Last Modified: Fri, 03 Nov 2017 17:08:41 GMT  
		Size: 4.5 MB (4529879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca307103ce923e7e89d35185be4df8e54c3c0b54d259b8880aa7bae107d4952`  
		Last Modified: Fri, 03 Nov 2017 17:08:39 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d16320f9fc35ea20ba7fb9b21f88e3f0f06c52d416682319f3b2a85a345a3d5`  
		Last Modified: Fri, 03 Nov 2017 17:08:39 GMT  
		Size: 938.0 KB (938019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801205b182b8d6f7acf36200b2ba07ed52ea224dfefe792b525224e4aacb4d4a`  
		Last Modified: Fri, 03 Nov 2017 17:08:48 GMT  
		Size: 25.6 MB (25619372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9cb605e6242f5ab505cbd229c7b2fdf2935a6254130070c12c4d8413616024`  
		Last Modified: Fri, 03 Nov 2017 17:08:40 GMT  
		Size: 6.9 MB (6926791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2799e1b1479136fbb3c3ba6df318d449990a3cf5fc3293a14142cde0d9f51980`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a6d5de3e6aaa1c06122a1b5cda3b4bcb98d54e5dc23f38896fc81e98cea769`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172fa2e52818dcedf69c727f6790f0f9744f8538da3f4222602aaa0ab9fa82c0`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c734f2707800c1189521a51409fed1508fb7e36c6e67eca5537d03c4b24ef0d`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 4.0 KB (4037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e7d712f1155d66243480cd441ec04e084a8e7e2d6a0653e27138b31b56d2ae`  
		Last Modified: Fri, 03 Nov 2017 17:08:38 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rabbitmq:management`

```console
$ docker pull rabbitmq@sha256:90b467d41e6655bb52d7114802c028eb359e220a7ec87c98a23a294af2b81ad4
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

### `rabbitmq:management` - linux; amd64

```console
$ docker pull rabbitmq@sha256:40a956f5198d4d2050d1545dc48bf38b5e0342c33d10bcd04c9e0a7e7bc851af
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.9 MB (62852369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ac724eab06670229b033f2516a2e3af2cdfb453495a9bbb040fea13b398ab5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:33:42 GMT
ADD file:45233d6b5c9b91e9437065d3e7c332d1c4eb4bce8e1079a4c1af342c450abe67 in / 
# Mon, 09 Oct 2017 21:33:43 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 02:41:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:41:43 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 02:41:43 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 02:42:10 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 02:42:40 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 02:42:41 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 02:42:41 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 02:42:42 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 02:43:16 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:43:16 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 02:43:17 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 02:43:17 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 02:43:18 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 02:43:19 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 13 Oct 2017 23:40:43 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 13 Oct 2017 23:40:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 13 Oct 2017 23:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2017 23:40:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 13 Oct 2017 23:40:45 GMT
CMD ["rabbitmq-server"]
# Fri, 13 Oct 2017 23:40:56 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 13 Oct 2017 23:40:57 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:bc95e04b23c06ba1b9bf092d07d1493177b218e0340bd2ed49dac351c1e34313`  
		Last Modified: Mon, 09 Oct 2017 21:42:28 GMT  
		Size: 22.5 MB (22492350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65f0b00e4cfb1535d0f4e7a63707172ae63483fb33140d777614f199afcb36`  
		Last Modified: Tue, 10 Oct 2017 02:43:59 GMT  
		Size: 4.5 MB (4498726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bd803179890909fcae186044c0e6ca1bc1d34e5fc05ef1ccea823e7be97540`  
		Last Modified: Tue, 10 Oct 2017 02:43:57 GMT  
		Size: 4.1 KB (4069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b05ca8302833edf783c50f03cd7ba0b8e12bc872b053eda3e3ae7e1f17e2b4b`  
		Last Modified: Tue, 10 Oct 2017 02:43:58 GMT  
		Size: 952.1 KB (952058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb5a4bbcce5a040eb83057f9e93d17663bb123f4e98168457444497f7d17b70`  
		Last Modified: Tue, 10 Oct 2017 02:44:03 GMT  
		Size: 27.7 MB (27703883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf840d8999f6fe46a162974c82378c38b3cf3dcccbbaff848c0fb199988aebe0`  
		Last Modified: Tue, 10 Oct 2017 02:44:00 GMT  
		Size: 7.2 MB (7194403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be339ca44883b1990e52771487402163d398a279755a501fdd8891ec71cf09d0`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce35cd9f9b5b917868095b3b074dd23d18e0e266f3ee68ff95e2c61467299812`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fe32a0a00d916ed4d632aae71d35d9d0baa5e5910d6bd179a24071c35bedb0`  
		Last Modified: Tue, 10 Oct 2017 02:43:55 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77408ca9e94eb4bfeb346ab10c602857525802c2279e7c6995fcdbc90269444a`  
		Last Modified: Fri, 13 Oct 2017 23:41:26 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db03407a1aba1c0a89dffe960394aae639885702e3faa65271b918c36c7905cd`  
		Last Modified: Fri, 13 Oct 2017 23:41:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b908f008ac2afe6632caccd124e3ee9bffd5ebcdb8ca5ca84ae7e014305e460f`  
		Last Modified: Fri, 13 Oct 2017 23:42:01 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management` - linux; arm variant v5

```console
$ docker pull rabbitmq@sha256:07150eac8a231b8c043f29aba9a9ba3d81aa4cdd16c8e3387621deb4d8fdf1f4
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58432562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00088686092d95f6db193285835d1af5662557d679f57a4c21d1d4ec648c0924`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:44:48 GMT
ADD file:ff9945b48b1ac236dcec24eb9dfaf52b7c151a3b11c8502391f0866dfb4e3ac3 in / 
# Mon, 09 Oct 2017 21:44:48 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 00:18:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:18:11 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 00:18:11 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 00:18:29 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 00:18:58 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:18:58 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 00:18:58 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 00:18:59 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 00:19:26 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 00:19:26 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 00:19:27 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 00:19:28 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 00:19:29 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 00:19:30 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Sat, 14 Oct 2017 14:14:24 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Sat, 14 Oct 2017 14:14:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 14 Oct 2017 14:14:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 Oct 2017 14:14:25 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Sat, 14 Oct 2017 14:14:26 GMT
CMD ["rabbitmq-server"]
# Sat, 14 Oct 2017 14:14:34 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Sat, 14 Oct 2017 14:14:34 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:836d5b6056a9815be79c76480a90299267f60201bd1e3396817003e6c14819cc`  
		Last Modified: Mon, 09 Oct 2017 21:50:56 GMT  
		Size: 21.2 MB (21166251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb896fba83bd09a35c68457554b35289860c23c46f27a8c3ef42f13146ebba1`  
		Last Modified: Tue, 10 Oct 2017 00:20:01 GMT  
		Size: 4.2 MB (4231979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61827a16c114b9741d761aa4c60a972ffe1e0b60147794e86b05653d67822e91`  
		Last Modified: Tue, 10 Oct 2017 00:20:00 GMT  
		Size: 4.1 KB (4079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877cd9511def30e56a5ce354e145e8a2b1a93daaae7eaaa42dc4219838aa1743`  
		Last Modified: Tue, 10 Oct 2017 00:20:00 GMT  
		Size: 942.8 KB (942752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea9e378899e98c99e93ae2d0874bd5d89e24134bd14a19c285bdf39a0a42ade`  
		Last Modified: Tue, 10 Oct 2017 00:20:05 GMT  
		Size: 25.2 MB (25170810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc82a29314b16531aa2172ac523ba535e3678f85efdd699164fbb0241ab8b62`  
		Last Modified: Tue, 10 Oct 2017 00:20:01 GMT  
		Size: 6.9 MB (6909811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c44a3d016cf9de95021782180a42d3660e20fc7d8e92a7fe5ce9ede7928ca2`  
		Last Modified: Tue, 10 Oct 2017 00:19:59 GMT  
		Size: 2.3 KB (2261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abfdcdd98b40291ad91791bea09bf277e75c3669c6607c7891b09130101bfa3`  
		Last Modified: Tue, 10 Oct 2017 00:19:58 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a72811da4bf8ca8a2d06cdc182aa54116bb12133e8d82ef2b018a8de29ed74`  
		Last Modified: Tue, 10 Oct 2017 00:19:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147d8cf0897dea9b024bf5c6efb6873db3d86dec857fca062b146f88b7b5a735`  
		Last Modified: Sat, 14 Oct 2017 14:14:43 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f355fd0b70caedf30aa384298307b8e40d922e9e341492dd3fde71f119fd7d7`  
		Last Modified: Sat, 14 Oct 2017 14:14:44 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77dcaa76990445223000f8a5eb10485f94e82d4817f74f142f106b0a4dd9ad0c`  
		Last Modified: Sat, 14 Oct 2017 14:15:02 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management` - linux; arm variant v7

```console
$ docker pull rabbitmq@sha256:353fc3a4b10cc0fd93baf80287c8e7c779c49d7fd5421091aa004286b3bf559c
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55688342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd5c488f599ef650e2dc6824d489473db268160f94789b74f5ec312eef58600d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:43 GMT
ADD file:b758c6c3ff989778bd740dde35c86b953fa09be913a7e02711b2881de6b8911d in / 
# Mon, 09 Oct 2017 21:45:44 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 13:07:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:07:42 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 13:07:42 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 13:07:58 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 13:08:17 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:08:17 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 13:08:17 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 13:08:18 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 13:08:39 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 13:08:39 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 13:08:40 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 13:08:41 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 13:08:42 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 13:08:43 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 13:08:43 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 13:08:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 13:08:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 13:08:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 13:08:45 GMT
CMD ["rabbitmq-server"]
# Fri, 03 Nov 2017 13:09:01 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 03 Nov 2017 13:09:01 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:59e81a3fde58ec8d4b8f2f58b98ef2f4d951d37dd9b99b016fd294a8e07d7796`  
		Last Modified: Mon, 09 Oct 2017 21:52:49 GMT  
		Size: 19.3 MB (19277135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2037b99f3c3dc51e8ace39aed9971155f34f325ac4f0a1e56a07c4d6c02f5ae6`  
		Last Modified: Fri, 03 Nov 2017 13:09:18 GMT  
		Size: 3.9 MB (3868347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f368172ea96bda944832762ad29b52dfe17ec5e6fae96eee37adc4e9d68674a5`  
		Last Modified: Fri, 03 Nov 2017 13:09:16 GMT  
		Size: 4.1 KB (4084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893cc1ae60f8bf72ac3020ccc60b22d9e0ad0cb0647e15bc4847d08c8985eee2`  
		Last Modified: Fri, 03 Nov 2017 13:09:16 GMT  
		Size: 926.1 KB (926097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13220cc1a683014bda9cfae7f7ee7015a26b28048f90f5aa3ed8b6a96f4b2813`  
		Last Modified: Fri, 03 Nov 2017 13:09:20 GMT  
		Size: 24.8 MB (24785610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269f4e069126132643c1c0be1faf600d55ff15e870066c527d03181904d99c5d`  
		Last Modified: Fri, 03 Nov 2017 13:09:17 GMT  
		Size: 6.8 MB (6820180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ae244f4f610a339fcbddf37612a15ec7b7f6674e3d888c3c4d36302283418e`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce7d85327b7bc7d59a7b54222a3e6babd7f8afd8eb080becb77fc52aed5a751`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dfa32e4b49700ed0130ebd563f40a2c381393983b571a9886435813102ad0c`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba15cd885dc21f438d366b40d0d9f595f2c25e063c60fa590ab4c0f6233ff94`  
		Last Modified: Fri, 03 Nov 2017 13:09:14 GMT  
		Size: 4.0 KB (4040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978a8434497fcb8e08cefc7484b515ac34fe23c281fb869d015f62b54673028c`  
		Last Modified: Fri, 03 Nov 2017 13:09:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34fa59eaf946f8e35134f1a0bf195874868c3ce1e2a025350fc57efe60ecbea`  
		Last Modified: Fri, 03 Nov 2017 13:09:54 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:4ad104ab7b291ca9aea4bb42e18de213ae21ef6a655d909c3568e2b36f465074
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57278563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9356e7f3d3e445f04242803fb4b5afb70fad5f726388635b781f4814733c3af7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:47:55 GMT
ADD file:3a528355cfc75437716aff3b517ef99ae602918d84d26dbafff0ed142248fb93 in / 
# Mon, 09 Oct 2017 21:47:56 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 04:57:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg2 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 04:57:04 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Tue, 10 Oct 2017 04:57:05 GMT
ENV GOSU_VERSION=1.10
# Tue, 10 Oct 2017 04:57:37 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Tue, 10 Oct 2017 04:58:35 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 04:58:36 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Tue, 10 Oct 2017 04:58:37 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2017 04:58:37 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Tue, 10 Oct 2017 04:58:38 GMT
ENV RABBITMQ_VERSION=3.6.12
# Tue, 10 Oct 2017 04:58:39 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Tue, 10 Oct 2017 04:58:39 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Tue, 10 Oct 2017 05:00:22 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 05:00:23 GMT
ENV HOME=/var/lib/rabbitmq
# Tue, 10 Oct 2017 05:00:25 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Tue, 10 Oct 2017 05:00:26 GMT
VOLUME [/var/lib/rabbitmq]
# Tue, 10 Oct 2017 05:00:28 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Tue, 10 Oct 2017 05:00:31 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Sat, 14 Oct 2017 13:52:47 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Sat, 14 Oct 2017 13:52:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 14 Oct 2017 13:52:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 Oct 2017 13:52:51 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Sat, 14 Oct 2017 13:52:51 GMT
CMD ["rabbitmq-server"]
# Sat, 14 Oct 2017 13:53:08 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Sat, 14 Oct 2017 13:53:09 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:e907afd6e25615a4d3eb554d930cef57b87e79ec82413889c2eac38beb4eb8f7`  
		Last Modified: Mon, 09 Oct 2017 22:03:08 GMT  
		Size: 20.3 MB (20337143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5e6d35928560b933b85b5a3f2a8e96b4520fbb8df138b3e739e56d0c1f355`  
		Last Modified: Tue, 10 Oct 2017 05:01:18 GMT  
		Size: 4.1 MB (4073554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a862ab821b342790326492507ca5d70bfb7016bef765606193f1f7139f60c5ed`  
		Last Modified: Tue, 10 Oct 2017 05:01:14 GMT  
		Size: 4.1 KB (4072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92799a54920b79013733790e444f13d8c65faa29c79cbdaf1bc8af85f637a233`  
		Last Modified: Tue, 10 Oct 2017 05:01:14 GMT  
		Size: 919.5 KB (919487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b119999eef1bcadabedd3a5319b03c6b83ede91ba8535059851547d3433b205`  
		Last Modified: Tue, 10 Oct 2017 05:01:19 GMT  
		Size: 25.0 MB (25042572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62f8525a3a982a102aa37bb3313876195b15d8781cd253ed238dd2b9dff151`  
		Last Modified: Tue, 10 Oct 2017 05:01:15 GMT  
		Size: 6.9 MB (6894852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc028e70f04f6ea4365223a1cfe4e5c4384d5921acac419f3c170b148f7c7bf`  
		Last Modified: Tue, 10 Oct 2017 05:01:10 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e99faa03c2a8a272f56208c644c12b384b69dea50be6da9f6be400c14b945c`  
		Last Modified: Tue, 10 Oct 2017 05:01:12 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8fa260bcaa52d81ba20c11111f8d15bab954b17b48666724536c604220d94e`  
		Last Modified: Tue, 10 Oct 2017 05:01:11 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306840de948d03472918a306c089409429606802ec8cf841e96dec707a2f7178`  
		Last Modified: Sat, 14 Oct 2017 13:53:27 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a7a978032478b38adb1f0107466d187e53380f7037d058c62e4937cd07fc09`  
		Last Modified: Sat, 14 Oct 2017 13:53:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3facaa930064fd14fbd9a077b63e5f3261d1e63bd15c3d1426575c6c4f8eca`  
		Last Modified: Sat, 14 Oct 2017 13:54:17 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management` - linux; 386

```console
$ docker pull rabbitmq@sha256:16ab1fd6ebf60e7fe32149ac86bf79cd5a2e2d573dec3267fd0d7d646514384c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63902453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a8039a2961a84491da6ac62bad7d9b065b333750e66543f8e7cf931c13ed028`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:36 GMT
ADD file:6582536277127947668f7bfdc1471a4e36170915b91a4cb841e7e1bfa1de6535 in / 
# Mon, 09 Oct 2017 21:45:36 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 10:45:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:45:12 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 10:45:13 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 10:45:28 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 10:46:03 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 10:46:04 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 10:46:04 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 10:46:25 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 10:46:25 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 10:46:26 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 10:46:27 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 10:46:27 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 10:46:28 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 10:46:28 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 10:46:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 10:46:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 10:46:30 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 10:46:30 GMT
CMD ["rabbitmq-server"]
# Fri, 03 Nov 2017 10:46:58 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 03 Nov 2017 10:46:58 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:b2b52fe46b29fe5d0689f26449c2114e40f0731d4ce3eb8c3941397b74205432`  
		Last Modified: Mon, 09 Oct 2017 21:53:42 GMT  
		Size: 23.1 MB (23128678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d407b136da0731f5f38279001e9dd426217937443cad0f16e1f242366290773`  
		Last Modified: Fri, 03 Nov 2017 10:47:13 GMT  
		Size: 4.8 MB (4803637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c93817e78345b4b5070c81e5a37d02afc2b5fe347a1a4bf59e09f6084814fd2`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 4.1 KB (4057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97eae59c75f8f814ab781f5239ac2e132b7b65c77e75b35023c603c539ca54f`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 931.5 KB (931524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aed670dee19fde6946658d7129e13520c1a0747f8b80b6f92dac5f6d974ae52`  
		Last Modified: Fri, 03 Nov 2017 10:47:24 GMT  
		Size: 27.8 MB (27818690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b61d6d0b60ec18280aeba946a05d62817afbe030f277af85b5f434021e90c9`  
		Last Modified: Fri, 03 Nov 2017 10:47:16 GMT  
		Size: 7.2 MB (7208985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec7d4cc3b5497bbbd6b2d1e9574dbedb6c7ad11805cff4c287ea444ddc2e298`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 2.3 KB (2259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eec554591344f78e35e3976d002d617623a52d123fc71e65d33c4d533d2b2e7`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e433f73af1167eff0dee1984c095bf5be36593fcead5b8cc820e2cb829aaed0`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8d6e0dbdbb04b44f7a0972fce6b0b1b19262e4fc5416bd1589af560f16c99f`  
		Last Modified: Fri, 03 Nov 2017 10:47:12 GMT  
		Size: 4.0 KB (4040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bab08cf9b00d8109139e1cb1cdec448b71fdae7d7f1260d4175771416a5f80`  
		Last Modified: Fri, 03 Nov 2017 10:47:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2aad62bc4e7f6b9b68a5196e492b29083b8ab4e68dfea4a93b469cb79aae29`  
		Last Modified: Fri, 03 Nov 2017 10:48:04 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:47fb5bf4afd56afb9e9ab383f1449cee19c3ab7a7e653d0b04037cf839cfab52
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60384672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c4dbfbbd301b5dbb171ca49da8419b76567c7aa2d00978e12759ced95ca846`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:56 GMT
ADD file:7edf73437495be24244c16841b563be06c15452963f41ac940fb5e105ed96027 in / 
# Mon, 09 Oct 2017 21:45:58 GMT
CMD ["bash"]
# Fri, 03 Nov 2017 07:12:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:12:51 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Fri, 03 Nov 2017 07:12:53 GMT
ENV GOSU_VERSION=1.10
# Fri, 03 Nov 2017 07:13:49 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Fri, 03 Nov 2017 07:15:26 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:15:28 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Fri, 03 Nov 2017 07:15:29 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Nov 2017 07:15:31 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Fri, 03 Nov 2017 07:15:33 GMT
ENV RABBITMQ_VERSION=3.6.12
# Fri, 03 Nov 2017 07:15:34 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Fri, 03 Nov 2017 07:15:35 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 07:16:54 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 07:16:55 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 07:17:00 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 07:17:01 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 07:17:06 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 07:17:11 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 07:17:13 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 07:17:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 07:17:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 07:17:21 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 07:17:23 GMT
CMD ["rabbitmq-server"]
# Fri, 03 Nov 2017 07:17:36 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 03 Nov 2017 07:17:39 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:c4860466fa1e6824151f4fa3a51ef0e9d7d3c3ba860e21d94e69988b65601260`  
		Last Modified: Mon, 09 Oct 2017 21:52:59 GMT  
		Size: 22.7 MB (22746217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebe4c87dcd1f7ef11d4d21752831bf4095ac42afe041706c35f1d7d4d0ca4f2`  
		Last Modified: Fri, 03 Nov 2017 07:18:05 GMT  
		Size: 4.4 MB (4360529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e5365525084de1c85fa29ef33d37c38b5f80621f5bcb26bb4882d71598c6f7`  
		Last Modified: Fri, 03 Nov 2017 07:18:03 GMT  
		Size: 4.1 KB (4106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600c3853740b7f4cff9cc799ae478f669bd54277a8dd375479a34ed1bb47a803`  
		Last Modified: Fri, 03 Nov 2017 07:18:02 GMT  
		Size: 920.7 KB (920695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993868ec534130e348e45aa6d64b471fa46eafbf061836cc9d2a56edf73e9382`  
		Last Modified: Fri, 03 Nov 2017 07:18:06 GMT  
		Size: 25.5 MB (25492533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca1b92e212aaef163244d5fdd9e135fdb8be8c9dbbb626061ee2882d941a553`  
		Last Modified: Fri, 03 Nov 2017 07:18:03 GMT  
		Size: 6.9 MB (6853702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483f96d1f500f9f69170bc6927d599a7f0cd1550f96b6ee3f90eb4185a1bffb`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b433db63f40c7cab3080cf36bd7beabbdf7d9eece3f2dc16a65b900c61180`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93971551a2c911c34ca2e9af47495efb2f27e2922e567d93dd94dfb9b773bd3`  
		Last Modified: Fri, 03 Nov 2017 07:17:58 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5494bb8bcc45452a84c216edffedb3103a15c3e209aba0561dfbc70e4312192e`  
		Last Modified: Fri, 03 Nov 2017 07:17:59 GMT  
		Size: 4.0 KB (4039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d56b2a4f9f8d7b11831a8f1952fe2c02613bcb014ab9d756b70b3b398b37269`  
		Last Modified: Fri, 03 Nov 2017 07:17:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e2264063017ef705c9dcc066695ab771b32f19f38ba34c158531e7d3f4c9fc`  
		Last Modified: Fri, 03 Nov 2017 07:18:40 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management` - linux; s390x

```console
$ docker pull rabbitmq@sha256:35d9ecb54b432f7591ecfe0cb1ee71d152199b0ae07ecdd8c9b21cd6a87b0a51
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60364970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a628fac494ad4d163ad91471c151b4ed5bcfbe2f318bc677224413d944cf4ce8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Mon, 09 Oct 2017 21:44:35 GMT
ADD file:ae4aaa6affe22f36ab5478771d5c84917f72de7a8dac16345a035709a1a5edf4 in / 
# Mon, 09 Oct 2017 21:44:36 GMT
CMD ["bash"]
# Thu, 02 Nov 2017 17:06:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 		dirmngr 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 17:06:41 GMT
RUN groupadd -r rabbitmq && useradd -r -d /var/lib/rabbitmq -m -g rabbitmq rabbitmq
# Thu, 02 Nov 2017 17:06:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 02 Nov 2017 17:07:21 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Thu, 02 Nov 2017 17:07:43 GMT
RUN set -ex; 	apt-get update; 	if apt-cache show erlang-base-hipe 2>/dev/null | grep -q 'Package: erlang-base-hipe'; then 		apt-get install -y --no-install-recommends 			erlang-base-hipe 		; 	fi; 	apt-get install -y --no-install-recommends 		erlang-asn1 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang-nox 		erlang-os-mon 		erlang-public-key 		erlang-ssl 		erlang-xmerl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 02 Nov 2017 17:07:44 GMT
ENV PATH=/usr/lib/rabbitmq/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 02 Nov 2017 17:07:44 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 02 Nov 2017 17:07:45 GMT
ENV RABBITMQ_DEBIAN_VERSION=3.6.12-1
# Fri, 03 Nov 2017 17:07:48 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 		wget -O rabbitmq-server.deb.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb.asc"; 	wget -O rabbitmq-server.deb     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server_${RABBITMQ_DEBIAN_VERSION}_all.deb"; 		apt-get purge -y --auto-remove ca-certificates wget; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.deb.asc rabbitmq-server.deb; 	rm -rf "$GNUPGHOME"; 		apt install -y --no-install-recommends ./rabbitmq-server.deb; 	dpkg -l | grep rabbitmq-server; 	rm -f rabbitmq-server.deb*; 		rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 17:07:48 GMT
ENV HOME=/var/lib/rabbitmq
# Fri, 03 Nov 2017 17:07:49 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Fri, 03 Nov 2017 17:07:50 GMT
VOLUME [/var/lib/rabbitmq]
# Fri, 03 Nov 2017 17:07:52 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Fri, 03 Nov 2017 17:07:53 GMT
RUN ln -sf "/usr/lib/rabbitmq/lib/rabbitmq_server-$RABBITMQ_VERSION/plugins" /plugins
# Fri, 03 Nov 2017 17:07:54 GMT
COPY file:7f3c1def1757a323e01e9cd9e65a31daea4925bdbddb08efd80abc7fe43d605e in /usr/local/bin/ 
# Fri, 03 Nov 2017 17:07:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Nov 2017 17:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Nov 2017 17:07:57 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Fri, 03 Nov 2017 17:07:57 GMT
CMD ["rabbitmq-server"]
# Fri, 03 Nov 2017 17:08:14 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Fri, 03 Nov 2017 17:08:15 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:671716cc49517eef5f430c695ce344d63e390cb65f58d30939f2ba615c953686`  
		Last Modified: Mon, 09 Oct 2017 21:49:09 GMT  
		Size: 22.3 MB (22339951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cae61f12be6f01ba06573d9393712e91821cd5496302310f550fe5842dea557`  
		Last Modified: Fri, 03 Nov 2017 17:08:41 GMT  
		Size: 4.5 MB (4529879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca307103ce923e7e89d35185be4df8e54c3c0b54d259b8880aa7bae107d4952`  
		Last Modified: Fri, 03 Nov 2017 17:08:39 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d16320f9fc35ea20ba7fb9b21f88e3f0f06c52d416682319f3b2a85a345a3d5`  
		Last Modified: Fri, 03 Nov 2017 17:08:39 GMT  
		Size: 938.0 KB (938019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801205b182b8d6f7acf36200b2ba07ed52ea224dfefe792b525224e4aacb4d4a`  
		Last Modified: Fri, 03 Nov 2017 17:08:48 GMT  
		Size: 25.6 MB (25619372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9cb605e6242f5ab505cbd229c7b2fdf2935a6254130070c12c4d8413616024`  
		Last Modified: Fri, 03 Nov 2017 17:08:40 GMT  
		Size: 6.9 MB (6926791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2799e1b1479136fbb3c3ba6df318d449990a3cf5fc3293a14142cde0d9f51980`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a6d5de3e6aaa1c06122a1b5cda3b4bcb98d54e5dc23f38896fc81e98cea769`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172fa2e52818dcedf69c727f6790f0f9744f8538da3f4222602aaa0ab9fa82c0`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c734f2707800c1189521a51409fed1508fb7e36c6e67eca5537d03c4b24ef0d`  
		Last Modified: Fri, 03 Nov 2017 17:08:37 GMT  
		Size: 4.0 KB (4037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e7d712f1155d66243480cd441ec04e084a8e7e2d6a0653e27138b31b56d2ae`  
		Last Modified: Fri, 03 Nov 2017 17:08:38 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9489f6c1d1f9d4090b7d9220b20aac5cc7e9588c9ddf66d0357f1eb8226071`  
		Last Modified: Fri, 03 Nov 2017 17:09:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rabbitmq:management-alpine`

```console
$ docker pull rabbitmq@sha256:cc6bb38a4167c70483b6f174d43bf43032a23b1d9c661530cfda228bf60e3f87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `rabbitmq:management-alpine` - linux; amd64

```console
$ docker pull rabbitmq@sha256:ef2b9b2cbfbe00330d8cfaaf8acef1127996756ee66bad0ac832aba8e63ae67f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23579858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4927e0fd02a40ab3ffc333a1326f9a21be7aec9059d82c2dfdc37580847a76f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:19:51 GMT
ADD file:1e87ff33d1b6765b793888cd50e01b2bd0dfe152b7dbb4048008bfc2658faea7 in / 
# Wed, 25 Oct 2017 23:19:51 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 03:02:21 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 03:02:25 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 03:02:32 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 03:02:32 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 03:02:32 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 03:02:33 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 03:02:33 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 03:02:42 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 03:02:42 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 03:02:43 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 03:02:43 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 03:02:44 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 03:02:44 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 03:02:45 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 03:02:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 03:02:45 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 03:02:45 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 03:02:59 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 03:02:59 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:b56ae66c29370df48e7377c8f9baa744a3958058a766793f821dadcb144a4647`  
		Last Modified: Wed, 25 Oct 2017 23:21:25 GMT  
		Size: 2.0 MB (1991435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827e0bce86e3c8fa677ac91f0c55a7a4071cc45c729b171aecbe04d35ae160d7`  
		Last Modified: Thu, 26 Oct 2017 03:03:23 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe01d115cb92dc0ab37de6b6ffa2073ea20d30dfc49c537fbba569cd6a494b8`  
		Last Modified: Thu, 26 Oct 2017 03:03:23 GMT  
		Size: 8.2 KB (8176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bfc0dbbf8b1d2f532779c4873b4c7e0237d6ecc86161b1c6f28e3b6bd3149f`  
		Last Modified: Thu, 26 Oct 2017 03:03:26 GMT  
		Size: 16.6 MB (16561644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b24f4fd26b3494d310561a28e2d9aeb08e7baba442eaef2cd8697c7ebd9d9f1`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 5.0 MB (5012671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfb0f3b402f9674b21d7ed079f6576ec1be80f333f41c404e8ce3feb193b813`  
		Last Modified: Thu, 26 Oct 2017 03:03:22 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521b2b4b2311f153d53f0b9bde9a164f45df9dfd531512c36195ba2ccf5a4c76`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cedbb525e85f1b9257e8b20d04b4ad39f1004c9dfbc673086815dd887f380c3`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f35995cc5f5daa05334d17a87482ac8728aadfb0f10f9d62b3d70f5986e5cc`  
		Last Modified: Thu, 26 Oct 2017 03:03:21 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f1f0f842cbbd9046d7b95afc926b8e22e4befd18e38ed5d4514e14105d2be`  
		Last Modified: Thu, 26 Oct 2017 03:04:25 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; arm variant v6

```console
$ docker pull rabbitmq@sha256:e8e0295fdf1734258af64b4f82784721e845b6a68146965bd1592c0e15c58d1a
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.4 MB (23413037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1379abcce7a4a22ec254dfd3fe56547de4c89c0b12cfaf5e044ea05c4205dfb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:35 GMT
ADD file:009348222efb3c4ca2e53c387fb34c488679ca07db39525a6c5cc214e46abffd in / 
# Wed, 25 Oct 2017 23:28:36 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:36 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 05:25:53 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 05:25:55 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 05:26:10 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 05:26:10 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 05:26:10 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 05:26:11 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 05:26:11 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 05:26:19 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 05:26:19 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 05:26:20 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 05:26:20 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 05:26:21 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 05:26:22 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 05:26:22 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 05:26:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 05:26:22 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 05:26:23 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 05:26:30 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 05:26:30 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:0864efeeb5cb8dca4eb53e5d6fd38486daee80fa326fe36d1ad254f8fa6bb310`  
		Last Modified: Sun, 23 Jul 2017 20:21:42 GMT  
		Size: 2.0 MB (1965988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda69762aee1588fa82aeabf1af6d6ad24f737cce1451fab2e0199849b1e12e`  
		Last Modified: Wed, 25 Oct 2017 23:28:45 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62a8c5580cc1c2fbf2f9ce119bc0c06403a12ad18167bde2ec94420810916db`  
		Last Modified: Thu, 26 Oct 2017 05:26:38 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b096e39434b5aeddcb2ec167b7bf570cac7b8b16e68324d3f46c6f4d41b69c79`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 8.4 KB (8374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ad9273316fa6f22cd2e8cf88c92f34c3210325fa1be2041153a96f4124476f`  
		Last Modified: Thu, 26 Oct 2017 05:26:41 GMT  
		Size: 16.4 MB (16420180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed982c9e7d5644c85267595b470c0f21f25093a865603ab33304248efdb68b5d`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 5.0 MB (5012332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b76830a9cb5b5f898068945d6af6325c7d97b36d50e521a12097d3e908fd0`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a31f9ee2285379d9d5106926e707698e7a3283f707a4573fec9731e6ede58b5`  
		Last Modified: Thu, 26 Oct 2017 05:26:36 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff38544dc85623170156958b2d5d51604efd94b336b47a6479cde0417667838f`  
		Last Modified: Thu, 26 Oct 2017 05:26:36 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564bee8c5f497342e71777f1adc38d1578f7c95ddefe18efa16fc01b3e7e2a52`  
		Last Modified: Thu, 26 Oct 2017 05:26:37 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fe4d4545d22113e1fa0e2fbc7ae69364213b6ca264274a71ad66ac045835d1`  
		Last Modified: Thu, 26 Oct 2017 05:26:49 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; arm64 variant v8

```console
$ docker pull rabbitmq@sha256:bf020d55089aa6f03eb3e259eefa2014a2191041616b46f4c7e56fd10fd09b76
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.3 MB (23318349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67e8f6bc203146953e13d3ce7086f40a6796ae711f8d8231aac5693d99175f9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:58 GMT
ADD file:45b5d3b8d5490ba7edfca2cf6f54cdcf49c772b0b3a2302ce69a7af061007aa4 in / 
# Wed, 25 Oct 2017 23:28:59 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:59 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 13:53:09 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 13:53:13 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 13:53:28 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 13:53:28 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 13:53:29 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 13:53:29 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 13:53:30 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 13:53:30 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 13:53:31 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 13:54:22 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 13:54:23 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 13:54:24 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 13:54:25 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 13:54:26 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 13:54:28 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 13:54:29 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 13:54:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 13:54:30 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 13:54:30 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 13:54:47 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 13:54:47 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:bb473f0ebc12fde1bd45c1bd3c46f2d3aab367b1b7739464771455b9972f7894`  
		Last Modified: Thu, 06 Jul 2017 09:54:42 GMT  
		Size: 1.9 MB (1914748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ff6b7ff3a208b8399e701e7ea1b7edbdc654c8c60d33c6f09a7803e2dda776`  
		Last Modified: Wed, 25 Oct 2017 23:29:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05834eac152e30997eb4f1aa4ffe8e952bd759c1a1009bd183dec80dca24cf86`  
		Last Modified: Thu, 26 Oct 2017 13:55:11 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd88a23486b40755f2e1192cb35d4fdaec20831c18ce83da31df3f8aa2f7b45c`  
		Last Modified: Thu, 26 Oct 2017 13:55:11 GMT  
		Size: 8.3 KB (8297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f9ba1206e6e4bfba21cef7f235482b41868ec966d5ebc44a4c4ac432a5fe03`  
		Last Modified: Thu, 26 Oct 2017 13:55:16 GMT  
		Size: 16.4 MB (16376872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5991837e23d785829d605fd052c61e10ed79a7cfb0dfee9dd40d6144bc9fad0f`  
		Last Modified: Thu, 26 Oct 2017 13:55:12 GMT  
		Size: 5.0 MB (5012322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf5663fa552ede671fc5ebf425b2ce3ff5257636b55df9564e556fe7ff85fce`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794d04d767a60fa6df4adb3af1f835701a3c2692e7f6b2d4a9db621a0bc8cd5f`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91155b0cb6bf92d1ab05fb7d13593e0a966eb79dd4e4173e3895d98dffe1c996`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969bbed547aa67091daaa801a46b062fd1c39f7835c81dd5052032056b6cf230`  
		Last Modified: Thu, 26 Oct 2017 13:55:09 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1643075e82e89fd6745e0baa4b9fd436da4f959fffedec9f0d149f84a7c16f8f`  
		Last Modified: Thu, 26 Oct 2017 13:56:10 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; 386

```console
$ docker pull rabbitmq@sha256:775482d2d2f81b04a7f91840ed0a169b185315f4dc226d515adaacb675e6f6dc
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23783181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:845026f49dc450aaf8e569e45ba76c8b1bf506da17e742b0a54fbddaf5bcf9f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:32:08 GMT
ADD file:4a952fc4b81d50b342e26a818dac48a148a4d5eddb878219650e579a5c9faeaa in / 
# Wed, 25 Oct 2017 23:32:08 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:32:08 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 10:44:24 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 10:44:28 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 10:44:50 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 10:44:50 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 10:44:50 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 10:44:51 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 10:44:51 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 10:45:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 10:45:05 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 10:45:06 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 10:45:06 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 10:45:07 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 10:45:07 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 10:45:08 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 10:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 10:45:08 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 10:45:08 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 10:45:16 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 10:45:16 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:ffe4428ef008913a7ec63449e4ad3aa536b26103943146a302591dfceb157d2f`  
		Last Modified: Sat, 17 Jun 2017 18:08:13 GMT  
		Size: 2.0 MB (2045593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4fe786260f2bd2710289e7c9487b423cb252a691fa501759b0768516122869`  
		Last Modified: Wed, 25 Oct 2017 23:32:27 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cf0f0a132c9bb882206147dffad08dc780f2bc82556cfbda9878a3218f1e7c`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00a9186496c6602ccd3efb4bb1780b42adb7028c8fa3cd3c1ff2f10bcfa33a3`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 8.3 KB (8305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc19938c3bf2e858347a9c7add1beac38af5a4f83b99d80ddc004aa4ad51e596`  
		Last Modified: Thu, 26 Oct 2017 10:45:30 GMT  
		Size: 16.7 MB (16710838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697b9a0ea77c953a543f168ba09045ae412f3b2bd0947b2bba8c18cd0cd2c70b`  
		Last Modified: Thu, 26 Oct 2017 10:45:30 GMT  
		Size: 5.0 MB (5012335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca279d1203917e8f98e0d5fe3f9de9bdde74bae202990b6388e1cc748caa726`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb3c81d25b2aa6fa5bf57aaf5f8ad6a5f27be02727e454818ff546e5a989c88`  
		Last Modified: Thu, 26 Oct 2017 10:45:29 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420233201c5d7a33d69bc90b4ac40d5db1285e61718701ffd97d4db8396a9508`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0b37b1c6d397d7b0daa633cac4b2d202e9656dd6340dc40496303190ed4a78`  
		Last Modified: Thu, 26 Oct 2017 10:45:28 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b719c08f02439306e8baee89f388d47a99542fc0eec294aaf615c425ec5253de`  
		Last Modified: Thu, 26 Oct 2017 10:45:59 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; ppc64le

```console
$ docker pull rabbitmq@sha256:1f2ed16a80e1b71fd652fe7520fa1ba2ac5c9b5a207199bc7aaec39c61d5a38e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23640124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0244f72e17b275644966d172a75c7023650024e2761d2541020cbb3592bd01f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:47 GMT
ADD file:e0be8616517d68cb80a2f9b74eb967cda22b9937bbcbe8b75b6153815a6f7761 in / 
# Wed, 25 Oct 2017 23:28:48 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:50 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 07:12:01 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 07:12:12 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 07:12:36 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 07:12:37 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 07:12:39 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 07:12:41 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 07:12:42 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 07:12:44 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 07:12:45 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 07:13:07 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 07:13:09 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 07:13:13 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 07:13:15 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 07:13:19 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 07:13:23 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 07:13:25 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 07:13:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 07:13:28 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 07:13:30 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 07:13:42 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 07:13:44 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:1e52418956f7d2a8ea35e8e6e3318fd08e005b27457d77868c225e7433bbfa02`  
		Last Modified: Thu, 20 Jul 2017 15:12:59 GMT  
		Size: 2.0 MB (2008578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf472f4e5bb7956ac20bb343b304e1d3de1f79160c0d158cccbe25980022d50`  
		Last Modified: Wed, 25 Oct 2017 23:29:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48c95ed960185dbd69324a206614e723f0086f80b46bd3223f233e4f1e278bc`  
		Last Modified: Thu, 26 Oct 2017 07:14:01 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a8242358db9adbde1a17b0e2b320c02112fcefa90d397ecc028a9729efcf94`  
		Last Modified: Thu, 26 Oct 2017 07:14:01 GMT  
		Size: 9.1 KB (9059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6db9581873eb0cadddc4d474e33cb2ec978c0d68e3ea124ce4f07ab2731d79`  
		Last Modified: Thu, 26 Oct 2017 07:14:04 GMT  
		Size: 16.6 MB (16603134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a991ac52f27ddaf9fb4021acf59b12957c4fa6251ab4d74159bb54ac63878009`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 5.0 MB (5013168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d098ea301752e2203c7ad872d2a38cc3da3efa183b01e61fe5c2fcde29efceb8`  
		Last Modified: Thu, 26 Oct 2017 07:14:00 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8727c952955dcfc3ce7e96c808c78bc91d43e6033164a46a7faffd11dc22fb69`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fe10e7f312fce5a9bf6ca051d683f86b1cef271217890a7ea53164ef81c99d`  
		Last Modified: Thu, 26 Oct 2017 07:13:58 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcba876c6e465f99a2952b71be993ce0d4d82ef4f70f72a59e58200cf263252f`  
		Last Modified: Thu, 26 Oct 2017 07:13:59 GMT  
		Size: 4.0 KB (4038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d8f64c426c0a1bf9de5b158513294037721b7e6c1c4fbc5e75f84a63743aae`  
		Last Modified: Thu, 26 Oct 2017 07:14:31 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rabbitmq:management-alpine` - linux; s390x

```console
$ docker pull rabbitmq@sha256:4af0a8312682b92651de05ff83aac54b00b55118b9babda060c043b4fdf9609b
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.8 MB (23819037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b62c33cd033388e2676822a15081284e991d3078ed4b51ebab5b72b7cb5a983`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["rabbitmq-server"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:40 GMT
ADD file:6fbdff4b4c08600e192f5da9b67a02c58759237fb40525d70712104c80c34c48 in / 
# Wed, 25 Oct 2017 23:28:40 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:40 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2017 17:06:39 GMT
RUN addgroup -S rabbitmq && adduser -S -h /var/lib/rabbitmq -G rabbitmq rabbitmq
# Thu, 26 Oct 2017 17:06:42 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 26 Oct 2017 17:06:55 GMT
RUN apk add --no-cache 		bash 		procps 		erlang-asn1 		erlang-hipe 		erlang-crypto 		erlang-eldap 		erlang-inets 		erlang-mnesia 		erlang 		erlang-os-mon 		erlang-public-key 		erlang-sasl 		erlang-ssl 		erlang-syntax-tools 		erlang-xmerl
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_LOGS=- RABBITMQ_SASL_LOGS=-
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_HOME=/opt/rabbitmq
# Thu, 26 Oct 2017 17:06:56 GMT
ENV PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Oct 2017 17:06:56 GMT
ENV RABBITMQ_GPG_KEY=0A9AF2115F4687BD29803A206B73A36E6026DFCA
# Thu, 26 Oct 2017 17:06:57 GMT
ENV RABBITMQ_VERSION=3.6.12
# Thu, 26 Oct 2017 17:06:57 GMT
ENV RABBITMQ_GITHUB_TAG=rabbitmq_v3_6_12
# Thu, 26 Oct 2017 17:07:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		ca-certificates 		gnupg 		libressl 		xz 	; 		wget -O rabbitmq-server.tar.xz.asc "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz.asc"; 	wget -O rabbitmq-server.tar.xz     "https://github.com/rabbitmq/rabbitmq-server/releases/download/$RABBITMQ_GITHUB_TAG/rabbitmq-server-generic-unix-${RABBITMQ_VERSION}.tar.xz"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$RABBITMQ_GPG_KEY"; 	gpg --batch --verify rabbitmq-server.tar.xz.asc rabbitmq-server.tar.xz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$RABBITMQ_HOME"; 	tar 		--extract 		--verbose 		--file rabbitmq-server.tar.xz 		--directory "$RABBITMQ_HOME" 		--strip-components 1 	; 	rm -f rabbitmq-server.tar.xz*; 		grep -qE '^SYS_PREFIX=\$\{RABBITMQ_HOME\}$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	sed -ri 's!^(SYS_PREFIX=).*$!\1!g' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 	grep -qE '^SYS_PREFIX=$' "$RABBITMQ_HOME/sbin/rabbitmq-defaults"; 		apk del .build-deps
# Thu, 26 Oct 2017 17:07:05 GMT
ENV HOME=/var/lib/rabbitmq
# Thu, 26 Oct 2017 17:07:06 GMT
RUN mkdir -p /var/lib/rabbitmq /etc/rabbitmq 	&& chown -R rabbitmq:rabbitmq /var/lib/rabbitmq /etc/rabbitmq 	&& chmod -R 777 /var/lib/rabbitmq /etc/rabbitmq
# Thu, 26 Oct 2017 17:07:06 GMT
VOLUME [/var/lib/rabbitmq]
# Thu, 26 Oct 2017 17:07:06 GMT
RUN ln -sf /var/lib/rabbitmq/.erlang.cookie /root/
# Thu, 26 Oct 2017 17:07:07 GMT
RUN ln -sf "$RABBITMQ_HOME/plugins" /plugins
# Thu, 26 Oct 2017 17:07:07 GMT
COPY file:59489bc2db97468b45a849e458889641a2f61b9a804db835bb9c32cb28661d1c in /usr/local/bin/ 
# Thu, 26 Oct 2017 17:07:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2017 17:07:08 GMT
EXPOSE 25672/tcp 4369/tcp 5671/tcp 5672/tcp
# Thu, 26 Oct 2017 17:07:08 GMT
CMD ["rabbitmq-server"]
# Thu, 26 Oct 2017 17:07:19 GMT
RUN rabbitmq-plugins enable --offline rabbitmq_management
# Thu, 26 Oct 2017 17:07:19 GMT
EXPOSE 15671/tcp 15672/tcp
```

-	Layers:
	-	`sha256:d45fd9d3c4f188ab1f3a4bf6a9f5202b3f1577dbb998f5f28e82d192e0c1f0e7`  
		Last Modified: Sat, 17 Jun 2017 20:41:42 GMT  
		Size: 2.1 MB (2065460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5978b6b34b3e943e0fd25dfb50991c0bad82a986cfdaa91c4de756431ba679`  
		Last Modified: Wed, 25 Oct 2017 23:28:59 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299a1fbc19bbea84dbf4d0b6e2e71fb847299b017209b1f9783faea14214c995`  
		Last Modified: Thu, 26 Oct 2017 17:07:31 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb76f2dd4162cae82233bc93ba436b63ca37e536d53c85a9f1d7343203e3c383`  
		Last Modified: Thu, 26 Oct 2017 17:07:31 GMT  
		Size: 8.6 KB (8604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac09bb55706d627cf6348c9d0bd891c2fe9a4155aee5d95264b92781371021db`  
		Last Modified: Thu, 26 Oct 2017 17:07:33 GMT  
		Size: 16.7 MB (16726549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e776aa2eebd7dc068e74be7736114ce80966ab2b25478d29763bc1ccf05c3e3`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 5.0 MB (5012317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57d3128b93c0f42a41ad6b2571d41e61c6096e070ee18ef58d34aeaf7318560`  
		Last Modified: Thu, 26 Oct 2017 17:07:29 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484c70be68b7dc1296d1199834238ebabbde1df9ce04ec3cf986a2096ad218b6`  
		Last Modified: Thu, 26 Oct 2017 17:07:29 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01611bf6acbe11966a7f1fe2e96d811430328e24513c20237576287afdd5079a`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 107.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f045868d086334dbd06f276dfb93c084fc32b243827527e36c2bc5a5d8583d`  
		Last Modified: Thu, 26 Oct 2017 17:07:30 GMT  
		Size: 4.0 KB (4036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed30107b153ffda65732449b2eea0bdac7dbd4327b3a82ef0fcd5553b0ca55fc`  
		Last Modified: Thu, 26 Oct 2017 17:07:50 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
