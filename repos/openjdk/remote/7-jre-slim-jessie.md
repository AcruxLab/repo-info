## `openjdk:7-jre-slim-jessie`

```console
$ docker pull openjdk@sha256:69ba65b00593b15ca3c47ad7b39143468725e2418e5e3f4504265c43c0be954c
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

### `openjdk:7-jre-slim-jessie` - linux; amd64

```console
$ docker pull openjdk@sha256:f12e0b89b89b305096f4cfc5d7206275186138c14e7641341d3d2dee58603dd2
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92714121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71746552de61c566feabe017c3456d999a61afcadfbab154bda3e9d192aa02ba`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 06:45:24 GMT
ADD file:50be6ceb11c382ed9674106471df123e9a76f549fe729b4751bc95662258f9e0 in / 
# Sat, 28 Apr 2018 06:45:24 GMT
CMD ["bash"]
# Wed, 06 Jun 2018 02:00:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Jun 2018 02:00:15 GMT
ENV LANG=C.UTF-8
# Wed, 06 Jun 2018 02:00:15 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 06 Jun 2018 02:00:16 GMT
RUN ln -svT "/usr/lib/jvm/java-7-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 06 Jun 2018 02:00:16 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Wed, 06 Jun 2018 02:00:17 GMT
ENV JAVA_VERSION=7u171
# Wed, 06 Jun 2018 02:00:17 GMT
ENV JAVA_DEBIAN_VERSION=7u171-2.6.13-1~deb8u1
# Wed, 06 Jun 2018 02:01:08 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-7-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:4d0d76e05f3c6caf923a71ca3b3d2cc8c834ca61779ae6b6d83547f3dd814980`  
		Last Modified: Sat, 28 Apr 2018 08:30:42 GMT  
		Size: 30.1 MB (30127297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd45ab3e8705100d059fefde01e2940d76606981926a01a09458dce1afca1a0`  
		Last Modified: Wed, 06 Jun 2018 02:20:57 GMT  
		Size: 463.7 KB (463731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b81648969360d1555321bbc2861ac7ffc37e749c6ad074769dea91e9b00387`  
		Last Modified: Wed, 06 Jun 2018 02:20:57 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ef42f9b69097a06b45e40258725d09d897141042e356843eba36b6c7ac60c2`  
		Last Modified: Wed, 06 Jun 2018 02:20:56 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db62de74fb121b367feaf6052aeac2c8f73174cc29b67548ec79f286f963db4`  
		Last Modified: Wed, 06 Jun 2018 02:21:16 GMT  
		Size: 62.1 MB (62122714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:7-jre-slim-jessie` - linux; arm variant v5

```console
$ docker pull openjdk@sha256:37e552cd56782a787491c8b2a7fe2651012b8a4c6e21e1627ddc550e184e2822
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.8 MB (80823269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:beeb1aa76fccfeef1084317043eb7db4e5ba0110c6b2d248d86d5cd96ff09f21`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 08:49:49 GMT
ADD file:e9274d48b6cf2508214a554b4dbe651b4dfa95bb52dba47a96fe8842bf606a87 in / 
# Sat, 28 Apr 2018 08:49:49 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 12:55:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:55:03 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:55:03 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 28 Apr 2018 12:55:04 GMT
RUN ln -svT "/usr/lib/jvm/java-7-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 28 Apr 2018 12:55:05 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Sat, 28 Apr 2018 12:55:05 GMT
ENV JAVA_VERSION=7u171
# Sat, 28 Apr 2018 12:55:05 GMT
ENV JAVA_DEBIAN_VERSION=7u171-2.6.13-1~deb8u1
# Tue, 15 May 2018 09:51:28 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-7-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:94b675ca74d2386dbd57e10d92f282f24ca3519fd21339c04af3f8f7e523617c`  
		Last Modified: Sat, 28 Apr 2018 08:57:53 GMT  
		Size: 28.4 MB (28435716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64413c45c2b1761082392f40b8eb4f8c01e04ace06cf565ed33520cde914a2f3`  
		Last Modified: Sat, 28 Apr 2018 13:30:17 GMT  
		Size: 456.4 KB (456447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc8503ffe14feee207fc8f6387fe1698d57ea88c261e13e32014df47d242ab2`  
		Last Modified: Sat, 28 Apr 2018 13:30:17 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3238929bec356935380aebd06a38df60f54e0b955554074db0321e380626388`  
		Last Modified: Sat, 28 Apr 2018 13:30:17 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a0bec81f3b28c1380f627f82e9057f904abe6b7bf4d14fd094be44feaf8967`  
		Last Modified: Tue, 15 May 2018 10:31:34 GMT  
		Size: 51.9 MB (51930728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:7-jre-slim-jessie` - linux; arm variant v7

```console
$ docker pull openjdk@sha256:d37b9e3b18285dfad955d87bdd088053db02c2000606d5c28b560ae6b48891de
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.5 MB (77533136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cc078d6284041d5c65cb7cfc0d5a73b0ba183b6a7108736065aa3af1f9a7882`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 11:59:37 GMT
ADD file:f8c645337024c026fbe602f5480bff6efe08526fe5ae5523df7dc29d240d16d2 in / 
# Sat, 28 Apr 2018 11:59:37 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 12:57:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:57:49 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:57:50 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 28 Apr 2018 12:57:57 GMT
RUN ln -svT "/usr/lib/jvm/java-7-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 28 Apr 2018 12:57:57 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Sat, 28 Apr 2018 12:57:58 GMT
ENV JAVA_VERSION=7u171
# Sat, 28 Apr 2018 12:57:58 GMT
ENV JAVA_DEBIAN_VERSION=7u171-2.6.13-1~deb8u1
# Tue, 15 May 2018 12:26:40 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-7-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:2d5e3d857ad4821de542179b9b489e90fd471e4cd9f25c4aa2a09561c37a7806`  
		Last Modified: Sat, 28 Apr 2018 12:11:15 GMT  
		Size: 26.3 MB (26297400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12f199f27c7efc052499b2e8ed53e8619167862acb1abe9a2f3baf9511f616f`  
		Last Modified: Sat, 28 Apr 2018 13:28:17 GMT  
		Size: 432.3 KB (432321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07998aba91636c8f624b6c3b61ed3a56f8b827314f55812e2183cf1f9e78e73`  
		Last Modified: Sat, 28 Apr 2018 13:28:17 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70beb70d7caf8b057153c16add67b8ed61b89307e4fe2cd6d1e48c086653401f`  
		Last Modified: Sat, 28 Apr 2018 13:28:17 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff67eb6912dfa6a0f451d2f7d97404c0798006575e954ef60e57dd99cc8f2461`  
		Last Modified: Tue, 15 May 2018 13:04:34 GMT  
		Size: 50.8 MB (50803038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:7-jre-slim-jessie` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:65ee2d6f9932f0ab54feea551f6fc5431861f1a26d4b36a1e1fa34ccdb3728ac
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.1 MB (81106429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df8894f5b56842a1fa3881460d5b0e295ec35b1de8caf6cff3afb4d823f58091`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 30 Apr 2018 23:23:15 GMT
ADD file:d88886292edb80d3898ba50f464cceb9c33709b3bb124f81e910bc9c6b0e7acc in / 
# Mon, 30 Apr 2018 23:23:18 GMT
CMD ["bash"]
# Tue, 01 May 2018 11:19:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 11:19:37 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 11:19:46 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 01 May 2018 11:19:53 GMT
RUN ln -svT "/usr/lib/jvm/java-7-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 01 May 2018 11:19:56 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Tue, 01 May 2018 11:19:59 GMT
ENV JAVA_VERSION=7u171
# Tue, 01 May 2018 11:20:03 GMT
ENV JAVA_DEBIAN_VERSION=7u171-2.6.13-1~deb8u1
# Tue, 15 May 2018 10:17:45 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-7-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:6d46b8f3eebfe36e412a394de4bf8a598e22d1fe11cd6b35f34e770473c170ea`  
		Last Modified: Mon, 30 Apr 2018 23:43:19 GMT  
		Size: 27.5 MB (27494590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c67f48d3f95f879f0a16939897151d838aeae71743f184d41d557ba719f896`  
		Last Modified: Tue, 01 May 2018 11:59:05 GMT  
		Size: 457.9 KB (457930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e4f5df17d67da29d0f5e8846dfb76e7f541e3c84f16d804a52313cf3f2d755`  
		Last Modified: Tue, 01 May 2018 11:59:04 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825cf0a868d42f586b37204e4c5bbc1ab2668b7d1d01156e2be933557a5fe1fd`  
		Last Modified: Tue, 01 May 2018 11:59:04 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49002e4d1e40979d09f418b85cd25d2755479a5e981f70e5b8bb1452f7cdd4e7`  
		Last Modified: Tue, 15 May 2018 11:09:11 GMT  
		Size: 53.2 MB (53153531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:7-jre-slim-jessie` - linux; 386

```console
$ docker pull openjdk@sha256:d51c1db25a24a01a966ab39f2ea9f09469068b9d502de69f3d642bbedbee9965
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104463516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e58f3ffac360d62be616f9e2671026b1c5204692a5e690b32bda9e48bf2eeebf`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 10:39:45 GMT
ADD file:335ca08e6c562d8b16f2a4e788c5e977ba9815526d92d6d48cc3b8093824da2d in / 
# Sat, 28 Apr 2018 10:39:45 GMT
CMD ["bash"]
# Thu, 31 May 2018 06:08:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 31 May 2018 06:08:40 GMT
ENV LANG=C.UTF-8
# Thu, 31 May 2018 06:08:41 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Thu, 31 May 2018 06:08:41 GMT
RUN ln -svT "/usr/lib/jvm/java-7-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Thu, 31 May 2018 06:08:41 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Thu, 31 May 2018 06:08:42 GMT
ENV JAVA_VERSION=7u171
# Thu, 31 May 2018 06:08:42 GMT
ENV JAVA_DEBIAN_VERSION=7u171-2.6.13-1~deb8u1
# Thu, 31 May 2018 06:10:11 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-7-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:175c17a0040b2274213f9504ec9e834814804aa24e25f9537af71fccc81a017f`  
		Last Modified: Sat, 28 Apr 2018 10:45:06 GMT  
		Size: 30.3 MB (30278658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c93922e68ccea08277f2a4c59128ace53b10fe857702b1d9b8a7efab5b03464`  
		Last Modified: Thu, 31 May 2018 06:46:06 GMT  
		Size: 466.3 KB (466282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55e5d35b28c2158509b6d34570c3e05dc1002434dc68c2ba455fdf9fa71b64a`  
		Last Modified: Thu, 31 May 2018 06:46:06 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5275fdf6127f8903bc3be2c6a5f857d61a31085bf986d759bec459cc250278d4`  
		Last Modified: Thu, 31 May 2018 06:46:06 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0470f88f2cb46677107b62dfaf22438b91722ccdc63e9d17af9f2cc785859056`  
		Last Modified: Thu, 31 May 2018 06:46:27 GMT  
		Size: 73.7 MB (73718197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:7-jre-slim-jessie` - linux; ppc64le

```console
$ docker pull openjdk@sha256:fd862fabed328f710cefb52800bfdca4fe2a7c0aaaa80ea0599aa699b515352c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.7 MB (83715372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f4148fdd35fbabd1b628c2d3da895b7db705020a8de951f561364a576fcdd88`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 08:18:08 GMT
ADD file:cc51ef60d7cb3b70c82127b8721de1b99378a9d4fc246dffa2ef5ffa2d9ab805 in / 
# Sat, 28 Apr 2018 08:18:09 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 09:38:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 09:38:39 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 09:38:41 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 28 Apr 2018 09:38:43 GMT
RUN ln -svT "/usr/lib/jvm/java-7-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 28 Apr 2018 09:38:43 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Sat, 28 Apr 2018 09:38:44 GMT
ENV JAVA_VERSION=7u171
# Sat, 28 Apr 2018 09:38:44 GMT
ENV JAVA_DEBIAN_VERSION=7u171-2.6.13-1~deb8u1
# Tue, 15 May 2018 09:08:35 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-7-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:7745ff03a317ccaa10ff03129a2330b1c154aecaf51a892b7d99d5e1dbeb86cc`  
		Last Modified: Sat, 28 Apr 2018 08:25:29 GMT  
		Size: 29.3 MB (29317351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904d9cae5b4e13977b3a3f5da2837f3842b44dd1ad001f63bae91c193e6384e7`  
		Last Modified: Sat, 28 Apr 2018 09:58:30 GMT  
		Size: 460.2 KB (460245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f46e6678f464aca7e6dd6754f68d28005443749f3cbf76be8b3e676a6947a1`  
		Last Modified: Sat, 28 Apr 2018 09:58:28 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5e5c5eac28805942423bb472b259179da4051103daa04229bfb914fbd74006`  
		Last Modified: Sat, 28 Apr 2018 09:58:29 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61fba54c73d5f296fcf885f182c4c7022c4770b99a19e1b8ddb2e14000a94bb8`  
		Last Modified: Tue, 15 May 2018 09:48:12 GMT  
		Size: 53.9 MB (53937397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:7-jre-slim-jessie` - linux; s390x

```console
$ docker pull openjdk@sha256:eb2559410736a7c8757a1897f0d72a6c200153d95d0c03cdeeab34f920a726e5
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.3 MB (84261456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14edd1a0009d468d150612f6aded5d93aeb19aa19889e61349d3173e17c79a1b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 11:42:53 GMT
ADD file:7c773d50957d6184975f5b22ef61757cd979893af5c77cdfef46dd28d8fc0296 in / 
# Sat, 28 Apr 2018 11:42:55 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 14:33:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 14:33:30 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 14:33:30 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 28 Apr 2018 14:33:31 GMT
RUN ln -svT "/usr/lib/jvm/java-7-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 28 Apr 2018 14:33:31 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Sat, 28 Apr 2018 14:33:31 GMT
ENV JAVA_VERSION=7u171
# Sat, 28 Apr 2018 14:33:31 GMT
ENV JAVA_DEBIAN_VERSION=7u171-2.6.13-1~deb8u1
# Tue, 15 May 2018 12:13:31 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-7-jre-headless="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:f4d03f2765a5584a0dc02af25ffd7c98d6e129d072a1fc30380b106603442102`  
		Last Modified: Sat, 28 Apr 2018 11:48:28 GMT  
		Size: 30.3 MB (30308304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53dd73eb8e6bfd44480a404637dfc711eb6cfa167bcacd7b692ee13e269920ad`  
		Last Modified: Sat, 28 Apr 2018 14:58:39 GMT  
		Size: 473.2 KB (473195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4b07ff4fb390ce7c50cd1a3f4c1856608817a2e55147026b2113f0e1c9d057`  
		Last Modified: Sat, 28 Apr 2018 14:58:39 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7c4bb4187f99b40f5b149b933b5730667a7287c28f52903d444450e9881cc3`  
		Last Modified: Sat, 28 Apr 2018 14:58:39 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f074f5978050fa0ec75183cc20e3e5de97baa6dc6a3c0346d313f3015e8b668`  
		Last Modified: Tue, 15 May 2018 12:49:42 GMT  
		Size: 53.5 MB (53479578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
