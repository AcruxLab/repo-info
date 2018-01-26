<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mongo`

-	[`mongo:3`](#mongo3)
-	[`mongo:3.0`](#mongo30)
-	[`mongo:3.0.15`](#mongo3015)
-	[`mongo:3.0.15-wheezy`](#mongo3015-wheezy)
-	[`mongo:3.0-wheezy`](#mongo30-wheezy)
-	[`mongo:3.2`](#mongo32)
-	[`mongo:3.2.18`](#mongo3218)
-	[`mongo:3.2.18-jessie`](#mongo3218-jessie)
-	[`mongo:3.2-jessie`](#mongo32-jessie)
-	[`mongo:3.4`](#mongo34)
-	[`mongo:3.4.10`](#mongo3410)
-	[`mongo:3.4.10-jessie`](#mongo3410-jessie)
-	[`mongo:3.4-jessie`](#mongo34-jessie)
-	[`mongo:3.6`](#mongo36)
-	[`mongo:3.6.2`](#mongo362)
-	[`mongo:3.6.2-jessie`](#mongo362-jessie)
-	[`mongo:3.6-jessie`](#mongo36-jessie)
-	[`mongo:3.7`](#mongo37)
-	[`mongo:3.7.1`](#mongo371)
-	[`mongo:3.7.1-jessie`](#mongo371-jessie)
-	[`mongo:3.7-jessie`](#mongo37-jessie)
-	[`mongo:3-jessie`](#mongo3-jessie)
-	[`mongo:jessie`](#mongojessie)
-	[`mongo:latest`](#mongolatest)
-	[`mongo:unstable`](#mongounstable)
-	[`mongo:unstable-jessie`](#mongounstable-jessie)

## `mongo:3`

```console
$ docker pull mongo@sha256:878b76e5834f37da98096296f4147f6ca4d94b1a9187986e9d6e59756e7ce865
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3` - linux; amd64

```console
$ docker pull mongo@sha256:8bb68343e860575cfe3e82c98f5f5baad3ab8a67f54062d3476f2276b576abb4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130406419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f57644645eb53a3d2256f460ade116ad3590252c28f63e5136c026423dc8286`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:21:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Dec 2017 01:21:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:21:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:21:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_MAJOR=3.6
# Mon, 15 Jan 2018 23:15:02 GMT
ENV MONGO_VERSION=3.6.2
# Mon, 15 Jan 2018 23:15:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 15 Jan 2018 23:15:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 15 Jan 2018 23:15:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 15 Jan 2018 23:15:25 GMT
VOLUME [/data/db /data/configdb]
# Mon, 15 Jan 2018 23:15:25 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Mon, 15 Jan 2018 23:15:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Jan 2018 23:15:26 GMT
EXPOSE 27017/tcp
# Mon, 15 Jan 2018 23:15:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6c28c0235b619029c8b8c9d512f97756a986bfa458e64b5aa45784af894ac3`  
		Last Modified: Thu, 21 Dec 2017 01:24:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6688308f715efc799218462de2504d5ea35be542dfc7bb1dbcbf9298f4c055d`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07c56202c1a956ce919db56d3e09890a3df459cefab949e517810b84e6c2378`  
		Last Modified: Mon, 15 Jan 2018 23:26:02 GMT  
		Size: 97.1 MB (97069699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd9b5a8a42871d8a15d6dd892cb7947fa345445ded44f610117ec4cbbe7bf81`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf24480e18299ebb064cdaa4947195f9996a9b443f3c44dcc9cc1dbe668b82e`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 3.7 KB (3718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.0`

```console
$ docker pull mongo@sha256:7520ff8ac26830e838633f3048f06322c2ba72a34cae8c54b56988a71994a9d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.14393.2007; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.0` - linux; amd64

```console
$ docker pull mongo@sha256:77f22f913d8e62559b58437df321f02aabd6beeb863b5292c66c175716846f60
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84530333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e28cba33aad0327cf5df59ca2cbea98487692775937b9b05d0a7d7780952ba11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:46:27 GMT
ADD file:664e20ea0b4805f811ed279f86823b281c39df127d0f73ae147468bc1a9e4020 in / 
# Tue, 12 Dec 2017 01:46:27 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:35:30 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:35:31 GMT
RUN echo 'deb http://deb.debian.org/debian wheezy-backports main' > /etc/apt/sources.list.d/backports.list
# Tue, 12 Dec 2017 02:35:43 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 		procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:15:47 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:15:47 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:16:02 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:16:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:16:05 GMT
ENV GPG_KEYS=492EAFE8CD016A07919F1D2B9ECBEC467F0CEB10
# Thu, 21 Dec 2017 01:16:06 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:16:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:16:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:16:07 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:16:07 GMT
ENV MONGO_MAJOR=3.0
# Thu, 21 Dec 2017 01:16:08 GMT
ENV MONGO_VERSION=3.0.15
# Thu, 21 Dec 2017 01:16:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian wheezy/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:16:21 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:16:24 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:16:24 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:16:24 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:16:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:16:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:16:26 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:16:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:b967c325a8b3055106908c059240f7ea99c3b22958080fa3a0c1688e1e6739d1`  
		Last Modified: Tue, 12 Dec 2017 02:00:41 GMT  
		Size: 19.2 MB (19164678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f4b68f5594ff127e3c87e19190ca62d695d260de2c4e1dfbc1a110dab8e2de`  
		Last Modified: Tue, 12 Dec 2017 02:41:17 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24baba5a242ee93e67a0fcfe657c4944872fd9fd2a064328454997b46cdbd62`  
		Last Modified: Tue, 12 Dec 2017 02:41:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af11f2476fef6def7b28fd2c24f84397a099411ed68ad67cf937d5f9b76a82d7`  
		Last Modified: Tue, 12 Dec 2017 02:41:15 GMT  
		Size: 2.7 MB (2660614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4b2bf33f8e8bc113a559558c7e0fdc1f4e695b2bec89c09ccafc7f1dff9019`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 810.6 KB (810648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2c0d1d2005390ed504d8dd433b7ce7c2f81d79abbc40e191d8e64e1d2b1729`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2fb164e25f84f88ebd54215876bc44293ae6dfd02646f473f87ea57cbbf853`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95455f9a86a6bacac05bdcca3ec35f202e59b2ace6dc2e5c14f3c1e1b154aab4`  
		Last Modified: Thu, 21 Dec 2017 01:21:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460daad09d9d797d449205a3892eb7727250f88cb0fd838eb3da4477673c1bfd`  
		Last Modified: Thu, 21 Dec 2017 01:22:13 GMT  
		Size: 61.9 MB (61886207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab0d8c194a10785d610e3bc5a44fc56aebdc1b74d9475c1aed4690a23569518`  
		Last Modified: Thu, 21 Dec 2017 01:21:59 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424da624b820d4a1a38ffb4556bdd657dcea49c09fdfd356aa66b45a1d995b27`  
		Last Modified: Thu, 21 Dec 2017 01:21:59 GMT  
		Size: 3.6 KB (3569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c9ad8e0e7784c98341e142dbd3bf28f8677fbbb98b85dbc7403a25779eb619`  
		Last Modified: Thu, 21 Dec 2017 01:21:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.0` - windows version 10.0.14393.2007; amd64

```console
$ docker pull mongo@sha256:6dbf2494234499c01c54a5caad54691ce567d07b93f82e85188168b3bbfff118
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5421073958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7badb99cb8a3219c4e5a4bbe440885366b31a145b7dda3534d50b1377d4dce9c`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Thu, 04 Jan 2018 20:07:32 GMT
RUN Install update 10.0.14393.2007
# Fri, 05 Jan 2018 02:38:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 05 Jan 2018 02:38:20 GMT
ENV MONGO_VERSION=3.0.15
# Fri, 05 Jan 2018 02:38:21 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.0.15-signed.msi
# Fri, 05 Jan 2018 02:38:22 GMT
ENV MONGO_DOWNLOAD_SHA256=0a10cb87da164df7a1d31180d2ea1f3b096dda6e3d7b9f95c184ef953a1677bb
# Fri, 05 Jan 2018 02:54:36 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 05 Jan 2018 02:54:37 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 05 Jan 2018 02:54:39 GMT
EXPOSE 27017/tcp
# Fri, 05 Jan 2018 02:54:40 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:449343c9d7e2919413898dc8a7e8780ef164b76a3b9dd19de104706edf05113a`  
		Last Modified: Thu, 04 Jan 2018 20:07:32 GMT  
		Size: 1.3 GB (1304019288 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7e8689c7b014746ecb94f640c979d8f83b6d8fa0afd27c93e33f46f2f0a68eed`  
		Last Modified: Fri, 05 Jan 2018 03:29:26 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9b11c943102bbbb5bcde72f98ffc0d66eace802a5ea5051bd84399beab497e`  
		Last Modified: Fri, 05 Jan 2018 03:29:26 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c63b0493068e847ab3dd806873742aea2aa4daabffe21f3a03c5a03bbf0c59`  
		Last Modified: Fri, 05 Jan 2018 03:29:26 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04bfbd639e8d62976aa4e30cad22842999ea26bab5006599be433fd51fbf90c`  
		Last Modified: Fri, 05 Jan 2018 03:29:24 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74072e98626fe4174170eec84315ae8ea4dd1d49c375be4639f789ad88e4496`  
		Last Modified: Fri, 05 Jan 2018 03:29:36 GMT  
		Size: 47.1 MB (47060416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553c4c321873a5049bb9785c44d235ae8fd10c8222d10f89b5b31edc542a9cf6`  
		Last Modified: Fri, 05 Jan 2018 03:29:24 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7385460c2ec2093137223e1811463ac2083099b45e7567827a44fc19278982f6`  
		Last Modified: Fri, 05 Jan 2018 03:29:24 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725672f336d71aa03c2b143222fded841af0217d937c87021ddc51eaff79ea80`  
		Last Modified: Fri, 05 Jan 2018 03:29:24 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.0` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:00389d2bd6ffd221dfd368ac17ecfc5e260eceb2047ee6863a71fbdc5bd75191
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2910420228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cdbab21328ecf02ab2f68ac4290edca6369ec007e8168c943cb98ceebd36437`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:53:47 GMT
ENV MONGO_VERSION=3.0.15
# Wed, 13 Dec 2017 02:53:48 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.0.15-signed.msi
# Wed, 13 Dec 2017 02:53:49 GMT
ENV MONGO_DOWNLOAD_SHA256=0a10cb87da164df7a1d31180d2ea1f3b096dda6e3d7b9f95c184ef953a1677bb
# Wed, 13 Dec 2017 02:55:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:55:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:56:01 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:56:02 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a4f70e8a55dd9ea85316b97f10c7d87d64d891d4a3893db509966ddf56ca77`  
		Last Modified: Tue, 19 Dec 2017 04:07:41 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f3ea3f4e8d1ec0b6a063c611c64ffb2378d0ea00164896c00a217f03d1d5d8`  
		Last Modified: Tue, 19 Dec 2017 04:07:41 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b39b3d13ed5c75186b92c5228062beafa6c75dc85824bf6ce76b7fdfefdeb0`  
		Last Modified: Tue, 19 Dec 2017 04:07:38 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d712635eedd07152360df86c29be50fe9b990b6e6542bc774957a913a31c050`  
		Last Modified: Tue, 19 Dec 2017 04:07:52 GMT  
		Size: 46.6 MB (46586800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603d2b16e18ce034f792da7086da5c088f939d755a4cdb266e8daae630494f63`  
		Last Modified: Tue, 19 Dec 2017 04:07:39 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15104271b3f326fbb100b4c990b242c7c5e2da4f1dc143fb1d7a517df9edd65`  
		Last Modified: Tue, 19 Dec 2017 04:07:38 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdce9f53f93a4baac40828dea63b2616bab3b23f5d5c007506f00400fa4c2510`  
		Last Modified: Tue, 19 Dec 2017 04:07:39 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.0.15`

```console
$ docker pull mongo@sha256:7520ff8ac26830e838633f3048f06322c2ba72a34cae8c54b56988a71994a9d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.14393.2007; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.0.15` - linux; amd64

```console
$ docker pull mongo@sha256:77f22f913d8e62559b58437df321f02aabd6beeb863b5292c66c175716846f60
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84530333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e28cba33aad0327cf5df59ca2cbea98487692775937b9b05d0a7d7780952ba11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:46:27 GMT
ADD file:664e20ea0b4805f811ed279f86823b281c39df127d0f73ae147468bc1a9e4020 in / 
# Tue, 12 Dec 2017 01:46:27 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:35:30 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:35:31 GMT
RUN echo 'deb http://deb.debian.org/debian wheezy-backports main' > /etc/apt/sources.list.d/backports.list
# Tue, 12 Dec 2017 02:35:43 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 		procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:15:47 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:15:47 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:16:02 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:16:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:16:05 GMT
ENV GPG_KEYS=492EAFE8CD016A07919F1D2B9ECBEC467F0CEB10
# Thu, 21 Dec 2017 01:16:06 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:16:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:16:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:16:07 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:16:07 GMT
ENV MONGO_MAJOR=3.0
# Thu, 21 Dec 2017 01:16:08 GMT
ENV MONGO_VERSION=3.0.15
# Thu, 21 Dec 2017 01:16:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian wheezy/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:16:21 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:16:24 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:16:24 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:16:24 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:16:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:16:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:16:26 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:16:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:b967c325a8b3055106908c059240f7ea99c3b22958080fa3a0c1688e1e6739d1`  
		Last Modified: Tue, 12 Dec 2017 02:00:41 GMT  
		Size: 19.2 MB (19164678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f4b68f5594ff127e3c87e19190ca62d695d260de2c4e1dfbc1a110dab8e2de`  
		Last Modified: Tue, 12 Dec 2017 02:41:17 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24baba5a242ee93e67a0fcfe657c4944872fd9fd2a064328454997b46cdbd62`  
		Last Modified: Tue, 12 Dec 2017 02:41:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af11f2476fef6def7b28fd2c24f84397a099411ed68ad67cf937d5f9b76a82d7`  
		Last Modified: Tue, 12 Dec 2017 02:41:15 GMT  
		Size: 2.7 MB (2660614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4b2bf33f8e8bc113a559558c7e0fdc1f4e695b2bec89c09ccafc7f1dff9019`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 810.6 KB (810648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2c0d1d2005390ed504d8dd433b7ce7c2f81d79abbc40e191d8e64e1d2b1729`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2fb164e25f84f88ebd54215876bc44293ae6dfd02646f473f87ea57cbbf853`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95455f9a86a6bacac05bdcca3ec35f202e59b2ace6dc2e5c14f3c1e1b154aab4`  
		Last Modified: Thu, 21 Dec 2017 01:21:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460daad09d9d797d449205a3892eb7727250f88cb0fd838eb3da4477673c1bfd`  
		Last Modified: Thu, 21 Dec 2017 01:22:13 GMT  
		Size: 61.9 MB (61886207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab0d8c194a10785d610e3bc5a44fc56aebdc1b74d9475c1aed4690a23569518`  
		Last Modified: Thu, 21 Dec 2017 01:21:59 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424da624b820d4a1a38ffb4556bdd657dcea49c09fdfd356aa66b45a1d995b27`  
		Last Modified: Thu, 21 Dec 2017 01:21:59 GMT  
		Size: 3.6 KB (3569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c9ad8e0e7784c98341e142dbd3bf28f8677fbbb98b85dbc7403a25779eb619`  
		Last Modified: Thu, 21 Dec 2017 01:21:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.0.15` - windows version 10.0.14393.2007; amd64

```console
$ docker pull mongo@sha256:6dbf2494234499c01c54a5caad54691ce567d07b93f82e85188168b3bbfff118
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5421073958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7badb99cb8a3219c4e5a4bbe440885366b31a145b7dda3534d50b1377d4dce9c`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Thu, 04 Jan 2018 20:07:32 GMT
RUN Install update 10.0.14393.2007
# Fri, 05 Jan 2018 02:38:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 05 Jan 2018 02:38:20 GMT
ENV MONGO_VERSION=3.0.15
# Fri, 05 Jan 2018 02:38:21 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.0.15-signed.msi
# Fri, 05 Jan 2018 02:38:22 GMT
ENV MONGO_DOWNLOAD_SHA256=0a10cb87da164df7a1d31180d2ea1f3b096dda6e3d7b9f95c184ef953a1677bb
# Fri, 05 Jan 2018 02:54:36 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 05 Jan 2018 02:54:37 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 05 Jan 2018 02:54:39 GMT
EXPOSE 27017/tcp
# Fri, 05 Jan 2018 02:54:40 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:449343c9d7e2919413898dc8a7e8780ef164b76a3b9dd19de104706edf05113a`  
		Last Modified: Thu, 04 Jan 2018 20:07:32 GMT  
		Size: 1.3 GB (1304019288 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7e8689c7b014746ecb94f640c979d8f83b6d8fa0afd27c93e33f46f2f0a68eed`  
		Last Modified: Fri, 05 Jan 2018 03:29:26 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9b11c943102bbbb5bcde72f98ffc0d66eace802a5ea5051bd84399beab497e`  
		Last Modified: Fri, 05 Jan 2018 03:29:26 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c63b0493068e847ab3dd806873742aea2aa4daabffe21f3a03c5a03bbf0c59`  
		Last Modified: Fri, 05 Jan 2018 03:29:26 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04bfbd639e8d62976aa4e30cad22842999ea26bab5006599be433fd51fbf90c`  
		Last Modified: Fri, 05 Jan 2018 03:29:24 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74072e98626fe4174170eec84315ae8ea4dd1d49c375be4639f789ad88e4496`  
		Last Modified: Fri, 05 Jan 2018 03:29:36 GMT  
		Size: 47.1 MB (47060416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553c4c321873a5049bb9785c44d235ae8fd10c8222d10f89b5b31edc542a9cf6`  
		Last Modified: Fri, 05 Jan 2018 03:29:24 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7385460c2ec2093137223e1811463ac2083099b45e7567827a44fc19278982f6`  
		Last Modified: Fri, 05 Jan 2018 03:29:24 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725672f336d71aa03c2b143222fded841af0217d937c87021ddc51eaff79ea80`  
		Last Modified: Fri, 05 Jan 2018 03:29:24 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.0.15` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:00389d2bd6ffd221dfd368ac17ecfc5e260eceb2047ee6863a71fbdc5bd75191
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2910420228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cdbab21328ecf02ab2f68ac4290edca6369ec007e8168c943cb98ceebd36437`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:53:47 GMT
ENV MONGO_VERSION=3.0.15
# Wed, 13 Dec 2017 02:53:48 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.0.15-signed.msi
# Wed, 13 Dec 2017 02:53:49 GMT
ENV MONGO_DOWNLOAD_SHA256=0a10cb87da164df7a1d31180d2ea1f3b096dda6e3d7b9f95c184ef953a1677bb
# Wed, 13 Dec 2017 02:55:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:55:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:56:01 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:56:02 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a4f70e8a55dd9ea85316b97f10c7d87d64d891d4a3893db509966ddf56ca77`  
		Last Modified: Tue, 19 Dec 2017 04:07:41 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f3ea3f4e8d1ec0b6a063c611c64ffb2378d0ea00164896c00a217f03d1d5d8`  
		Last Modified: Tue, 19 Dec 2017 04:07:41 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b39b3d13ed5c75186b92c5228062beafa6c75dc85824bf6ce76b7fdfefdeb0`  
		Last Modified: Tue, 19 Dec 2017 04:07:38 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d712635eedd07152360df86c29be50fe9b990b6e6542bc774957a913a31c050`  
		Last Modified: Tue, 19 Dec 2017 04:07:52 GMT  
		Size: 46.6 MB (46586800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603d2b16e18ce034f792da7086da5c088f939d755a4cdb266e8daae630494f63`  
		Last Modified: Tue, 19 Dec 2017 04:07:39 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15104271b3f326fbb100b4c990b242c7c5e2da4f1dc143fb1d7a517df9edd65`  
		Last Modified: Tue, 19 Dec 2017 04:07:38 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdce9f53f93a4baac40828dea63b2616bab3b23f5d5c007506f00400fa4c2510`  
		Last Modified: Tue, 19 Dec 2017 04:07:39 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.0.15-wheezy`

```console
$ docker pull mongo@sha256:b2534b3119e159ee021c15600e67ad6945fa6eb5bf40e5f20defeae807734d69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.0.15-wheezy` - linux; amd64

```console
$ docker pull mongo@sha256:77f22f913d8e62559b58437df321f02aabd6beeb863b5292c66c175716846f60
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84530333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e28cba33aad0327cf5df59ca2cbea98487692775937b9b05d0a7d7780952ba11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:46:27 GMT
ADD file:664e20ea0b4805f811ed279f86823b281c39df127d0f73ae147468bc1a9e4020 in / 
# Tue, 12 Dec 2017 01:46:27 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:35:30 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:35:31 GMT
RUN echo 'deb http://deb.debian.org/debian wheezy-backports main' > /etc/apt/sources.list.d/backports.list
# Tue, 12 Dec 2017 02:35:43 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 		procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:15:47 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:15:47 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:16:02 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:16:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:16:05 GMT
ENV GPG_KEYS=492EAFE8CD016A07919F1D2B9ECBEC467F0CEB10
# Thu, 21 Dec 2017 01:16:06 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:16:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:16:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:16:07 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:16:07 GMT
ENV MONGO_MAJOR=3.0
# Thu, 21 Dec 2017 01:16:08 GMT
ENV MONGO_VERSION=3.0.15
# Thu, 21 Dec 2017 01:16:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian wheezy/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:16:21 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:16:24 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:16:24 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:16:24 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:16:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:16:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:16:26 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:16:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:b967c325a8b3055106908c059240f7ea99c3b22958080fa3a0c1688e1e6739d1`  
		Last Modified: Tue, 12 Dec 2017 02:00:41 GMT  
		Size: 19.2 MB (19164678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f4b68f5594ff127e3c87e19190ca62d695d260de2c4e1dfbc1a110dab8e2de`  
		Last Modified: Tue, 12 Dec 2017 02:41:17 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24baba5a242ee93e67a0fcfe657c4944872fd9fd2a064328454997b46cdbd62`  
		Last Modified: Tue, 12 Dec 2017 02:41:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af11f2476fef6def7b28fd2c24f84397a099411ed68ad67cf937d5f9b76a82d7`  
		Last Modified: Tue, 12 Dec 2017 02:41:15 GMT  
		Size: 2.7 MB (2660614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4b2bf33f8e8bc113a559558c7e0fdc1f4e695b2bec89c09ccafc7f1dff9019`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 810.6 KB (810648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2c0d1d2005390ed504d8dd433b7ce7c2f81d79abbc40e191d8e64e1d2b1729`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2fb164e25f84f88ebd54215876bc44293ae6dfd02646f473f87ea57cbbf853`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95455f9a86a6bacac05bdcca3ec35f202e59b2ace6dc2e5c14f3c1e1b154aab4`  
		Last Modified: Thu, 21 Dec 2017 01:21:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460daad09d9d797d449205a3892eb7727250f88cb0fd838eb3da4477673c1bfd`  
		Last Modified: Thu, 21 Dec 2017 01:22:13 GMT  
		Size: 61.9 MB (61886207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab0d8c194a10785d610e3bc5a44fc56aebdc1b74d9475c1aed4690a23569518`  
		Last Modified: Thu, 21 Dec 2017 01:21:59 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424da624b820d4a1a38ffb4556bdd657dcea49c09fdfd356aa66b45a1d995b27`  
		Last Modified: Thu, 21 Dec 2017 01:21:59 GMT  
		Size: 3.6 KB (3569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c9ad8e0e7784c98341e142dbd3bf28f8677fbbb98b85dbc7403a25779eb619`  
		Last Modified: Thu, 21 Dec 2017 01:21:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.0-wheezy`

```console
$ docker pull mongo@sha256:b2534b3119e159ee021c15600e67ad6945fa6eb5bf40e5f20defeae807734d69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.0-wheezy` - linux; amd64

```console
$ docker pull mongo@sha256:77f22f913d8e62559b58437df321f02aabd6beeb863b5292c66c175716846f60
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84530333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e28cba33aad0327cf5df59ca2cbea98487692775937b9b05d0a7d7780952ba11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:46:27 GMT
ADD file:664e20ea0b4805f811ed279f86823b281c39df127d0f73ae147468bc1a9e4020 in / 
# Tue, 12 Dec 2017 01:46:27 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:35:30 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:35:31 GMT
RUN echo 'deb http://deb.debian.org/debian wheezy-backports main' > /etc/apt/sources.list.d/backports.list
# Tue, 12 Dec 2017 02:35:43 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 		procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:15:47 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:15:47 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:16:02 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:16:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:16:05 GMT
ENV GPG_KEYS=492EAFE8CD016A07919F1D2B9ECBEC467F0CEB10
# Thu, 21 Dec 2017 01:16:06 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:16:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:16:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:16:07 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:16:07 GMT
ENV MONGO_MAJOR=3.0
# Thu, 21 Dec 2017 01:16:08 GMT
ENV MONGO_VERSION=3.0.15
# Thu, 21 Dec 2017 01:16:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian wheezy/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:16:21 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:16:24 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:16:24 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:16:24 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:16:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:16:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:16:26 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:16:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:b967c325a8b3055106908c059240f7ea99c3b22958080fa3a0c1688e1e6739d1`  
		Last Modified: Tue, 12 Dec 2017 02:00:41 GMT  
		Size: 19.2 MB (19164678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f4b68f5594ff127e3c87e19190ca62d695d260de2c4e1dfbc1a110dab8e2de`  
		Last Modified: Tue, 12 Dec 2017 02:41:17 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24baba5a242ee93e67a0fcfe657c4944872fd9fd2a064328454997b46cdbd62`  
		Last Modified: Tue, 12 Dec 2017 02:41:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af11f2476fef6def7b28fd2c24f84397a099411ed68ad67cf937d5f9b76a82d7`  
		Last Modified: Tue, 12 Dec 2017 02:41:15 GMT  
		Size: 2.7 MB (2660614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4b2bf33f8e8bc113a559558c7e0fdc1f4e695b2bec89c09ccafc7f1dff9019`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 810.6 KB (810648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2c0d1d2005390ed504d8dd433b7ce7c2f81d79abbc40e191d8e64e1d2b1729`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2fb164e25f84f88ebd54215876bc44293ae6dfd02646f473f87ea57cbbf853`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95455f9a86a6bacac05bdcca3ec35f202e59b2ace6dc2e5c14f3c1e1b154aab4`  
		Last Modified: Thu, 21 Dec 2017 01:21:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460daad09d9d797d449205a3892eb7727250f88cb0fd838eb3da4477673c1bfd`  
		Last Modified: Thu, 21 Dec 2017 01:22:13 GMT  
		Size: 61.9 MB (61886207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab0d8c194a10785d610e3bc5a44fc56aebdc1b74d9475c1aed4690a23569518`  
		Last Modified: Thu, 21 Dec 2017 01:21:59 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424da624b820d4a1a38ffb4556bdd657dcea49c09fdfd356aa66b45a1d995b27`  
		Last Modified: Thu, 21 Dec 2017 01:21:59 GMT  
		Size: 3.6 KB (3569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c9ad8e0e7784c98341e142dbd3bf28f8677fbbb98b85dbc7403a25779eb619`  
		Last Modified: Thu, 21 Dec 2017 01:21:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.2`

```console
$ docker pull mongo@sha256:fbb95eaa5a0c84d0d2098775f166003c568a79f993d91309cee7cda4135bbbfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.14393.2007; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.2` - linux; amd64

```console
$ docker pull mongo@sha256:99956969bc26f22650eae3c8ded898f1a0d2b172f8c3b12264459291e50b4d2c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.2 MB (104184765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a418e907f3f37c73be41c969e322962956b2a54e544084846ae4c85f503be7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:17:02 GMT
ENV GPG_KEYS=DFFA3DCF326E302C4787673A01C4E7FAAAB2461C 	42F3E95A2C4F08279C4960ADD68FA50FEA312927
# Thu, 21 Dec 2017 01:17:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:17:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:17:06 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_MAJOR=3.2
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_VERSION=3.2.18
# Thu, 21 Dec 2017 01:17:07 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:17:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:17:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:17:25 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:17:26 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:17:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:17:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:17:27 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:17:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc977f80d9b54fb489113d6bca4c2d46cb7ca05350b2aebb5600cfdbbab0fbf2`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 3.6 KB (3597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66827fc3b9db49a38fead890e65ee4cf13bd901f37d035a7fcbc50998ebc6966`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e912770bc2c7515034fbfa85483723b7cd8218f77ace4a96b1b89f0626170252`  
		Last Modified: Thu, 21 Dec 2017 01:23:32 GMT  
		Size: 70.8 MB (70845919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708e66e1928c3fe6ce818cfb0b88572aba860e34e06eef5f1230dd89ec64cf99`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b508231daf5410e2319031abd5fd613c48381b6a38e837c14b5b5157f844dfe`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 3.6 KB (3569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7323cb076d46824e7836df95dcd71ae59aa719bb207d189d0bcf78f26222bc90`  
		Last Modified: Thu, 21 Dec 2017 01:23:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.2` - windows version 10.0.14393.2007; amd64

```console
$ docker pull mongo@sha256:e861cf2ec90b70167a81bde4e575f57e90691b7bf54f322d1e36e41bf6fb228d
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5431581851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a5c9d5f38e7e185f0f48425f76c1d4df069c573cd55b1892b5463173aaecf74`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Thu, 04 Jan 2018 20:07:32 GMT
RUN Install update 10.0.14393.2007
# Fri, 05 Jan 2018 02:38:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 05 Jan 2018 02:54:58 GMT
ENV MONGO_VERSION=3.2.18
# Fri, 05 Jan 2018 02:54:59 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.2.18-signed.msi
# Fri, 05 Jan 2018 02:55:00 GMT
ENV MONGO_DOWNLOAD_SHA256=f86aba3b01fc3b50ffecfe1ae11cd9d3e0456b3e84cc25e9cc2eb40bcfa40452
# Fri, 05 Jan 2018 02:57:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 05 Jan 2018 02:57:28 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 05 Jan 2018 02:57:30 GMT
EXPOSE 27017/tcp
# Fri, 05 Jan 2018 02:57:31 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:449343c9d7e2919413898dc8a7e8780ef164b76a3b9dd19de104706edf05113a`  
		Last Modified: Thu, 04 Jan 2018 20:07:32 GMT  
		Size: 1.3 GB (1304019288 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7e8689c7b014746ecb94f640c979d8f83b6d8fa0afd27c93e33f46f2f0a68eed`  
		Last Modified: Fri, 05 Jan 2018 03:29:26 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6ed512d86bd9d3a8b8b47abbbcabe4061539a48448d43677d1a4189078ea0c`  
		Last Modified: Fri, 05 Jan 2018 03:29:50 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9db960ec35e4cb176d7829bc3e9514b17e6c72fa4969e17ae44318d304e2a6f`  
		Last Modified: Fri, 05 Jan 2018 03:29:50 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666e31dad3c808b393f4c74d0577591676d714d6d6e65dcfc3553eaf7ab75ed8`  
		Last Modified: Fri, 05 Jan 2018 03:29:48 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beca61b27caba48b26a421f9675ed749e51d3031d71dca186c3ee32810f34e77`  
		Last Modified: Fri, 05 Jan 2018 03:30:02 GMT  
		Size: 57.6 MB (57568333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4876df11d8c141788429649d82c87c1520c226823be82ec703817d713bea8039`  
		Last Modified: Fri, 05 Jan 2018 03:29:48 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde7d988e5403e6bbd5abed523fc17a9ab031686a29ced1550c8197db9bd122d`  
		Last Modified: Fri, 05 Jan 2018 03:29:48 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5cc462cef18d08eb57b96f8589e89b2c4216659a46af1d4e303bc6e7ee673b`  
		Last Modified: Fri, 05 Jan 2018 03:29:48 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.2` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:221495d2b9b7a642fa59fb6640c5bbc1efdfc0ec8fddd8b84e2b93b35bc9ab6b
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2916434524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2a0f0b7b41be06d7d22d922fbdb8183c10277249b84615c7adbdfabfd70345a`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:58:40 GMT
ENV MONGO_VERSION=3.2.18
# Wed, 13 Dec 2017 02:58:41 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.2.18-signed.msi
# Wed, 13 Dec 2017 02:58:42 GMT
ENV MONGO_DOWNLOAD_SHA256=f86aba3b01fc3b50ffecfe1ae11cd9d3e0456b3e84cc25e9cc2eb40bcfa40452
# Wed, 13 Dec 2017 03:00:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:00:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:00:22 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:00:23 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b144e842ac867249c947aa0cf6cf59e6fcfbcc49e6efb2e7f0742dbc20ad51`  
		Last Modified: Tue, 19 Dec 2017 04:08:40 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a66e6991fc46847e0d0c8add3693bab61b5b83da78d5c40608e55a28c2c58d`  
		Last Modified: Tue, 19 Dec 2017 04:08:40 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8fb4692c41b99c2be66bd7f2a704c2e6d0ec417f74897ec824a4bcc63e6062`  
		Last Modified: Tue, 19 Dec 2017 04:08:38 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3901e8f2cbaccbbf2ed1272e07ccc92366ffd5ff3f102f07c431b332b52bbd`  
		Last Modified: Tue, 19 Dec 2017 04:08:52 GMT  
		Size: 52.6 MB (52601081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257eb31b051e51e455018425175f8873db12de2b0d695cf1801362366a6f19d6`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad3a97356c88a1060f27de644028c806b2ae706532c438abf9ab257d1eb0e6b`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71cc34ffd5375d43282d15f2441bea0f89e1bba25a1d6315cc2f20b84cac17b6`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.2.18`

```console
$ docker pull mongo@sha256:fbb95eaa5a0c84d0d2098775f166003c568a79f993d91309cee7cda4135bbbfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.14393.2007; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.2.18` - linux; amd64

```console
$ docker pull mongo@sha256:99956969bc26f22650eae3c8ded898f1a0d2b172f8c3b12264459291e50b4d2c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.2 MB (104184765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a418e907f3f37c73be41c969e322962956b2a54e544084846ae4c85f503be7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:17:02 GMT
ENV GPG_KEYS=DFFA3DCF326E302C4787673A01C4E7FAAAB2461C 	42F3E95A2C4F08279C4960ADD68FA50FEA312927
# Thu, 21 Dec 2017 01:17:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:17:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:17:06 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_MAJOR=3.2
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_VERSION=3.2.18
# Thu, 21 Dec 2017 01:17:07 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:17:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:17:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:17:25 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:17:26 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:17:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:17:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:17:27 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:17:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc977f80d9b54fb489113d6bca4c2d46cb7ca05350b2aebb5600cfdbbab0fbf2`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 3.6 KB (3597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66827fc3b9db49a38fead890e65ee4cf13bd901f37d035a7fcbc50998ebc6966`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e912770bc2c7515034fbfa85483723b7cd8218f77ace4a96b1b89f0626170252`  
		Last Modified: Thu, 21 Dec 2017 01:23:32 GMT  
		Size: 70.8 MB (70845919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708e66e1928c3fe6ce818cfb0b88572aba860e34e06eef5f1230dd89ec64cf99`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b508231daf5410e2319031abd5fd613c48381b6a38e837c14b5b5157f844dfe`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 3.6 KB (3569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7323cb076d46824e7836df95dcd71ae59aa719bb207d189d0bcf78f26222bc90`  
		Last Modified: Thu, 21 Dec 2017 01:23:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.2.18` - windows version 10.0.14393.2007; amd64

```console
$ docker pull mongo@sha256:e861cf2ec90b70167a81bde4e575f57e90691b7bf54f322d1e36e41bf6fb228d
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5431581851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a5c9d5f38e7e185f0f48425f76c1d4df069c573cd55b1892b5463173aaecf74`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Thu, 04 Jan 2018 20:07:32 GMT
RUN Install update 10.0.14393.2007
# Fri, 05 Jan 2018 02:38:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 05 Jan 2018 02:54:58 GMT
ENV MONGO_VERSION=3.2.18
# Fri, 05 Jan 2018 02:54:59 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.2.18-signed.msi
# Fri, 05 Jan 2018 02:55:00 GMT
ENV MONGO_DOWNLOAD_SHA256=f86aba3b01fc3b50ffecfe1ae11cd9d3e0456b3e84cc25e9cc2eb40bcfa40452
# Fri, 05 Jan 2018 02:57:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 05 Jan 2018 02:57:28 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 05 Jan 2018 02:57:30 GMT
EXPOSE 27017/tcp
# Fri, 05 Jan 2018 02:57:31 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:449343c9d7e2919413898dc8a7e8780ef164b76a3b9dd19de104706edf05113a`  
		Last Modified: Thu, 04 Jan 2018 20:07:32 GMT  
		Size: 1.3 GB (1304019288 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7e8689c7b014746ecb94f640c979d8f83b6d8fa0afd27c93e33f46f2f0a68eed`  
		Last Modified: Fri, 05 Jan 2018 03:29:26 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6ed512d86bd9d3a8b8b47abbbcabe4061539a48448d43677d1a4189078ea0c`  
		Last Modified: Fri, 05 Jan 2018 03:29:50 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9db960ec35e4cb176d7829bc3e9514b17e6c72fa4969e17ae44318d304e2a6f`  
		Last Modified: Fri, 05 Jan 2018 03:29:50 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666e31dad3c808b393f4c74d0577591676d714d6d6e65dcfc3553eaf7ab75ed8`  
		Last Modified: Fri, 05 Jan 2018 03:29:48 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beca61b27caba48b26a421f9675ed749e51d3031d71dca186c3ee32810f34e77`  
		Last Modified: Fri, 05 Jan 2018 03:30:02 GMT  
		Size: 57.6 MB (57568333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4876df11d8c141788429649d82c87c1520c226823be82ec703817d713bea8039`  
		Last Modified: Fri, 05 Jan 2018 03:29:48 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde7d988e5403e6bbd5abed523fc17a9ab031686a29ced1550c8197db9bd122d`  
		Last Modified: Fri, 05 Jan 2018 03:29:48 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5cc462cef18d08eb57b96f8589e89b2c4216659a46af1d4e303bc6e7ee673b`  
		Last Modified: Fri, 05 Jan 2018 03:29:48 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.2.18` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:221495d2b9b7a642fa59fb6640c5bbc1efdfc0ec8fddd8b84e2b93b35bc9ab6b
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2916434524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2a0f0b7b41be06d7d22d922fbdb8183c10277249b84615c7adbdfabfd70345a`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:58:40 GMT
ENV MONGO_VERSION=3.2.18
# Wed, 13 Dec 2017 02:58:41 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.2.18-signed.msi
# Wed, 13 Dec 2017 02:58:42 GMT
ENV MONGO_DOWNLOAD_SHA256=f86aba3b01fc3b50ffecfe1ae11cd9d3e0456b3e84cc25e9cc2eb40bcfa40452
# Wed, 13 Dec 2017 03:00:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:00:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:00:22 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:00:23 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b144e842ac867249c947aa0cf6cf59e6fcfbcc49e6efb2e7f0742dbc20ad51`  
		Last Modified: Tue, 19 Dec 2017 04:08:40 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a66e6991fc46847e0d0c8add3693bab61b5b83da78d5c40608e55a28c2c58d`  
		Last Modified: Tue, 19 Dec 2017 04:08:40 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8fb4692c41b99c2be66bd7f2a704c2e6d0ec417f74897ec824a4bcc63e6062`  
		Last Modified: Tue, 19 Dec 2017 04:08:38 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3901e8f2cbaccbbf2ed1272e07ccc92366ffd5ff3f102f07c431b332b52bbd`  
		Last Modified: Tue, 19 Dec 2017 04:08:52 GMT  
		Size: 52.6 MB (52601081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257eb31b051e51e455018425175f8873db12de2b0d695cf1801362366a6f19d6`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad3a97356c88a1060f27de644028c806b2ae706532c438abf9ab257d1eb0e6b`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71cc34ffd5375d43282d15f2441bea0f89e1bba25a1d6315cc2f20b84cac17b6`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.2.18-jessie`

```console
$ docker pull mongo@sha256:ac7624fb058e0258419803a4197ce4cd764095a860bfb428e9e8498d80fe4025
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.2.18-jessie` - linux; amd64

```console
$ docker pull mongo@sha256:99956969bc26f22650eae3c8ded898f1a0d2b172f8c3b12264459291e50b4d2c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.2 MB (104184765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a418e907f3f37c73be41c969e322962956b2a54e544084846ae4c85f503be7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:17:02 GMT
ENV GPG_KEYS=DFFA3DCF326E302C4787673A01C4E7FAAAB2461C 	42F3E95A2C4F08279C4960ADD68FA50FEA312927
# Thu, 21 Dec 2017 01:17:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:17:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:17:06 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_MAJOR=3.2
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_VERSION=3.2.18
# Thu, 21 Dec 2017 01:17:07 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:17:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:17:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:17:25 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:17:26 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:17:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:17:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:17:27 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:17:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc977f80d9b54fb489113d6bca4c2d46cb7ca05350b2aebb5600cfdbbab0fbf2`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 3.6 KB (3597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66827fc3b9db49a38fead890e65ee4cf13bd901f37d035a7fcbc50998ebc6966`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e912770bc2c7515034fbfa85483723b7cd8218f77ace4a96b1b89f0626170252`  
		Last Modified: Thu, 21 Dec 2017 01:23:32 GMT  
		Size: 70.8 MB (70845919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708e66e1928c3fe6ce818cfb0b88572aba860e34e06eef5f1230dd89ec64cf99`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b508231daf5410e2319031abd5fd613c48381b6a38e837c14b5b5157f844dfe`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 3.6 KB (3569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7323cb076d46824e7836df95dcd71ae59aa719bb207d189d0bcf78f26222bc90`  
		Last Modified: Thu, 21 Dec 2017 01:23:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.2-jessie`

```console
$ docker pull mongo@sha256:ac7624fb058e0258419803a4197ce4cd764095a860bfb428e9e8498d80fe4025
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.2-jessie` - linux; amd64

```console
$ docker pull mongo@sha256:99956969bc26f22650eae3c8ded898f1a0d2b172f8c3b12264459291e50b4d2c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.2 MB (104184765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a418e907f3f37c73be41c969e322962956b2a54e544084846ae4c85f503be7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:17:02 GMT
ENV GPG_KEYS=DFFA3DCF326E302C4787673A01C4E7FAAAB2461C 	42F3E95A2C4F08279C4960ADD68FA50FEA312927
# Thu, 21 Dec 2017 01:17:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:17:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:17:06 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_MAJOR=3.2
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_VERSION=3.2.18
# Thu, 21 Dec 2017 01:17:07 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:17:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:17:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:17:25 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:17:26 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:17:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:17:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:17:27 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:17:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc977f80d9b54fb489113d6bca4c2d46cb7ca05350b2aebb5600cfdbbab0fbf2`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 3.6 KB (3597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66827fc3b9db49a38fead890e65ee4cf13bd901f37d035a7fcbc50998ebc6966`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e912770bc2c7515034fbfa85483723b7cd8218f77ace4a96b1b89f0626170252`  
		Last Modified: Thu, 21 Dec 2017 01:23:32 GMT  
		Size: 70.8 MB (70845919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708e66e1928c3fe6ce818cfb0b88572aba860e34e06eef5f1230dd89ec64cf99`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b508231daf5410e2319031abd5fd613c48381b6a38e837c14b5b5157f844dfe`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 3.6 KB (3569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7323cb076d46824e7836df95dcd71ae59aa719bb207d189d0bcf78f26222bc90`  
		Last Modified: Thu, 21 Dec 2017 01:23:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4`

```console
$ docker pull mongo@sha256:b84baeffd0f14bebaf057b36de9414ee41584a897351795f4a3889257cf19b6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.14393.2007; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.4` - linux; amd64

```console
$ docker pull mongo@sha256:77dd9838010b4de7f7274d4b3a0cf57fe51890de2f284dc80e81f752ff883550
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131854682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e905a87e116de6dcfc7860d2c24afaf4b87ee0c8db295494a144a1a3d24ac1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:19:41 GMT
ENV GPG_KEYS=0C49F3730359A14518585931BC711F9BA15703C6
# Thu, 21 Dec 2017 01:19:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:19:44 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:19:44 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:19:44 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:19:44 GMT
ENV MONGO_MAJOR=3.4
# Thu, 21 Dec 2017 01:19:45 GMT
ENV MONGO_VERSION=3.4.10
# Thu, 21 Dec 2017 01:19:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:20:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:20:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:20:54 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:20:54 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:20:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:20:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:20:56 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:20:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b17a05532222a454ee2adb0f8fb5e1e189f20b5a732082107712a92f0d5c784`  
		Last Modified: Thu, 21 Dec 2017 01:24:00 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1723351cb8b477e49637a166a9f6e1392c8ecdcef5df971d33348e2aeaecd3e7`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dd8437755a7eca2d118b41346592b0e55d4529d05aedc5180563d26b2c832e`  
		Last Modified: Thu, 21 Dec 2017 01:24:16 GMT  
		Size: 98.5 MB (98517998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61012c0435729d9c1eb7125e91a3db7ffa9492e1224ee9fe356415df24d11ad7`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76aeb242d479c37f92572a4077aba093f3433e0401c9a56d3391dff44861e370`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 3.6 KB (3571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc8171e92f4532da660f8d79d2d40ea612c785860ae359be8f463e525f0230c`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.4` - windows version 10.0.14393.2007; amd64

```console
$ docker pull mongo@sha256:3f1dc34f2da33af68327358d6b3cd03dd1510685b5b9122135dd4901bdf760b0
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5441722307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7824ed2b768e3615699c88117f0071087616a0ce56a59e48907e197c94b7ae14`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Thu, 04 Jan 2018 20:07:32 GMT
RUN Install update 10.0.14393.2007
# Fri, 05 Jan 2018 02:38:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 05 Jan 2018 02:57:44 GMT
ENV MONGO_VERSION=3.4.10
# Fri, 05 Jan 2018 02:57:45 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.10-signed.msi
# Fri, 05 Jan 2018 02:57:46 GMT
ENV MONGO_DOWNLOAD_SHA256=6b650bdf62792fb44445edfee2100b9a8d861710348c8bbd3b93f56d11d5e7ea
# Fri, 05 Jan 2018 03:00:01 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 05 Jan 2018 03:00:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 05 Jan 2018 03:00:05 GMT
EXPOSE 27017/tcp
# Fri, 05 Jan 2018 03:00:06 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:449343c9d7e2919413898dc8a7e8780ef164b76a3b9dd19de104706edf05113a`  
		Last Modified: Thu, 04 Jan 2018 20:07:32 GMT  
		Size: 1.3 GB (1304019288 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7e8689c7b014746ecb94f640c979d8f83b6d8fa0afd27c93e33f46f2f0a68eed`  
		Last Modified: Fri, 05 Jan 2018 03:29:26 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02097f6a68c26f33c17204ffccb87065bb6c1dddf9292aabdc5d0cfd5e85f5ee`  
		Last Modified: Fri, 05 Jan 2018 03:30:17 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4556ca69527ee909f60b6fb4d531cafe45206281526cadcfde6f14335d9d68af`  
		Last Modified: Fri, 05 Jan 2018 03:30:17 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:051995d82c52c619f43b898ff1617f3babffa147dbe1947c2c3d9d1b22ec837d`  
		Last Modified: Fri, 05 Jan 2018 03:30:14 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68069dd0d2b7ff3e611e3b0a6c0037abf1dc78e277089f153954918710519dd5`  
		Last Modified: Fri, 05 Jan 2018 03:30:37 GMT  
		Size: 67.7 MB (67708742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0716c245a7299dc321097c8c2f74c8cd54ba39eb2336277d43eab2aaa4d188`  
		Last Modified: Fri, 05 Jan 2018 03:30:14 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e02cb68857161cbd6d8575fee89783ca7e13b497240a7f38e41f76f859ba6f`  
		Last Modified: Fri, 05 Jan 2018 03:30:14 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03322bd68565b6e1b936ed40c538349761d037d248bd1cc710f927712f00c41`  
		Last Modified: Fri, 05 Jan 2018 03:30:15 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.4` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:29302f0f0eee02cb1df6ecedb46c0ba3f2e51c2a47379f4ad7de5795e0e8c332
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2926599685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba42d72049e85b3e5b42280dfd62ed78e80bb8e7101d91b64e16840ad5fa6959`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 03:03:04 GMT
ENV MONGO_VERSION=3.4.10
# Wed, 13 Dec 2017 03:03:05 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.10-signed.msi
# Wed, 13 Dec 2017 03:03:05 GMT
ENV MONGO_DOWNLOAD_SHA256=6b650bdf62792fb44445edfee2100b9a8d861710348c8bbd3b93f56d11d5e7ea
# Wed, 13 Dec 2017 03:04:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:04:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:04:55 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:04:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3897e104207f2d5fcfbeb59db966ec737475f376aaf98b3b77e20bd0d28a99`  
		Last Modified: Tue, 19 Dec 2017 04:09:38 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f909469ec493bd10b7bad5b5fb130796da35ceffdd10017495d139676f7cd`  
		Last Modified: Tue, 19 Dec 2017 04:09:38 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2306bda02ae76915dce1b47898ce5b4599e9cd01ef0dbe5abfa25fdeb461a1`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b8495b3df676b97f4c3e13a85c40754d9e20c470e12801f3333501163338ed`  
		Last Modified: Tue, 19 Dec 2017 04:09:52 GMT  
		Size: 62.8 MB (62766246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad9a53e77635aaccd959073dcf5e3923c5240a7e5bfb8899bc5a63a91e91b7e`  
		Last Modified: Tue, 19 Dec 2017 04:09:35 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebecba35c2e569980a8b7b04578cf30e0d719bbb9a7dbbf5f6e103cae3d7fd2a`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9286875f590bc8985af9b15c002756168e9695752fa557785aea4a360c886318`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4.10`

```console
$ docker pull mongo@sha256:b84baeffd0f14bebaf057b36de9414ee41584a897351795f4a3889257cf19b6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.14393.2007; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.4.10` - linux; amd64

```console
$ docker pull mongo@sha256:77dd9838010b4de7f7274d4b3a0cf57fe51890de2f284dc80e81f752ff883550
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131854682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e905a87e116de6dcfc7860d2c24afaf4b87ee0c8db295494a144a1a3d24ac1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:19:41 GMT
ENV GPG_KEYS=0C49F3730359A14518585931BC711F9BA15703C6
# Thu, 21 Dec 2017 01:19:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:19:44 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:19:44 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:19:44 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:19:44 GMT
ENV MONGO_MAJOR=3.4
# Thu, 21 Dec 2017 01:19:45 GMT
ENV MONGO_VERSION=3.4.10
# Thu, 21 Dec 2017 01:19:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:20:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:20:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:20:54 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:20:54 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:20:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:20:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:20:56 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:20:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b17a05532222a454ee2adb0f8fb5e1e189f20b5a732082107712a92f0d5c784`  
		Last Modified: Thu, 21 Dec 2017 01:24:00 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1723351cb8b477e49637a166a9f6e1392c8ecdcef5df971d33348e2aeaecd3e7`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dd8437755a7eca2d118b41346592b0e55d4529d05aedc5180563d26b2c832e`  
		Last Modified: Thu, 21 Dec 2017 01:24:16 GMT  
		Size: 98.5 MB (98517998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61012c0435729d9c1eb7125e91a3db7ffa9492e1224ee9fe356415df24d11ad7`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76aeb242d479c37f92572a4077aba093f3433e0401c9a56d3391dff44861e370`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 3.6 KB (3571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc8171e92f4532da660f8d79d2d40ea612c785860ae359be8f463e525f0230c`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.4.10` - windows version 10.0.14393.2007; amd64

```console
$ docker pull mongo@sha256:3f1dc34f2da33af68327358d6b3cd03dd1510685b5b9122135dd4901bdf760b0
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5441722307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7824ed2b768e3615699c88117f0071087616a0ce56a59e48907e197c94b7ae14`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Thu, 04 Jan 2018 20:07:32 GMT
RUN Install update 10.0.14393.2007
# Fri, 05 Jan 2018 02:38:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 05 Jan 2018 02:57:44 GMT
ENV MONGO_VERSION=3.4.10
# Fri, 05 Jan 2018 02:57:45 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.10-signed.msi
# Fri, 05 Jan 2018 02:57:46 GMT
ENV MONGO_DOWNLOAD_SHA256=6b650bdf62792fb44445edfee2100b9a8d861710348c8bbd3b93f56d11d5e7ea
# Fri, 05 Jan 2018 03:00:01 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 05 Jan 2018 03:00:03 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 05 Jan 2018 03:00:05 GMT
EXPOSE 27017/tcp
# Fri, 05 Jan 2018 03:00:06 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:449343c9d7e2919413898dc8a7e8780ef164b76a3b9dd19de104706edf05113a`  
		Last Modified: Thu, 04 Jan 2018 20:07:32 GMT  
		Size: 1.3 GB (1304019288 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7e8689c7b014746ecb94f640c979d8f83b6d8fa0afd27c93e33f46f2f0a68eed`  
		Last Modified: Fri, 05 Jan 2018 03:29:26 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02097f6a68c26f33c17204ffccb87065bb6c1dddf9292aabdc5d0cfd5e85f5ee`  
		Last Modified: Fri, 05 Jan 2018 03:30:17 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4556ca69527ee909f60b6fb4d531cafe45206281526cadcfde6f14335d9d68af`  
		Last Modified: Fri, 05 Jan 2018 03:30:17 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:051995d82c52c619f43b898ff1617f3babffa147dbe1947c2c3d9d1b22ec837d`  
		Last Modified: Fri, 05 Jan 2018 03:30:14 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68069dd0d2b7ff3e611e3b0a6c0037abf1dc78e277089f153954918710519dd5`  
		Last Modified: Fri, 05 Jan 2018 03:30:37 GMT  
		Size: 67.7 MB (67708742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0716c245a7299dc321097c8c2f74c8cd54ba39eb2336277d43eab2aaa4d188`  
		Last Modified: Fri, 05 Jan 2018 03:30:14 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e02cb68857161cbd6d8575fee89783ca7e13b497240a7f38e41f76f859ba6f`  
		Last Modified: Fri, 05 Jan 2018 03:30:14 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03322bd68565b6e1b936ed40c538349761d037d248bd1cc710f927712f00c41`  
		Last Modified: Fri, 05 Jan 2018 03:30:15 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.4.10` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:29302f0f0eee02cb1df6ecedb46c0ba3f2e51c2a47379f4ad7de5795e0e8c332
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2926599685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba42d72049e85b3e5b42280dfd62ed78e80bb8e7101d91b64e16840ad5fa6959`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 03:03:04 GMT
ENV MONGO_VERSION=3.4.10
# Wed, 13 Dec 2017 03:03:05 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.10-signed.msi
# Wed, 13 Dec 2017 03:03:05 GMT
ENV MONGO_DOWNLOAD_SHA256=6b650bdf62792fb44445edfee2100b9a8d861710348c8bbd3b93f56d11d5e7ea
# Wed, 13 Dec 2017 03:04:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:04:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:04:55 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:04:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3897e104207f2d5fcfbeb59db966ec737475f376aaf98b3b77e20bd0d28a99`  
		Last Modified: Tue, 19 Dec 2017 04:09:38 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f909469ec493bd10b7bad5b5fb130796da35ceffdd10017495d139676f7cd`  
		Last Modified: Tue, 19 Dec 2017 04:09:38 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2306bda02ae76915dce1b47898ce5b4599e9cd01ef0dbe5abfa25fdeb461a1`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b8495b3df676b97f4c3e13a85c40754d9e20c470e12801f3333501163338ed`  
		Last Modified: Tue, 19 Dec 2017 04:09:52 GMT  
		Size: 62.8 MB (62766246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad9a53e77635aaccd959073dcf5e3923c5240a7e5bfb8899bc5a63a91e91b7e`  
		Last Modified: Tue, 19 Dec 2017 04:09:35 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebecba35c2e569980a8b7b04578cf30e0d719bbb9a7dbbf5f6e103cae3d7fd2a`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9286875f590bc8985af9b15c002756168e9695752fa557785aea4a360c886318`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4.10-jessie`

```console
$ docker pull mongo@sha256:38829565a5781afeecb287a6a2da6535396712718a63a4e2dcc7f006a0611cd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.4.10-jessie` - linux; amd64

```console
$ docker pull mongo@sha256:77dd9838010b4de7f7274d4b3a0cf57fe51890de2f284dc80e81f752ff883550
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131854682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e905a87e116de6dcfc7860d2c24afaf4b87ee0c8db295494a144a1a3d24ac1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:19:41 GMT
ENV GPG_KEYS=0C49F3730359A14518585931BC711F9BA15703C6
# Thu, 21 Dec 2017 01:19:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:19:44 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:19:44 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:19:44 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:19:44 GMT
ENV MONGO_MAJOR=3.4
# Thu, 21 Dec 2017 01:19:45 GMT
ENV MONGO_VERSION=3.4.10
# Thu, 21 Dec 2017 01:19:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:20:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:20:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:20:54 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:20:54 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:20:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:20:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:20:56 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:20:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b17a05532222a454ee2adb0f8fb5e1e189f20b5a732082107712a92f0d5c784`  
		Last Modified: Thu, 21 Dec 2017 01:24:00 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1723351cb8b477e49637a166a9f6e1392c8ecdcef5df971d33348e2aeaecd3e7`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dd8437755a7eca2d118b41346592b0e55d4529d05aedc5180563d26b2c832e`  
		Last Modified: Thu, 21 Dec 2017 01:24:16 GMT  
		Size: 98.5 MB (98517998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61012c0435729d9c1eb7125e91a3db7ffa9492e1224ee9fe356415df24d11ad7`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76aeb242d479c37f92572a4077aba093f3433e0401c9a56d3391dff44861e370`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 3.6 KB (3571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc8171e92f4532da660f8d79d2d40ea612c785860ae359be8f463e525f0230c`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4-jessie`

```console
$ docker pull mongo@sha256:38829565a5781afeecb287a6a2da6535396712718a63a4e2dcc7f006a0611cd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.4-jessie` - linux; amd64

```console
$ docker pull mongo@sha256:77dd9838010b4de7f7274d4b3a0cf57fe51890de2f284dc80e81f752ff883550
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131854682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e905a87e116de6dcfc7860d2c24afaf4b87ee0c8db295494a144a1a3d24ac1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:19:41 GMT
ENV GPG_KEYS=0C49F3730359A14518585931BC711F9BA15703C6
# Thu, 21 Dec 2017 01:19:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:19:44 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:19:44 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:19:44 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:19:44 GMT
ENV MONGO_MAJOR=3.4
# Thu, 21 Dec 2017 01:19:45 GMT
ENV MONGO_VERSION=3.4.10
# Thu, 21 Dec 2017 01:19:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:20:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:20:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:20:54 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:20:54 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:20:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:20:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:20:56 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:20:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b17a05532222a454ee2adb0f8fb5e1e189f20b5a732082107712a92f0d5c784`  
		Last Modified: Thu, 21 Dec 2017 01:24:00 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1723351cb8b477e49637a166a9f6e1392c8ecdcef5df971d33348e2aeaecd3e7`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dd8437755a7eca2d118b41346592b0e55d4529d05aedc5180563d26b2c832e`  
		Last Modified: Thu, 21 Dec 2017 01:24:16 GMT  
		Size: 98.5 MB (98517998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61012c0435729d9c1eb7125e91a3db7ffa9492e1224ee9fe356415df24d11ad7`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76aeb242d479c37f92572a4077aba093f3433e0401c9a56d3391dff44861e370`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 3.6 KB (3571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc8171e92f4532da660f8d79d2d40ea612c785860ae359be8f463e525f0230c`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6`

```console
$ docker pull mongo@sha256:878b76e5834f37da98096296f4147f6ca4d94b1a9187986e9d6e59756e7ce865
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.6` - linux; amd64

```console
$ docker pull mongo@sha256:8bb68343e860575cfe3e82c98f5f5baad3ab8a67f54062d3476f2276b576abb4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130406419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f57644645eb53a3d2256f460ade116ad3590252c28f63e5136c026423dc8286`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:21:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Dec 2017 01:21:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:21:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:21:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_MAJOR=3.6
# Mon, 15 Jan 2018 23:15:02 GMT
ENV MONGO_VERSION=3.6.2
# Mon, 15 Jan 2018 23:15:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 15 Jan 2018 23:15:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 15 Jan 2018 23:15:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 15 Jan 2018 23:15:25 GMT
VOLUME [/data/db /data/configdb]
# Mon, 15 Jan 2018 23:15:25 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Mon, 15 Jan 2018 23:15:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Jan 2018 23:15:26 GMT
EXPOSE 27017/tcp
# Mon, 15 Jan 2018 23:15:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6c28c0235b619029c8b8c9d512f97756a986bfa458e64b5aa45784af894ac3`  
		Last Modified: Thu, 21 Dec 2017 01:24:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6688308f715efc799218462de2504d5ea35be542dfc7bb1dbcbf9298f4c055d`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07c56202c1a956ce919db56d3e09890a3df459cefab949e517810b84e6c2378`  
		Last Modified: Mon, 15 Jan 2018 23:26:02 GMT  
		Size: 97.1 MB (97069699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd9b5a8a42871d8a15d6dd892cb7947fa345445ded44f610117ec4cbbe7bf81`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf24480e18299ebb064cdaa4947195f9996a9b443f3c44dcc9cc1dbe668b82e`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 3.7 KB (3718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.2`

```console
$ docker pull mongo@sha256:878b76e5834f37da98096296f4147f6ca4d94b1a9187986e9d6e59756e7ce865
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.6.2` - linux; amd64

```console
$ docker pull mongo@sha256:8bb68343e860575cfe3e82c98f5f5baad3ab8a67f54062d3476f2276b576abb4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130406419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f57644645eb53a3d2256f460ade116ad3590252c28f63e5136c026423dc8286`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:21:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Dec 2017 01:21:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:21:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:21:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_MAJOR=3.6
# Mon, 15 Jan 2018 23:15:02 GMT
ENV MONGO_VERSION=3.6.2
# Mon, 15 Jan 2018 23:15:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 15 Jan 2018 23:15:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 15 Jan 2018 23:15:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 15 Jan 2018 23:15:25 GMT
VOLUME [/data/db /data/configdb]
# Mon, 15 Jan 2018 23:15:25 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Mon, 15 Jan 2018 23:15:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Jan 2018 23:15:26 GMT
EXPOSE 27017/tcp
# Mon, 15 Jan 2018 23:15:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6c28c0235b619029c8b8c9d512f97756a986bfa458e64b5aa45784af894ac3`  
		Last Modified: Thu, 21 Dec 2017 01:24:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6688308f715efc799218462de2504d5ea35be542dfc7bb1dbcbf9298f4c055d`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07c56202c1a956ce919db56d3e09890a3df459cefab949e517810b84e6c2378`  
		Last Modified: Mon, 15 Jan 2018 23:26:02 GMT  
		Size: 97.1 MB (97069699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd9b5a8a42871d8a15d6dd892cb7947fa345445ded44f610117ec4cbbe7bf81`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf24480e18299ebb064cdaa4947195f9996a9b443f3c44dcc9cc1dbe668b82e`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 3.7 KB (3718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.2-jessie`

```console
$ docker pull mongo@sha256:878b76e5834f37da98096296f4147f6ca4d94b1a9187986e9d6e59756e7ce865
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.6.2-jessie` - linux; amd64

```console
$ docker pull mongo@sha256:8bb68343e860575cfe3e82c98f5f5baad3ab8a67f54062d3476f2276b576abb4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130406419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f57644645eb53a3d2256f460ade116ad3590252c28f63e5136c026423dc8286`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:21:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Dec 2017 01:21:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:21:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:21:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_MAJOR=3.6
# Mon, 15 Jan 2018 23:15:02 GMT
ENV MONGO_VERSION=3.6.2
# Mon, 15 Jan 2018 23:15:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 15 Jan 2018 23:15:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 15 Jan 2018 23:15:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 15 Jan 2018 23:15:25 GMT
VOLUME [/data/db /data/configdb]
# Mon, 15 Jan 2018 23:15:25 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Mon, 15 Jan 2018 23:15:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Jan 2018 23:15:26 GMT
EXPOSE 27017/tcp
# Mon, 15 Jan 2018 23:15:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6c28c0235b619029c8b8c9d512f97756a986bfa458e64b5aa45784af894ac3`  
		Last Modified: Thu, 21 Dec 2017 01:24:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6688308f715efc799218462de2504d5ea35be542dfc7bb1dbcbf9298f4c055d`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07c56202c1a956ce919db56d3e09890a3df459cefab949e517810b84e6c2378`  
		Last Modified: Mon, 15 Jan 2018 23:26:02 GMT  
		Size: 97.1 MB (97069699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd9b5a8a42871d8a15d6dd892cb7947fa345445ded44f610117ec4cbbe7bf81`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf24480e18299ebb064cdaa4947195f9996a9b443f3c44dcc9cc1dbe668b82e`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 3.7 KB (3718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-jessie`

```console
$ docker pull mongo@sha256:878b76e5834f37da98096296f4147f6ca4d94b1a9187986e9d6e59756e7ce865
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.6-jessie` - linux; amd64

```console
$ docker pull mongo@sha256:8bb68343e860575cfe3e82c98f5f5baad3ab8a67f54062d3476f2276b576abb4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130406419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f57644645eb53a3d2256f460ade116ad3590252c28f63e5136c026423dc8286`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:21:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Dec 2017 01:21:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:21:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:21:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_MAJOR=3.6
# Mon, 15 Jan 2018 23:15:02 GMT
ENV MONGO_VERSION=3.6.2
# Mon, 15 Jan 2018 23:15:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 15 Jan 2018 23:15:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 15 Jan 2018 23:15:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 15 Jan 2018 23:15:25 GMT
VOLUME [/data/db /data/configdb]
# Mon, 15 Jan 2018 23:15:25 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Mon, 15 Jan 2018 23:15:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Jan 2018 23:15:26 GMT
EXPOSE 27017/tcp
# Mon, 15 Jan 2018 23:15:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6c28c0235b619029c8b8c9d512f97756a986bfa458e64b5aa45784af894ac3`  
		Last Modified: Thu, 21 Dec 2017 01:24:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6688308f715efc799218462de2504d5ea35be542dfc7bb1dbcbf9298f4c055d`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07c56202c1a956ce919db56d3e09890a3df459cefab949e517810b84e6c2378`  
		Last Modified: Mon, 15 Jan 2018 23:26:02 GMT  
		Size: 97.1 MB (97069699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd9b5a8a42871d8a15d6dd892cb7947fa345445ded44f610117ec4cbbe7bf81`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf24480e18299ebb064cdaa4947195f9996a9b443f3c44dcc9cc1dbe668b82e`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 3.7 KB (3718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.7`

```console
$ docker pull mongo@sha256:3fec5f6e91a23bd5a438fdce9de99b1e17f2372f99268294b051019daa59a5a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.7` - linux; amd64

```console
$ docker pull mongo@sha256:d8d5850b183a280ba3f810effa400063a48f1acd71dc31b1d79c311dcc58721d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130395752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b616bd2250f66a81afb4fc67839685c3493bc9348d720e2a3596c6312a27a2de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jan 2018 18:15:46 GMT
ENV GPG_KEYS=BD8C80D9C729D00524E068E03DAB71713396F72B
# Wed, 17 Jan 2018 18:15:50 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jan 2018 18:15:51 GMT
ARG MONGO_PACKAGE=mongodb-org-unstable
# Wed, 17 Jan 2018 18:15:51 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jan 2018 18:15:51 GMT
ENV MONGO_PACKAGE=mongodb-org-unstable MONGO_REPO=repo.mongodb.org
# Wed, 17 Jan 2018 18:15:51 GMT
ENV MONGO_MAJOR=3.7
# Wed, 17 Jan 2018 18:15:52 GMT
ENV MONGO_VERSION=3.7.1
# Wed, 17 Jan 2018 18:15:52 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jan 2018 18:16:11 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jan 2018 18:16:12 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jan 2018 18:16:12 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jan 2018 18:16:12 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Wed, 17 Jan 2018 18:16:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jan 2018 18:16:13 GMT
EXPOSE 27017/tcp
# Wed, 17 Jan 2018 18:16:13 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43077dfd3530b92b029f94d3396d3957d873d0856b3d1c7dbbac30bfc376f77a`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76a2d037a9d6d16450c77e225c04b8c7141cbd61264abd692def207616c4d39`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6e30e505796afd3bf3154ea36aa105c577f7cd0c5c1893f7067dc2c466105b`  
		Last Modified: Wed, 17 Jan 2018 18:16:54 GMT  
		Size: 97.1 MB (97059039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43de95800fae416e4fd2fafb7e85a99af691510518b116c17548f9c9a703f26f`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c812544e6864c9c703a5f36e5829a0e76ef8c1d501f0f5cb97f82b75012b17f`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 3.7 KB (3717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.7.1`

```console
$ docker pull mongo@sha256:3fec5f6e91a23bd5a438fdce9de99b1e17f2372f99268294b051019daa59a5a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.7.1` - linux; amd64

```console
$ docker pull mongo@sha256:d8d5850b183a280ba3f810effa400063a48f1acd71dc31b1d79c311dcc58721d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130395752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b616bd2250f66a81afb4fc67839685c3493bc9348d720e2a3596c6312a27a2de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jan 2018 18:15:46 GMT
ENV GPG_KEYS=BD8C80D9C729D00524E068E03DAB71713396F72B
# Wed, 17 Jan 2018 18:15:50 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jan 2018 18:15:51 GMT
ARG MONGO_PACKAGE=mongodb-org-unstable
# Wed, 17 Jan 2018 18:15:51 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jan 2018 18:15:51 GMT
ENV MONGO_PACKAGE=mongodb-org-unstable MONGO_REPO=repo.mongodb.org
# Wed, 17 Jan 2018 18:15:51 GMT
ENV MONGO_MAJOR=3.7
# Wed, 17 Jan 2018 18:15:52 GMT
ENV MONGO_VERSION=3.7.1
# Wed, 17 Jan 2018 18:15:52 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jan 2018 18:16:11 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jan 2018 18:16:12 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jan 2018 18:16:12 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jan 2018 18:16:12 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Wed, 17 Jan 2018 18:16:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jan 2018 18:16:13 GMT
EXPOSE 27017/tcp
# Wed, 17 Jan 2018 18:16:13 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43077dfd3530b92b029f94d3396d3957d873d0856b3d1c7dbbac30bfc376f77a`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76a2d037a9d6d16450c77e225c04b8c7141cbd61264abd692def207616c4d39`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6e30e505796afd3bf3154ea36aa105c577f7cd0c5c1893f7067dc2c466105b`  
		Last Modified: Wed, 17 Jan 2018 18:16:54 GMT  
		Size: 97.1 MB (97059039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43de95800fae416e4fd2fafb7e85a99af691510518b116c17548f9c9a703f26f`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c812544e6864c9c703a5f36e5829a0e76ef8c1d501f0f5cb97f82b75012b17f`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 3.7 KB (3717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.7.1-jessie`

```console
$ docker pull mongo@sha256:3fec5f6e91a23bd5a438fdce9de99b1e17f2372f99268294b051019daa59a5a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.7.1-jessie` - linux; amd64

```console
$ docker pull mongo@sha256:d8d5850b183a280ba3f810effa400063a48f1acd71dc31b1d79c311dcc58721d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130395752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b616bd2250f66a81afb4fc67839685c3493bc9348d720e2a3596c6312a27a2de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jan 2018 18:15:46 GMT
ENV GPG_KEYS=BD8C80D9C729D00524E068E03DAB71713396F72B
# Wed, 17 Jan 2018 18:15:50 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jan 2018 18:15:51 GMT
ARG MONGO_PACKAGE=mongodb-org-unstable
# Wed, 17 Jan 2018 18:15:51 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jan 2018 18:15:51 GMT
ENV MONGO_PACKAGE=mongodb-org-unstable MONGO_REPO=repo.mongodb.org
# Wed, 17 Jan 2018 18:15:51 GMT
ENV MONGO_MAJOR=3.7
# Wed, 17 Jan 2018 18:15:52 GMT
ENV MONGO_VERSION=3.7.1
# Wed, 17 Jan 2018 18:15:52 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jan 2018 18:16:11 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jan 2018 18:16:12 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jan 2018 18:16:12 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jan 2018 18:16:12 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Wed, 17 Jan 2018 18:16:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jan 2018 18:16:13 GMT
EXPOSE 27017/tcp
# Wed, 17 Jan 2018 18:16:13 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43077dfd3530b92b029f94d3396d3957d873d0856b3d1c7dbbac30bfc376f77a`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76a2d037a9d6d16450c77e225c04b8c7141cbd61264abd692def207616c4d39`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6e30e505796afd3bf3154ea36aa105c577f7cd0c5c1893f7067dc2c466105b`  
		Last Modified: Wed, 17 Jan 2018 18:16:54 GMT  
		Size: 97.1 MB (97059039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43de95800fae416e4fd2fafb7e85a99af691510518b116c17548f9c9a703f26f`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c812544e6864c9c703a5f36e5829a0e76ef8c1d501f0f5cb97f82b75012b17f`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 3.7 KB (3717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.7-jessie`

```console
$ docker pull mongo@sha256:3fec5f6e91a23bd5a438fdce9de99b1e17f2372f99268294b051019daa59a5a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.7-jessie` - linux; amd64

```console
$ docker pull mongo@sha256:d8d5850b183a280ba3f810effa400063a48f1acd71dc31b1d79c311dcc58721d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130395752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b616bd2250f66a81afb4fc67839685c3493bc9348d720e2a3596c6312a27a2de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jan 2018 18:15:46 GMT
ENV GPG_KEYS=BD8C80D9C729D00524E068E03DAB71713396F72B
# Wed, 17 Jan 2018 18:15:50 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jan 2018 18:15:51 GMT
ARG MONGO_PACKAGE=mongodb-org-unstable
# Wed, 17 Jan 2018 18:15:51 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jan 2018 18:15:51 GMT
ENV MONGO_PACKAGE=mongodb-org-unstable MONGO_REPO=repo.mongodb.org
# Wed, 17 Jan 2018 18:15:51 GMT
ENV MONGO_MAJOR=3.7
# Wed, 17 Jan 2018 18:15:52 GMT
ENV MONGO_VERSION=3.7.1
# Wed, 17 Jan 2018 18:15:52 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jan 2018 18:16:11 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jan 2018 18:16:12 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jan 2018 18:16:12 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jan 2018 18:16:12 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Wed, 17 Jan 2018 18:16:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jan 2018 18:16:13 GMT
EXPOSE 27017/tcp
# Wed, 17 Jan 2018 18:16:13 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43077dfd3530b92b029f94d3396d3957d873d0856b3d1c7dbbac30bfc376f77a`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76a2d037a9d6d16450c77e225c04b8c7141cbd61264abd692def207616c4d39`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6e30e505796afd3bf3154ea36aa105c577f7cd0c5c1893f7067dc2c466105b`  
		Last Modified: Wed, 17 Jan 2018 18:16:54 GMT  
		Size: 97.1 MB (97059039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43de95800fae416e4fd2fafb7e85a99af691510518b116c17548f9c9a703f26f`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c812544e6864c9c703a5f36e5829a0e76ef8c1d501f0f5cb97f82b75012b17f`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 3.7 KB (3717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-jessie`

```console
$ docker pull mongo@sha256:878b76e5834f37da98096296f4147f6ca4d94b1a9187986e9d6e59756e7ce865
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3-jessie` - linux; amd64

```console
$ docker pull mongo@sha256:8bb68343e860575cfe3e82c98f5f5baad3ab8a67f54062d3476f2276b576abb4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130406419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f57644645eb53a3d2256f460ade116ad3590252c28f63e5136c026423dc8286`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:21:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Dec 2017 01:21:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:21:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:21:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_MAJOR=3.6
# Mon, 15 Jan 2018 23:15:02 GMT
ENV MONGO_VERSION=3.6.2
# Mon, 15 Jan 2018 23:15:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 15 Jan 2018 23:15:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 15 Jan 2018 23:15:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 15 Jan 2018 23:15:25 GMT
VOLUME [/data/db /data/configdb]
# Mon, 15 Jan 2018 23:15:25 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Mon, 15 Jan 2018 23:15:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Jan 2018 23:15:26 GMT
EXPOSE 27017/tcp
# Mon, 15 Jan 2018 23:15:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6c28c0235b619029c8b8c9d512f97756a986bfa458e64b5aa45784af894ac3`  
		Last Modified: Thu, 21 Dec 2017 01:24:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6688308f715efc799218462de2504d5ea35be542dfc7bb1dbcbf9298f4c055d`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07c56202c1a956ce919db56d3e09890a3df459cefab949e517810b84e6c2378`  
		Last Modified: Mon, 15 Jan 2018 23:26:02 GMT  
		Size: 97.1 MB (97069699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd9b5a8a42871d8a15d6dd892cb7947fa345445ded44f610117ec4cbbe7bf81`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf24480e18299ebb064cdaa4947195f9996a9b443f3c44dcc9cc1dbe668b82e`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 3.7 KB (3718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:jessie`

```console
$ docker pull mongo@sha256:878b76e5834f37da98096296f4147f6ca4d94b1a9187986e9d6e59756e7ce865
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:jessie` - linux; amd64

```console
$ docker pull mongo@sha256:8bb68343e860575cfe3e82c98f5f5baad3ab8a67f54062d3476f2276b576abb4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130406419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f57644645eb53a3d2256f460ade116ad3590252c28f63e5136c026423dc8286`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:21:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Dec 2017 01:21:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:21:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:21:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_MAJOR=3.6
# Mon, 15 Jan 2018 23:15:02 GMT
ENV MONGO_VERSION=3.6.2
# Mon, 15 Jan 2018 23:15:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 15 Jan 2018 23:15:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 15 Jan 2018 23:15:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 15 Jan 2018 23:15:25 GMT
VOLUME [/data/db /data/configdb]
# Mon, 15 Jan 2018 23:15:25 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Mon, 15 Jan 2018 23:15:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Jan 2018 23:15:26 GMT
EXPOSE 27017/tcp
# Mon, 15 Jan 2018 23:15:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6c28c0235b619029c8b8c9d512f97756a986bfa458e64b5aa45784af894ac3`  
		Last Modified: Thu, 21 Dec 2017 01:24:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6688308f715efc799218462de2504d5ea35be542dfc7bb1dbcbf9298f4c055d`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07c56202c1a956ce919db56d3e09890a3df459cefab949e517810b84e6c2378`  
		Last Modified: Mon, 15 Jan 2018 23:26:02 GMT  
		Size: 97.1 MB (97069699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd9b5a8a42871d8a15d6dd892cb7947fa345445ded44f610117ec4cbbe7bf81`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf24480e18299ebb064cdaa4947195f9996a9b443f3c44dcc9cc1dbe668b82e`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 3.7 KB (3718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:latest`

```console
$ docker pull mongo@sha256:878b76e5834f37da98096296f4147f6ca4d94b1a9187986e9d6e59756e7ce865
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:latest` - linux; amd64

```console
$ docker pull mongo@sha256:8bb68343e860575cfe3e82c98f5f5baad3ab8a67f54062d3476f2276b576abb4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130406419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f57644645eb53a3d2256f460ade116ad3590252c28f63e5136c026423dc8286`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:21:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Dec 2017 01:21:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:21:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:21:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_MAJOR=3.6
# Mon, 15 Jan 2018 23:15:02 GMT
ENV MONGO_VERSION=3.6.2
# Mon, 15 Jan 2018 23:15:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 15 Jan 2018 23:15:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 15 Jan 2018 23:15:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 15 Jan 2018 23:15:25 GMT
VOLUME [/data/db /data/configdb]
# Mon, 15 Jan 2018 23:15:25 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Mon, 15 Jan 2018 23:15:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Jan 2018 23:15:26 GMT
EXPOSE 27017/tcp
# Mon, 15 Jan 2018 23:15:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6c28c0235b619029c8b8c9d512f97756a986bfa458e64b5aa45784af894ac3`  
		Last Modified: Thu, 21 Dec 2017 01:24:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6688308f715efc799218462de2504d5ea35be542dfc7bb1dbcbf9298f4c055d`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07c56202c1a956ce919db56d3e09890a3df459cefab949e517810b84e6c2378`  
		Last Modified: Mon, 15 Jan 2018 23:26:02 GMT  
		Size: 97.1 MB (97069699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd9b5a8a42871d8a15d6dd892cb7947fa345445ded44f610117ec4cbbe7bf81`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf24480e18299ebb064cdaa4947195f9996a9b443f3c44dcc9cc1dbe668b82e`  
		Last Modified: Mon, 15 Jan 2018 23:25:37 GMT  
		Size: 3.7 KB (3718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:unstable`

```console
$ docker pull mongo@sha256:3fec5f6e91a23bd5a438fdce9de99b1e17f2372f99268294b051019daa59a5a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:unstable` - linux; amd64

```console
$ docker pull mongo@sha256:d8d5850b183a280ba3f810effa400063a48f1acd71dc31b1d79c311dcc58721d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130395752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b616bd2250f66a81afb4fc67839685c3493bc9348d720e2a3596c6312a27a2de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jan 2018 18:15:46 GMT
ENV GPG_KEYS=BD8C80D9C729D00524E068E03DAB71713396F72B
# Wed, 17 Jan 2018 18:15:50 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jan 2018 18:15:51 GMT
ARG MONGO_PACKAGE=mongodb-org-unstable
# Wed, 17 Jan 2018 18:15:51 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jan 2018 18:15:51 GMT
ENV MONGO_PACKAGE=mongodb-org-unstable MONGO_REPO=repo.mongodb.org
# Wed, 17 Jan 2018 18:15:51 GMT
ENV MONGO_MAJOR=3.7
# Wed, 17 Jan 2018 18:15:52 GMT
ENV MONGO_VERSION=3.7.1
# Wed, 17 Jan 2018 18:15:52 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jan 2018 18:16:11 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jan 2018 18:16:12 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jan 2018 18:16:12 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jan 2018 18:16:12 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Wed, 17 Jan 2018 18:16:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jan 2018 18:16:13 GMT
EXPOSE 27017/tcp
# Wed, 17 Jan 2018 18:16:13 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43077dfd3530b92b029f94d3396d3957d873d0856b3d1c7dbbac30bfc376f77a`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76a2d037a9d6d16450c77e225c04b8c7141cbd61264abd692def207616c4d39`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6e30e505796afd3bf3154ea36aa105c577f7cd0c5c1893f7067dc2c466105b`  
		Last Modified: Wed, 17 Jan 2018 18:16:54 GMT  
		Size: 97.1 MB (97059039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43de95800fae416e4fd2fafb7e85a99af691510518b116c17548f9c9a703f26f`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c812544e6864c9c703a5f36e5829a0e76ef8c1d501f0f5cb97f82b75012b17f`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 3.7 KB (3717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:unstable-jessie`

```console
$ docker pull mongo@sha256:3fec5f6e91a23bd5a438fdce9de99b1e17f2372f99268294b051019daa59a5a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:unstable-jessie` - linux; amd64

```console
$ docker pull mongo@sha256:d8d5850b183a280ba3f810effa400063a48f1acd71dc31b1d79c311dcc58721d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130395752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b616bd2250f66a81afb4fc67839685c3493bc9348d720e2a3596c6312a27a2de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Jan 2018 18:15:46 GMT
ENV GPG_KEYS=BD8C80D9C729D00524E068E03DAB71713396F72B
# Wed, 17 Jan 2018 18:15:50 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 17 Jan 2018 18:15:51 GMT
ARG MONGO_PACKAGE=mongodb-org-unstable
# Wed, 17 Jan 2018 18:15:51 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 17 Jan 2018 18:15:51 GMT
ENV MONGO_PACKAGE=mongodb-org-unstable MONGO_REPO=repo.mongodb.org
# Wed, 17 Jan 2018 18:15:51 GMT
ENV MONGO_MAJOR=3.7
# Wed, 17 Jan 2018 18:15:52 GMT
ENV MONGO_VERSION=3.7.1
# Wed, 17 Jan 2018 18:15:52 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Jan 2018 18:16:11 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Jan 2018 18:16:12 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Jan 2018 18:16:12 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Jan 2018 18:16:12 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Wed, 17 Jan 2018 18:16:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Jan 2018 18:16:13 GMT
EXPOSE 27017/tcp
# Wed, 17 Jan 2018 18:16:13 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43077dfd3530b92b029f94d3396d3957d873d0856b3d1c7dbbac30bfc376f77a`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76a2d037a9d6d16450c77e225c04b8c7141cbd61264abd692def207616c4d39`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6e30e505796afd3bf3154ea36aa105c577f7cd0c5c1893f7067dc2c466105b`  
		Last Modified: Wed, 17 Jan 2018 18:16:54 GMT  
		Size: 97.1 MB (97059039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43de95800fae416e4fd2fafb7e85a99af691510518b116c17548f9c9a703f26f`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c812544e6864c9c703a5f36e5829a0e76ef8c1d501f0f5cb97f82b75012b17f`  
		Last Modified: Wed, 17 Jan 2018 18:16:39 GMT  
		Size: 3.7 KB (3717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
