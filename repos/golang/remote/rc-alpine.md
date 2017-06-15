## `golang:rc-alpine`

```console
$ docker pull golang@sha256:c38ae20f711b570a2954bc0d82f6c458fd486670e096b1837dbbbcfaf27e03d8
```

-	Platforms:
	-	linux; amd64

### `golang:rc-alpine` - linux; amd64

-	Docker Version: 1.12.6
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.4 MB (77357271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14cea0631c902d0305363063c79ff3103e2ddf5cee78761ad17e9dcfb96fa64f`

```dockerfile
# Tue, 27 Dec 2016 18:17:25 GMT
ADD file:92ab746eb22dd3ed2b87469c719adf3c1bed7302653bbd76baafd7cfd95e911e in / 
# Wed, 04 Jan 2017 21:05:32 GMT
RUN apk add --no-cache ca-certificates
# Fri, 27 Jan 2017 22:40:25 GMT
ENV GOLANG_VERSION=1.8rc3
# Fri, 27 Jan 2017 22:40:26 GMT
ENV GOLANG_SRC_URL=https://golang.org/dl/go1.8rc3.src.tar.gz
# Fri, 27 Jan 2017 22:40:26 GMT
ENV GOLANG_SRC_SHA256=38b1c1738f111f7bccdd372efca2aa98a7bad1ca2cb21767ba69f34ae007499c
# Fri, 27 Jan 2017 22:40:27 GMT
COPY file:8bfad5c310fe0639fcf658b30e2f65d04df13ad329573b58a3e782441bb7839c in / 
# Fri, 27 Jan 2017 22:41:24 GMT
RUN set -ex 	&& apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 		&& export GOROOT_BOOTSTRAP="$(go env GOROOT)" 		&& wget -q "$GOLANG_SRC_URL" -O golang.tar.gz 	&& echo "$GOLANG_SRC_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz 	&& cd /usr/local/go/src 	&& patch -p2 -i /no-pic.patch 	&& ./make.bash 		&& rm -rf /*.patch 	&& apk del .build-deps
# Fri, 27 Jan 2017 22:41:25 GMT
ENV GOPATH=/go
# Fri, 27 Jan 2017 22:41:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2017 22:41:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 27 Jan 2017 22:41:27 GMT
WORKDIR /go
# Fri, 27 Jan 2017 22:41:28 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
```

-	Layers:
	-	`sha256:0a8490d0dfd399b3a50e9aaa81dba0d425c3868762d46526b41be00886bcc28b`  
		Last Modified: Tue, 27 Dec 2016 18:19:22 GMT  
		Size: 1.9 MB (1902063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb658c9d1694c3ba35ef345a0f46dcb9776452cccfa11aa7d41f288392fd6556`  
		Last Modified: Wed, 04 Jan 2017 23:49:03 GMT  
		Size: 352.7 KB (352746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b77659c964ebe0d002d9b13573767c193373f4b9ffa9fe95c193bf9b594c589`  
		Last Modified: Fri, 27 Jan 2017 22:56:56 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56df225bacc5e66a4bc0008e768c20e6a7967917e7204b325b4794738ca1876b`  
		Last Modified: Fri, 27 Jan 2017 22:57:20 GMT  
		Size: 75.1 MB (75100544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b037eb6f8a481272e46e7c9f668e7ce2cc9d7472b7e1c3ad570d93d3d5aa2fc`  
		Last Modified: Fri, 27 Jan 2017 22:56:56 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da4af2aec2aeb5609d2f948b24fd541eb250279d93ee551ecba9bf2711c5365`  
		Last Modified: Fri, 27 Jan 2017 22:56:56 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
