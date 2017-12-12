## `debian:oldoldstable-backports`

```console
$ docker pull debian@sha256:784eef1603b8e5537753c1823a58c7133e8689f3beffaba80ba4225b118d5ed5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `debian:oldoldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:601c6d10e641328f4d0c671347377489773d3deef33fbfa0a4b34865ae41af6b
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38110051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0a7a8b43df72831d68769eb845c050b19d975bf965b8c4e0a1b67a0bd800aab`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:50 GMT
ADD file:d0211c74db49159a472468fd9561525c8829bc80ad9fee8e2250d2ec3141fed8 in / 
# Tue, 12 Dec 2017 01:41:50 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 01:41:59 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c8d8f76914b3724c95de164533d58cf5d2753f47559e926fc169728d341c196c`  
		Last Modified: Tue, 12 Dec 2017 01:49:16 GMT  
		Size: 38.1 MB (38109823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c57842a79d41af03dd7c84d48e7a3cba4b73ce13696f2e34e9891c5f054a9c`  
		Last Modified: Tue, 12 Dec 2017 01:49:37 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:4578a6effa0c0b69105694b35c34bf860c9c873445fda6fe895f355b8199567d
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36949211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cf13d4f5c8fe974fc815b3065ac6491a903a8f0a16521a2332d56dd84e6b6ca`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 20:57:58 GMT
ADD file:faa442008df3acb0265ee75153d629160177cafd45dd0262357523f8c183f01c in / 
# Tue, 12 Dec 2017 20:57:59 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 20:58:09 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:57cbef3272b511ddf7b47a3216d28a2cd0fce39b31215d5506c486d7da8fb54d`  
		Last Modified: Tue, 12 Dec 2017 21:08:04 GMT  
		Size: 36.9 MB (36948984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b1f3f30a2cbd92f3a490611e2893b5e70ac57af8a6eea34fb56ad24e9e59ad`  
		Last Modified: Tue, 12 Dec 2017 21:08:26 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:035561a83bb088612682910cd5319e44e06e60df4d7dce79629b1e91f51bb1ff
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35662044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32906eab138836ac68587402865d2fe43f943142dc93b9a4cd28d8472bc63b33`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 13:28:18 GMT
ADD file:1b754591dd6066d83a1ce20710a8e05a5b3de6e4d62614e1b948eb3472dccee9 in / 
# Tue, 12 Dec 2017 13:28:19 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 13:28:35 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:25b7eb61899e875cc3b897e6aaf595eb97694d0a9c59d4999d5c17b4fc84d035`  
		Last Modified: Tue, 12 Dec 2017 13:40:14 GMT  
		Size: 35.7 MB (35661819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06aac857546988af59c8afdb1034282dc16a16cc7991b8c5df1199b40303106`  
		Last Modified: Tue, 12 Dec 2017 13:40:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:1fffc7337703a78e3b80ebe21f36919f8982ac3a842be74943a6a595ac2c1fd0
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37439543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c56603936c5f9ede5c2e7020bb3bfc373233db53c85ac90c9f8fca916cbb818`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 14:21:30 GMT
ADD file:69c866b1832ee07bdf5ef10057c25e8adcf44ef8309c9b5449db59893b4d107e in / 
# Tue, 12 Dec 2017 14:21:30 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:21:58 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:78dd03bd86acbd5985b15655e65c8e39173aa21b84c49feb789ca909579fdbec`  
		Last Modified: Tue, 12 Dec 2017 14:51:57 GMT  
		Size: 37.4 MB (37439315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cfd0abfa94196341955d2d4ee56ec77ab12849c040baf6e5c88a0204ba61bf`  
		Last Modified: Tue, 12 Dec 2017 14:54:36 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
