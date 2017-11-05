## `maven:alpine`

```console
$ docker pull maven@sha256:db36a5f4a5d589dca4b18ec69873ab64d3ae48348a72c6b1268d296f899d4c25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `maven:alpine` - linux; amd64

```console
$ docker pull maven@sha256:3de1f64186426fdbd3f732a327f41eb72f9b87f6942eba02108de931d28b9278
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.6 MB (82623720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:293423a981a7effa3bbb76dcb3c210671ec7bd560bf5be945f3d377fd37426e4`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 10 May 2017 16:38:16 GMT
ADD file:63f63606d6e289eb607c90e31de81802258906712727e473a2898f0f1ae55bb5 in / 
# Wed, 10 May 2017 16:38:17 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2017 22:39:51 GMT
ENV LANG=C.UTF-8
# Wed, 10 May 2017 22:39:53 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 10 May 2017 22:39:54 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
# Wed, 10 May 2017 22:39:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Wed, 10 May 2017 22:39:55 GMT
ENV JAVA_VERSION=8u121
# Wed, 10 May 2017 22:39:56 GMT
ENV JAVA_ALPINE_VERSION=8.121.13-r0
# Wed, 10 May 2017 22:40:01 GMT
RUN set -x 	&& apk add --no-cache 		openjdk8="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sat, 04 Nov 2017 23:44:27 GMT
RUN apk add --no-cache curl tar bash
# Sat, 04 Nov 2017 23:44:27 GMT
ARG MAVEN_VERSION=3.5.2
# Sat, 04 Nov 2017 23:44:28 GMT
ARG USER_HOME_DIR=/root
# Sat, 04 Nov 2017 23:44:28 GMT
ARG SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff
# Sat, 04 Nov 2017 23:44:28 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries
# Sat, 04 Nov 2017 23:44:29 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries MAVEN_VERSION=3.5.2 SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha256sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 04 Nov 2017 23:44:29 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 04 Nov 2017 23:44:30 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 04 Nov 2017 23:44:30 GMT
COPY file:e4099db07053a2301f4263d416cab324c1f89ee74c752bebec511d8b59464cb6 in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 04 Nov 2017 23:44:30 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Sat, 04 Nov 2017 23:44:30 GMT
VOLUME [/root/.m2]
# Sat, 04 Nov 2017 23:44:31 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 04 Nov 2017 23:44:31 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:cfc728c1c5584d8e0ae69368fc9c34d54d72651355573ba42554c2469a0a6299`  
		Last Modified: Wed, 10 May 2017 16:41:01 GMT  
		Size: 2.0 MB (1967906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b12b87f0a0e1bc0a163558cc56861b86355598153fb9e35273ece1dabe81cae`  
		Last Modified: Fri, 12 May 2017 15:19:23 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d6497a92f9de7c9b828962ad09a648e1d72687dda6bb986a72e95c61bb3dad`  
		Last Modified: Fri, 12 May 2017 15:19:30 GMT  
		Size: 70.0 MB (70004148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399bf97523476b8d4e2f8f9e3502e84e3830692fa1a821cd26c6faa4bbde9d6b`  
		Last Modified: Sat, 04 Nov 2017 23:44:52 GMT  
		Size: 1.8 MB (1766505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e41e7b89fb836d0b1ccdce50ac7e47fd16c3788692cf1671381fadaa8761149`  
		Last Modified: Sat, 04 Nov 2017 23:44:53 GMT  
		Size: 8.9 MB (8883843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1017f315d511fe2beb8d9367f9994bb5e5d40928d990b58995f6ea9c2424cc03`  
		Last Modified: Sat, 04 Nov 2017 23:44:52 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bc7fb81913133d8d1b51b5c8e72f689b527acb125559b160c0e0e27c67490d`  
		Last Modified: Sat, 04 Nov 2017 23:44:52 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:alpine` - linux; arm variant v6

```console
$ docker pull maven@sha256:d87135f72b67410dccef73e1a200da3a23a4975bb9116e5d85cce1b6522efb19
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79723663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e52c547252308b10398dc9dda3c6215519aa700450b50bddf8157d012d21e06b`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Sat, 13 May 2017 05:35:49 GMT
ADD file:be7cfe66d037514dfa5b3049f3c2912458d1f83132ef9d13780c84a85353cc80 in / 
# Sat, 13 May 2017 05:35:49 GMT
CMD ["sh"]
# Mon, 15 May 2017 20:51:35 GMT
ENV LANG=C.UTF-8
# Mon, 15 May 2017 20:51:35 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 15 May 2017 20:51:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
# Mon, 15 May 2017 20:51:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Mon, 15 May 2017 20:51:36 GMT
ENV JAVA_VERSION=8u121
# Mon, 15 May 2017 20:51:36 GMT
ENV JAVA_ALPINE_VERSION=8.121.13-r0
# Mon, 15 May 2017 20:51:57 GMT
RUN set -x 	&& apk add --no-cache 		openjdk8="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 02 Nov 2017 04:20:37 GMT
RUN apk add --no-cache curl tar bash
# Thu, 02 Nov 2017 04:20:38 GMT
ARG MAVEN_VERSION=3.5.2
# Thu, 02 Nov 2017 04:20:38 GMT
ARG USER_HOME_DIR=/root
# Thu, 02 Nov 2017 04:20:38 GMT
ARG SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff
# Thu, 02 Nov 2017 04:20:38 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries
# Thu, 02 Nov 2017 04:20:41 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries MAVEN_VERSION=3.5.2 SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha256sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 02 Nov 2017 04:20:41 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 02 Nov 2017 04:20:41 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 02 Nov 2017 04:20:42 GMT
COPY file:e4099db07053a2301f4263d416cab324c1f89ee74c752bebec511d8b59464cb6 in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 02 Nov 2017 04:20:42 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Thu, 02 Nov 2017 04:20:42 GMT
VOLUME [/root/.m2]
# Thu, 02 Nov 2017 04:20:42 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 02 Nov 2017 04:20:42 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:47c5ef52fac1f1ab481cccaf684fd041d64aaca4b9fd16d2fef19ef1aaaed084`  
		Last Modified: Sat, 13 May 2017 05:38:04 GMT  
		Size: 1.9 MB (1867536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448b7b9cbe4a50a14e8f4ad8bc21a46a12e6aead982e8354f4b9192e05f97229`  
		Last Modified: Mon, 15 May 2017 20:52:19 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0387f11a0fdf56938c2749103a9f4c8bba6c7468eca97367dcdda7587356fb55`  
		Last Modified: Mon, 15 May 2017 20:52:43 GMT  
		Size: 67.3 MB (67259533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab4f7efd36b25e9ca353c07bb8278bbdabbf8ad0e1a3bbe418aa8c3d287a7f6`  
		Last Modified: Thu, 02 Nov 2017 04:20:52 GMT  
		Size: 1.7 MB (1711397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7815d428f18b1f1757498b691cfd2749f4144774bf1260624c268cc810cdb581`  
		Last Modified: Thu, 02 Nov 2017 04:20:54 GMT  
		Size: 8.9 MB (8883874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4364a6d6c87fd246d2e7e45e3d6f0693f47bb5f07c53fad30863bdc9288da5e`  
		Last Modified: Thu, 02 Nov 2017 04:20:51 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58857d5e58afdc16ac393d8b732366165ea38f3d849acd555ea614144005cd70`  
		Last Modified: Thu, 02 Nov 2017 04:20:51 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:alpine` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:c871b95afd44e8bacea3d0f1b634f037b075cc7c6be7b3c5e9e74f10a26fe7d1
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.8 MB (80839680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdac1580d86ac7a1ba401030a1917ae55aeba0efb20b8e262822d14955821ed6`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Sat, 13 May 2017 04:30:45 GMT
ADD file:9f1ff42c8ce7ac20d3240b160b66bd68fa996e33d29b349b3bcf775fb7508fbe in / 
# Sat, 13 May 2017 04:30:45 GMT
CMD ["sh"]
# Mon, 15 May 2017 20:50:21 GMT
ENV LANG=C.UTF-8
# Mon, 15 May 2017 20:50:22 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 15 May 2017 20:50:23 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
# Mon, 15 May 2017 20:50:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Mon, 15 May 2017 20:50:24 GMT
ENV JAVA_VERSION=8u121
# Mon, 15 May 2017 20:50:25 GMT
ENV JAVA_ALPINE_VERSION=8.121.13-r0
# Mon, 15 May 2017 20:50:45 GMT
RUN set -x 	&& apk add --no-cache 		openjdk8="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 02 Nov 2017 18:22:32 GMT
RUN apk add --no-cache curl tar bash
# Thu, 02 Nov 2017 18:22:33 GMT
ARG MAVEN_VERSION=3.5.2
# Thu, 02 Nov 2017 18:22:33 GMT
ARG USER_HOME_DIR=/root
# Thu, 02 Nov 2017 18:22:34 GMT
ARG SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff
# Thu, 02 Nov 2017 18:22:35 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries
# Thu, 02 Nov 2017 18:22:42 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries MAVEN_VERSION=3.5.2 SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha256sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 02 Nov 2017 18:22:43 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 02 Nov 2017 18:22:43 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 02 Nov 2017 18:22:44 GMT
COPY file:e4099db07053a2301f4263d416cab324c1f89ee74c752bebec511d8b59464cb6 in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 02 Nov 2017 18:22:45 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Thu, 02 Nov 2017 18:22:46 GMT
VOLUME [/root/.m2]
# Thu, 02 Nov 2017 18:22:46 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 02 Nov 2017 18:22:47 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:10e6ef928f7294aaad4aad1470c568a87b6ee39b60a161319bb493571c134b63`  
		Last Modified: Wed, 19 Jul 2017 16:32:21 GMT  
		Size: 1.9 MB (1895963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d88fc9116cb1407f6e4285f521536fb397674037ccca2e1e6cc84da8827d67`  
		Last Modified: Mon, 15 May 2017 20:51:12 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ca86fc5b835f15cf1ed677f3dd8a8a6d1876706c39cdf4eea5ebc712e4bc44`  
		Last Modified: Mon, 15 May 2017 20:51:31 GMT  
		Size: 68.4 MB (68380138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99917f0b448604b5c974cc4d10555faf32651327a92e87bfde0d763bfe29174e`  
		Last Modified: Thu, 02 Nov 2017 18:23:34 GMT  
		Size: 1.7 MB (1678413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d928aab5d20ac1e0ef1318a809d00292edd586d0e3ebe60794722430ad9ca6`  
		Last Modified: Thu, 02 Nov 2017 18:23:35 GMT  
		Size: 8.9 MB (8883832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12d42fab7b93fa237470d1f84e97205fdfbffada8b8c514c736cb3cdd33c589`  
		Last Modified: Thu, 02 Nov 2017 18:23:33 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b1dc155e03f67274cbea84c18fdef4377471f0b5acb0f5afb87fdf6e721b29`  
		Last Modified: Thu, 02 Nov 2017 18:23:33 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:alpine` - linux; 386

```console
$ docker pull maven@sha256:57fa99f3a61565ee63ffb5ae6a48a837b10f85fccb6eb6f7a6e7d38b57889075
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83426366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:701258ebc02ab380af2523c60bfd88c4dc9283fa713a9074f0462d63404502b5`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Sat, 13 May 2017 04:29:27 GMT
ADD file:e900452b23e54c736cfe6d382244128cf76b1de073045356c3e614872f4a4d0e in / 
# Sat, 13 May 2017 04:29:28 GMT
CMD ["sh"]
# Mon, 15 May 2017 21:00:12 GMT
ENV LANG=C.UTF-8
# Mon, 15 May 2017 21:00:13 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Mon, 15 May 2017 21:00:13 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
# Mon, 15 May 2017 21:00:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.8-openjdk/jre/bin:/usr/lib/jvm/java-1.8-openjdk/bin
# Mon, 15 May 2017 21:00:14 GMT
ENV JAVA_VERSION=8u121
# Mon, 15 May 2017 21:00:14 GMT
ENV JAVA_ALPINE_VERSION=8.121.13-r0
# Mon, 15 May 2017 21:00:33 GMT
RUN set -x 	&& apk add --no-cache 		openjdk8="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 02 Nov 2017 01:37:22 GMT
RUN apk add --no-cache curl tar bash
# Thu, 02 Nov 2017 01:37:23 GMT
ARG MAVEN_VERSION=3.5.2
# Thu, 02 Nov 2017 01:37:23 GMT
ARG USER_HOME_DIR=/root
# Thu, 02 Nov 2017 01:37:23 GMT
ARG SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff
# Thu, 02 Nov 2017 01:37:23 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries
# Thu, 02 Nov 2017 01:37:25 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries MAVEN_VERSION=3.5.2 SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha256sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 02 Nov 2017 01:37:25 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 02 Nov 2017 01:37:25 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 02 Nov 2017 01:37:25 GMT
COPY file:e4099db07053a2301f4263d416cab324c1f89ee74c752bebec511d8b59464cb6 in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 02 Nov 2017 01:37:26 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Thu, 02 Nov 2017 01:37:26 GMT
VOLUME [/root/.m2]
# Thu, 02 Nov 2017 01:37:26 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 02 Nov 2017 01:37:26 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:613687d8794057a97a070d4c975c4bd357238d5819c54b14ed7e6133546c45b2`  
		Last Modified: Sat, 13 May 2017 04:29:32 GMT  
		Size: 2.0 MB (2017241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f865c8d151e4d09c228efd9df1262334e85b6073b92790c24a49f0fedf3b3b0`  
		Last Modified: Mon, 15 May 2017 21:07:25 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc3022b8c09bc01aa37b15837de27eefe4f7ff14c21c5c366423499047c5870`  
		Last Modified: Mon, 15 May 2017 21:07:32 GMT  
		Size: 70.6 MB (70645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36af3b4cc17db7933732ad76a8d471e4d924f15c2f3ad5d0ade3ec32c423e7c8`  
		Last Modified: Thu, 02 Nov 2017 01:37:48 GMT  
		Size: 1.9 MB (1878261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767d6df3b77afa7227adbe52ad296f23e386dacda07eade374af71ef24274d2c`  
		Last Modified: Thu, 02 Nov 2017 01:37:48 GMT  
		Size: 8.9 MB (8883841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9bd202ffc3a7e39a818596180e197799690ac544ad6ea3b96d69a38bad5907b`  
		Last Modified: Thu, 02 Nov 2017 01:37:47 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb48f3945235762f5d8749e4d86e57550a98e019b093becc6037406f2f7c0833`  
		Last Modified: Thu, 02 Nov 2017 01:37:47 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
