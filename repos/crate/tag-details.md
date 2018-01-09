<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `crate`

-	[`crate:2.0`](#crate20)
-	[`crate:2.0.7`](#crate207)
-	[`crate:2.1`](#crate21)
-	[`crate:2.1.10`](#crate2110)
-	[`crate:2.2`](#crate22)
-	[`crate:2.2.5`](#crate225)
-	[`crate:latest`](#cratelatest)

## `crate:2.0`

```console
$ docker pull crate@sha256:6bd487920fc2e9b6a8e0ea48ecd24da0593bed5eb44a6f2a0974ac89a1b5b157
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `crate:2.0` - linux; amd64

```console
$ docker pull crate@sha256:2183a78afcd4f90bb2688003541b04fa2ae27acf8082d0420c22e51a084c6bc1
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126532762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc82bfc4e3354b3033584d0a2da6cd69c746421eeca717e1cedf5bd42640abac`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 09 Jan 2018 21:13:01 GMT
ADD file:df48d6d6df42a01380557aebd4ca02807fc08a76a1d1b36d957e59a41c69db0b in / 
# Tue, 09 Jan 2018 21:13:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Jan 2018 21:54:39 GMT
MAINTAINER Crate.IO GmbH office@crate.io
# Tue, 09 Jan 2018 21:54:40 GMT
ENV GOSU_VERSION=1.9
# Tue, 09 Jan 2018 21:55:08 GMT
RUN set -x     && apk add --no-cache --virtual .gosu-deps         dpkg         gnupg         curl     && export ARCH=$(echo $(dpkg --print-architecture) | cut -d"-" -f3)     && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$ARCH"     && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$ARCH.asc"     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4     && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu     && rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc     && chmod +x /usr/local/bin/gosu     && gosu nobody true     && apk del .gosu-deps
# Tue, 09 Jan 2018 21:55:09 GMT
RUN addgroup crate && adduser -G crate -H crate -D
# Tue, 09 Jan 2018 21:56:47 GMT
ENV CRATE_VERSION=2.0.7
# Tue, 09 Jan 2018 21:57:43 GMT
RUN apk add --no-cache --virtual .crate-rundeps         openjdk8-jre-base         python3         openssl         sigar     && apk add --no-cache --virtual .build-deps         curl         gnupg         tar     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-$CRATE_VERSION.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-$CRATE_VERSION.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-$CRATE_VERSION.tar.gz.asc crate-$CRATE_VERSION.tar.gz     && rm -r "$GNUPGHOME" crate-$CRATE_VERSION.tar.gz.asc     && mkdir /crate     && tar -xf crate-$CRATE_VERSION.tar.gz -C /crate --strip-components=1     && rm crate-$CRATE_VERSION.tar.gz     && ln -s /usr/bin/python3 /usr/bin/python     && rm /crate/plugins/crate-sigar/libsigar-amd64-linux.so     && apk del .build-deps
# Tue, 09 Jan 2018 21:57:44 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jan 2018 21:57:44 GMT
VOLUME [/data]
# Tue, 09 Jan 2018 21:57:44 GMT
ADD file:f6ed1d4a953eca6984e33a751c11c6838562c006ffa19ab36d121906728e94db in /crate/config/crate.yml 
# Tue, 09 Jan 2018 21:57:45 GMT
ADD file:10c08bc017b942a11ef7f1221f33b8224b4549e98c74b9f84e2495fcfb60d8ce in /crate/config/log4j2.properties 
# Tue, 09 Jan 2018 21:57:45 GMT
COPY file:9517f117528edc569ebb34a2c1d3d7bcf342cb124f3b833a681768549d61ebfb in / 
# Tue, 09 Jan 2018 21:57:45 GMT
WORKDIR /data
# Tue, 09 Jan 2018 21:57:46 GMT
EXPOSE 4200/tcp 4300/tcp 5432/tcp 5433/tcp 5434/tcp 5435/tcp 5436/tcp 5437/tcp 5438/tcp 5439/tcp 5440/tcp 5441/tcp 5442/tcp 5443/tcp 5444/tcp 5445/tcp 5446/tcp 5447/tcp 5448/tcp 5449/tcp 5450/tcp 5451/tcp 5452/tcp 5453/tcp 5454/tcp 5455/tcp 5456/tcp 5457/tcp 5458/tcp 5459/tcp 5460/tcp 5461/tcp 5462/tcp 5463/tcp 5464/tcp 5465/tcp 5466/tcp 5467/tcp 5468/tcp 5469/tcp 5470/tcp 5471/tcp 5472/tcp 5473/tcp 5474/tcp 5475/tcp 5476/tcp 5477/tcp 5478/tcp 5479/tcp 5480/tcp 5481/tcp 5482/tcp 5483/tcp 5484/tcp 5485/tcp 5486/tcp 5487/tcp 5488/tcp 5489/tcp 5490/tcp 5491/tcp 5492/tcp 5493/tcp 5494/tcp 5495/tcp 5496/tcp 5497/tcp 5498/tcp 5499/tcp 5500/tcp 5501/tcp 5502/tcp 5503/tcp 5504/tcp 5505/tcp 5506/tcp 5507/tcp 5508/tcp 5509/tcp 5510/tcp 5511/tcp 5512/tcp 5513/tcp 5514/tcp 5515/tcp 5516/tcp 5517/tcp 5518/tcp 5519/tcp 5520/tcp 5521/tcp 5522/tcp 5523/tcp 5524/tcp 5525/tcp 5526/tcp 5527/tcp 5528/tcp 5529/tcp 5530/tcp 5531/tcp 5532/tcp
# Tue, 09 Jan 2018 21:57:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Jan 2018 21:57:46 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:550fe1bea624a5c62551cf09f3aa10886eed133794844af1dfb775118309387e`  
		Last Modified: Tue, 09 Jan 2018 21:15:20 GMT  
		Size: 2.0 MB (1970140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a978fe7044d71089ea637c37c568c9df275d1a6ad05b0b34e475496914e9a58e`  
		Last Modified: Tue, 09 Jan 2018 21:59:26 GMT  
		Size: 592.4 KB (592371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25eebb3b80cb7de09a89560ce9ba7da3435a0b6528d3e21de78b9578ee0a8e90`  
		Last Modified: Tue, 09 Jan 2018 21:59:25 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f735806177d568463fe7d1844af222a44087ed0e20aef17db1834c199f54f9`  
		Last Modified: Tue, 09 Jan 2018 22:00:24 GMT  
		Size: 124.0 MB (123967555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29a88f967a0e1380dcc9dc0046d05bce9dc1ad8997ba21ec0ab6ed137012237`  
		Last Modified: Tue, 09 Jan 2018 22:00:12 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c3c1ae12d1d2435d1de73fcae0555ec4fc9763e9cfb8ef192b91d05ef43a2d`  
		Last Modified: Tue, 09 Jan 2018 22:00:12 GMT  
		Size: 937.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af320c3899ea4114972e99b9ceb36385935066073a40dfd94e5768be834a9562`  
		Last Modified: Tue, 09 Jan 2018 22:00:13 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97b20567e616b79216bba539892a140650506e781a6089cfab722d6adcee3d5`  
		Last Modified: Tue, 09 Jan 2018 22:00:12 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:2.0.7`

```console
$ docker pull crate@sha256:6bd487920fc2e9b6a8e0ea48ecd24da0593bed5eb44a6f2a0974ac89a1b5b157
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `crate:2.0.7` - linux; amd64

```console
$ docker pull crate@sha256:2183a78afcd4f90bb2688003541b04fa2ae27acf8082d0420c22e51a084c6bc1
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126532762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc82bfc4e3354b3033584d0a2da6cd69c746421eeca717e1cedf5bd42640abac`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 09 Jan 2018 21:13:01 GMT
ADD file:df48d6d6df42a01380557aebd4ca02807fc08a76a1d1b36d957e59a41c69db0b in / 
# Tue, 09 Jan 2018 21:13:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Jan 2018 21:54:39 GMT
MAINTAINER Crate.IO GmbH office@crate.io
# Tue, 09 Jan 2018 21:54:40 GMT
ENV GOSU_VERSION=1.9
# Tue, 09 Jan 2018 21:55:08 GMT
RUN set -x     && apk add --no-cache --virtual .gosu-deps         dpkg         gnupg         curl     && export ARCH=$(echo $(dpkg --print-architecture) | cut -d"-" -f3)     && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$ARCH"     && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$ARCH.asc"     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4     && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu     && rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc     && chmod +x /usr/local/bin/gosu     && gosu nobody true     && apk del .gosu-deps
# Tue, 09 Jan 2018 21:55:09 GMT
RUN addgroup crate && adduser -G crate -H crate -D
# Tue, 09 Jan 2018 21:56:47 GMT
ENV CRATE_VERSION=2.0.7
# Tue, 09 Jan 2018 21:57:43 GMT
RUN apk add --no-cache --virtual .crate-rundeps         openjdk8-jre-base         python3         openssl         sigar     && apk add --no-cache --virtual .build-deps         curl         gnupg         tar     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-$CRATE_VERSION.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-$CRATE_VERSION.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-$CRATE_VERSION.tar.gz.asc crate-$CRATE_VERSION.tar.gz     && rm -r "$GNUPGHOME" crate-$CRATE_VERSION.tar.gz.asc     && mkdir /crate     && tar -xf crate-$CRATE_VERSION.tar.gz -C /crate --strip-components=1     && rm crate-$CRATE_VERSION.tar.gz     && ln -s /usr/bin/python3 /usr/bin/python     && rm /crate/plugins/crate-sigar/libsigar-amd64-linux.so     && apk del .build-deps
# Tue, 09 Jan 2018 21:57:44 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jan 2018 21:57:44 GMT
VOLUME [/data]
# Tue, 09 Jan 2018 21:57:44 GMT
ADD file:f6ed1d4a953eca6984e33a751c11c6838562c006ffa19ab36d121906728e94db in /crate/config/crate.yml 
# Tue, 09 Jan 2018 21:57:45 GMT
ADD file:10c08bc017b942a11ef7f1221f33b8224b4549e98c74b9f84e2495fcfb60d8ce in /crate/config/log4j2.properties 
# Tue, 09 Jan 2018 21:57:45 GMT
COPY file:9517f117528edc569ebb34a2c1d3d7bcf342cb124f3b833a681768549d61ebfb in / 
# Tue, 09 Jan 2018 21:57:45 GMT
WORKDIR /data
# Tue, 09 Jan 2018 21:57:46 GMT
EXPOSE 4200/tcp 4300/tcp 5432/tcp 5433/tcp 5434/tcp 5435/tcp 5436/tcp 5437/tcp 5438/tcp 5439/tcp 5440/tcp 5441/tcp 5442/tcp 5443/tcp 5444/tcp 5445/tcp 5446/tcp 5447/tcp 5448/tcp 5449/tcp 5450/tcp 5451/tcp 5452/tcp 5453/tcp 5454/tcp 5455/tcp 5456/tcp 5457/tcp 5458/tcp 5459/tcp 5460/tcp 5461/tcp 5462/tcp 5463/tcp 5464/tcp 5465/tcp 5466/tcp 5467/tcp 5468/tcp 5469/tcp 5470/tcp 5471/tcp 5472/tcp 5473/tcp 5474/tcp 5475/tcp 5476/tcp 5477/tcp 5478/tcp 5479/tcp 5480/tcp 5481/tcp 5482/tcp 5483/tcp 5484/tcp 5485/tcp 5486/tcp 5487/tcp 5488/tcp 5489/tcp 5490/tcp 5491/tcp 5492/tcp 5493/tcp 5494/tcp 5495/tcp 5496/tcp 5497/tcp 5498/tcp 5499/tcp 5500/tcp 5501/tcp 5502/tcp 5503/tcp 5504/tcp 5505/tcp 5506/tcp 5507/tcp 5508/tcp 5509/tcp 5510/tcp 5511/tcp 5512/tcp 5513/tcp 5514/tcp 5515/tcp 5516/tcp 5517/tcp 5518/tcp 5519/tcp 5520/tcp 5521/tcp 5522/tcp 5523/tcp 5524/tcp 5525/tcp 5526/tcp 5527/tcp 5528/tcp 5529/tcp 5530/tcp 5531/tcp 5532/tcp
# Tue, 09 Jan 2018 21:57:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Jan 2018 21:57:46 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:550fe1bea624a5c62551cf09f3aa10886eed133794844af1dfb775118309387e`  
		Last Modified: Tue, 09 Jan 2018 21:15:20 GMT  
		Size: 2.0 MB (1970140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a978fe7044d71089ea637c37c568c9df275d1a6ad05b0b34e475496914e9a58e`  
		Last Modified: Tue, 09 Jan 2018 21:59:26 GMT  
		Size: 592.4 KB (592371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25eebb3b80cb7de09a89560ce9ba7da3435a0b6528d3e21de78b9578ee0a8e90`  
		Last Modified: Tue, 09 Jan 2018 21:59:25 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f735806177d568463fe7d1844af222a44087ed0e20aef17db1834c199f54f9`  
		Last Modified: Tue, 09 Jan 2018 22:00:24 GMT  
		Size: 124.0 MB (123967555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29a88f967a0e1380dcc9dc0046d05bce9dc1ad8997ba21ec0ab6ed137012237`  
		Last Modified: Tue, 09 Jan 2018 22:00:12 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c3c1ae12d1d2435d1de73fcae0555ec4fc9763e9cfb8ef192b91d05ef43a2d`  
		Last Modified: Tue, 09 Jan 2018 22:00:12 GMT  
		Size: 937.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af320c3899ea4114972e99b9ceb36385935066073a40dfd94e5768be834a9562`  
		Last Modified: Tue, 09 Jan 2018 22:00:13 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97b20567e616b79216bba539892a140650506e781a6089cfab722d6adcee3d5`  
		Last Modified: Tue, 09 Jan 2018 22:00:12 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:2.1`

```console
$ docker pull crate@sha256:b6e3509b35d3e13649d9ddf217b536a1869c89c6e633aee2ed270c6a35141ae3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `crate:2.1` - linux; amd64

```console
$ docker pull crate@sha256:e94bd75941f74894b6421dcdc89222042d7fa565b7819bbbfbb2386010612d52
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129127060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d30ddb5b10b7fc2582830e5f0cd5104529b2fd2628bcaea2face9acd361de39`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 09 Jan 2018 21:13:01 GMT
ADD file:df48d6d6df42a01380557aebd4ca02807fc08a76a1d1b36d957e59a41c69db0b in / 
# Tue, 09 Jan 2018 21:13:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Jan 2018 21:54:39 GMT
MAINTAINER Crate.IO GmbH office@crate.io
# Tue, 09 Jan 2018 21:54:40 GMT
ENV GOSU_VERSION=1.9
# Tue, 09 Jan 2018 21:55:08 GMT
RUN set -x     && apk add --no-cache --virtual .gosu-deps         dpkg         gnupg         curl     && export ARCH=$(echo $(dpkg --print-architecture) | cut -d"-" -f3)     && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$ARCH"     && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$ARCH.asc"     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4     && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu     && rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc     && chmod +x /usr/local/bin/gosu     && gosu nobody true     && apk del .gosu-deps
# Tue, 09 Jan 2018 21:55:09 GMT
RUN addgroup crate && adduser -G crate -H crate -D
# Tue, 09 Jan 2018 21:55:09 GMT
ENV CRATE_VERSION=2.1.10
# Tue, 09 Jan 2018 21:56:00 GMT
RUN apk add --no-cache --virtual .crate-rundeps         openjdk8-jre-base         python3         openssl         sigar     && apk add --no-cache --virtual .build-deps         curl         gnupg         tar     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-$CRATE_VERSION.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-$CRATE_VERSION.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-$CRATE_VERSION.tar.gz.asc crate-$CRATE_VERSION.tar.gz     && rm -r "$GNUPGHOME" crate-$CRATE_VERSION.tar.gz.asc     && mkdir /crate     && tar -xf crate-$CRATE_VERSION.tar.gz -C /crate --strip-components=1     && rm crate-$CRATE_VERSION.tar.gz     && ln -s /usr/bin/python3 /usr/bin/python     && rm /crate/lib/sigar/libsigar-amd64-linux.so     && apk del .build-deps
# Tue, 09 Jan 2018 21:56:07 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jan 2018 21:56:08 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 09 Jan 2018 21:56:08 GMT
VOLUME [/data]
# Tue, 09 Jan 2018 21:56:08 GMT
ADD file:c0b3bba944a2572094279072da088c4f681b13f9bed768ebd567555831729fab in /crate/config/crate.yml 
# Tue, 09 Jan 2018 21:56:09 GMT
ADD file:10c08bc017b942a11ef7f1221f33b8224b4549e98c74b9f84e2495fcfb60d8ce in /crate/config/log4j2.properties 
# Tue, 09 Jan 2018 21:56:09 GMT
COPY file:9517f117528edc569ebb34a2c1d3d7bcf342cb124f3b833a681768549d61ebfb in / 
# Tue, 09 Jan 2018 21:56:18 GMT
WORKDIR /data
# Tue, 09 Jan 2018 21:56:18 GMT
EXPOSE 4200/tcp 4300/tcp 5432/tcp
# Tue, 09 Jan 2018 21:56:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Jan 2018 21:56:19 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:550fe1bea624a5c62551cf09f3aa10886eed133794844af1dfb775118309387e`  
		Last Modified: Tue, 09 Jan 2018 21:15:20 GMT  
		Size: 2.0 MB (1970140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a978fe7044d71089ea637c37c568c9df275d1a6ad05b0b34e475496914e9a58e`  
		Last Modified: Tue, 09 Jan 2018 21:59:26 GMT  
		Size: 592.4 KB (592371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25eebb3b80cb7de09a89560ce9ba7da3435a0b6528d3e21de78b9578ee0a8e90`  
		Last Modified: Tue, 09 Jan 2018 21:59:25 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36e42d1b203ec5b7f4e7a439fd90845dbf9f8660082f4d5b40332b27b02617c`  
		Last Modified: Tue, 09 Jan 2018 21:59:36 GMT  
		Size: 126.6 MB (126561840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2babe52ceb528482515137af488f41446a67f223e0e1560eca1831ab05e560bb`  
		Last Modified: Tue, 09 Jan 2018 21:59:23 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccdb4837af562b60f8733fa6309dbec9b9a49e60b3b721b3d55b9387593da92a`  
		Last Modified: Tue, 09 Jan 2018 21:59:24 GMT  
		Size: 934.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d837332a44b2820d8fc3f7fe3e2c1eaa068dbc090aa244a44cf2164cf194ca`  
		Last Modified: Tue, 09 Jan 2018 21:59:24 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec591f5690293fdccb09dbca32604f8a47a20cc7ce7247d1eca26a8338b199c`  
		Last Modified: Tue, 09 Jan 2018 21:59:25 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:2.1.10`

```console
$ docker pull crate@sha256:b6e3509b35d3e13649d9ddf217b536a1869c89c6e633aee2ed270c6a35141ae3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `crate:2.1.10` - linux; amd64

```console
$ docker pull crate@sha256:e94bd75941f74894b6421dcdc89222042d7fa565b7819bbbfbb2386010612d52
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129127060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d30ddb5b10b7fc2582830e5f0cd5104529b2fd2628bcaea2face9acd361de39`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 09 Jan 2018 21:13:01 GMT
ADD file:df48d6d6df42a01380557aebd4ca02807fc08a76a1d1b36d957e59a41c69db0b in / 
# Tue, 09 Jan 2018 21:13:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Jan 2018 21:54:39 GMT
MAINTAINER Crate.IO GmbH office@crate.io
# Tue, 09 Jan 2018 21:54:40 GMT
ENV GOSU_VERSION=1.9
# Tue, 09 Jan 2018 21:55:08 GMT
RUN set -x     && apk add --no-cache --virtual .gosu-deps         dpkg         gnupg         curl     && export ARCH=$(echo $(dpkg --print-architecture) | cut -d"-" -f3)     && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$ARCH"     && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$ARCH.asc"     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4     && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu     && rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc     && chmod +x /usr/local/bin/gosu     && gosu nobody true     && apk del .gosu-deps
# Tue, 09 Jan 2018 21:55:09 GMT
RUN addgroup crate && adduser -G crate -H crate -D
# Tue, 09 Jan 2018 21:55:09 GMT
ENV CRATE_VERSION=2.1.10
# Tue, 09 Jan 2018 21:56:00 GMT
RUN apk add --no-cache --virtual .crate-rundeps         openjdk8-jre-base         python3         openssl         sigar     && apk add --no-cache --virtual .build-deps         curl         gnupg         tar     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-$CRATE_VERSION.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-$CRATE_VERSION.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-$CRATE_VERSION.tar.gz.asc crate-$CRATE_VERSION.tar.gz     && rm -r "$GNUPGHOME" crate-$CRATE_VERSION.tar.gz.asc     && mkdir /crate     && tar -xf crate-$CRATE_VERSION.tar.gz -C /crate --strip-components=1     && rm crate-$CRATE_VERSION.tar.gz     && ln -s /usr/bin/python3 /usr/bin/python     && rm /crate/lib/sigar/libsigar-amd64-linux.so     && apk del .build-deps
# Tue, 09 Jan 2018 21:56:07 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jan 2018 21:56:08 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 09 Jan 2018 21:56:08 GMT
VOLUME [/data]
# Tue, 09 Jan 2018 21:56:08 GMT
ADD file:c0b3bba944a2572094279072da088c4f681b13f9bed768ebd567555831729fab in /crate/config/crate.yml 
# Tue, 09 Jan 2018 21:56:09 GMT
ADD file:10c08bc017b942a11ef7f1221f33b8224b4549e98c74b9f84e2495fcfb60d8ce in /crate/config/log4j2.properties 
# Tue, 09 Jan 2018 21:56:09 GMT
COPY file:9517f117528edc569ebb34a2c1d3d7bcf342cb124f3b833a681768549d61ebfb in / 
# Tue, 09 Jan 2018 21:56:18 GMT
WORKDIR /data
# Tue, 09 Jan 2018 21:56:18 GMT
EXPOSE 4200/tcp 4300/tcp 5432/tcp
# Tue, 09 Jan 2018 21:56:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Jan 2018 21:56:19 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:550fe1bea624a5c62551cf09f3aa10886eed133794844af1dfb775118309387e`  
		Last Modified: Tue, 09 Jan 2018 21:15:20 GMT  
		Size: 2.0 MB (1970140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a978fe7044d71089ea637c37c568c9df275d1a6ad05b0b34e475496914e9a58e`  
		Last Modified: Tue, 09 Jan 2018 21:59:26 GMT  
		Size: 592.4 KB (592371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25eebb3b80cb7de09a89560ce9ba7da3435a0b6528d3e21de78b9578ee0a8e90`  
		Last Modified: Tue, 09 Jan 2018 21:59:25 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36e42d1b203ec5b7f4e7a439fd90845dbf9f8660082f4d5b40332b27b02617c`  
		Last Modified: Tue, 09 Jan 2018 21:59:36 GMT  
		Size: 126.6 MB (126561840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2babe52ceb528482515137af488f41446a67f223e0e1560eca1831ab05e560bb`  
		Last Modified: Tue, 09 Jan 2018 21:59:23 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccdb4837af562b60f8733fa6309dbec9b9a49e60b3b721b3d55b9387593da92a`  
		Last Modified: Tue, 09 Jan 2018 21:59:24 GMT  
		Size: 934.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d837332a44b2820d8fc3f7fe3e2c1eaa068dbc090aa244a44cf2164cf194ca`  
		Last Modified: Tue, 09 Jan 2018 21:59:24 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec591f5690293fdccb09dbca32604f8a47a20cc7ce7247d1eca26a8338b199c`  
		Last Modified: Tue, 09 Jan 2018 21:59:25 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:2.2`

```console
$ docker pull crate@sha256:411b2c3f4af8b031f1440a612f3e0b113e4bd1091fd33bfa00c49fd54d9d42ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `crate:2.2` - linux; amd64

```console
$ docker pull crate@sha256:fe920b05301bb97dac9fbf4ae0804547f2f09393af4b78ff99c414a0367c8153
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128810907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18a26cb2f21cbec41f860e2085d83f5fc3e2d5a30419f4042ae56f091492a76b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 09 Jan 2018 21:10:58 GMT
ADD file:093f0723fa46f6cdbd6f7bd146448bb70ecce54254c35701feeceb956414622f in / 
# Tue, 09 Jan 2018 21:10:58 GMT
CMD ["/bin/sh"]
# Tue, 09 Jan 2018 21:53:00 GMT
MAINTAINER Crate.IO GmbH office@crate.io
# Tue, 09 Jan 2018 21:53:01 GMT
ENV GOSU_VERSION=1.9
# Tue, 09 Jan 2018 21:53:40 GMT
RUN set -x     && apk add --no-cache --virtual .gosu-deps         dpkg         gnupg         curl     && export ARCH=$(echo $(dpkg --print-architecture) | cut -d"-" -f3)     && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$ARCH"     && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$ARCH.asc"     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4     && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu     && rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc     && chmod +x /usr/local/bin/gosu     && gosu nobody true     && apk del .gosu-deps
# Tue, 09 Jan 2018 21:53:41 GMT
RUN addgroup crate && adduser -G crate -H crate -D
# Tue, 09 Jan 2018 21:53:41 GMT
ENV CRATE_VERSION=2.2.5
# Tue, 09 Jan 2018 21:54:25 GMT
RUN apk add --no-cache --virtual .crate-rundeps         openjdk8-jre-base         python3         openssl         sigar     && apk add --no-cache --virtual .build-deps         curl         gnupg         tar     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-$CRATE_VERSION.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-$CRATE_VERSION.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-$CRATE_VERSION.tar.gz.asc crate-$CRATE_VERSION.tar.gz     && rm -r "$GNUPGHOME" crate-$CRATE_VERSION.tar.gz.asc     && mkdir /crate     && tar -xf crate-$CRATE_VERSION.tar.gz -C /crate --strip-components=1     && rm crate-$CRATE_VERSION.tar.gz     && ln -s /usr/bin/python3 /usr/bin/python     && rm /crate/lib/sigar/libsigar-amd64-linux.so     && apk del .build-deps
# Tue, 09 Jan 2018 21:54:25 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jan 2018 21:54:25 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 09 Jan 2018 21:54:25 GMT
VOLUME [/data]
# Tue, 09 Jan 2018 21:54:26 GMT
ADD file:c0b3bba944a2572094279072da088c4f681b13f9bed768ebd567555831729fab in /crate/config/crate.yml 
# Tue, 09 Jan 2018 21:54:26 GMT
ADD file:10c08bc017b942a11ef7f1221f33b8224b4549e98c74b9f84e2495fcfb60d8ce in /crate/config/log4j2.properties 
# Tue, 09 Jan 2018 21:54:27 GMT
COPY file:9517f117528edc569ebb34a2c1d3d7bcf342cb124f3b833a681768549d61ebfb in / 
# Tue, 09 Jan 2018 21:54:27 GMT
WORKDIR /data
# Tue, 09 Jan 2018 21:54:27 GMT
EXPOSE 4200/tcp 4300/tcp 5432/tcp
# Tue, 09 Jan 2018 21:54:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Jan 2018 21:54:28 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:ff3a5c916c92643ff77519ffa742d3ec61b7f591b6b7504599d95a4a41134e28`  
		Last Modified: Tue, 09 Jan 2018 21:13:34 GMT  
		Size: 2.1 MB (2065537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8b79b83f80d98af54e2362535a327791df92a7bd49f1d30543f4ae43c984cd`  
		Last Modified: Tue, 09 Jan 2018 21:58:11 GMT  
		Size: 593.1 KB (593125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e46e2d22f238dfae62d2b15f537f7515f3e2f886025f6088c91e292814cd7cb`  
		Last Modified: Tue, 09 Jan 2018 21:58:10 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d9eb3958b06320486298eafd15792adc9b737b262306a5ebf6039a8dec6ac4`  
		Last Modified: Tue, 09 Jan 2018 21:58:32 GMT  
		Size: 126.1 MB (126149533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327c02a62458d5ff922db1b47733f64883f4ba817024733b49db861988633948`  
		Last Modified: Tue, 09 Jan 2018 21:58:09 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c4e90ce9d6d52230e05ae85d2ba4f36b0e3359c6092d36d24334bb382d0be8`  
		Last Modified: Tue, 09 Jan 2018 21:58:08 GMT  
		Size: 936.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1847f74aa0eddc54c5c1f31a379939f579c9e5e4a93d4cb142d7297ee71970b3`  
		Last Modified: Tue, 09 Jan 2018 21:58:08 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d61ee766bb5d67b291d020040c2ff699df4c47fb77aebe1a89b5c12d604e809`  
		Last Modified: Tue, 09 Jan 2018 21:58:08 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:2.2.5`

```console
$ docker pull crate@sha256:411b2c3f4af8b031f1440a612f3e0b113e4bd1091fd33bfa00c49fd54d9d42ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `crate:2.2.5` - linux; amd64

```console
$ docker pull crate@sha256:fe920b05301bb97dac9fbf4ae0804547f2f09393af4b78ff99c414a0367c8153
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128810907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18a26cb2f21cbec41f860e2085d83f5fc3e2d5a30419f4042ae56f091492a76b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 09 Jan 2018 21:10:58 GMT
ADD file:093f0723fa46f6cdbd6f7bd146448bb70ecce54254c35701feeceb956414622f in / 
# Tue, 09 Jan 2018 21:10:58 GMT
CMD ["/bin/sh"]
# Tue, 09 Jan 2018 21:53:00 GMT
MAINTAINER Crate.IO GmbH office@crate.io
# Tue, 09 Jan 2018 21:53:01 GMT
ENV GOSU_VERSION=1.9
# Tue, 09 Jan 2018 21:53:40 GMT
RUN set -x     && apk add --no-cache --virtual .gosu-deps         dpkg         gnupg         curl     && export ARCH=$(echo $(dpkg --print-architecture) | cut -d"-" -f3)     && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$ARCH"     && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$ARCH.asc"     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4     && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu     && rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc     && chmod +x /usr/local/bin/gosu     && gosu nobody true     && apk del .gosu-deps
# Tue, 09 Jan 2018 21:53:41 GMT
RUN addgroup crate && adduser -G crate -H crate -D
# Tue, 09 Jan 2018 21:53:41 GMT
ENV CRATE_VERSION=2.2.5
# Tue, 09 Jan 2018 21:54:25 GMT
RUN apk add --no-cache --virtual .crate-rundeps         openjdk8-jre-base         python3         openssl         sigar     && apk add --no-cache --virtual .build-deps         curl         gnupg         tar     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-$CRATE_VERSION.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-$CRATE_VERSION.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-$CRATE_VERSION.tar.gz.asc crate-$CRATE_VERSION.tar.gz     && rm -r "$GNUPGHOME" crate-$CRATE_VERSION.tar.gz.asc     && mkdir /crate     && tar -xf crate-$CRATE_VERSION.tar.gz -C /crate --strip-components=1     && rm crate-$CRATE_VERSION.tar.gz     && ln -s /usr/bin/python3 /usr/bin/python     && rm /crate/lib/sigar/libsigar-amd64-linux.so     && apk del .build-deps
# Tue, 09 Jan 2018 21:54:25 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jan 2018 21:54:25 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 09 Jan 2018 21:54:25 GMT
VOLUME [/data]
# Tue, 09 Jan 2018 21:54:26 GMT
ADD file:c0b3bba944a2572094279072da088c4f681b13f9bed768ebd567555831729fab in /crate/config/crate.yml 
# Tue, 09 Jan 2018 21:54:26 GMT
ADD file:10c08bc017b942a11ef7f1221f33b8224b4549e98c74b9f84e2495fcfb60d8ce in /crate/config/log4j2.properties 
# Tue, 09 Jan 2018 21:54:27 GMT
COPY file:9517f117528edc569ebb34a2c1d3d7bcf342cb124f3b833a681768549d61ebfb in / 
# Tue, 09 Jan 2018 21:54:27 GMT
WORKDIR /data
# Tue, 09 Jan 2018 21:54:27 GMT
EXPOSE 4200/tcp 4300/tcp 5432/tcp
# Tue, 09 Jan 2018 21:54:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Jan 2018 21:54:28 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:ff3a5c916c92643ff77519ffa742d3ec61b7f591b6b7504599d95a4a41134e28`  
		Last Modified: Tue, 09 Jan 2018 21:13:34 GMT  
		Size: 2.1 MB (2065537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8b79b83f80d98af54e2362535a327791df92a7bd49f1d30543f4ae43c984cd`  
		Last Modified: Tue, 09 Jan 2018 21:58:11 GMT  
		Size: 593.1 KB (593125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e46e2d22f238dfae62d2b15f537f7515f3e2f886025f6088c91e292814cd7cb`  
		Last Modified: Tue, 09 Jan 2018 21:58:10 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d9eb3958b06320486298eafd15792adc9b737b262306a5ebf6039a8dec6ac4`  
		Last Modified: Tue, 09 Jan 2018 21:58:32 GMT  
		Size: 126.1 MB (126149533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327c02a62458d5ff922db1b47733f64883f4ba817024733b49db861988633948`  
		Last Modified: Tue, 09 Jan 2018 21:58:09 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c4e90ce9d6d52230e05ae85d2ba4f36b0e3359c6092d36d24334bb382d0be8`  
		Last Modified: Tue, 09 Jan 2018 21:58:08 GMT  
		Size: 936.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1847f74aa0eddc54c5c1f31a379939f579c9e5e4a93d4cb142d7297ee71970b3`  
		Last Modified: Tue, 09 Jan 2018 21:58:08 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d61ee766bb5d67b291d020040c2ff699df4c47fb77aebe1a89b5c12d604e809`  
		Last Modified: Tue, 09 Jan 2018 21:58:08 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `crate:latest`

```console
$ docker pull crate@sha256:411b2c3f4af8b031f1440a612f3e0b113e4bd1091fd33bfa00c49fd54d9d42ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `crate:latest` - linux; amd64

```console
$ docker pull crate@sha256:fe920b05301bb97dac9fbf4ae0804547f2f09393af4b78ff99c414a0367c8153
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128810907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18a26cb2f21cbec41f860e2085d83f5fc3e2d5a30419f4042ae56f091492a76b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["crate"]`

```dockerfile
# Tue, 09 Jan 2018 21:10:58 GMT
ADD file:093f0723fa46f6cdbd6f7bd146448bb70ecce54254c35701feeceb956414622f in / 
# Tue, 09 Jan 2018 21:10:58 GMT
CMD ["/bin/sh"]
# Tue, 09 Jan 2018 21:53:00 GMT
MAINTAINER Crate.IO GmbH office@crate.io
# Tue, 09 Jan 2018 21:53:01 GMT
ENV GOSU_VERSION=1.9
# Tue, 09 Jan 2018 21:53:40 GMT
RUN set -x     && apk add --no-cache --virtual .gosu-deps         dpkg         gnupg         curl     && export ARCH=$(echo $(dpkg --print-architecture) | cut -d"-" -f3)     && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$ARCH"     && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$ARCH.asc"     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4     && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu     && rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc     && chmod +x /usr/local/bin/gosu     && gosu nobody true     && apk del .gosu-deps
# Tue, 09 Jan 2018 21:53:41 GMT
RUN addgroup crate && adduser -G crate -H crate -D
# Tue, 09 Jan 2018 21:53:41 GMT
ENV CRATE_VERSION=2.2.5
# Tue, 09 Jan 2018 21:54:25 GMT
RUN apk add --no-cache --virtual .crate-rundeps         openjdk8-jre-base         python3         openssl         sigar     && apk add --no-cache --virtual .build-deps         curl         gnupg         tar     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-$CRATE_VERSION.tar.gz     && curl -fSL -O https://cdn.crate.io/downloads/releases/crate-$CRATE_VERSION.tar.gz.asc     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 90C23FC6585BC0717F8FBFC37FAAE51A06F6EAEB     && gpg --batch --verify crate-$CRATE_VERSION.tar.gz.asc crate-$CRATE_VERSION.tar.gz     && rm -r "$GNUPGHOME" crate-$CRATE_VERSION.tar.gz.asc     && mkdir /crate     && tar -xf crate-$CRATE_VERSION.tar.gz -C /crate --strip-components=1     && rm crate-$CRATE_VERSION.tar.gz     && ln -s /usr/bin/python3 /usr/bin/python     && rm /crate/lib/sigar/libsigar-amd64-linux.so     && apk del .build-deps
# Tue, 09 Jan 2018 21:54:25 GMT
ENV PATH=/crate/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jan 2018 21:54:25 GMT
ENV CRATE_HEAP_SIZE=512M
# Tue, 09 Jan 2018 21:54:25 GMT
VOLUME [/data]
# Tue, 09 Jan 2018 21:54:26 GMT
ADD file:c0b3bba944a2572094279072da088c4f681b13f9bed768ebd567555831729fab in /crate/config/crate.yml 
# Tue, 09 Jan 2018 21:54:26 GMT
ADD file:10c08bc017b942a11ef7f1221f33b8224b4549e98c74b9f84e2495fcfb60d8ce in /crate/config/log4j2.properties 
# Tue, 09 Jan 2018 21:54:27 GMT
COPY file:9517f117528edc569ebb34a2c1d3d7bcf342cb124f3b833a681768549d61ebfb in / 
# Tue, 09 Jan 2018 21:54:27 GMT
WORKDIR /data
# Tue, 09 Jan 2018 21:54:27 GMT
EXPOSE 4200/tcp 4300/tcp 5432/tcp
# Tue, 09 Jan 2018 21:54:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Jan 2018 21:54:28 GMT
CMD ["crate"]
```

-	Layers:
	-	`sha256:ff3a5c916c92643ff77519ffa742d3ec61b7f591b6b7504599d95a4a41134e28`  
		Last Modified: Tue, 09 Jan 2018 21:13:34 GMT  
		Size: 2.1 MB (2065537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8b79b83f80d98af54e2362535a327791df92a7bd49f1d30543f4ae43c984cd`  
		Last Modified: Tue, 09 Jan 2018 21:58:11 GMT  
		Size: 593.1 KB (593125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e46e2d22f238dfae62d2b15f537f7515f3e2f886025f6088c91e292814cd7cb`  
		Last Modified: Tue, 09 Jan 2018 21:58:10 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d9eb3958b06320486298eafd15792adc9b737b262306a5ebf6039a8dec6ac4`  
		Last Modified: Tue, 09 Jan 2018 21:58:32 GMT  
		Size: 126.1 MB (126149533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327c02a62458d5ff922db1b47733f64883f4ba817024733b49db861988633948`  
		Last Modified: Tue, 09 Jan 2018 21:58:09 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c4e90ce9d6d52230e05ae85d2ba4f36b0e3359c6092d36d24334bb382d0be8`  
		Last Modified: Tue, 09 Jan 2018 21:58:08 GMT  
		Size: 936.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1847f74aa0eddc54c5c1f31a379939f579c9e5e4a93d4cb142d7297ee71970b3`  
		Last Modified: Tue, 09 Jan 2018 21:58:08 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d61ee766bb5d67b291d020040c2ff699df4c47fb77aebe1a89b5c12d604e809`  
		Last Modified: Tue, 09 Jan 2018 21:58:08 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
