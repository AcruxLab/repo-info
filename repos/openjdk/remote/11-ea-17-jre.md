## `openjdk:11-ea-17-jre`

```console
$ docker pull openjdk@sha256:d6016930fd74e63d173ae11354df7561d96fff432654d5cb1fbdcf2d666f293c
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

### `openjdk:11-ea-17-jre` - linux; amd64

```console
$ docker pull openjdk@sha256:c3cf7f6842588e2c62abccc470c4b46882e2e7b9a6706e0114344913ba744ff2
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.4 MB (245441610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80c85b13aea82a14bac6b402bc5861d94dc982130606772ec159bb5435b1f151`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 06:49:58 GMT
ADD file:229ad62fdc5e079bf925fb084264841ce27bf7125beb1fd821cbd6ed5132b37c in / 
# Sat, 28 Apr 2018 06:49:59 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 23:11:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 23:11:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 06 Jun 2018 18:39:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Jun 2018 18:39:49 GMT
ENV LANG=C.UTF-8
# Wed, 06 Jun 2018 18:39:50 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 06 Jun 2018 18:39:51 GMT
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 06 Jun 2018 18:39:51 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 12 Jun 2018 00:28:46 GMT
ENV JAVA_VERSION=11-ea+17
# Tue, 12 Jun 2018 00:28:46 GMT
ENV JAVA_DEBIAN_VERSION=11~17-2
# Tue, 12 Jun 2018 00:29:25 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-11-jre="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:e7cb83f94a464daabb5fa4e63ae521d65d7956bfcb3619bc75857f7d598ff12c`  
		Last Modified: Sat, 28 Apr 2018 08:58:22 GMT  
		Size: 48.3 MB (48303234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea75eac4dae2f20cbd6fa1d55bc23e09e128934c845cd07f16ce17d88bf39af5`  
		Last Modified: Tue, 05 Jun 2018 23:39:45 GMT  
		Size: 7.0 MB (7030508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c35a0f820b4b715ac0c1825dacb71e27c6e5bbbc9320b94c42a479cb1f55eb`  
		Last Modified: Tue, 05 Jun 2018 23:39:49 GMT  
		Size: 10.3 MB (10334570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ef45ead295c4ee8d4d01af89bfa975475808968dd96d1917ded74eb4eca49e`  
		Last Modified: Wed, 06 Jun 2018 18:54:50 GMT  
		Size: 845.0 KB (844985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8173ebf385fa72497d72391cc38b3f3ad948853d501395bae26094545a03436`  
		Last Modified: Wed, 06 Jun 2018 18:54:49 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18856c258b6551e949ca5472158dba9ce7635a1a2b27e3ebe402dc00926a2790`  
		Last Modified: Wed, 06 Jun 2018 18:54:50 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d92b1e8bad7a8d5fb6638ab1d813cf825f7372e4c11e2ee372dc9c9d6ec568`  
		Last Modified: Tue, 12 Jun 2018 00:43:12 GMT  
		Size: 178.9 MB (178927944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:11-ea-17-jre` - linux; arm variant v5

```console
$ docker pull openjdk@sha256:3f97cf3ecef6b16e87949e034e60e883881efa16075d524f147758badd0b23da
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.6 MB (224643988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daa76ec11f31d257b1ba8b80362fa3c8c8fdb0711fbf2f5bf8a340bef20a94f7`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 08:51:39 GMT
ADD file:289dd78ee91d70cba0d1bc2f296c3c14565c2fc5a7545ded07d727de72e2c7af in / 
# Sat, 28 Apr 2018 08:51:39 GMT
CMD ["bash"]
# Sat, 05 May 2018 08:57:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 05 May 2018 08:57:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 05 May 2018 09:19:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 05 May 2018 09:19:08 GMT
ENV LANG=C.UTF-8
# Sat, 05 May 2018 09:19:09 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 05 May 2018 09:19:10 GMT
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 05 May 2018 09:19:11 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 12 Jun 2018 08:58:34 GMT
ENV JAVA_VERSION=11-ea+17
# Tue, 12 Jun 2018 08:58:34 GMT
ENV JAVA_DEBIAN_VERSION=11~17-2
# Tue, 12 Jun 2018 08:59:33 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-11-jre="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:e55988127988d265ae9a533cadc5ee50c9a724a2602f8677daa3d5ca1354a4c8`  
		Last Modified: Sat, 28 Apr 2018 08:59:59 GMT  
		Size: 46.3 MB (46298645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafc48823c28e5748b4391dec0c3ace05a68f5a65301bb16529fbf5cfdcf4ba2`  
		Last Modified: Sat, 05 May 2018 09:11:24 GMT  
		Size: 7.8 MB (7807554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab5f6db056b1ea7d4547374cc334a044271698f505521bb613b98b4e9d62fff`  
		Last Modified: Sat, 05 May 2018 09:11:25 GMT  
		Size: 9.2 MB (9194241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16073a84548c03437560da2931d6276f5698e1b26256817ec343c389cfd1c66a`  
		Last Modified: Sat, 05 May 2018 09:40:37 GMT  
		Size: 849.9 KB (849869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7511e3d44dd1677ace4c49728e92bc682e66c906f2d94d5a76db694717d1923c`  
		Last Modified: Sat, 05 May 2018 09:40:37 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855ae9a6b0d9285f5fd78459cb29e4089de21e1dcfb2f422edbd12db27296e26`  
		Last Modified: Sat, 05 May 2018 09:40:37 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2411b8e0b6436e5e72a186f71a73fea1262def0e4929a1652bc930871e3a85cf`  
		Last Modified: Tue, 12 Jun 2018 09:09:33 GMT  
		Size: 160.5 MB (160493312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:11-ea-17-jre` - linux; arm variant v7

```console
$ docker pull openjdk@sha256:1c4ad194a724ae58986163d28ab19ec3b227268277d18247973e221058446994
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.8 MB (219806572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd2e420a3695e88a4fa21a70b046e0248c53d93cbaaf0c04cfab17a4b14a1817`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:02:19 GMT
ADD file:b8fa078b9ddc39737b1c9eaeea11c4d1a71fb53d2ac6747fa0eab346280119a5 in / 
# Sat, 28 Apr 2018 12:02:20 GMT
CMD ["bash"]
# Sat, 05 May 2018 12:10:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 05 May 2018 12:10:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 05 May 2018 12:47:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 05 May 2018 12:47:14 GMT
ENV LANG=C.UTF-8
# Sat, 05 May 2018 12:47:16 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 05 May 2018 12:47:18 GMT
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 05 May 2018 12:47:18 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 12 Jun 2018 12:00:36 GMT
ENV JAVA_VERSION=11-ea+17
# Tue, 12 Jun 2018 12:00:36 GMT
ENV JAVA_DEBIAN_VERSION=11~17-2
# Tue, 12 Jun 2018 12:01:28 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-11-jre="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:bd36ef86ab3a0249a38384d63e39dbf85bd3f64d4e9ae0179795e2da5754d3fc`  
		Last Modified: Sat, 28 Apr 2018 12:13:46 GMT  
		Size: 44.2 MB (44193727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2182099ef994efdc26b1608eeb96ebb41405847c6f253e40c752ec9246cce60`  
		Last Modified: Sat, 05 May 2018 12:33:28 GMT  
		Size: 7.5 MB (7535807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fedbfebaf2860a81e319ee9a8c18137fb801f56d7729af7b4698f98e05c62b`  
		Last Modified: Sat, 05 May 2018 12:33:28 GMT  
		Size: 8.9 MB (8899307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4a3e738acdd9a9a58a2aae6f1746bfb228f3db2f19111110fa026ecbbbfa56`  
		Last Modified: Sat, 05 May 2018 13:10:03 GMT  
		Size: 833.5 KB (833517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2675718e4005b12e6c5113e924d01d09028ba80a4aa158bcdd2cde1983eac2`  
		Last Modified: Sat, 05 May 2018 13:10:03 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184c701159bb95571dd96ec48e59c940cf0b1c99277727bb8dd2e6deda95487e`  
		Last Modified: Sat, 05 May 2018 13:10:03 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b873748a27db003f1a93a0a70b83cf5a115b5bfe761d34b0051f95750843c6d4`  
		Last Modified: Tue, 12 Jun 2018 12:17:21 GMT  
		Size: 158.3 MB (158343846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:11-ea-17-jre` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:5f50dab3de047f8f5d22991d547bbe55ce5d070c0537e28c7e3c18421a700022
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.4 MB (229368452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2418e9d5754e71f3c9e6c4906fb5ced18654a9d2ceebc78465ddde009fbb968`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 30 Apr 2018 23:27:31 GMT
ADD file:ebaa7f02c60ac8138d085ce979847d36a1a8ce243bcef9b7e81e3e667d060dcb in / 
# Mon, 30 Apr 2018 23:27:34 GMT
CMD ["bash"]
# Sat, 05 May 2018 09:27:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 05 May 2018 09:28:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 05 May 2018 11:10:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 05 May 2018 11:10:02 GMT
ENV LANG=C.UTF-8
# Sat, 05 May 2018 11:10:05 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 05 May 2018 11:10:09 GMT
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 05 May 2018 11:10:10 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 12 Jun 2018 09:04:47 GMT
ENV JAVA_VERSION=11-ea+17
# Tue, 12 Jun 2018 09:04:48 GMT
ENV JAVA_DEBIAN_VERSION=11~17-2
# Tue, 12 Jun 2018 09:11:29 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-11-jre="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:ed5c004c8effeb24e6eee983af18662b0d28341fbbd46983746399c6df3358c8`  
		Last Modified: Mon, 30 Apr 2018 23:47:36 GMT  
		Size: 45.6 MB (45610129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8023415c45ba32335bb869e25328b3b2c70e3ad264f1129bb133addb1fbfef4a`  
		Last Modified: Sat, 05 May 2018 10:25:46 GMT  
		Size: 7.9 MB (7867437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2793192206e4ab032f5152356b71ea402af9d6cfd3812ad4e29857c76a039af6`  
		Last Modified: Sat, 05 May 2018 10:25:45 GMT  
		Size: 9.2 MB (9190303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e00dfc0b129c4ab2194347ddc38f66136387e9921b5f11f3ed3612ee9c840f`  
		Last Modified: Sat, 05 May 2018 12:39:12 GMT  
		Size: 843.0 KB (843039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0ff915ee587518b4d37f32230fd2b29388359c6dd67adc9e61cf15fbce46b6`  
		Last Modified: Sat, 05 May 2018 12:39:11 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c9430658318b096a24aa78870a521a4fb1d3e37c82b91243b8a28ec6de822a`  
		Last Modified: Sat, 05 May 2018 12:39:11 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3deda04fe4c96097ab022604095f5dc9ce545bae473de9e4c81cf2ea5e1199b0`  
		Last Modified: Tue, 12 Jun 2018 09:43:56 GMT  
		Size: 165.9 MB (165857177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:11-ea-17-jre` - linux; 386

```console
$ docker pull openjdk@sha256:a0c643e44981b80b42ec67acd60922ea0a6b37645c03b9c99f4d31b62b90573d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.6 MB (246560791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9a2b2203ed017b3fc0c434627d45ca84aac2b2040c485267c2696b11430a268`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 10:40:49 GMT
ADD file:cb21908d8f286f1381ea180209120314676afa1ce4d5d480e0310fe70a4c96d4 in / 
# Sat, 28 Apr 2018 10:40:49 GMT
CMD ["bash"]
# Wed, 06 Jun 2018 11:38:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Jun 2018 11:38:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 06 Jun 2018 13:15:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Jun 2018 13:15:36 GMT
ENV LANG=C.UTF-8
# Wed, 06 Jun 2018 13:15:37 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 06 Jun 2018 13:15:37 GMT
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 06 Jun 2018 13:15:38 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 12 Jun 2018 10:49:24 GMT
ENV JAVA_VERSION=11-ea+17
# Tue, 12 Jun 2018 10:49:24 GMT
ENV JAVA_DEBIAN_VERSION=11~17-2
# Tue, 12 Jun 2018 10:50:39 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-11-jre="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:33fb16074d5de3f73c0e2941c01c03e5dc69cfb8f568b7fbc3e29926b575fef0`  
		Last Modified: Sat, 28 Apr 2018 10:47:25 GMT  
		Size: 49.1 MB (49090181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a686f4eb752c82ac41a17df9c6701b1f073f7a2d9e420555cd2a5cb0dcbbea8a`  
		Last Modified: Wed, 06 Jun 2018 12:14:55 GMT  
		Size: 7.2 MB (7182217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9c2ebf9e0747fb0a03a84261c3698af2618b3c2fb833bdee559337f846c39f`  
		Last Modified: Wed, 06 Jun 2018 12:14:53 GMT  
		Size: 10.7 MB (10657958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2ea037d45b21831b2089139002e70c5892a3434cbad1c5dd8888afa9a09e66`  
		Last Modified: Wed, 06 Jun 2018 13:36:57 GMT  
		Size: 852.7 KB (852734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc6d422f837d347dc78ad60d6c3a26c9b5a01b6f533f2c9b24319568dd910ab`  
		Last Modified: Wed, 06 Jun 2018 13:36:58 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7adf2e8a4e22fcdadade2becfa89eea53cbbc451842b58abf578dccb19a7170`  
		Last Modified: Wed, 06 Jun 2018 13:36:57 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcc34007717816ad922debc764f44359da40326fa5ddb33e92a18773a18f9db`  
		Last Modified: Tue, 12 Jun 2018 11:07:58 GMT  
		Size: 178.8 MB (178777332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:11-ea-17-jre` - linux; ppc64le

```console
$ docker pull openjdk@sha256:839894aedb71d071ec12510eb0c06e5100f73bfcac572bef2cf7575b476702c0
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.3 MB (237328123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bad4673e07f659d4153b0400c5a50c7d1837d5d6b1e2092ac1609bc4c84539`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 08:19:13 GMT
ADD file:320268259acdc4e2a105be735ea4ee0cb1398bb05ce729d46f4a54fa3c3c84e3 in / 
# Sat, 28 Apr 2018 08:19:15 GMT
CMD ["bash"]
# Sat, 05 May 2018 09:16:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 05 May 2018 09:16:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 05 May 2018 13:40:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 05 May 2018 13:40:58 GMT
ENV LANG=C.UTF-8
# Sat, 05 May 2018 13:41:00 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 05 May 2018 13:41:02 GMT
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 05 May 2018 13:41:06 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 12 Jun 2018 08:38:15 GMT
ENV JAVA_VERSION=11-ea+17
# Tue, 12 Jun 2018 08:38:21 GMT
ENV JAVA_DEBIAN_VERSION=11~17-2
# Tue, 12 Jun 2018 08:42:04 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-11-jre="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:354f055c313d4d07201e01fd4de9af4aca89e3df17572870e56c5b8945e48443`  
		Last Modified: Sat, 28 Apr 2018 08:27:42 GMT  
		Size: 49.8 MB (49754912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77e4d2b61d28a226758713bae6bf933182cc9aa5eea6834696ef5865b36a2d2`  
		Last Modified: Sat, 05 May 2018 10:56:29 GMT  
		Size: 8.3 MB (8252158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee38bf91c1472a5fafe06a2f5ba7ea5bf20d82e4c77308ccb3bb26c3068d95c5`  
		Last Modified: Sat, 05 May 2018 10:56:40 GMT  
		Size: 9.7 MB (9711623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac66d4df0eb05e246b8290fe8e98d0dc23c04705d9e2e79abed62b95a7329a0a`  
		Last Modified: Sat, 05 May 2018 14:50:15 GMT  
		Size: 852.5 KB (852475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09abe145510be9656286d6cbd8cfed6e7efc4f1079ce629e458b56c291939a9`  
		Last Modified: Sat, 05 May 2018 14:50:14 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcfc84ce5c8614175802345c31d29d0829ae536a87ca8e08abb26167c05f191`  
		Last Modified: Sat, 05 May 2018 14:50:14 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c521c0c9be9700cfce646d23adcbd3a0f1c18df08cb6574a86be18b929e0267`  
		Last Modified: Tue, 12 Jun 2018 09:10:49 GMT  
		Size: 168.8 MB (168756585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:11-ea-17-jre` - linux; s390x

```console
$ docker pull openjdk@sha256:22b2829d2618b63f741554fa0ab4082140364bedede114687bb52642bef92b90
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.8 MB (207840741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c33bbfa2e2d40959a3432c13dc6d9f9ef789f4db56956b50575865519abc0a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 11:43:52 GMT
ADD file:2ebc77cf35fadaf6ffd85f0d203bf60b217e15aa3c15737aac14f71008535107 in / 
# Sat, 28 Apr 2018 11:43:52 GMT
CMD ["bash"]
# Sat, 05 May 2018 12:33:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 05 May 2018 12:34:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 05 May 2018 13:04:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 05 May 2018 13:04:48 GMT
ENV LANG=C.UTF-8
# Sat, 05 May 2018 13:04:49 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 05 May 2018 13:04:49 GMT
RUN ln -svT "/usr/lib/jvm/java-11-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 05 May 2018 13:04:50 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 12 Jun 2018 11:52:14 GMT
ENV JAVA_VERSION=11-ea+17
# Tue, 12 Jun 2018 11:52:14 GMT
ENV JAVA_DEBIAN_VERSION=11~17-2
# Tue, 12 Jun 2018 11:52:53 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-11-jre="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:893cc85742608c84d1d6314416656d650a83dae134d0d1e22a839b39a03cbf3e`  
		Last Modified: Sat, 28 Apr 2018 11:49:42 GMT  
		Size: 47.4 MB (47350246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6465ae4acbbbfe22cde44168d0262178f375ac945898fbe73420bec2cc2ccbe0`  
		Last Modified: Sat, 05 May 2018 12:46:57 GMT  
		Size: 8.1 MB (8124442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47a8c562fcb2d700f3403a2f6b5d1c62f5961afce859416ff6a03520adf95a5`  
		Last Modified: Sat, 05 May 2018 12:46:57 GMT  
		Size: 9.4 MB (9414344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d454588c8ff8bb223303585c77d5babc9049e62b88dc7e14e1b2060311433972`  
		Last Modified: Sat, 05 May 2018 13:20:02 GMT  
		Size: 867.2 KB (867200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b294e615c7f7bb31f89759db3ec8dc4a53c969332be38669eb8d9e5095a5370`  
		Last Modified: Sat, 05 May 2018 13:20:02 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e86c86c15985e0643c28d68750f469e1b0390060cc9bfa5f577d44452f55b2`  
		Last Modified: Thu, 10 May 2018 13:12:35 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1131aae057a64199f319c4b9703f305c17c382d937887960f67bfef0a9cfe53`  
		Last Modified: Tue, 12 Jun 2018 12:00:02 GMT  
		Size: 142.1 MB (142084139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
