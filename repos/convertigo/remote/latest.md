## `convertigo:latest`

```console
$ docker pull convertigo@sha256:f89e5326e7a7d54e6d1a779086aac5c4d5906d09c5fe39917e43c05780da33ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `convertigo:latest` - linux; amd64

```console
$ docker pull convertigo@sha256:7ac10bff7221a70b333f94b83ced02109d47802b7fc95b4798ca27c0af3e9bee
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318165423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7157e96e680911663ccb2f5b4ae3ee397002167e52c356f3afd25c753a81590f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Sat, 28 Apr 2018 07:08:53 GMT
ADD file:9572fdb59dfbb9b032f3331bbc2a08b31e0aef5fbde44c8f2008d22bf5290cf2 in / 
# Sat, 28 Apr 2018 07:08:53 GMT
CMD ["bash"]
# Fri, 04 May 2018 17:41:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 04 May 2018 17:41:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 04 May 2018 23:51:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 04 May 2018 23:51:32 GMT
ENV LANG=C.UTF-8
# Fri, 04 May 2018 23:51:33 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 04 May 2018 23:51:34 GMT
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Fri, 04 May 2018 23:51:34 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Fri, 04 May 2018 23:51:34 GMT
ENV JAVA_VERSION=8u171
# Fri, 04 May 2018 23:51:34 GMT
ENV JAVA_DEBIAN_VERSION=8u171-b11-1~deb9u1
# Fri, 04 May 2018 23:51:35 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20170531+nmu1
# Mon, 14 May 2018 22:44:43 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-8-jre="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Mon, 14 May 2018 22:44:45 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 15 May 2018 00:00:08 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 15 May 2018 00:00:09 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 May 2018 00:00:10 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 15 May 2018 00:00:10 GMT
WORKDIR /usr/local/tomcat
# Tue, 15 May 2018 00:00:10 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 15 May 2018 00:00:11 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 15 May 2018 00:00:11 GMT
ENV OPENSSL_VERSION=1.1.0f-3+deb9u2
# Tue, 15 May 2018 00:00:12 GMT
RUN set -ex; 	currentVersion="$(dpkg-query --show --showformat '${Version}\n' openssl)"; 	if dpkg --compare-versions "$currentVersion" '<<' "$OPENSSL_VERSION"; then 		if ! grep -q stretch /etc/apt/sources.list; then 			{ 				echo 'deb http://deb.debian.org/debian stretch main'; 				echo 'deb http://security.debian.org stretch/updates main'; 				echo 'deb http://deb.debian.org/debian stretch-updates main'; 			} > /etc/apt/sources.list.d/stretch.list; 			{ 				echo 'Package: *'; 				echo 'Pin: release n=stretch*'; 				echo 'Pin-Priority: -10'; 				echo; 				echo 'Package: openssl libssl*'; 				echo "Pin: version $OPENSSL_VERSION"; 				echo 'Pin-Priority: 990'; 			} > /etc/apt/preferences.d/stretch-openssl; 		fi; 		apt-get update; 		apt-get install -y --no-install-recommends openssl="$OPENSSL_VERSION"; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 May 2018 00:00:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libapr1 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 00:00:28 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 15 May 2018 00:00:28 GMT
ENV TOMCAT_MAJOR=7
# Tue, 15 May 2018 00:00:28 GMT
ENV TOMCAT_VERSION=7.0.88
# Tue, 15 May 2018 00:00:28 GMT
ENV TOMCAT_SHA512=5adb54155f2da0d59c86af9b6df5cce110e608b7f894cd0398821797cf87502bd2938bc8494e021daf1990b337267c391e90e129c907e9a548d23cb52b2a8451
# Tue, 15 May 2018 00:00:29 GMT
ENV TOMCAT_TGZ_URLS=https://www.apache.org/dyn/closer.cgi?action=download&filename=tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz 	https://www-us.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz 	https://www.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz 	https://archive.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz
# Tue, 15 May 2018 00:00:29 GMT
ENV TOMCAT_ASC_URLS=https://www.apache.org/dyn/closer.cgi?action=download&filename=tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz.asc 	https://www-us.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz.asc 	https://www.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz.asc 	https://archive.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz.asc
# Tue, 15 May 2018 00:01:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 		apt-get install -y --no-install-recommends gnupg dirmngr; 		export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 		apt-get install -y --no-install-recommends wget ca-certificates; 		success=; 	for url in $TOMCAT_TGZ_URLS; do 		if wget -O tomcat.tar.gz "$url"; then 			success=1; 			break; 		fi; 	done; 	[ -n "$success" ]; 		echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum -c -; 		success=; 	for url in $TOMCAT_ASC_URLS; do 		if wget -O tomcat.tar.gz.asc "$url"; then 			success=1; 			break; 		fi; 	done; 	[ -n "$success" ]; 		gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xvf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xvf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 		"openjdk-${JAVA_VERSION%%[.~bu-]*}-jdk=$JAVA_DEBIAN_VERSION" 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$(which apr-1-config)" 			--with-java-home="$(docker-java-home)" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +
# Tue, 15 May 2018 00:01:46 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 May 2018 00:01:47 GMT
EXPOSE 8080/tcp
# Tue, 15 May 2018 00:01:47 GMT
CMD ["catalina.sh" "run"]
# Tue, 15 May 2018 03:46:29 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Tue, 15 May 2018 03:46:29 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 15 May 2018 03:46:30 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 15 May 2018 03:46:30 GMT
WORKDIR /usr/local/tomcat
# Tue, 15 May 2018 03:46:34 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     unzip   && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 03:46:34 GMT
ENV GOSU_VERSION=1.10
# Tue, 15 May 2018 03:46:34 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Tue, 15 May 2018 03:46:34 GMT
ENV TINI_VERSION=0.16.1
# Tue, 15 May 2018 03:46:34 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Tue, 15 May 2018 03:46:41 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Tue, 15 May 2018 03:46:42 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace
# Tue, 15 May 2018 03:46:43 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000"/'         conf/server.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Fri, 18 May 2018 18:19:25 GMT
ENV CONVERTIGO_VERSION=7.5.2
# Fri, 18 May 2018 18:19:25 GMT
ENV CONVERTIGO_REVISION=44730
# Fri, 18 May 2018 18:19:25 GMT
ENV CONVERTIGO_WAR_URL=https://devplatform.s3.amazonaws.com/refbin/cems/7.5.2/convertigo-7.5.2-v44730-linux32.war
# Fri, 18 May 2018 18:19:26 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Fri, 18 May 2018 18:19:54 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && chmod a+x WEB-INF/xvnc/*         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Fri, 18 May 2018 18:19:54 GMT
COPY file:03a78619febe6c5b17d175b71a6dbe271ce2c70c52e354c6642b986d1b28fc2e in webapps/ROOT/index.html 
# Fri, 18 May 2018 18:19:55 GMT
COPY file:0a47ea62001ca3cec3ce66ba5a1de976c240bea17f36878bcf94b75e4f0cdf86 in / 
# Fri, 18 May 2018 18:19:55 GMT
ENV SWT_GTK3=0
# Fri, 18 May 2018 18:19:55 GMT
WORKDIR /workspace
# Fri, 18 May 2018 18:19:55 GMT
VOLUME [/workspace]
# Fri, 18 May 2018 18:19:56 GMT
EXPOSE 28080/tcp
# Fri, 18 May 2018 18:19:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 18 May 2018 18:19:56 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:cc1a78bfd46becbfc3abb8a74d9a70a0e0dc7a5809bbd12e814f9382db003707`  
		Last Modified: Sat, 28 Apr 2018 09:27:54 GMT  
		Size: 45.3 MB (45318159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861473222a6f5fb6abe08f0cdebf56b5f42758b0a7430bbbf47a3d365198e5e`  
		Last Modified: Fri, 04 May 2018 18:20:41 GMT  
		Size: 10.8 MB (10773612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0b9c3b5ae080d11df6df788ce96a45b684d7b050fd017c06b4ea5a40f58545`  
		Last Modified: Fri, 04 May 2018 18:20:39 GMT  
		Size: 4.3 MB (4335883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae14ee39877acb45fb6c2157e51ddcd4690ac64ed50b0bbd417eb101518ef81d`  
		Last Modified: Sat, 05 May 2018 00:08:21 GMT  
		Size: 853.1 KB (853090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8085c1b536f02629bdd8a7a1ba474b47b4c842019776b964d5d34e9100a1c07a`  
		Last Modified: Sat, 05 May 2018 00:08:20 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1431e84c0ce069ca47afe14c3caab9012a2c46f70788f1bdf4b2ec5e4a7e63`  
		Last Modified: Sat, 05 May 2018 00:08:20 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0e3df5a1fd8d55deb4e05d5d22c6ebea2ecf9aab66b5d074a020339cf4fc28`  
		Last Modified: Mon, 14 May 2018 23:18:26 GMT  
		Size: 122.1 MB (122140587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cb611ced6ca04659961659e0c74ec16433c5ae37a268283d342196ee6cf5fe`  
		Last Modified: Mon, 14 May 2018 23:17:54 GMT  
		Size: 272.1 KB (272121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268dc3e43e662375abdbff24802f2b48058c6da25963c01574ce8b40d28d6950`  
		Last Modified: Tue, 15 May 2018 00:29:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a7e8d254c73f479737498b150a8f4b2c975d67dbf5c34c703addb145a896b2`  
		Last Modified: Tue, 15 May 2018 00:29:12 GMT  
		Size: 528.7 KB (528711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653b71875aa8e6391682d2ed81f676a2a9347febd6e64d073845474145e59eff`  
		Last Modified: Tue, 15 May 2018 00:29:13 GMT  
		Size: 11.3 MB (11257081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae0c1ee7ea7a9e41c4a5cb4aa68c260bd984ac23535a7f4165764ff2753f29a`  
		Last Modified: Tue, 15 May 2018 00:29:10 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8255f2a3a613cbd064832eb3c6010e0be90450dbffb02743dc7e54bc359e4dc8`  
		Last Modified: Tue, 15 May 2018 03:49:46 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4352889832fe8cfc18165a6dc7d8548b322497b1b053b50ef87bb6021f73b9be`  
		Last Modified: Tue, 15 May 2018 03:49:47 GMT  
		Size: 509.3 KB (509295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2507a1326b254df0ff23c29412d27760a188eb0aaabc92c8e2ac9f82a56068`  
		Last Modified: Tue, 15 May 2018 03:49:43 GMT  
		Size: 4.3 KB (4262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aec01770264d92976d879835a2607b56dfad8f940c7193172a105f4d82c7500`  
		Last Modified: Tue, 15 May 2018 03:49:44 GMT  
		Size: 25.9 KB (25930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ffa7e506b9b59f36957bc7b00257419c5be7fc2e328b89cf71de49b459c233`  
		Last Modified: Fri, 18 May 2018 18:20:55 GMT  
		Size: 122.1 MB (122144163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a095d8c2d70e4a236d7d149864ec0ca873ff24282aee648569ee4a42d050939d`  
		Last Modified: Fri, 18 May 2018 18:20:47 GMT  
		Size: 466.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d64403392b9039ed66f87948266e7d6ce0b99a0f57a921713d39df10d40b7d`  
		Last Modified: Fri, 18 May 2018 18:20:47 GMT  
		Size: 1.1 KB (1072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `convertigo:latest` - linux; arm variant v7

```console
$ docker pull convertigo@sha256:25804f94453324477e9bf395aee5b8c91940b6b020ee373e0c6cbd35a78f9769
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.4 MB (330424320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e66c9fe3988fc7fe51ec6029275a88260ee0da6edeeacbf3b75b91bbf9342bd1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Sat, 28 Apr 2018 12:04:18 GMT
ADD file:c7fba27b02c4bda63faef7eb30156a55feb4c0e9ecd529a24dd8d62942c2f83c in / 
# Sat, 28 Apr 2018 12:04:19 GMT
CMD ["bash"]
# Sat, 05 May 2018 12:13:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 05 May 2018 12:13:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 05 May 2018 12:59:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 05 May 2018 12:59:16 GMT
ENV LANG=C.UTF-8
# Sat, 05 May 2018 12:59:17 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 05 May 2018 12:59:18 GMT
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 05 May 2018 12:59:18 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Sat, 05 May 2018 12:59:19 GMT
ENV JAVA_VERSION=8u171
# Sat, 05 May 2018 12:59:27 GMT
ENV JAVA_DEBIAN_VERSION=8u171-b11-1~deb9u1
# Sat, 05 May 2018 12:59:27 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20170531+nmu1
# Sat, 05 May 2018 13:00:26 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-8-jre="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Sat, 05 May 2018 13:00:28 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Sat, 05 May 2018 15:54:31 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 May 2018 15:54:31 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 May 2018 15:54:32 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 May 2018 15:54:33 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 May 2018 15:54:33 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 May 2018 15:54:34 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 May 2018 15:54:34 GMT
ENV OPENSSL_VERSION=1.1.0f-3+deb9u2
# Sat, 05 May 2018 15:54:35 GMT
RUN set -ex; 	currentVersion="$(dpkg-query --show --showformat '${Version}\n' openssl)"; 	if dpkg --compare-versions "$currentVersion" '<<' "$OPENSSL_VERSION"; then 		if ! grep -q stretch /etc/apt/sources.list; then 			{ 				echo 'deb http://deb.debian.org/debian stretch main'; 				echo 'deb http://security.debian.org stretch/updates main'; 				echo 'deb http://deb.debian.org/debian stretch-updates main'; 			} > /etc/apt/sources.list.d/stretch.list; 			{ 				echo 'Package: *'; 				echo 'Pin: release n=stretch*'; 				echo 'Pin-Priority: -10'; 				echo; 				echo 'Package: openssl libssl*'; 				echo "Pin: version $OPENSSL_VERSION"; 				echo 'Pin-Priority: 990'; 			} > /etc/apt/preferences.d/stretch-openssl; 		fi; 		apt-get update; 		apt-get install -y --no-install-recommends openssl="$OPENSSL_VERSION"; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 05 May 2018 15:54:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libapr1 	&& rm -rf /var/lib/apt/lists/*
# Sat, 05 May 2018 15:54:48 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 05 May 2018 15:54:48 GMT
ENV TOMCAT_MAJOR=7
# Tue, 15 May 2018 13:02:30 GMT
ENV TOMCAT_VERSION=7.0.88
# Tue, 15 May 2018 13:02:30 GMT
ENV TOMCAT_SHA512=5adb54155f2da0d59c86af9b6df5cce110e608b7f894cd0398821797cf87502bd2938bc8494e021daf1990b337267c391e90e129c907e9a548d23cb52b2a8451
# Tue, 15 May 2018 13:02:31 GMT
ENV TOMCAT_TGZ_URLS=https://www.apache.org/dyn/closer.cgi?action=download&filename=tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz 	https://www-us.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz 	https://www.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz 	https://archive.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz
# Tue, 15 May 2018 13:02:40 GMT
ENV TOMCAT_ASC_URLS=https://www.apache.org/dyn/closer.cgi?action=download&filename=tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz.asc 	https://www-us.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz.asc 	https://www.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz.asc 	https://archive.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz.asc
# Tue, 15 May 2018 13:03:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 		apt-get install -y --no-install-recommends gnupg dirmngr; 		export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 		apt-get install -y --no-install-recommends wget ca-certificates; 		success=; 	for url in $TOMCAT_TGZ_URLS; do 		if wget -O tomcat.tar.gz "$url"; then 			success=1; 			break; 		fi; 	done; 	[ -n "$success" ]; 		echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum -c -; 		success=; 	for url in $TOMCAT_ASC_URLS; do 		if wget -O tomcat.tar.gz.asc "$url"; then 			success=1; 			break; 		fi; 	done; 	[ -n "$success" ]; 		gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xvf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xvf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 		"openjdk-${JAVA_VERSION%%[.~bu-]*}-jdk=$JAVA_DEBIAN_VERSION" 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$(which apr-1-config)" 			--with-java-home="$(docker-java-home)" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +
# Tue, 15 May 2018 13:03:18 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 May 2018 13:03:18 GMT
EXPOSE 8080/tcp
# Tue, 15 May 2018 13:03:19 GMT
CMD ["catalina.sh" "run"]
# Tue, 15 May 2018 13:59:09 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Tue, 15 May 2018 13:59:10 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 15 May 2018 13:59:11 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 15 May 2018 13:59:11 GMT
WORKDIR /usr/local/tomcat
# Tue, 15 May 2018 13:59:16 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     unzip   && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 13:59:21 GMT
ENV GOSU_VERSION=1.10
# Tue, 15 May 2018 13:59:21 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Tue, 15 May 2018 13:59:22 GMT
ENV TINI_VERSION=0.16.1
# Tue, 15 May 2018 13:59:22 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Tue, 15 May 2018 13:59:36 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Tue, 15 May 2018 13:59:45 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace
# Tue, 15 May 2018 13:59:46 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000"/'         conf/server.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Sat, 19 May 2018 11:58:07 GMT
ENV CONVERTIGO_VERSION=7.5.2
# Sat, 19 May 2018 11:58:08 GMT
ENV CONVERTIGO_REVISION=44730
# Sat, 19 May 2018 11:58:08 GMT
ENV CONVERTIGO_WAR_URL=https://devplatform.s3.amazonaws.com/refbin/cems/7.5.2/convertigo-7.5.2-v44730-linux32.war
# Sat, 19 May 2018 11:58:18 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Sat, 19 May 2018 11:58:34 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && chmod a+x WEB-INF/xvnc/*         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Sat, 19 May 2018 11:58:44 GMT
COPY file:03a78619febe6c5b17d175b71a6dbe271ce2c70c52e354c6642b986d1b28fc2e in webapps/ROOT/index.html 
# Sat, 19 May 2018 11:58:44 GMT
COPY file:0a47ea62001ca3cec3ce66ba5a1de976c240bea17f36878bcf94b75e4f0cdf86 in / 
# Sat, 19 May 2018 11:58:45 GMT
ENV SWT_GTK3=0
# Sat, 19 May 2018 11:58:45 GMT
WORKDIR /workspace
# Sat, 19 May 2018 11:58:46 GMT
VOLUME [/workspace]
# Sat, 19 May 2018 11:58:46 GMT
EXPOSE 28080/tcp
# Sat, 19 May 2018 11:58:47 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 19 May 2018 11:58:47 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:5483105d09166836731e940c850827dd1a4fe16b04d1921eea4d8da7c98e99bc`  
		Last Modified: Sat, 28 Apr 2018 12:15:18 GMT  
		Size: 42.1 MB (42063737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed57f83cc7c78757972312a1b5a30524f861523c5390d062845f18c696f48ea`  
		Last Modified: Sat, 05 May 2018 12:35:37 GMT  
		Size: 9.5 MB (9472475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859203aede279201e8caf07cf2963456c56bac72a64071079dc9db6fb65ed1a2`  
		Last Modified: Sat, 05 May 2018 12:35:34 GMT  
		Size: 3.9 MB (3912835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df26ddf71ea9e82f175e400809b8f06871dd0937c5a90f4ffe95286544a9f719`  
		Last Modified: Sat, 05 May 2018 13:29:05 GMT  
		Size: 830.3 KB (830332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c21322a9c89724512d6ea5faa10299c60c8a605d6f563c84c28177db8d2770`  
		Last Modified: Sat, 05 May 2018 13:29:05 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2270f04a4be61f52577232813fff92e797d3fc190d52f71411afc26b0911f8e4`  
		Last Modified: Sat, 05 May 2018 13:29:04 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2dc1aba58c8cd285639cac6b03c823e5fcdb91aa8922652e7d9387aaca6fa4`  
		Last Modified: Sat, 05 May 2018 13:29:37 GMT  
		Size: 139.5 MB (139501760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02869ec2bb3864b06abd435610eb6849d5c62426517de1a603ef6fe43c7d3815`  
		Last Modified: Sat, 05 May 2018 13:29:05 GMT  
		Size: 272.1 KB (272082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289a355206a5e4f55a89ee04aff3ea7521228ac5dd89e2068978f78acbbd0a54`  
		Last Modified: Sat, 05 May 2018 16:08:23 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf947ee846151b3e82b979ab8f3027c037e1a8dc7a1c2976128213dcb515eced`  
		Last Modified: Sat, 05 May 2018 16:08:24 GMT  
		Size: 519.8 KB (519803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1f00448e99e4b6411164a93c0f97ab144d73536d7df1b89859f327519c275f`  
		Last Modified: Tue, 15 May 2018 13:26:49 GMT  
		Size: 11.2 MB (11191681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f86e7063b07c27175d075526026d1dcba7bf5351953bc2518cff3789b030995`  
		Last Modified: Tue, 15 May 2018 13:26:45 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f7d541c898318e3a17ff746571fe3cd60942c284c03acb7e2648f34379bcd6`  
		Last Modified: Tue, 15 May 2018 14:03:19 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84851132115e3cc1956288c0ff2c19362f7b3796dd9117d4e078d50dc656f923`  
		Last Modified: Tue, 15 May 2018 14:03:18 GMT  
		Size: 482.7 KB (482666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b00412f18c8e4ced6d0b71151978972f252845e8d7d1b3908c47423c8224c9`  
		Last Modified: Tue, 15 May 2018 14:03:17 GMT  
		Size: 4.3 KB (4347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976e1d180ee93cd913f2fdd8194f711efeb751330a9798f78f78fb5a45b5eb37`  
		Last Modified: Tue, 15 May 2018 14:03:17 GMT  
		Size: 25.9 KB (25929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efde0f54879b21ecb389b3224e3b51f9518b8543d0637b1bf39d5f3dc5a2edea`  
		Last Modified: Sat, 19 May 2018 11:59:39 GMT  
		Size: 122.1 MB (122144110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b27d9acbd132e3cff155445eb0ccdd1321f8336602a803a88f13142346a2cb9`  
		Last Modified: Sat, 19 May 2018 11:59:22 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a25397dd01b09f3e0ef0335928b3732b7454bff2cc9c4a73ed418ebb03146a`  
		Last Modified: Sat, 19 May 2018 11:59:22 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `convertigo:latest` - linux; arm64 variant v8

```console
$ docker pull convertigo@sha256:fb6250abdfafd9604e0278a88565aa40d64fa051ddd8d32e85e1094dab503ff6
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.2 MB (305192863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb0ba78b5abb0fc757860433cd239fab35acb6d136bf139ed09d3eb0d524f7f0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Mon, 30 Apr 2018 23:31:58 GMT
ADD file:245a8cfe59ea071e4e215a722e0d4b4b14fa95dd6ffd03739fe048433cfaf523 in / 
# Mon, 30 Apr 2018 23:32:00 GMT
CMD ["bash"]
# Sat, 05 May 2018 09:38:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 05 May 2018 09:39:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 05 May 2018 12:03:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Sat, 05 May 2018 12:03:34 GMT
ENV LANG=C.UTF-8
# Sat, 05 May 2018 12:03:38 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Sat, 05 May 2018 12:03:42 GMT
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Sat, 05 May 2018 12:03:43 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Sat, 05 May 2018 12:03:45 GMT
ENV JAVA_VERSION=8u171
# Sat, 05 May 2018 12:03:46 GMT
ENV JAVA_DEBIAN_VERSION=8u171-b11-1~deb9u1
# Sat, 05 May 2018 12:03:47 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20170531+nmu1
# Tue, 15 May 2018 09:57:07 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-8-jre="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Tue, 15 May 2018 09:57:13 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Tue, 15 May 2018 11:40:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 15 May 2018 11:40:59 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 May 2018 11:41:04 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 15 May 2018 11:41:05 GMT
WORKDIR /usr/local/tomcat
# Tue, 15 May 2018 11:41:06 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 15 May 2018 11:41:07 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 15 May 2018 11:41:08 GMT
ENV OPENSSL_VERSION=1.1.0f-3+deb9u2
# Tue, 15 May 2018 11:41:11 GMT
RUN set -ex; 	currentVersion="$(dpkg-query --show --showformat '${Version}\n' openssl)"; 	if dpkg --compare-versions "$currentVersion" '<<' "$OPENSSL_VERSION"; then 		if ! grep -q stretch /etc/apt/sources.list; then 			{ 				echo 'deb http://deb.debian.org/debian stretch main'; 				echo 'deb http://security.debian.org stretch/updates main'; 				echo 'deb http://deb.debian.org/debian stretch-updates main'; 			} > /etc/apt/sources.list.d/stretch.list; 			{ 				echo 'Package: *'; 				echo 'Pin: release n=stretch*'; 				echo 'Pin-Priority: -10'; 				echo; 				echo 'Package: openssl libssl*'; 				echo "Pin: version $OPENSSL_VERSION"; 				echo 'Pin-Priority: 990'; 			} > /etc/apt/preferences.d/stretch-openssl; 		fi; 		apt-get update; 		apt-get install -y --no-install-recommends openssl="$OPENSSL_VERSION"; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 May 2018 11:41:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libapr1 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 11:41:32 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 15 May 2018 11:41:33 GMT
ENV TOMCAT_MAJOR=7
# Tue, 15 May 2018 11:41:34 GMT
ENV TOMCAT_VERSION=7.0.88
# Tue, 15 May 2018 11:41:35 GMT
ENV TOMCAT_SHA512=5adb54155f2da0d59c86af9b6df5cce110e608b7f894cd0398821797cf87502bd2938bc8494e021daf1990b337267c391e90e129c907e9a548d23cb52b2a8451
# Tue, 15 May 2018 11:41:35 GMT
ENV TOMCAT_TGZ_URLS=https://www.apache.org/dyn/closer.cgi?action=download&filename=tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz 	https://www-us.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz 	https://www.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz 	https://archive.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz
# Tue, 15 May 2018 11:41:36 GMT
ENV TOMCAT_ASC_URLS=https://www.apache.org/dyn/closer.cgi?action=download&filename=tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz.asc 	https://www-us.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz.asc 	https://www.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz.asc 	https://archive.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz.asc
# Tue, 15 May 2018 11:43:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 		apt-get install -y --no-install-recommends gnupg dirmngr; 		export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 		apt-get install -y --no-install-recommends wget ca-certificates; 		success=; 	for url in $TOMCAT_TGZ_URLS; do 		if wget -O tomcat.tar.gz "$url"; then 			success=1; 			break; 		fi; 	done; 	[ -n "$success" ]; 		echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum -c -; 		success=; 	for url in $TOMCAT_ASC_URLS; do 		if wget -O tomcat.tar.gz.asc "$url"; then 			success=1; 			break; 		fi; 	done; 	[ -n "$success" ]; 		gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xvf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xvf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 		"openjdk-${JAVA_VERSION%%[.~bu-]*}-jdk=$JAVA_DEBIAN_VERSION" 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$(which apr-1-config)" 			--with-java-home="$(docker-java-home)" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +
# Tue, 15 May 2018 11:43:57 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 May 2018 11:43:57 GMT
EXPOSE 8080/tcp
# Tue, 15 May 2018 11:43:58 GMT
CMD ["catalina.sh" "run"]
# Tue, 15 May 2018 14:27:52 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Tue, 15 May 2018 14:27:52 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 15 May 2018 14:27:55 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 15 May 2018 14:27:55 GMT
WORKDIR /usr/local/tomcat
# Tue, 15 May 2018 14:28:03 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     unzip   && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 14:28:04 GMT
ENV GOSU_VERSION=1.10
# Tue, 15 May 2018 14:28:04 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Tue, 15 May 2018 14:28:05 GMT
ENV TINI_VERSION=0.16.1
# Tue, 15 May 2018 14:28:06 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Tue, 15 May 2018 14:28:14 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Tue, 15 May 2018 14:28:18 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace
# Tue, 15 May 2018 14:28:20 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000"/'         conf/server.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Sat, 19 May 2018 08:39:31 GMT
ENV CONVERTIGO_VERSION=7.5.2
# Sat, 19 May 2018 08:39:31 GMT
ENV CONVERTIGO_REVISION=44730
# Sat, 19 May 2018 08:39:32 GMT
ENV CONVERTIGO_WAR_URL=https://devplatform.s3.amazonaws.com/refbin/cems/7.5.2/convertigo-7.5.2-v44730-linux32.war
# Sat, 19 May 2018 08:39:39 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Sat, 19 May 2018 08:40:27 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && chmod a+x WEB-INF/xvnc/*         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Sat, 19 May 2018 08:40:28 GMT
COPY file:03a78619febe6c5b17d175b71a6dbe271ce2c70c52e354c6642b986d1b28fc2e in webapps/ROOT/index.html 
# Sat, 19 May 2018 08:40:29 GMT
COPY file:0a47ea62001ca3cec3ce66ba5a1de976c240bea17f36878bcf94b75e4f0cdf86 in / 
# Sat, 19 May 2018 08:40:30 GMT
ENV SWT_GTK3=0
# Sat, 19 May 2018 08:40:31 GMT
WORKDIR /workspace
# Sat, 19 May 2018 08:40:32 GMT
VOLUME [/workspace]
# Sat, 19 May 2018 08:40:33 GMT
EXPOSE 28080/tcp
# Sat, 19 May 2018 08:40:34 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 19 May 2018 08:40:35 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:142bf25d8d1b3ebc9dfbedd586e70a011594690acf48b2695bfce01e3a2cf0d5`  
		Last Modified: Mon, 30 Apr 2018 23:52:13 GMT  
		Size: 43.1 MB (43109349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd3e9bbb1f760ff8cab41817920c5822422ba1eaab36a233c8f43348791e03d`  
		Last Modified: Sat, 05 May 2018 10:29:53 GMT  
		Size: 9.7 MB (9722189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5534647756e8399143ad6e1639b6433b9a3364809ac4520f62199ea46e638a2e`  
		Last Modified: Sat, 05 May 2018 10:29:50 GMT  
		Size: 4.1 MB (4088086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabf35448f16b9e3326e8f780f01877aba13f9ec6815f975d4da42043dbf329`  
		Last Modified: Sat, 05 May 2018 13:00:53 GMT  
		Size: 839.3 KB (839299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0802d24798c77025ece2adb6489409aa0f5789f4e82aa4242a0d9d622696157a`  
		Last Modified: Sat, 05 May 2018 13:00:52 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ab48d1ba995a67328f25f0660cdf40027abdd6587d59727f7ba0f72c4beb4b`  
		Last Modified: Sat, 05 May 2018 13:00:53 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c450eedb74d167d4e5fc41e7d53a2b506218189e9184552476d6a66b9cad348`  
		Last Modified: Tue, 15 May 2018 11:02:00 GMT  
		Size: 112.7 MB (112745447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f571a7544609d6069b1a1275b0c87cd79aace6c30f4537b8860f62b95d6a06`  
		Last Modified: Tue, 15 May 2018 11:01:25 GMT  
		Size: 272.1 KB (272102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2beff2a79a5503fa863be2e8659f1e37156c79c42e0368e600e0d1b3135abf9`  
		Last Modified: Tue, 15 May 2018 13:48:14 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb465c04a842556b30ca8b689e08bff0b01e48d07401f7cb3f3def5b7f0503c`  
		Last Modified: Tue, 15 May 2018 13:48:15 GMT  
		Size: 513.3 KB (513304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49789bfae698830dbf32a2e5b23a83ea975402ff87d44307a13355f44649095d`  
		Last Modified: Tue, 15 May 2018 13:48:17 GMT  
		Size: 11.2 MB (11249368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62a7c100e8c90f7292a7a07c3cc875da3dbdb0e83a1b73a0d562ba9e04f97ec`  
		Last Modified: Tue, 15 May 2018 13:48:14 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4c42a1ea0153125457666c22eb608bffa9dab6028492d252fc940c8b8f7232`  
		Last Modified: Tue, 15 May 2018 14:33:48 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5952dc6b25c32b0fe27e2fcbcf6b8ef2fdeab06524a497ed35071c2b670fef`  
		Last Modified: Tue, 15 May 2018 14:33:50 GMT  
		Size: 476.8 KB (476841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cd369e6a458115afa5389a3a4ef79cebf3a793494a6b85bc8f03eee2825e3a`  
		Last Modified: Tue, 15 May 2018 14:33:46 GMT  
		Size: 4.3 KB (4269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36130c6a51d2fce4327b0abf2281b12ed47457381292b5af88176fa795853684`  
		Last Modified: Tue, 15 May 2018 14:33:46 GMT  
		Size: 25.9 KB (25928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa6001a76307a9dd43b6dda1a1908e348a99c16fe2c8f4dc40f995dfefb3af4`  
		Last Modified: Sat, 19 May 2018 08:43:07 GMT  
		Size: 122.1 MB (122144147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae9f48fdda3ef7d98ca05cecd67f00f5a0ec1e356c9aebadfaf6e40c618fb67`  
		Last Modified: Sat, 19 May 2018 08:42:47 GMT  
		Size: 466.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e2a53462581b4d597b103c3d78ac1308886d45779cab314f47ee3ec703f24c`  
		Last Modified: Sat, 19 May 2018 08:42:47 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `convertigo:latest` - linux; 386

```console
$ docker pull convertigo@sha256:8a622abdd094ab098138e12715a15d9f011131c3bafa139d6164201de23f325a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.6 MB (334566972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:714a252733ae64a1d9e8985cf902e1fd728f054412727973e9bd82c4cbfcf2cf`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Sat, 28 Apr 2018 10:41:35 GMT
ADD file:df99f919c7f5a407abee5c74ea019e497e559a75bdd21b36ae581e81230884c3 in / 
# Sat, 28 Apr 2018 10:41:36 GMT
CMD ["bash"]
# Sat, 05 May 2018 11:06:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 05 May 2018 11:06:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 31 May 2018 06:00:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 31 May 2018 06:00:19 GMT
ENV LANG=C.UTF-8
# Thu, 31 May 2018 06:00:19 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Thu, 31 May 2018 06:00:20 GMT
RUN ln -svT "/usr/lib/jvm/java-8-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Thu, 31 May 2018 06:00:20 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Thu, 31 May 2018 06:00:20 GMT
ENV JAVA_VERSION=8u171
# Thu, 31 May 2018 06:00:20 GMT
ENV JAVA_DEBIAN_VERSION=8u171-b11-1~deb9u1
# Thu, 31 May 2018 06:00:21 GMT
ENV CA_CERTIFICATES_JAVA_VERSION=20170531+nmu1
# Thu, 31 May 2018 06:01:42 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y --no-install-recommends 		openjdk-8-jre="$JAVA_DEBIAN_VERSION" 		ca-certificates-java="$CA_CERTIFICATES_JAVA_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Thu, 31 May 2018 06:01:44 GMT
RUN /var/lib/dpkg/info/ca-certificates-java.postinst configure
# Thu, 31 May 2018 12:34:20 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 31 May 2018 12:34:20 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 May 2018 12:34:21 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 31 May 2018 12:34:21 GMT
WORKDIR /usr/local/tomcat
# Thu, 31 May 2018 12:34:21 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 31 May 2018 12:34:21 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 31 May 2018 12:34:22 GMT
ENV OPENSSL_VERSION=1.1.0f-3+deb9u2
# Thu, 31 May 2018 12:34:22 GMT
RUN set -ex; 	currentVersion="$(dpkg-query --show --showformat '${Version}\n' openssl)"; 	if dpkg --compare-versions "$currentVersion" '<<' "$OPENSSL_VERSION"; then 		if ! grep -q stretch /etc/apt/sources.list; then 			{ 				echo 'deb http://deb.debian.org/debian stretch main'; 				echo 'deb http://security.debian.org stretch/updates main'; 				echo 'deb http://deb.debian.org/debian stretch-updates main'; 			} > /etc/apt/sources.list.d/stretch.list; 			{ 				echo 'Package: *'; 				echo 'Pin: release n=stretch*'; 				echo 'Pin-Priority: -10'; 				echo; 				echo 'Package: openssl libssl*'; 				echo "Pin: version $OPENSSL_VERSION"; 				echo 'Pin-Priority: 990'; 			} > /etc/apt/preferences.d/stretch-openssl; 		fi; 		apt-get update; 		apt-get install -y --no-install-recommends openssl="$OPENSSL_VERSION"; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 31 May 2018 12:34:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libapr1 	&& rm -rf /var/lib/apt/lists/*
# Thu, 31 May 2018 12:34:29 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 31 May 2018 12:34:29 GMT
ENV TOMCAT_MAJOR=7
# Thu, 31 May 2018 12:34:29 GMT
ENV TOMCAT_VERSION=7.0.88
# Thu, 31 May 2018 12:34:30 GMT
ENV TOMCAT_SHA512=5adb54155f2da0d59c86af9b6df5cce110e608b7f894cd0398821797cf87502bd2938bc8494e021daf1990b337267c391e90e129c907e9a548d23cb52b2a8451
# Thu, 31 May 2018 12:34:30 GMT
ENV TOMCAT_TGZ_URLS=https://www.apache.org/dyn/closer.cgi?action=download&filename=tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz 	https://www-us.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz 	https://www.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz 	https://archive.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz
# Thu, 31 May 2018 12:34:30 GMT
ENV TOMCAT_ASC_URLS=https://www.apache.org/dyn/closer.cgi?action=download&filename=tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz.asc 	https://www-us.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz.asc 	https://www.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz.asc 	https://archive.apache.org/dist/tomcat/tomcat-7/v7.0.88/bin/apache-tomcat-7.0.88.tar.gz.asc
# Thu, 31 May 2018 12:35:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 		apt-get install -y --no-install-recommends gnupg dirmngr; 		export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 		apt-get install -y --no-install-recommends wget ca-certificates; 		success=; 	for url in $TOMCAT_TGZ_URLS; do 		if wget -O tomcat.tar.gz "$url"; then 			success=1; 			break; 		fi; 	done; 	[ -n "$success" ]; 		echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum -c -; 		success=; 	for url in $TOMCAT_ASC_URLS; do 		if wget -O tomcat.tar.gz.asc "$url"; then 			success=1; 			break; 		fi; 	done; 	[ -n "$success" ]; 		gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xvf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xvf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 		"openjdk-${JAVA_VERSION%%[.~bu-]*}-jdk=$JAVA_DEBIAN_VERSION" 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$(which apr-1-config)" 			--with-java-home="$(docker-java-home)" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +
# Thu, 31 May 2018 12:35:28 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 31 May 2018 12:35:29 GMT
EXPOSE 8080/tcp
# Thu, 31 May 2018 12:35:29 GMT
CMD ["catalina.sh" "run"]
# Thu, 31 May 2018 15:52:58 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Thu, 31 May 2018 15:52:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 31 May 2018 15:52:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 31 May 2018 15:52:59 GMT
WORKDIR /usr/local/tomcat
# Thu, 31 May 2018 15:53:07 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     unzip   && rm -rf /var/lib/apt/lists/*
# Thu, 31 May 2018 15:53:07 GMT
ENV GOSU_VERSION=1.10
# Thu, 31 May 2018 15:53:07 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Thu, 31 May 2018 15:53:07 GMT
ENV TINI_VERSION=0.16.1
# Thu, 31 May 2018 15:53:07 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Thu, 31 May 2018 15:53:17 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Thu, 31 May 2018 15:53:18 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace
# Thu, 31 May 2018 15:53:18 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000"/'         conf/server.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Thu, 31 May 2018 15:53:19 GMT
ENV CONVERTIGO_VERSION=7.5.2
# Thu, 31 May 2018 15:53:19 GMT
ENV CONVERTIGO_REVISION=44730
# Thu, 31 May 2018 15:53:19 GMT
ENV CONVERTIGO_WAR_URL=https://devplatform.s3.amazonaws.com/refbin/cems/7.5.2/convertigo-7.5.2-v44730-linux32.war
# Thu, 31 May 2018 15:53:19 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Thu, 31 May 2018 16:06:00 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && chmod a+x WEB-INF/xvnc/*         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Thu, 31 May 2018 16:06:01 GMT
COPY file:03a78619febe6c5b17d175b71a6dbe271ce2c70c52e354c6642b986d1b28fc2e in webapps/ROOT/index.html 
# Thu, 31 May 2018 16:06:01 GMT
COPY file:0a47ea62001ca3cec3ce66ba5a1de976c240bea17f36878bcf94b75e4f0cdf86 in / 
# Thu, 31 May 2018 16:06:01 GMT
ENV SWT_GTK3=0
# Thu, 31 May 2018 16:06:01 GMT
WORKDIR /workspace
# Thu, 31 May 2018 16:06:02 GMT
VOLUME [/workspace]
# Thu, 31 May 2018 16:06:02 GMT
EXPOSE 28080/tcp
# Thu, 31 May 2018 16:06:02 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 31 May 2018 16:06:02 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:5b858ae16eb844c6834e74a5c76644142d36957121de3f9bccf66d4c10b18816`  
		Last Modified: Sat, 28 Apr 2018 10:48:56 GMT  
		Size: 46.0 MB (46044885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25af6543ea0fe065b8b039ef338aa11ccccc8921a78894d40c0594a1821e8c89`  
		Last Modified: Sat, 05 May 2018 11:40:01 GMT  
		Size: 10.8 MB (10783664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84eefdd216b0b19250871d762b9dd06baa7cb1a1a4094f165e32161cc7269754`  
		Last Modified: Sat, 05 May 2018 11:39:59 GMT  
		Size: 4.6 MB (4555015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d10acf93fb4090a69fda86b6a3dc3cd3552cc833909a17b891e6ca821a68e4b`  
		Last Modified: Thu, 31 May 2018 06:39:06 GMT  
		Size: 862.0 KB (861956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9ece753f4d8bde247346f65ee1b72b347fa6416bb007e968c16b092aac315a`  
		Last Modified: Thu, 31 May 2018 06:39:05 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d201bcc9a375c2e12f15912782fe0e8c176c4d4c586a7b1235fa9cf3208468`  
		Last Modified: Thu, 31 May 2018 06:39:05 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7612845683c3cf806d2deb77598d26bb793e3f83b90334dc62aca1b5a629b70`  
		Last Modified: Thu, 31 May 2018 06:39:48 GMT  
		Size: 122.6 MB (122580084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8056aecb21d5dd5e26d74316964617f2e3a92461accd1d5d0b651763ed31acfc`  
		Last Modified: Thu, 31 May 2018 06:39:05 GMT  
		Size: 272.1 KB (272120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd12896519229c1b0ea0cc0a94d85c4f255bd417890d58b26f7e6345d3d7595`  
		Last Modified: Thu, 31 May 2018 13:16:09 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35aece1f785759cb24629541a1d6d66ef24ee6ff372f4bb2f22e1938ed9fd281`  
		Last Modified: Thu, 31 May 2018 13:16:09 GMT  
		Size: 540.6 KB (540589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00272862fbabcf700083cc2b28345d642fa1ccdfb945799031a089dd09738748`  
		Last Modified: Thu, 31 May 2018 13:16:12 GMT  
		Size: 11.2 MB (11170022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0742c661766b337f95e9f7cfeff578b286588cc21dd4bc815c1c650c1f34236`  
		Last Modified: Thu, 31 May 2018 13:16:08 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5671353d731112221437cecd6c0bc175b07f6ec218c8927bcc7afbb26195605`  
		Last Modified: Thu, 31 May 2018 16:25:41 GMT  
		Size: 1.0 MB (1028877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d2639d9155b683c42516e51ab3b8f33e59dc38d38dea2845aa07aeb232f102`  
		Last Modified: Thu, 31 May 2018 16:25:41 GMT  
		Size: 489.2 KB (489166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c114343396948a6a96711646b5ddecaa62fcad8e634f98bf712f38bc5387449c`  
		Last Modified: Thu, 31 May 2018 16:25:36 GMT  
		Size: 4.2 KB (4250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048e26949ee66c2b9157581dcbc302896b97bdac58b1b4fdb58a1de5da6563ce`  
		Last Modified: Thu, 31 May 2018 16:25:37 GMT  
		Size: 25.9 KB (25937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ee292962e505382df33e9ccaf1c4dac5621904fb49f230cc348f6040dbb73`  
		Last Modified: Thu, 31 May 2018 16:26:53 GMT  
		Size: 136.2 MB (136208206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4076f0353600c8658c191d4b9eb8a42afef73fb0da92405f8ed5c7280742029e`  
		Last Modified: Thu, 31 May 2018 16:25:36 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90235f7bb5d63ef59f709f8a5a3465178a56c0ed8b22b89971864742ea0298e9`  
		Last Modified: Thu, 31 May 2018 16:25:36 GMT  
		Size: 1.1 KB (1070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
