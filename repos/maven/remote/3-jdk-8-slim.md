## `maven:3-jdk-8-slim`

```console
$ docker pull maven@sha256:1609e497cb0e8d7b7df5bb4fbe58722e41a09258b4cce55d148e7fedd3f75f89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `maven:3-jdk-8-slim` - linux; amd64

```console
$ docker pull maven@sha256:c24566d6edd0c8845d07854aa092de3fa0ea2293fd6f1fdb136993cc23dc891a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.7 MB (103691218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63638675a59c7c2bcd753028c1f7371ecf84b76dcdb8fc3b531b87a27aaa4302`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Sat, 28 Apr 2018 07:09:59 GMT
ADD file:ec5be7eec56a749752ca284359ece04f5eb0b981eac08b8855454c6b16e3893c in / 
# Sat, 28 Apr 2018 07:09:59 GMT
CMD ["bash"]
# Wed, 06 Jun 2018 01:54:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Jun 2018 01:54:56 GMT
ENV LANG=C.UTF-8
# Wed, 06 Jun 2018 01:54:57 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Wed, 06 Jun 2018 01:54:58 GMT
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Wed, 06 Jun 2018 01:56:59 GMT
ENV JAVA_HOME=/docker-java-home
# Wed, 06 Jun 2018 01:56:59 GMT
ENV JAVA_VERSION=8u171
# Wed, 06 Jun 2018 01:56:59 GMT
ENV JAVA_DEBIAN_VERSION=8u171-b11-1~deb9u1
# Wed, 06 Jun 2018 01:57:00 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20170531+nmu1
# Wed, 06 Jun 2018 01:57:29 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-8-jdk-headless="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Wed, 06 Jun 2018 01:57:31 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Fri, 22 Jun 2018 17:24:55 GMT
ARG MAVEN_VERSION=3.5.4
# Fri, 22 Jun 2018 17:24:55 GMT
ARG USER_HOME_DIR=/root
# Fri, 22 Jun 2018 17:24:55 GMT
ARG SHA=ce50b1c91364cb77efe3776f756a6d92b76d9038b0a0782f7d53acf1e997a14d
# Fri, 22 Jun 2018 17:24:56 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.4/binaries
# Fri, 22 Jun 2018 17:25:08 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.4/binaries MAVEN_VERSION=3.5.4 SHA=ce50b1c91364cb77efe3776f756a6d92b76d9038b0a0782f7d53acf1e997a14d USER_HOME_DIR=/root
RUN apt-get update &&     apt-get install -y       curl procps   && rm -rf /var/lib/apt/lists/*
# Fri, 22 Jun 2018 17:25:17 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.4/binaries MAVEN_VERSION=3.5.4 SHA=ce50b1c91364cb77efe3776f756a6d92b76d9038b0a0782f7d53acf1e997a14d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha256sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 22 Jun 2018 17:25:17 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 22 Jun 2018 17:25:17 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 22 Jun 2018 17:25:18 GMT
COPY file:fb726a12bbbf8ff54c8d9fceef4fa3018c11a435bfa04ee5f73156c544907861 in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 22 Jun 2018 17:25:18 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Fri, 22 Jun 2018 17:25:18 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 22 Jun 2018 17:25:18 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:f2aa67a397c49232112953088506d02074a1fe577f65dc2052f158a3e5da52e8`  
		Last Modified: Sat, 28 Apr 2018 09:31:20 GMT  
		Size: 22.5 MB (22496029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44ea3e7c4ff00a9a43f29069ca7249f6a31ef8a7365ed89b7f22f8d436ec0a5`  
		Last Modified: Wed, 06 Jun 2018 02:14:43 GMT  
		Size: 454.9 KB (454851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ffd93428115226c4bae15842cfda8645782d5d26ddd3193688abf73a3a7daf9`  
		Last Modified: Wed, 06 Jun 2018 02:14:42 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd00e3c2b114a3541c50a56a3f9391a30b3f2948cf59347f3ce0e416e4e609fb`  
		Last Modified: Wed, 06 Jun 2018 02:14:42 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7381531c4298eb35d6eed2843b277c2f8c9abdc8561ff9546423a96e098f867`  
		Last Modified: Wed, 06 Jun 2018 02:18:22 GMT  
		Size: 67.5 MB (67525282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fcc82e8f1ff7674c86b6b25e9e83c5ba3deca48f1dfc988ad48df9f1d8d41e`  
		Last Modified: Wed, 06 Jun 2018 02:18:00 GMT  
		Size: 272.1 KB (272103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcf81df5f55e3c3cff0f5361b885b768925c7458c564a5e41f303289b1ed09b`  
		Last Modified: Fri, 22 Jun 2018 17:34:16 GMT  
		Size: 4.0 MB (3952248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebbb395697238f8fd1ee5e8b7cdd8d81f9d28272ca758d7eac01af20d9a57bd`  
		Last Modified: Fri, 22 Jun 2018 17:34:16 GMT  
		Size: 9.0 MB (8989210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aea5d7c94afef42e33af46b69dd5ca8801ed3d2527cb6c02706bb2a3c2161f5`  
		Last Modified: Fri, 22 Jun 2018 17:34:15 GMT  
		Size: 752.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585c7a324d45ef3775d1f7c8a9537fb12602c407a4ffced22c46961db562ae80`  
		Last Modified: Fri, 22 Jun 2018 17:34:14 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
