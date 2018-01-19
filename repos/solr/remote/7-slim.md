## `solr:7-slim`

```console
$ docker pull solr@sha256:84413a04b16f80ab7a732dd8e5d125a5e1d92c5da872b065f0bfb60a68ee42c9
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

### `solr:7-slim` - linux; amd64

```console
$ docker pull solr@sha256:c84d9021ab9b990914fa4ef44c39d97edc9d260ec33e3d457053b2bcfcd12e49
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.5 MB (236490199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d20c7736550b3a9ab9a6a824a05711b0b98f022e1eefdb954c4db945f416de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Tue, 12 Dec 2017 01:44:43 GMT
ADD file:f30a8b5b7cdc9ba33a250899308b490baa9f7a9b29d3a85bd16200aa0a28a04a in / 
# Tue, 12 Dec 2017 01:44:43 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 05:34:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 05:34:55 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 05:34:56 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 12 Dec 2017 05:34:56 GMT
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 12 Dec 2017 05:38:19 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Tue, 12 Dec 2017 05:38:19 GMT
ENV JAVA_VERSION=8u151
# Tue, 12 Dec 2017 05:38:20 GMT
ENV JAVA_DEBIAN_VERSION=8u151-b12-1~deb9u1
# Tue, 12 Dec 2017 05:38:20 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20170531+nmu1
# Tue, 12 Dec 2017 05:38:40 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-8-jre-headless="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Tue, 12 Dec 2017 05:38:47 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 12 Dec 2017 08:10:05 GMT
MAINTAINER Martijn Koster "mak-docker@greenhills.co.uk"
# Tue, 12 Dec 2017 08:10:06 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 12 Dec 2017 08:10:13 GMT
RUN apt-get update &&   apt-get -y install lsof procps wget gpg &&   rm -rf /var/lib/apt/lists/*
# Fri, 19 Jan 2018 00:05:21 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_VERSION=7.2.1 SOLR_URL=https://archive.apache.org/dist/lucene/solr/7.2.1/solr-7.2.1.tgz SOLR_SHA256=1dbe8dda842d2008210c0c56d56b714713444fb4e05390bb0bcdec29cf957748 SOLR_KEYS=052C5B48A480B9CEA9E218A5F98C13CFA5A135D8 PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 Jan 2018 00:05:23 GMT
RUN groupadd -r --gid $SOLR_GID $SOLR_GROUP &&   useradd -r --uid $SOLR_UID --gid $SOLR_GID $SOLR_USER
# Fri, 19 Jan 2018 00:05:36 GMT
RUN set -e; for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 19 Jan 2018 00:05:52 GMT
RUN mkdir -p /opt/solr &&   echo "downloading $SOLR_URL" &&   wget -nv $SOLR_URL -O /opt/solr.tgz &&   echo "downloading $SOLR_URL.asc" &&   wget -nv $SOLR_URL.asc -O /opt/solr.tgz.asc &&   echo "$SOLR_SHA256 */opt/solr.tgz" | sha256sum -c - &&   (>&2 ls -l /opt/solr.tgz /opt/solr.tgz.asc) &&   gpg --batch --verify /opt/solr.tgz.asc /opt/solr.tgz &&   tar -C /opt/solr --extract --file /opt/solr.tgz --strip-components=1 &&   rm /opt/solr.tgz* &&   rm -Rf /opt/solr/docs/ &&   mkdir -p /opt/solr/server/solr/lib /opt/solr/server/solr/mycores /opt/solr/server/logs /docker-entrypoint-initdb.d /opt/docker-solr &&   sed -i -e 's/"\$(whoami)" == "root"/$(id -u) == 0/' /opt/solr/bin/solr &&   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr &&   sed -i -e '/-Dsolr.clustering.enabled=true/ a SOLR_OPTS="$SOLR_OPTS -Dsun.net.inetaddr.ttl=60 -Dsun.net.inetaddr.negative.ttl=60"' /opt/solr/bin/solr.in.sh &&   chown -R $SOLR_USER:$SOLR_GROUP /opt/solr
# Fri, 19 Jan 2018 00:05:52 GMT
COPY dir:ccd481d71dbb5316781a49f67183387866aea7b61c29d2719e1b5d8b040c48b4 in /opt/docker-solr/scripts 
# Fri, 19 Jan 2018 00:05:53 GMT
RUN chown -R $SOLR_USER:$SOLR_GROUP /opt/docker-solr
# Fri, 19 Jan 2018 00:05:53 GMT
EXPOSE 8983/tcp
# Fri, 19 Jan 2018 00:05:53 GMT
WORKDIR /opt/solr
# Fri, 19 Jan 2018 00:05:54 GMT
USER [solr]
# Fri, 19 Jan 2018 00:05:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Jan 2018 00:05:54 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:e7bb522d92ff6d4e5b2087409b0fc783c2e3b06acf87bee739ee47d90bf02e96`  
		Last Modified: Tue, 12 Dec 2017 01:54:56 GMT  
		Size: 22.5 MB (22485719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf3a7df1b51f6278abe3864a0d83f04c9b9d4885b4d64cf68cb40ac650f91a5`  
		Last Modified: Tue, 12 Dec 2017 05:49:02 GMT  
		Size: 454.8 KB (454819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c98005fcff8d144c0e901a6f8b6c20f7aab34f1c93f9d8679f342cd4640c5c`  
		Last Modified: Tue, 12 Dec 2017 05:49:01 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39dcc90226db797991bfa856bcbec2e3a60afa66c263912ec507073813bbe945`  
		Last Modified: Tue, 12 Dec 2017 05:49:01 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693e7ee438449dbeb5311161c6b7551a36b6a16e1cc801f11a82752335a83423`  
		Last Modified: Tue, 12 Dec 2017 05:50:30 GMT  
		Size: 56.0 MB (55998926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb083d9c54cfb8d861eda9fbf2466b0be061872c74751624d604dda6c9b75d29`  
		Last Modified: Tue, 12 Dec 2017 05:50:16 GMT  
		Size: 272.1 KB (272124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730691b6b3933b86537e0d9ff846c34e684d0d6f55dfba52b481d89a99b1e4e6`  
		Last Modified: Tue, 12 Dec 2017 08:15:45 GMT  
		Size: 4.0 MB (3966984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb514c52c4c7b634d12f100d16339a4006370e61f4d921a987469af02ec58a2`  
		Last Modified: Fri, 19 Jan 2018 00:35:39 GMT  
		Size: 4.3 KB (4333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711468685248ee51cf66041415b365c0e9ee5652bbc70d44f9b414097a3185b0`  
		Last Modified: Fri, 19 Jan 2018 00:35:39 GMT  
		Size: 4.0 KB (3988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e550f0dc5b1b77420924e9ac919d7bd6a6b6d7c70a992c1a8bc29afa288c1845`  
		Last Modified: Fri, 19 Jan 2018 00:35:54 GMT  
		Size: 153.3 MB (153294459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea472aa597699e59f8042e0fe3b8635bf30acdb1685aec861817afc741a26ba6`  
		Last Modified: Fri, 19 Jan 2018 00:35:39 GMT  
		Size: 4.2 KB (4231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9b5402f4dff4496dc75144995664baa1f203562b86310614b85b8887850f94`  
		Last Modified: Fri, 19 Jan 2018 00:35:41 GMT  
		Size: 4.2 KB (4237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:7-slim` - linux; arm variant v5

```console
$ docker pull solr@sha256:bc386a54b1a47e7344a61f5de556e5f3e6e72a861b7d277691728d0e3d4e73a8
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.7 MB (225689749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e00fdcd290cfb38c9c860f773fb67600bb90b778962a52382e1897a23a35ed1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Tue, 12 Dec 2017 21:02:20 GMT
ADD file:f69e5781e9ff2a9867d94175d91d31553e07613bf4b50a1064274ed21a5ed353 in / 
# Tue, 12 Dec 2017 21:02:21 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 23:35:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 23:35:32 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 23:35:34 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 12 Dec 2017 23:35:36 GMT
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 12 Dec 2017 23:38:13 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Tue, 12 Dec 2017 23:38:13 GMT
ENV JAVA_VERSION=8u151
# Tue, 12 Dec 2017 23:38:14 GMT
ENV JAVA_DEBIAN_VERSION=8u151-b12-1~deb9u1
# Tue, 12 Dec 2017 23:38:14 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20170531+nmu1
# Tue, 12 Dec 2017 23:38:44 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-8-jre-headless="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Tue, 12 Dec 2017 23:38:49 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Wed, 13 Dec 2017 02:48:56 GMT
MAINTAINER Martijn Koster "mak-docker@greenhills.co.uk"
# Wed, 13 Dec 2017 02:48:56 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 13 Dec 2017 02:49:08 GMT
RUN apt-get update &&   apt-get -y install lsof procps wget gpg &&   rm -rf /var/lib/apt/lists/*
# Fri, 19 Jan 2018 04:47:04 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_VERSION=7.2.1 SOLR_URL=https://archive.apache.org/dist/lucene/solr/7.2.1/solr-7.2.1.tgz SOLR_SHA256=1dbe8dda842d2008210c0c56d56b714713444fb4e05390bb0bcdec29cf957748 SOLR_KEYS=052C5B48A480B9CEA9E218A5F98C13CFA5A135D8 PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 Jan 2018 04:47:05 GMT
RUN groupadd -r --gid $SOLR_GID $SOLR_GROUP &&   useradd -r --uid $SOLR_UID --gid $SOLR_GID $SOLR_USER
# Fri, 19 Jan 2018 04:47:09 GMT
RUN set -e; for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 19 Jan 2018 04:47:24 GMT
RUN mkdir -p /opt/solr &&   echo "downloading $SOLR_URL" &&   wget -nv $SOLR_URL -O /opt/solr.tgz &&   echo "downloading $SOLR_URL.asc" &&   wget -nv $SOLR_URL.asc -O /opt/solr.tgz.asc &&   echo "$SOLR_SHA256 */opt/solr.tgz" | sha256sum -c - &&   (>&2 ls -l /opt/solr.tgz /opt/solr.tgz.asc) &&   gpg --batch --verify /opt/solr.tgz.asc /opt/solr.tgz &&   tar -C /opt/solr --extract --file /opt/solr.tgz --strip-components=1 &&   rm /opt/solr.tgz* &&   rm -Rf /opt/solr/docs/ &&   mkdir -p /opt/solr/server/solr/lib /opt/solr/server/solr/mycores /opt/solr/server/logs /docker-entrypoint-initdb.d /opt/docker-solr &&   sed -i -e 's/"\$(whoami)" == "root"/$(id -u) == 0/' /opt/solr/bin/solr &&   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr &&   sed -i -e '/-Dsolr.clustering.enabled=true/ a SOLR_OPTS="$SOLR_OPTS -Dsun.net.inetaddr.ttl=60 -Dsun.net.inetaddr.negative.ttl=60"' /opt/solr/bin/solr.in.sh &&   chown -R $SOLR_USER:$SOLR_GROUP /opt/solr
# Fri, 19 Jan 2018 04:47:24 GMT
COPY dir:ccd481d71dbb5316781a49f67183387866aea7b61c29d2719e1b5d8b040c48b4 in /opt/docker-solr/scripts 
# Fri, 19 Jan 2018 04:47:25 GMT
RUN chown -R $SOLR_USER:$SOLR_GROUP /opt/docker-solr
# Fri, 19 Jan 2018 04:47:25 GMT
EXPOSE 8983/tcp
# Fri, 19 Jan 2018 04:47:25 GMT
WORKDIR /opt/solr
# Fri, 19 Jan 2018 04:47:25 GMT
USER [solr]
# Fri, 19 Jan 2018 04:47:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Jan 2018 04:47:26 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:20f319b2549a8d631c2e8034bfc3f9c12042d86a686470a8addd2fb7bc8c688c`  
		Last Modified: Tue, 12 Dec 2017 21:12:53 GMT  
		Size: 21.2 MB (21160630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65052ec7ef0bdb21ddce084fc2ca3ebb905b33a9a818895001dd55d624efe03`  
		Last Modified: Tue, 12 Dec 2017 23:54:39 GMT  
		Size: 447.6 KB (447650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07680ae7da06d4a0f024421827636cf16555c42f45227a88ad625c8ef912c759`  
		Last Modified: Tue, 12 Dec 2017 23:54:39 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58646084886efde46909359e34fd12541f48ec6173c42b5aa4e27cb0deb8813c`  
		Last Modified: Tue, 12 Dec 2017 23:54:40 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28cd75912c5edcdc3510c7250c1dd59f28596cb2818114904f20977527c53811`  
		Last Modified: Tue, 12 Dec 2017 23:57:05 GMT  
		Size: 46.7 MB (46726494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f836b50d9ff8fe1e891b4aeb6021ea88e654171ad94b141e87ac191e474d588`  
		Last Modified: Tue, 12 Dec 2017 23:56:54 GMT  
		Size: 272.2 KB (272191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5cf39fdb16dcb29894c3a32e4a26c7fc553ba179afe9ca08b733b10dd5f3e9`  
		Last Modified: Wed, 13 Dec 2017 03:00:15 GMT  
		Size: 3.8 MB (3771144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a014c9358f12d7bb1bc87932a2a07b420d1d09c8aab4b30ddf7259ac1c32e99`  
		Last Modified: Fri, 19 Jan 2018 04:50:57 GMT  
		Size: 4.3 KB (4266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb1c12a288001f416fe25d696ebb0fe3605ad84fe0437b1d39a94c1c7cf4099`  
		Last Modified: Fri, 19 Jan 2018 04:50:57 GMT  
		Size: 4.0 KB (4010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5e50d69be3a56895642f7b7d2c6ef892759581ebf399f3b27259ab1444bd84`  
		Last Modified: Fri, 19 Jan 2018 04:51:16 GMT  
		Size: 153.3 MB (153294495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c249c654cdd915373a04721aed16cca7dfa3cf8af63a47a40cd33dd83d5ee6d`  
		Last Modified: Fri, 19 Jan 2018 04:50:57 GMT  
		Size: 4.3 KB (4255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a194cd0dd5618880d67f5ddf5451a6e5f777c82b0cf4f9ff287d433a0d3024d6`  
		Last Modified: Fri, 19 Jan 2018 04:50:59 GMT  
		Size: 4.2 KB (4236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:7-slim` - linux; arm variant v7

```console
$ docker pull solr@sha256:f5b6711861c5b4eaa3c8f229a6cca688913a1c86b00e4c97efeb507bb282ca06
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.9 MB (222925633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d41d6139eb747662f04ebd581c3938c35271eb26af59faa070a384680037846f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Mon, 09 Oct 2017 21:45:43 GMT
ADD file:b758c6c3ff989778bd740dde35c86b953fa09be913a7e02711b2881de6b8911d in / 
# Mon, 09 Oct 2017 21:45:44 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 23:05:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Mon, 09 Oct 2017 23:05:30 GMT
ENV LANG=C.UTF-8
# Mon, 09 Oct 2017 23:05:32 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 09 Oct 2017 23:05:33 GMT
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Mon, 09 Oct 2017 23:07:42 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Mon, 09 Oct 2017 23:07:43 GMT
ENV JAVA_VERSION=8u141
# Mon, 09 Oct 2017 23:07:43 GMT
ENV JAVA_DEBIAN_VERSION=8u141-b15-1~deb9u1
# Mon, 09 Oct 2017 23:07:43 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20170531+nmu1
# Mon, 09 Oct 2017 23:08:10 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-8-jre-headless="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Mon, 09 Oct 2017 23:08:18 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 10 Oct 2017 01:28:50 GMT
MAINTAINER Martijn Koster "mak-docker@greenhills.co.uk"
# Tue, 10 Oct 2017 01:28:50 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 10 Oct 2017 01:28:58 GMT
RUN apt-get update &&   apt-get -y install lsof procps wget gpg &&   rm -rf /var/lib/apt/lists/*
# Fri, 19 Jan 2018 02:55:55 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_VERSION=7.2.1 SOLR_URL=https://archive.apache.org/dist/lucene/solr/7.2.1/solr-7.2.1.tgz SOLR_SHA256=1dbe8dda842d2008210c0c56d56b714713444fb4e05390bb0bcdec29cf957748 SOLR_KEYS=052C5B48A480B9CEA9E218A5F98C13CFA5A135D8 PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 Jan 2018 02:55:56 GMT
RUN groupadd -r --gid $SOLR_GID $SOLR_GROUP &&   useradd -r --uid $SOLR_UID --gid $SOLR_GID $SOLR_USER
# Fri, 19 Jan 2018 02:55:59 GMT
RUN set -e; for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 19 Jan 2018 02:56:18 GMT
RUN mkdir -p /opt/solr &&   echo "downloading $SOLR_URL" &&   wget -nv $SOLR_URL -O /opt/solr.tgz &&   echo "downloading $SOLR_URL.asc" &&   wget -nv $SOLR_URL.asc -O /opt/solr.tgz.asc &&   echo "$SOLR_SHA256 */opt/solr.tgz" | sha256sum -c - &&   (>&2 ls -l /opt/solr.tgz /opt/solr.tgz.asc) &&   gpg --batch --verify /opt/solr.tgz.asc /opt/solr.tgz &&   tar -C /opt/solr --extract --file /opt/solr.tgz --strip-components=1 &&   rm /opt/solr.tgz* &&   rm -Rf /opt/solr/docs/ &&   mkdir -p /opt/solr/server/solr/lib /opt/solr/server/solr/mycores /opt/solr/server/logs /docker-entrypoint-initdb.d /opt/docker-solr &&   sed -i -e 's/"\$(whoami)" == "root"/$(id -u) == 0/' /opt/solr/bin/solr &&   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr &&   sed -i -e '/-Dsolr.clustering.enabled=true/ a SOLR_OPTS="$SOLR_OPTS -Dsun.net.inetaddr.ttl=60 -Dsun.net.inetaddr.negative.ttl=60"' /opt/solr/bin/solr.in.sh &&   chown -R $SOLR_USER:$SOLR_GROUP /opt/solr
# Fri, 19 Jan 2018 02:56:19 GMT
COPY dir:ccd481d71dbb5316781a49f67183387866aea7b61c29d2719e1b5d8b040c48b4 in /opt/docker-solr/scripts 
# Fri, 19 Jan 2018 02:56:20 GMT
RUN chown -R $SOLR_USER:$SOLR_GROUP /opt/docker-solr
# Fri, 19 Jan 2018 02:56:20 GMT
EXPOSE 8983/tcp
# Fri, 19 Jan 2018 02:56:20 GMT
WORKDIR /opt/solr
# Fri, 19 Jan 2018 02:56:20 GMT
USER [solr]
# Fri, 19 Jan 2018 02:56:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Jan 2018 02:56:21 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:59e81a3fde58ec8d4b8f2f58b98ef2f4d951d37dd9b99b016fd294a8e07d7796`  
		Last Modified: Mon, 09 Oct 2017 21:52:49 GMT  
		Size: 19.3 MB (19277135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6226915187b9d61d290e04413a4ccdf021b5e0fc267ba8129cc0126cab1f1a93`  
		Last Modified: Mon, 09 Oct 2017 23:24:02 GMT  
		Size: 430.6 KB (430580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98b9b3c90ff2ee65efc9f88b2383f6f1760df78bcd965fa0b22e001977eaf96`  
		Last Modified: Mon, 09 Oct 2017 23:24:01 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377cafaae0c7321b0549f3949d78826675109fe908cb8521f39fe433ccfced7c`  
		Last Modified: Mon, 09 Oct 2017 23:24:01 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a90e76db87bd029fe0cc5b41e212f46198e84bcdd6fd9d8100d543019ca3ec0`  
		Last Modified: Mon, 09 Oct 2017 23:25:48 GMT  
		Size: 46.2 MB (46152339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d672e3cc87b30249aae8cf95548eb623752b0a5c2e9e70c1a578c7895b2c909d`  
		Last Modified: Mon, 09 Oct 2017 23:25:36 GMT  
		Size: 272.2 KB (272181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3348db73a5179352f7c9415360de082aefe0b3a8015a2c4fd26d9ee95a665061`  
		Last Modified: Tue, 10 Oct 2017 01:37:52 GMT  
		Size: 3.5 MB (3481666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a2ce3cadccf98a65a15ea370967d0ffaabf26dcb5e21398aae000df113afef`  
		Last Modified: Fri, 19 Jan 2018 03:00:01 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99027f3770e7b34dc997b6cfe37f4fa83086bcd36adf4a3202e1fcdf34716d7a`  
		Last Modified: Fri, 19 Jan 2018 03:00:01 GMT  
		Size: 4.0 KB (4016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a438c114e380e68cd427e7526ed484687940b66f28008cf3e72498f49eaabc96`  
		Last Modified: Fri, 19 Jan 2018 03:00:18 GMT  
		Size: 153.3 MB (153294583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc998a8fcca8713a5872b6968a9527fc600c20298d3a75aee74b618d067ce04`  
		Last Modified: Fri, 19 Jan 2018 03:00:01 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae21a561b67ca090fd17896606190367bece288c92e8f603110b0df9077f686`  
		Last Modified: Fri, 19 Jan 2018 03:00:01 GMT  
		Size: 4.2 KB (4235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:7-slim` - linux; arm64 variant v8

```console
$ docker pull solr@sha256:6530dcd99b2859e0aeb5a9b06f306786bbbcd7f35fdc20ea781aa54c7e11693c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.1 MB (226149107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da06e16f6f398c773d456917a215bf6f937a83cde65729ee6087a8851864a22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Tue, 12 Dec 2017 18:34:13 GMT
ADD file:6e068c7cc5397bfb4ec60dab4d410c5d3ba724f20ad0129d2032fb509f0eadcd in / 
# Tue, 12 Dec 2017 18:34:14 GMT
CMD ["bash"]
# Wed, 13 Dec 2017 02:17:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2017 02:17:38 GMT
ENV LANG=C.UTF-8
# Wed, 13 Dec 2017 02:17:40 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 13 Dec 2017 02:17:57 GMT
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 13 Dec 2017 02:20:45 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Wed, 13 Dec 2017 02:20:46 GMT
ENV JAVA_VERSION=8u151
# Wed, 13 Dec 2017 02:20:47 GMT
ENV JAVA_DEBIAN_VERSION=8u151-b12-1~deb9u1
# Wed, 13 Dec 2017 02:20:48 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20170531+nmu1
# Wed, 13 Dec 2017 02:21:54 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-8-jre-headless="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Wed, 13 Dec 2017 02:22:07 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Wed, 13 Dec 2017 02:59:52 GMT
MAINTAINER Martijn Koster "mak-docker@greenhills.co.uk"
# Wed, 13 Dec 2017 02:59:52 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 13 Dec 2017 03:02:21 GMT
RUN apt-get update &&   apt-get -y install lsof procps wget gpg &&   rm -rf /var/lib/apt/lists/*
# Fri, 19 Jan 2018 00:52:15 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_VERSION=7.2.1 SOLR_URL=https://archive.apache.org/dist/lucene/solr/7.2.1/solr-7.2.1.tgz SOLR_SHA256=1dbe8dda842d2008210c0c56d56b714713444fb4e05390bb0bcdec29cf957748 SOLR_KEYS=052C5B48A480B9CEA9E218A5F98C13CFA5A135D8 PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 Jan 2018 00:52:17 GMT
RUN groupadd -r --gid $SOLR_GID $SOLR_GROUP &&   useradd -r --uid $SOLR_UID --gid $SOLR_GID $SOLR_USER
# Fri, 19 Jan 2018 00:52:22 GMT
RUN set -e; for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 19 Jan 2018 00:53:08 GMT
RUN mkdir -p /opt/solr &&   echo "downloading $SOLR_URL" &&   wget -nv $SOLR_URL -O /opt/solr.tgz &&   echo "downloading $SOLR_URL.asc" &&   wget -nv $SOLR_URL.asc -O /opt/solr.tgz.asc &&   echo "$SOLR_SHA256 */opt/solr.tgz" | sha256sum -c - &&   (>&2 ls -l /opt/solr.tgz /opt/solr.tgz.asc) &&   gpg --batch --verify /opt/solr.tgz.asc /opt/solr.tgz &&   tar -C /opt/solr --extract --file /opt/solr.tgz --strip-components=1 &&   rm /opt/solr.tgz* &&   rm -Rf /opt/solr/docs/ &&   mkdir -p /opt/solr/server/solr/lib /opt/solr/server/solr/mycores /opt/solr/server/logs /docker-entrypoint-initdb.d /opt/docker-solr &&   sed -i -e 's/"\$(whoami)" == "root"/$(id -u) == 0/' /opt/solr/bin/solr &&   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr &&   sed -i -e '/-Dsolr.clustering.enabled=true/ a SOLR_OPTS="$SOLR_OPTS -Dsun.net.inetaddr.ttl=60 -Dsun.net.inetaddr.negative.ttl=60"' /opt/solr/bin/solr.in.sh &&   chown -R $SOLR_USER:$SOLR_GROUP /opt/solr
# Fri, 19 Jan 2018 00:53:09 GMT
COPY dir:ccd481d71dbb5316781a49f67183387866aea7b61c29d2719e1b5d8b040c48b4 in /opt/docker-solr/scripts 
# Fri, 19 Jan 2018 00:53:10 GMT
RUN chown -R $SOLR_USER:$SOLR_GROUP /opt/docker-solr
# Fri, 19 Jan 2018 00:53:11 GMT
EXPOSE 8983/tcp
# Fri, 19 Jan 2018 00:53:12 GMT
WORKDIR /opt/solr
# Fri, 19 Jan 2018 00:53:12 GMT
USER [solr]
# Fri, 19 Jan 2018 00:53:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Jan 2018 00:53:13 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:fcad8cfc11c78a53ccf9aafafcb3ded5044dbd181977e6255aea54fbe164f131`  
		Last Modified: Tue, 12 Dec 2017 18:49:05 GMT  
		Size: 20.3 MB (20331270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c64863fb48f3c775969ad8bd727b09f3c8f60396a469d5c70006c3ba2a3aa5`  
		Last Modified: Wed, 13 Dec 2017 02:27:43 GMT  
		Size: 440.8 KB (440783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48bc6f700f2b94cbba0ece43bb24936ab2e94ceae7f46573d3373c9551bbf7fe`  
		Last Modified: Wed, 13 Dec 2017 02:27:43 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba1aa71856da230cafe9c4121837cf6fd0f5c2c17d9c98ac22c767e7cf6e668`  
		Last Modified: Wed, 13 Dec 2017 02:27:44 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5663ce84487e3faa8b2686217a32cf2cb7bc73587b63ccdb2af477458aecd70`  
		Last Modified: Wed, 13 Dec 2017 02:30:26 GMT  
		Size: 48.2 MB (48152403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d1920fed140df205c75b511b6557ffcd700bd2b7db283c44a36283a305e90e`  
		Last Modified: Wed, 13 Dec 2017 02:30:11 GMT  
		Size: 272.1 KB (272081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e779bef3c8dc8fc65b087f82e1c8a8f83120671848eb407d74d8f77be3345ce`  
		Last Modified: Wed, 13 Dec 2017 03:15:20 GMT  
		Size: 3.6 MB (3640954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076a56bd209cb062bd81a0f001683e43f5d725d326cd86d5a347cb68d681f1ff`  
		Last Modified: Fri, 19 Jan 2018 01:06:38 GMT  
		Size: 4.4 KB (4364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317e62d2db29028c62c10568ad8885997c8dc247a9f730a8e6f4444e54d2ced0`  
		Last Modified: Fri, 19 Jan 2018 01:06:38 GMT  
		Size: 4.0 KB (3983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c474890a14b8295598f268748cad576e6385b5a96d77e97458ff5f8c590c90`  
		Last Modified: Fri, 19 Jan 2018 01:06:59 GMT  
		Size: 153.3 MB (153294424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7c2588318704420159cb2ffd86e5f6e8c68587472623be2e02508ded52d49d`  
		Last Modified: Fri, 19 Jan 2018 01:06:39 GMT  
		Size: 4.2 KB (4230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c648e8eaea392e0674d9127ad91a7653fb09245a69d215b2f5e8f0bac7f7c36f`  
		Last Modified: Fri, 19 Jan 2018 01:06:38 GMT  
		Size: 4.2 KB (4236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:7-slim` - linux; 386

```console
$ docker pull solr@sha256:c9060c3dbd893b75ab755e07e8ff0e757cf82c2c2424a563b5c5f6d90664057a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.9 MB (236925255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f5523be5e7a352750938e42349a12ca8f88e585f2834d74e2b634750bb92372`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Tue, 12 Dec 2017 14:36:09 GMT
ADD file:ef60a5257bf2b5766f692e39f5922bbd6161e45de184b7b138522d53a477c7af in / 
# Tue, 12 Dec 2017 14:36:09 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 18:49:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 18:49:16 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 18:49:17 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 12 Dec 2017 18:49:18 GMT
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 12 Dec 2017 18:50:15 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Tue, 12 Dec 2017 18:50:15 GMT
ENV JAVA_VERSION=8u151
# Tue, 12 Dec 2017 18:50:16 GMT
ENV JAVA_DEBIAN_VERSION=8u151-b12-1~deb9u1
# Tue, 12 Dec 2017 18:50:16 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20170531+nmu1
# Tue, 12 Dec 2017 18:50:52 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-8-jre-headless="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Tue, 12 Dec 2017 18:51:40 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Wed, 13 Dec 2017 18:54:45 GMT
MAINTAINER Martijn Koster "mak-docker@greenhills.co.uk"
# Wed, 13 Dec 2017 18:54:45 GMT
ARG SOLR_DOWNLOAD_SERVER
# Wed, 13 Dec 2017 18:54:59 GMT
RUN apt-get update &&   apt-get -y install lsof procps wget gpg &&   rm -rf /var/lib/apt/lists/*
# Fri, 19 Jan 2018 07:55:06 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_VERSION=7.2.1 SOLR_URL=https://archive.apache.org/dist/lucene/solr/7.2.1/solr-7.2.1.tgz SOLR_SHA256=1dbe8dda842d2008210c0c56d56b714713444fb4e05390bb0bcdec29cf957748 SOLR_KEYS=052C5B48A480B9CEA9E218A5F98C13CFA5A135D8 PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 Jan 2018 07:55:08 GMT
RUN groupadd -r --gid $SOLR_GID $SOLR_GROUP &&   useradd -r --uid $SOLR_UID --gid $SOLR_GID $SOLR_USER
# Fri, 19 Jan 2018 07:55:11 GMT
RUN set -e; for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 19 Jan 2018 07:55:29 GMT
RUN mkdir -p /opt/solr &&   echo "downloading $SOLR_URL" &&   wget -nv $SOLR_URL -O /opt/solr.tgz &&   echo "downloading $SOLR_URL.asc" &&   wget -nv $SOLR_URL.asc -O /opt/solr.tgz.asc &&   echo "$SOLR_SHA256 */opt/solr.tgz" | sha256sum -c - &&   (>&2 ls -l /opt/solr.tgz /opt/solr.tgz.asc) &&   gpg --batch --verify /opt/solr.tgz.asc /opt/solr.tgz &&   tar -C /opt/solr --extract --file /opt/solr.tgz --strip-components=1 &&   rm /opt/solr.tgz* &&   rm -Rf /opt/solr/docs/ &&   mkdir -p /opt/solr/server/solr/lib /opt/solr/server/solr/mycores /opt/solr/server/logs /docker-entrypoint-initdb.d /opt/docker-solr &&   sed -i -e 's/"\$(whoami)" == "root"/$(id -u) == 0/' /opt/solr/bin/solr &&   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr &&   sed -i -e '/-Dsolr.clustering.enabled=true/ a SOLR_OPTS="$SOLR_OPTS -Dsun.net.inetaddr.ttl=60 -Dsun.net.inetaddr.negative.ttl=60"' /opt/solr/bin/solr.in.sh &&   chown -R $SOLR_USER:$SOLR_GROUP /opt/solr
# Fri, 19 Jan 2018 07:55:29 GMT
COPY dir:ccd481d71dbb5316781a49f67183387866aea7b61c29d2719e1b5d8b040c48b4 in /opt/docker-solr/scripts 
# Fri, 19 Jan 2018 07:55:30 GMT
RUN chown -R $SOLR_USER:$SOLR_GROUP /opt/docker-solr
# Fri, 19 Jan 2018 07:55:30 GMT
EXPOSE 8983/tcp
# Fri, 19 Jan 2018 07:55:31 GMT
WORKDIR /opt/solr
# Fri, 19 Jan 2018 07:55:31 GMT
USER [solr]
# Fri, 19 Jan 2018 07:55:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Jan 2018 07:55:31 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:4dbce982b05e209cf10a433462dc417f7816c47b0c1a151c8c93206b299b9a14`  
		Last Modified: Tue, 12 Dec 2017 15:03:13 GMT  
		Size: 23.1 MB (23122456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594d2ff3a2959654cb056a6cc499d910f29f37321940fdb0f60d119c31528ac6`  
		Last Modified: Tue, 12 Dec 2017 19:38:43 GMT  
		Size: 463.5 KB (463470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32efb0ce68171bdf8e5e876db66fc50811b491dabc077b3d35172f1286b4793a`  
		Last Modified: Tue, 12 Dec 2017 19:38:51 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02613bb9328128d056d071d315402c64aedb2c7b730cf211f79713ce7415e73`  
		Last Modified: Tue, 12 Dec 2017 19:38:42 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcc559cf6f8a75a850edb216dd0258ffc3e59eb02f07a5ed762b5a8afd281a0`  
		Last Modified: Tue, 12 Dec 2017 19:40:52 GMT  
		Size: 55.5 MB (55545032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0437c26ed57f9bcc9c0c90b32da2273931aacd18096d84bc71ecf7f1e7322d`  
		Last Modified: Tue, 12 Dec 2017 19:40:37 GMT  
		Size: 272.2 KB (272164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20c154c082248d74094ca2582e06c2e3c90dca03180cfffbf17e0aaf2251a4e`  
		Last Modified: Wed, 13 Dec 2017 20:40:58 GMT  
		Size: 4.2 MB (4210781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e7c925783f67ac3c0fefff8d54fc534761704accb8b4f3b4c4bc0d685c62e7`  
		Last Modified: Fri, 19 Jan 2018 09:04:02 GMT  
		Size: 4.3 KB (4266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9818a0c9459a755a7921b686c9a2afc5064eb3b6e77a87a5b54c52c1da43a4`  
		Last Modified: Fri, 19 Jan 2018 09:04:02 GMT  
		Size: 4.0 KB (3987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200258d0704e54ae994823f86a520422e32569d8b36e322ce3e8df5bd978d359`  
		Last Modified: Fri, 19 Jan 2018 09:04:19 GMT  
		Size: 153.3 MB (153294258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7b541d2d15f1efe8ff070e3490312cca31d0746c2b19693613ab45665e025`  
		Last Modified: Fri, 19 Jan 2018 09:04:02 GMT  
		Size: 4.2 KB (4227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7629d935ce1e3914f39dedcda19b8eb8d7cb9b9355e75792afade6019eac7617`  
		Last Modified: Fri, 19 Jan 2018 09:04:02 GMT  
		Size: 4.2 KB (4235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:7-slim` - linux; ppc64le

```console
$ docker pull solr@sha256:d5cad5536ead16560e83d2ae52487a3cf0adcf4a8bb76f8dc2d8c13746b67a2e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.4 MB (229351191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f13e10338c042d38aa2511f5a78dced84b7890b7d9a85e09a7741bf015cdec30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Tue, 12 Dec 2017 01:35:41 GMT
ADD file:896602a6d015367badb26a7ac0bcafc9aa04cbba205925631d315874b6d289ab in / 
# Tue, 12 Dec 2017 01:35:42 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 03:57:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 03:57:01 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 03:57:04 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 12 Dec 2017 03:57:07 GMT
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 12 Dec 2017 04:08:36 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Tue, 12 Dec 2017 04:08:40 GMT
ENV JAVA_VERSION=8u151
# Tue, 12 Dec 2017 04:08:42 GMT
ENV JAVA_DEBIAN_VERSION=8u151-b12-1~deb9u1
# Tue, 12 Dec 2017 04:08:43 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20170531+nmu1
# Tue, 12 Dec 2017 04:11:25 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-8-jre-headless="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Tue, 12 Dec 2017 04:11:34 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 12 Dec 2017 12:03:45 GMT
MAINTAINER Martijn Koster "mak-docker@greenhills.co.uk"
# Tue, 12 Dec 2017 12:03:46 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 12 Dec 2017 12:04:47 GMT
RUN apt-get update &&   apt-get -y install lsof procps wget gpg &&   rm -rf /var/lib/apt/lists/*
# Fri, 19 Jan 2018 12:48:06 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_VERSION=7.2.1 SOLR_URL=https://archive.apache.org/dist/lucene/solr/7.2.1/solr-7.2.1.tgz SOLR_SHA256=1dbe8dda842d2008210c0c56d56b714713444fb4e05390bb0bcdec29cf957748 SOLR_KEYS=052C5B48A480B9CEA9E218A5F98C13CFA5A135D8 PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 Jan 2018 12:48:13 GMT
RUN groupadd -r --gid $SOLR_GID $SOLR_GROUP &&   useradd -r --uid $SOLR_UID --gid $SOLR_GID $SOLR_USER
# Fri, 19 Jan 2018 12:48:20 GMT
RUN set -e; for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 19 Jan 2018 12:49:47 GMT
RUN mkdir -p /opt/solr &&   echo "downloading $SOLR_URL" &&   wget -nv $SOLR_URL -O /opt/solr.tgz &&   echo "downloading $SOLR_URL.asc" &&   wget -nv $SOLR_URL.asc -O /opt/solr.tgz.asc &&   echo "$SOLR_SHA256 */opt/solr.tgz" | sha256sum -c - &&   (>&2 ls -l /opt/solr.tgz /opt/solr.tgz.asc) &&   gpg --batch --verify /opt/solr.tgz.asc /opt/solr.tgz &&   tar -C /opt/solr --extract --file /opt/solr.tgz --strip-components=1 &&   rm /opt/solr.tgz* &&   rm -Rf /opt/solr/docs/ &&   mkdir -p /opt/solr/server/solr/lib /opt/solr/server/solr/mycores /opt/solr/server/logs /docker-entrypoint-initdb.d /opt/docker-solr &&   sed -i -e 's/"\$(whoami)" == "root"/$(id -u) == 0/' /opt/solr/bin/solr &&   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr &&   sed -i -e '/-Dsolr.clustering.enabled=true/ a SOLR_OPTS="$SOLR_OPTS -Dsun.net.inetaddr.ttl=60 -Dsun.net.inetaddr.negative.ttl=60"' /opt/solr/bin/solr.in.sh &&   chown -R $SOLR_USER:$SOLR_GROUP /opt/solr
# Fri, 19 Jan 2018 12:49:48 GMT
COPY dir:ccd481d71dbb5316781a49f67183387866aea7b61c29d2719e1b5d8b040c48b4 in /opt/docker-solr/scripts 
# Fri, 19 Jan 2018 12:49:52 GMT
RUN chown -R $SOLR_USER:$SOLR_GROUP /opt/docker-solr
# Fri, 19 Jan 2018 12:49:53 GMT
EXPOSE 8983/tcp
# Fri, 19 Jan 2018 12:49:54 GMT
WORKDIR /opt/solr
# Fri, 19 Jan 2018 12:49:57 GMT
USER [solr]
# Fri, 19 Jan 2018 12:49:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Jan 2018 12:49:59 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:b8b738bec437a97371af422179183d09cdb031f677b2dba4deaed774655ee9d8`  
		Last Modified: Tue, 12 Dec 2017 01:42:57 GMT  
		Size: 22.7 MB (22739713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526c4e4a82552c0009f666d9199512d3cf5cd397b914ccaaed0a1d80ee6a37d0`  
		Last Modified: Tue, 12 Dec 2017 04:20:58 GMT  
		Size: 449.8 KB (449767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e5614e1ec52998918779b56f1c68b70afba320748cc697497dd8f66004102d`  
		Last Modified: Tue, 12 Dec 2017 04:20:57 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51004c1b2e651697ab322f6718900e01da20de1d2b7301f9039344231d4e3ad6`  
		Last Modified: Tue, 12 Dec 2017 04:20:57 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ba4c991d51de56b538b40c302b50ff268d863b6081fa12de878b52fe1c64e8`  
		Last Modified: Tue, 12 Dec 2017 04:23:07 GMT  
		Size: 48.6 MB (48635573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65aa697b950f112d6d504a0d7c144ea94fa4c8b407ec052f38515e89fdb9466`  
		Last Modified: Tue, 12 Dec 2017 04:22:56 GMT  
		Size: 272.0 KB (272043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718b7c105bb54ed01e657cb993187fbf2604f97a40adf25c14da61800454fe70`  
		Last Modified: Tue, 12 Dec 2017 12:36:14 GMT  
		Size: 3.9 MB (3942322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4f32e78abd9480619b344db95013c177baf326958676708b8979d92c373aeb`  
		Last Modified: Fri, 19 Jan 2018 13:08:54 GMT  
		Size: 4.3 KB (4339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286c1a81a152cc70cb778e49841c9e14fa3c4ae2d06f77132b144844675f6510`  
		Last Modified: Fri, 19 Jan 2018 13:08:55 GMT  
		Size: 4.0 KB (4009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a0b1072e34e2fcc4b2edd132498590707c77c84947519ed216c4776e2e1f40`  
		Last Modified: Fri, 19 Jan 2018 13:09:08 GMT  
		Size: 153.3 MB (153294551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0bbbd58b26e4a5d4305334859065db0bc85dcd52071de762c69415b0f7f74f4`  
		Last Modified: Fri, 19 Jan 2018 13:08:54 GMT  
		Size: 4.3 KB (4257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fc3d95afe6a3e261f2a685f46c0acbca1b613c00c676e97c8f55c81dcc3173`  
		Last Modified: Fri, 19 Jan 2018 13:08:54 GMT  
		Size: 4.2 KB (4237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `solr:7-slim` - linux; s390x

```console
$ docker pull solr@sha256:662f6439db90c897ccbe30f2d8f0fecbbbf2d3f5b6fb4b75839c8ec2afbbd92e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.3 MB (228259088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb92bd906cad1ef945671dbaf47edd03a07b4a5021d13640f55a0f7f9e8461bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["solr-foreground"]`

```dockerfile
# Tue, 12 Dec 2017 06:25:50 GMT
ADD file:8cd208817150f41f5b21f5c2b6641af023ddeaa6d842fe490190e20effe94a08 in / 
# Tue, 12 Dec 2017 06:25:51 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:39:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:39:00 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 07:39:01 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 12 Dec 2017 07:39:01 GMT
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 12 Dec 2017 07:40:48 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Tue, 12 Dec 2017 07:40:48 GMT
ENV JAVA_VERSION=8u151
# Tue, 12 Dec 2017 07:40:48 GMT
ENV JAVA_DEBIAN_VERSION=8u151-b12-1~deb9u1
# Tue, 12 Dec 2017 07:40:49 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20170531+nmu1
# Tue, 12 Dec 2017 07:41:11 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-8-jre-headless="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Tue, 12 Dec 2017 07:41:13 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 12 Dec 2017 11:51:40 GMT
MAINTAINER Martijn Koster "mak-docker@greenhills.co.uk"
# Tue, 12 Dec 2017 11:51:41 GMT
ARG SOLR_DOWNLOAD_SERVER
# Tue, 12 Dec 2017 11:51:54 GMT
RUN apt-get update &&   apt-get -y install lsof procps wget gpg &&   rm -rf /var/lib/apt/lists/*
# Fri, 19 Jan 2018 07:13:25 GMT
ENV SOLR_USER=solr SOLR_UID=8983 SOLR_GROUP=solr SOLR_GID=8983 SOLR_VERSION=7.2.1 SOLR_URL=https://archive.apache.org/dist/lucene/solr/7.2.1/solr-7.2.1.tgz SOLR_SHA256=1dbe8dda842d2008210c0c56d56b714713444fb4e05390bb0bcdec29cf957748 SOLR_KEYS=052C5B48A480B9CEA9E218A5F98C13CFA5A135D8 PATH=/opt/solr/bin:/opt/docker-solr/scripts:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 Jan 2018 07:13:25 GMT
RUN groupadd -r --gid $SOLR_GID $SOLR_GROUP &&   useradd -r --uid $SOLR_UID --gid $SOLR_GID $SOLR_USER
# Fri, 19 Jan 2018 07:13:28 GMT
RUN set -e; for key in $SOLR_KEYS; do     found='';     for server in       ha.pool.sks-keyservers.net       hkp://keyserver.ubuntu.com:80       hkp://p80.pool.sks-keyservers.net:80       pgp.mit.edu     ; do       echo "  trying $server for $key";       gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$key" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch $key from several disparate servers -- network issues?" && exit 1;   done;   exit 0
# Fri, 19 Jan 2018 07:14:25 GMT
RUN mkdir -p /opt/solr &&   echo "downloading $SOLR_URL" &&   wget -nv $SOLR_URL -O /opt/solr.tgz &&   echo "downloading $SOLR_URL.asc" &&   wget -nv $SOLR_URL.asc -O /opt/solr.tgz.asc &&   echo "$SOLR_SHA256 */opt/solr.tgz" | sha256sum -c - &&   (>&2 ls -l /opt/solr.tgz /opt/solr.tgz.asc) &&   gpg --batch --verify /opt/solr.tgz.asc /opt/solr.tgz &&   tar -C /opt/solr --extract --file /opt/solr.tgz --strip-components=1 &&   rm /opt/solr.tgz* &&   rm -Rf /opt/solr/docs/ &&   mkdir -p /opt/solr/server/solr/lib /opt/solr/server/solr/mycores /opt/solr/server/logs /docker-entrypoint-initdb.d /opt/docker-solr &&   sed -i -e 's/"\$(whoami)" == "root"/$(id -u) == 0/' /opt/solr/bin/solr &&   sed -i -e 's/lsof -PniTCP:/lsof -t -PniTCP:/' /opt/solr/bin/solr &&   sed -i -e '/-Dsolr.clustering.enabled=true/ a SOLR_OPTS="$SOLR_OPTS -Dsun.net.inetaddr.ttl=60 -Dsun.net.inetaddr.negative.ttl=60"' /opt/solr/bin/solr.in.sh &&   chown -R $SOLR_USER:$SOLR_GROUP /opt/solr
# Fri, 19 Jan 2018 07:14:25 GMT
COPY dir:ccd481d71dbb5316781a49f67183387866aea7b61c29d2719e1b5d8b040c48b4 in /opt/docker-solr/scripts 
# Fri, 19 Jan 2018 07:14:26 GMT
RUN chown -R $SOLR_USER:$SOLR_GROUP /opt/docker-solr
# Fri, 19 Jan 2018 07:14:26 GMT
EXPOSE 8983/tcp
# Fri, 19 Jan 2018 07:14:26 GMT
WORKDIR /opt/solr
# Fri, 19 Jan 2018 07:14:26 GMT
USER [solr]
# Fri, 19 Jan 2018 07:14:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Jan 2018 07:14:27 GMT
CMD ["solr-foreground"]
```

-	Layers:
	-	`sha256:da91ecedba56836763b256841bfd01198234139e3e4824510318c25fa8cf140a`  
		Last Modified: Tue, 12 Dec 2017 06:31:22 GMT  
		Size: 22.3 MB (22333855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530a993dc54ccfec513ceaf61463bccb2bd4dadaf0947423da948ae904d6a7c3`  
		Last Modified: Tue, 12 Dec 2017 07:48:03 GMT  
		Size: 465.7 KB (465710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0da9f88284bdc2730fe7f74c1150a506d1ff936a4edc9c4b9b641b1c124183d`  
		Last Modified: Tue, 12 Dec 2017 07:48:05 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69c8d612be2772e9480cc833b516c81bd80618c08a5f59e8406050fd52d978e`  
		Last Modified: Tue, 12 Dec 2017 07:48:03 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7038c267b7c7a8ac741f45ce6238f1eac1e09b07cece0a759f1db32b16789a9`  
		Last Modified: Tue, 12 Dec 2017 07:49:30 GMT  
		Size: 47.8 MB (47847247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d83d2b2c7a504accf2e70581c068900dda49c36aa967e44ebd9c7dffe904009`  
		Last Modified: Tue, 12 Dec 2017 07:49:22 GMT  
		Size: 272.2 KB (272151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e9b36a26b685e58d1670c35d1828039e3208830d4537ffd2225e70cbca7196`  
		Last Modified: Tue, 12 Dec 2017 11:59:21 GMT  
		Size: 4.0 MB (4028423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d6f9d49a1d2948a18a15b7abac0a92611753f92cc64c03c7682595491681a29`  
		Last Modified: Fri, 19 Jan 2018 07:23:57 GMT  
		Size: 4.4 KB (4371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825c606a995c7545108c8e60f00bcef6a25cb7fce2b808796678b5076a93792d`  
		Last Modified: Fri, 19 Jan 2018 07:23:57 GMT  
		Size: 4.0 KB (3992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0093b4f4e20990fff4c5fa06a1e47b3b3ece97b5e57fc6f39d8463a70e7ef1e0`  
		Last Modified: Fri, 19 Jan 2018 07:24:09 GMT  
		Size: 153.3 MB (153294496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445cce4d78376e183c81e5cc3e032eb009488ad70b3c952258c2539e1f98a0d9`  
		Last Modified: Fri, 19 Jan 2018 07:23:59 GMT  
		Size: 4.2 KB (4229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6723ffce00c6d75d6e903c8f7bfea2925a44543b36a54799561a55b3779a94d3`  
		Last Modified: Fri, 19 Jan 2018 07:23:57 GMT  
		Size: 4.2 KB (4235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
