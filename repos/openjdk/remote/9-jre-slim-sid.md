## `openjdk:9-jre-slim-sid`

```console
$ docker pull openjdk@sha256:82ea8fbc3e5b84c04fa2f89e45d079562901a21adbfc6927b99dbb0151181635
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

### `openjdk:9-jre-slim-sid` - linux; amd64

```console
$ docker pull openjdk@sha256:7f99e5d82399ee424cec6d4094eb5b51629e40c26e43fddb03b54f03db338272
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102604406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a3578a54b7e8f128e68e71800d3e0d2aa2c0b65f1f100668f5c3818704821bd`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 07:02:48 GMT
ADD file:4ac5b74448a361591479d0374d36fef5832baedf42ca81cbd6fbd8ac037ad414 in / 
# Sat, 28 Apr 2018 07:02:49 GMT
CMD ["bash"]
# Tue, 01 May 2018 09:40:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 09:40:17 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 09:40:18 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 01 May 2018 11:00:51 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 01 May 2018 11:00:51 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 01 May 2018 11:00:51 GMT
ENV JAVA_VERSION=9.0.4+12
# Tue, 01 May 2018 11:00:51 GMT
ENV JAVA_DEBIAN_VERSION=9.0.4+12-4
# Mon, 14 May 2018 22:39:55 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-9-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:c2ad77de49cedb25345a40be4f3ccc592075053d2d1b4cafcc67a011c070df60`  
		Last Modified: Sat, 28 Apr 2018 09:01:30 GMT  
		Size: 26.0 MB (26007039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6485a2cca95b289b549728c0c66bb1b463cdb7a204d224291f28c111a64a371`  
		Last Modified: Tue, 01 May 2018 14:02:46 GMT  
		Size: 460.5 KB (460510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4ea4e6ab41ff82240aed63937b358af3ee0d7749491ea788298b5cd38027cd`  
		Last Modified: Tue, 01 May 2018 14:02:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649f9534d72bc7ab44e527f83b63f51976a27696dc7ccbef9db571a111943a92`  
		Last Modified: Tue, 01 May 2018 16:08:07 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3fcb6a0075d8e297e30126427ed1a6557a31223d4e5a44a0e7643ed1c2d87d`  
		Last Modified: Mon, 14 May 2018 23:12:18 GMT  
		Size: 76.1 MB (76136489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:9-jre-slim-sid` - linux; arm variant v5

```console
$ docker pull openjdk@sha256:6959ebf524a916e43055cd88196c87d1aa462a2b52c46a3d7523ff0c637ca8a4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.0 MB (86001030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67874aaeed4852f1d7a0efe616758ed258d5c8fffa6d50611439a5dafed4bd84`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 08:51:57 GMT
ADD file:4bb0a1afcce11262886b693c92f368728f7ca179f516dcfd86a6a74d9941a2bd in / 
# Sat, 28 Apr 2018 08:51:57 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 12:33:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:33:18 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:33:19 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 28 Apr 2018 12:43:12 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 28 Apr 2018 12:43:13 GMT
ENV JAVA_HOME=/docker-java-home
# Sat, 28 Apr 2018 12:43:13 GMT
ENV JAVA_VERSION=9.0.4+12
# Sat, 28 Apr 2018 12:43:13 GMT
ENV JAVA_DEBIAN_VERSION=9.0.4+12-4
# Tue, 15 May 2018 09:42:38 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-9-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:d8a6a213c8dfd9e72ad11408970d74e2be7ffdfbac3683ed1a40c28534145e4a`  
		Last Modified: Sat, 28 Apr 2018 09:00:19 GMT  
		Size: 24.0 MB (23990346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe23918d5c3df5c5737b91e6e16035342f47e61426f3dd0265882e998ef16a4`  
		Last Modified: Sat, 28 Apr 2018 13:02:15 GMT  
		Size: 454.0 KB (453984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3278875f078d656ef3d6c8ce9702f8344f1343454d75403da10d4e583f90931`  
		Last Modified: Sat, 28 Apr 2018 13:02:15 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9dbfd25a8aacdb785bb88625b5386d6a6ac1a5c949ece261c79ebd30009759`  
		Last Modified: Sat, 28 Apr 2018 13:17:22 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b396c694ab84a285f5aecbecbd898ea63441b0005b7e9c4c9809afeb6394b4dd`  
		Last Modified: Tue, 15 May 2018 10:14:02 GMT  
		Size: 61.6 MB (61556331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:9-jre-slim-sid` - linux; arm variant v7

```console
$ docker pull openjdk@sha256:3647f5d267a9f17264a2615a52d82203335e3e2e7f44d0288b49c3785cc66277
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.9 MB (85909784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26ba18d24306c8bce7bbcb13c8ff90d9e827ee4922fb06266537edae185e53c2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:02:41 GMT
ADD file:51a6f559367fc724be19aeee6bd277b378069389bc848507cfa991829488f7a6 in / 
# Sat, 28 Apr 2018 12:02:41 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 12:38:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:38:04 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:38:05 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 28 Apr 2018 12:47:33 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 28 Apr 2018 12:47:33 GMT
ENV JAVA_HOME=/docker-java-home
# Sat, 28 Apr 2018 12:47:34 GMT
ENV JAVA_VERSION=9.0.4+12
# Sat, 28 Apr 2018 12:47:35 GMT
ENV JAVA_DEBIAN_VERSION=9.0.4+12-4
# Tue, 15 May 2018 12:14:25 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-9-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:e896ce6a07096665b9b10eea8b8d7a9f0f6e26c3d88bd463db48304823b92890`  
		Last Modified: Sat, 28 Apr 2018 12:14:08 GMT  
		Size: 22.0 MB (21967210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925e7bf3333e528dfd915abfbcbc560f820ce29a375d884865566688160e4eed`  
		Last Modified: Sat, 28 Apr 2018 13:05:56 GMT  
		Size: 436.6 KB (436647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc2cc177a3ab014156f5c72f5b4f97a9fb66c88c1f2d8c79cdf90ed2dab6a6c`  
		Last Modified: Sat, 28 Apr 2018 13:05:56 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ccb997b52fc92a7c297f6b56be1f7c3f0a231772051e22da26267550fad9e97`  
		Last Modified: Sat, 28 Apr 2018 13:16:53 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39fa33f4e7f0ccc13c6eaf36297974f81964fff1dc21679b5462993ccce82891`  
		Last Modified: Tue, 15 May 2018 12:54:27 GMT  
		Size: 63.5 MB (63505557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:9-jre-slim-sid` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:f4759813e2f9ed89996770f814e3bacaeb2216e86f26f60b94b1b996d0a6fb35
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.8 MB (88807915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d20ed81b4e90cbd8d377ded64d818b977edb01ebd21a958675ec4baaf37d916a`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 30 Apr 2018 23:28:38 GMT
ADD file:0c141fd79d3e8c492efc85f35f6f2273b082454831ae4e4e58f2bb99395ac72b in / 
# Mon, 30 Apr 2018 23:28:47 GMT
CMD ["bash"]
# Tue, 01 May 2018 10:26:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 10:26:43 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 10:26:45 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 01 May 2018 10:56:53 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 01 May 2018 10:56:53 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 01 May 2018 10:56:54 GMT
ENV JAVA_VERSION=9.0.4+12
# Tue, 01 May 2018 10:56:55 GMT
ENV JAVA_DEBIAN_VERSION=9.0.4+12-4
# Tue, 15 May 2018 09:41:07 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-9-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:8a965c5efd07de5feb761f2ff7f7c9319fbd736849e5c372d102a79db79c4f2f`  
		Last Modified: Mon, 30 Apr 2018 23:48:28 GMT  
		Size: 23.4 MB (23364515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca2f61f6ee678d7988be608168e9c185ba5c895ae0c465aae1111cc9b9f381e`  
		Last Modified: Tue, 01 May 2018 11:43:20 GMT  
		Size: 445.3 KB (445326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c81d59c641d2ddc2a09929f5b5d1a2b5181d4c465d5d47ac607bb97deb6f8a`  
		Last Modified: Tue, 01 May 2018 11:43:20 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3359846d10d5ef13605aa0470f33e1cb5fd5e8e6977c33a370b2abacad0613f`  
		Last Modified: Tue, 01 May 2018 11:51:49 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc3a51a42fd310bb6e0861cff02acec5b5156d339847cb499f1b23da837402d`  
		Last Modified: Tue, 15 May 2018 10:53:55 GMT  
		Size: 65.0 MB (64997705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:9-jre-slim-sid` - linux; 386

```console
$ docker pull openjdk@sha256:a658a414a7d0382fb8dfab36d951bef9cb4090d3d7da2330d45c54e6f501d21d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108268175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87f258765a63b6954e51dc9130ff25d327481b6bac0bdbf22c2a1e5726bc3ec6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 10:40:59 GMT
ADD file:9e204bd06575325653d9ca924ded453fa1a0f9eb3fe6d0fb8390160b39768da9 in / 
# Sat, 28 Apr 2018 10:40:59 GMT
CMD ["bash"]
# Thu, 31 May 2018 05:46:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 31 May 2018 05:46:06 GMT
ENV LANG=C.UTF-8
# Thu, 31 May 2018 05:46:07 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Thu, 31 May 2018 05:57:10 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Thu, 31 May 2018 05:57:10 GMT
ENV JAVA_HOME=/docker-java-home
# Thu, 31 May 2018 05:57:10 GMT
ENV JAVA_VERSION=9.0.4+12
# Thu, 31 May 2018 05:57:10 GMT
ENV JAVA_DEBIAN_VERSION=9.0.4+12-4
# Thu, 31 May 2018 05:57:38 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-9-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:b0b251c3fa17d0cdbdd0cb21b207843e9e733533c09d41956b9606a7c6aaf613`  
		Last Modified: Sat, 28 Apr 2018 10:47:45 GMT  
		Size: 26.7 MB (26687092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5bd07609d18b01a4468533d1ef2f44d73ce4a39eb21ca52f111fe56eaf4e07`  
		Last Modified: Thu, 31 May 2018 06:18:02 GMT  
		Size: 469.1 KB (469106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2eb62cc483e44adba330b0e961bb185427b884355d6c1d64fe31215e6f821e`  
		Last Modified: Thu, 31 May 2018 06:18:02 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3301dd0fa6befe5d3eac4eb461cb6c2be8b132e9445e869931c35daa01b55f01`  
		Last Modified: Thu, 31 May 2018 06:33:41 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d6cf3bad415c2efddcf9ed91a505d0db9330656fe2019e29b292e3cb3c1144`  
		Last Modified: Thu, 31 May 2018 06:34:10 GMT  
		Size: 81.1 MB (81111607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:9-jre-slim-sid` - linux; ppc64le

```console
$ docker pull openjdk@sha256:794a4d8e267bbf38b754b4ea22b1f0316eb18ee35cd7d1002afbcf93f18220a1
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.9 MB (93905277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b5cc6fe0aa9e19c29c8a10c1691d7e6039905ed27d02a62ed804c76ddcbd78e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 08:19:31 GMT
ADD file:0f2a0abf96fc92379da26343d7babcee966430e13e320ed58e9b026f81a35dc0 in / 
# Sat, 28 Apr 2018 08:19:33 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 09:22:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 09:22:50 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 09:22:53 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 28 Apr 2018 09:30:54 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 28 Apr 2018 09:30:56 GMT
ENV JAVA_HOME=/docker-java-home
# Sat, 28 Apr 2018 09:30:57 GMT
ENV JAVA_VERSION=9.0.4+12
# Sat, 28 Apr 2018 09:30:58 GMT
ENV JAVA_DEBIAN_VERSION=9.0.4+12-4
# Tue, 15 May 2018 08:46:16 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-9-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:62552d209895f0ed53682f7309596edd291c8529683e854dd1fb36398d01bf69`  
		Last Modified: Sat, 28 Apr 2018 08:28:10 GMT  
		Size: 27.3 MB (27275595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ff6d72f21b69924c949ee40aec368655f2ab6a94c0a4a2067453fce44edabe`  
		Last Modified: Sat, 28 Apr 2018 09:48:20 GMT  
		Size: 455.2 KB (455169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d6f4b35b1a81554702460476a2fe3bd916579be94638ded8ee84048b7e208b`  
		Last Modified: Sat, 28 Apr 2018 09:48:19 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8d4e6285cb453ad45b8fffd593683ce971561e5dc3e3894511a103c2e0f3ef`  
		Last Modified: Sat, 28 Apr 2018 09:52:22 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d0a24dd34a9dfb1c5c4cb9b74cfbfc3874866e562e347365f904e1008882b5`  
		Last Modified: Tue, 15 May 2018 09:35:37 GMT  
		Size: 66.2 MB (66174142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:9-jre-slim-sid` - linux; s390x

```console
$ docker pull openjdk@sha256:2f5ee959238147bdccfb09d7806fdc6c420f38536d986f8e7d38ea217c630b2c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91457765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74df437155d474e80373ce4fe8089f0b68121665cf5dcb9da472981c3bb57756`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 11:44:07 GMT
ADD file:e38be352b5f5592b16e7137f372c3c15b62fa18d58036f3756f302a0b0bb631b in / 
# Sat, 28 Apr 2018 11:44:07 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 14:19:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 14:19:52 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 14:19:52 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 28 Apr 2018 14:26:54 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 28 Apr 2018 14:26:55 GMT
ENV JAVA_HOME=/docker-java-home
# Sat, 28 Apr 2018 14:26:55 GMT
ENV JAVA_VERSION=9.0.4+12
# Sat, 28 Apr 2018 14:26:55 GMT
ENV JAVA_DEBIAN_VERSION=9.0.4+12-4
# Tue, 15 May 2018 12:03:57 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-9-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:bff59799036649cecf076e4900a64b601dd41fb4774da5d260797609e96f77d2`  
		Last Modified: Sat, 28 Apr 2018 11:50:00 GMT  
		Size: 25.1 MB (25056085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00321480668e2c88c597070fd4a0503df76d083adfe3488d69f82f37cf3a1143`  
		Last Modified: Sat, 28 Apr 2018 14:37:59 GMT  
		Size: 471.3 KB (471260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0b7fa65f7725d173d1d9261b5c223d16d2f1f2a2850391fb2cd3eca5082060`  
		Last Modified: Sat, 28 Apr 2018 14:37:58 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0a4327ddb4df4bb93acb5eae40ad36e95b2347b79c0e675f2a5e62293f6a68`  
		Last Modified: Sat, 28 Apr 2018 14:48:49 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12e682761ef0a8595f992222b0e12d42179c0e6c161773b6d5427791ddb3e44`  
		Last Modified: Tue, 15 May 2018 12:35:19 GMT  
		Size: 65.9 MB (65930053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
