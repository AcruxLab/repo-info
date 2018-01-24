## `traefik:cancoillotte-alpine`

```console
$ docker pull traefik@sha256:8cec7f413af331a1bcbf18484a589c48a9fd8c122dc3e36f805477444d2e2c5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:cancoillotte-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:6382b1254492992f4f87225ef3d52c84e3000de47c350e4b466530dac23e61b7
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16320059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e085fa33a8830bbc4a4de30e26e346ba00450eb89946d8f9593b8590fb44e6c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Jan 2018 21:10:38 GMT
ADD file:6edc55fb54ec9fc3658c8f5176a70e792103a516154442f94fed8e0290e4960e in / 
# Tue, 09 Jan 2018 21:10:38 GMT
CMD ["/bin/sh"]
# Wed, 10 Jan 2018 01:28:51 GMT
RUN apk --no-cache add ca-certificates
# Tue, 23 Jan 2018 20:49:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	apk add --no-cache --virtual .fetch-deps libressl; 	wget -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.5.0/traefik_linux-$arch"; 	apk del .fetch-deps; 	chmod +x /usr/local/bin/traefik
# Tue, 23 Jan 2018 20:49:20 GMT
COPY file:41f5bd1ea0a61e819b7d8c5489c305d4f2798046917dd6b6695318f555981727 in / 
# Tue, 23 Jan 2018 20:49:21 GMT
EXPOSE 80/tcp
# Tue, 23 Jan 2018 20:49:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 Jan 2018 20:49:21 GMT
CMD ["traefik"]
# Tue, 23 Jan 2018 20:49:21 GMT
LABEL org.label-schema.vendor=Containous org.label-schema.url=https://traefik.io org.label-schema.name=Traefik org.label-schema.description=A modern reverse-proxy org.label-schema.version=v1.5.0 org.label-schema.docker.schema-version=1.0
```

-	Layers:
	-	`sha256:605ce1bd3f3164f2949a30501cc596f52a72de05da1306ab360055f0d7130c32`  
		Last Modified: Tue, 09 Jan 2018 21:13:17 GMT  
		Size: 2.0 MB (1991747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3eb27e4ab8454370b50d5b8d9c153713bebe12c43d63dac2ae368fcce7d6d4`  
		Last Modified: Wed, 10 Jan 2018 01:30:19 GMT  
		Size: 351.0 KB (350991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28eb0e1da02b737c3aa350f3eec9e1a4c3af0f6a825d165374d838c989152c6`  
		Last Modified: Tue, 23 Jan 2018 21:07:30 GMT  
		Size: 14.0 MB (13976982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0841dda3a7ebb024838a5431e9d35fb3c5addb97a9bd092f3ab99f01a8dea422`  
		Last Modified: Tue, 23 Jan 2018 21:07:26 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:cancoillotte-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:546fe2a648e09d1ace000039beb1848006c8aa12e05f300107ba63a13bb063e7
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15436872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67680e2131dcdd2b972b3dbbe47a7cf87b39b74b1c40480d886356eab106d769`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:35 GMT
ADD file:009348222efb3c4ca2e53c387fb34c488679ca07db39525a6c5cc214e46abffd in / 
# Wed, 25 Oct 2017 23:28:36 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:36 GMT
CMD ["/bin/sh"]
# Wed, 15 Nov 2017 00:48:35 GMT
RUN apk --no-cache add ca-certificates
# Wed, 24 Jan 2018 00:48:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	apk add --no-cache --virtual .fetch-deps libressl; 	wget -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.5.0/traefik_linux-$arch"; 	apk del .fetch-deps; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Jan 2018 00:48:38 GMT
COPY file:41f5bd1ea0a61e819b7d8c5489c305d4f2798046917dd6b6695318f555981727 in / 
# Wed, 24 Jan 2018 00:48:38 GMT
EXPOSE 80/tcp
# Wed, 24 Jan 2018 00:48:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Jan 2018 00:48:39 GMT
CMD ["traefik"]
# Wed, 24 Jan 2018 00:48:39 GMT
LABEL org.label-schema.vendor=Containous org.label-schema.url=https://traefik.io org.label-schema.name=Traefik org.label-schema.description=A modern reverse-proxy org.label-schema.version=v1.5.0 org.label-schema.docker.schema-version=1.0
```

-	Layers:
	-	`sha256:0864efeeb5cb8dca4eb53e5d6fd38486daee80fa326fe36d1ad254f8fa6bb310`  
		Last Modified: Sun, 23 Jul 2017 20:21:42 GMT  
		Size: 2.0 MB (1965988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda69762aee1588fa82aeabf1af6d6ad24f737cce1451fab2e0199849b1e12e`  
		Last Modified: Wed, 25 Oct 2017 23:28:45 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a327851d323fa2321bd95a42227f24138450e43ea70af9570970baf49ae6ba`  
		Last Modified: Wed, 15 Nov 2017 00:49:06 GMT  
		Size: 352.2 KB (352157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bdf1c7e0b3040fd6b5642ea5836dd7960165c1e4a74bf304e4090f6898dbfe`  
		Last Modified: Wed, 24 Jan 2018 00:49:09 GMT  
		Size: 13.1 MB (13118216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5600652bb5fcf499ce95da19da729e8d3349bbe5a189b7e5aaba37584f46b9b3`  
		Last Modified: Wed, 24 Jan 2018 00:49:05 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:cancoillotte-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:d7acf8040032ca7feadc6fbd6d6723a6759a4d722906ebbc31e85806586376ad
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15050761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e9f4bb0376841fb971d5294fcfb2c80e1b821d274038364bcfca75138983ab9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 25 Oct 2017 23:28:58 GMT
ADD file:45b5d3b8d5490ba7edfca2cf6f54cdcf49c772b0b3a2302ce69a7af061007aa4 in / 
# Wed, 25 Oct 2017 23:28:59 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Wed, 25 Oct 2017 23:28:59 GMT
CMD ["/bin/sh"]
# Wed, 15 Nov 2017 05:55:26 GMT
RUN apk --no-cache add ca-certificates
# Wed, 24 Jan 2018 05:55:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	apk add --no-cache --virtual .fetch-deps libressl; 	wget -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.5.0/traefik_linux-$arch"; 	apk del .fetch-deps; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Jan 2018 05:55:24 GMT
COPY file:41f5bd1ea0a61e819b7d8c5489c305d4f2798046917dd6b6695318f555981727 in / 
# Wed, 24 Jan 2018 05:55:25 GMT
EXPOSE 80/tcp
# Wed, 24 Jan 2018 05:55:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Jan 2018 05:55:26 GMT
CMD ["traefik"]
# Wed, 24 Jan 2018 05:55:27 GMT
LABEL org.label-schema.vendor=Containous org.label-schema.url=https://traefik.io org.label-schema.name=Traefik org.label-schema.description=A modern reverse-proxy org.label-schema.version=v1.5.0 org.label-schema.docker.schema-version=1.0
```

-	Layers:
	-	`sha256:bb473f0ebc12fde1bd45c1bd3c46f2d3aab367b1b7739464771455b9972f7894`  
		Last Modified: Thu, 06 Jul 2017 09:54:42 GMT  
		Size: 1.9 MB (1914748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ff6b7ff3a208b8399e701e7ea1b7edbdc654c8c60d33c6f09a7803e2dda776`  
		Last Modified: Wed, 25 Oct 2017 23:29:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fcc5af9467e49f936c4812ee156fc62e6efaa954ca3165d15b03ae39805932f`  
		Last Modified: Wed, 15 Nov 2017 05:58:01 GMT  
		Size: 351.5 KB (351494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db996edd2013847e6441ef1a18ea9008eb354cbde114f72810bbb845fe0a0b3`  
		Last Modified: Wed, 24 Jan 2018 05:56:59 GMT  
		Size: 12.8 MB (12784001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29015987bca21088952b08d12fe7bb64791480ea1ec92a2528c364f320723b95`  
		Last Modified: Wed, 24 Jan 2018 05:56:54 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
