## `buildpack-deps:artful-scm`

```console
$ docker pull buildpack-deps@sha256:4f2d3669d4b57a1e1e9a1b3382d8b3523df0bebb69c040d44f85c08f5acf35b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:artful-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:98ca044e679dfa5b4b320459871518f8ba5deef8333d7089e0befe32bafbd96d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.0 MB (90951356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a7274e44c0c3dd3b18f1ef03e92e6ffe3265b9cdd66afad82b117e88fd2d4c8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Oct 2017 16:49:44 GMT
ADD file:c5fd97d776dc13116460fbfe9516f1a028ba5788ea39ee71d8e9cfe7caed676f in / 
# Thu, 19 Oct 2017 16:49:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Oct 2017 16:49:45 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Oct 2017 16:49:46 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Thu, 19 Oct 2017 16:49:47 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Oct 2017 16:49:47 GMT
CMD ["/bin/bash"]
# Thu, 19 Oct 2017 17:11:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 19 Oct 2017 17:11:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg2 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 19 Oct 2017 17:12:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d26cfb4142faf488780cb8080f737aa1e5db91805163d83448842f64084bb724`  
		Last Modified: Thu, 19 Oct 2017 16:50:57 GMT  
		Size: 39.2 MB (39215977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e69583643894064c76a95e3d11683364de4efab032b9a5b9fda912300d2ee7`  
		Last Modified: Thu, 19 Oct 2017 16:50:51 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23612a50167e73f5f4a0835016d48e4d1f3718e475dc7ce034ab1f97f87a4559`  
		Last Modified: Thu, 19 Oct 2017 16:50:51 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f87853aa05b46566e39ee0f6a3a98f44a5a9ebcc7d1c70aeaa0652a7dbb55a3`  
		Last Modified: Thu, 19 Oct 2017 16:50:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196b8aba5fb6c607ab9d6dacf5cb959ab3852b39648371b4cf3cb1d0de1a1788`  
		Last Modified: Thu, 19 Oct 2017 16:50:51 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a6cbeb56ae3697a9b14ec463d7c5468f7d8a2b7da2ecc83f8a4444b99beedf`  
		Last Modified: Thu, 19 Oct 2017 17:14:42 GMT  
		Size: 6.0 MB (6034673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc2f56127f4001b8229a63547299975f77e71be100190bf936980059e51118d`  
		Last Modified: Thu, 19 Oct 2017 17:15:09 GMT  
		Size: 45.7 MB (45698447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:artful-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7b9b459a64c5db6c3a53b2242e6361cd2289208931c8513b5735d0d283503634
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.0 MB (82019011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20d551d32a0f058040ad8ab7a11e9ff97b91ab168a8b3cef6c626daa16cdea1d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Oct 2017 16:55:51 GMT
ADD file:e295a2804e9021d3aebf237c767f9f2130874c00153f74ffdeba3eaab30fbaac in / 
# Thu, 19 Oct 2017 16:55:52 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Oct 2017 16:55:52 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Oct 2017 16:55:53 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Thu, 19 Oct 2017 16:55:54 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Oct 2017 16:55:54 GMT
CMD ["/bin/bash"]
# Thu, 19 Oct 2017 17:13:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 00:06:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Nov 2017 00:06:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6aee42d1a16f080f5e31ecdb42ad2cd6f4a207e0a500a908cf7bfda5ff192992`  
		Last Modified: Thu, 19 Oct 2017 16:56:56 GMT  
		Size: 35.1 MB (35054496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc204a5c135c178768b589f1b3ba0b7bb133676a405801d33a046bab704808cd`  
		Last Modified: Thu, 19 Oct 2017 16:56:47 GMT  
		Size: 837.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875211a9caba9133760f30d72afd4d4d26c5cd02c41842e0c1c2ea3eb4b3e99c`  
		Last Modified: Thu, 19 Oct 2017 16:56:47 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7239c8aa2ef420bca9bd3ad2a162ec45b8326c4445ee6a04d2bc7db21062b34`  
		Last Modified: Thu, 19 Oct 2017 16:56:47 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3296b67840d45438ac734401161bf6344bbb00228c9a13cefb2d87d769fbf9f5`  
		Last Modified: Thu, 19 Oct 2017 16:56:47 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9056c14ebd1e3f1737712ae8bc184cac07a2cd941a3859a14852404bc7bb9890`  
		Last Modified: Thu, 19 Oct 2017 17:17:59 GMT  
		Size: 5.1 MB (5101409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eba2b9a7968a54f18b586e32b719167016a7986e1134c77308512b490b564b6`  
		Last Modified: Fri, 03 Nov 2017 00:25:26 GMT  
		Size: 41.9 MB (41860839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:artful-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d0f796c029db773ade19f35c99833af018bdef084c9bdf517c955004449da9cb
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85436510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b50c374e5bd827be5b520af1c8766ad52eea3f0e0cb2e77126abc15e87479819`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Oct 2017 16:56:03 GMT
ADD file:910e149f9bb1b98604e675d9e071d6de38047c2a16daf5352e66c7916b8f01f2 in / 
# Thu, 19 Oct 2017 16:56:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Oct 2017 16:56:06 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Oct 2017 16:56:08 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Thu, 19 Oct 2017 16:56:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Oct 2017 16:56:10 GMT
CMD ["/bin/bash"]
# Thu, 19 Oct 2017 17:18:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Nov 2017 09:31:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Nov 2017 09:32:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e5b0ba60fd18373323fbf61d66aadd15f7f147f73b6d9123fda3f14ea88c83c4`  
		Last Modified: Thu, 19 Oct 2017 16:58:07 GMT  
		Size: 36.2 MB (36214016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffa0e39786f334992f3365c97ca0618d3616fdb61cb35c320e38376b2ac9f3a`  
		Last Modified: Thu, 19 Oct 2017 16:57:55 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b855c81f8b3ebe0829512446549542bdbfa6bf01395779ce92bd73a70c804abb`  
		Last Modified: Thu, 19 Oct 2017 16:57:55 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3894de6a565f29a27d72202ceff1e27c6827932cd8502734b58d0a4aca81c34e`  
		Last Modified: Thu, 19 Oct 2017 16:57:55 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8331bf35497522328c16f2d7305b6bfb1d6df9c987d7e48611083cb9fae96996`  
		Last Modified: Thu, 19 Oct 2017 16:56:56 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6facbff585a5109624d1b150e3dcd167deccf602968fdbf0f9a0e43f5fef3b0`  
		Last Modified: Thu, 19 Oct 2017 17:33:18 GMT  
		Size: 5.3 MB (5298614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e2d4686bfda58bf7a83cfa79ce30bdd80db4d37a28a36147e1fc7f8e761b29`  
		Last Modified: Fri, 03 Nov 2017 10:43:22 GMT  
		Size: 43.9 MB (43921644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:artful-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:5d4c197986ef8033e7366a6a55ac820ce1baa9da59cf3421404bbc480ae33fb9
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.4 MB (93430627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19282c94ddac14c7a522e0e6a9b0398e54fe9b00054fe2d04f8e76d6f29a454f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Oct 2017 16:56:07 GMT
ADD file:076cee6466bce5b77bbc3b6b359831aa5810b3497b7ebdfbfa18b455ebd31a29 in / 
# Thu, 19 Oct 2017 16:56:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Oct 2017 16:56:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Oct 2017 16:56:09 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Thu, 19 Oct 2017 16:56:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Oct 2017 16:56:10 GMT
CMD ["/bin/bash"]
# Thu, 19 Oct 2017 17:13:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 23:06:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Nov 2017 23:07:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a83e1d13695f175cd2f542162df4f77ac453af29c8e6bd7eb98d7a7e7ab3828`  
		Last Modified: Thu, 19 Oct 2017 16:57:02 GMT  
		Size: 40.0 MB (40037962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb63f1ac3d814a8a905b9b349010f37e65d877d7c1282f54c1758690253b4bd`  
		Last Modified: Thu, 19 Oct 2017 16:56:57 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77dd6cd1aef7efb5c960f2bf83aaec92bff425fc042ee74ee716e5c05f5c5dd5`  
		Last Modified: Thu, 19 Oct 2017 16:56:57 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf247371706b0726dc00efbb0855246efa3d866f5d0a2260422457ef01424e0`  
		Last Modified: Thu, 19 Oct 2017 16:56:56 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8331bf35497522328c16f2d7305b6bfb1d6df9c987d7e48611083cb9fae96996`  
		Last Modified: Thu, 19 Oct 2017 16:56:56 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08155ce50231367d35326ae407be7c4493064f6baf53f29e4054caa3ed9198ec`  
		Last Modified: Thu, 19 Oct 2017 17:19:56 GMT  
		Size: 6.1 MB (6099489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2589f012033d9311c9a90a25ff9c70200985ec0d0657df3eec55b2f77e2a985`  
		Last Modified: Fri, 03 Nov 2017 00:04:39 GMT  
		Size: 47.3 MB (47290921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:artful-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8120068b386cdd7571b3a1ed9e97ce20701ac9ad0603536c4a13530424c7b29d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.6 MB (101623619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:962ebe220ae703d9c04993472a1343fb0d71bc2bfebdc6c77364ddc5ccbd7c94`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Oct 2017 16:56:00 GMT
ADD file:b74122be4f1003f3a8afd759e1e56733eb7d8ac02698486b65556e831ffe5627 in / 
# Thu, 19 Oct 2017 16:56:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Oct 2017 16:56:14 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Oct 2017 16:56:21 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Thu, 19 Oct 2017 16:56:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Oct 2017 16:56:32 GMT
CMD ["/bin/bash"]
# Thu, 19 Oct 2017 17:15:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 15:45:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Nov 2017 15:48:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2337aaea32bf8cd758fe4f931358024fd68cb4d79019859326d9665a66b75cb9`  
		Last Modified: Thu, 19 Oct 2017 16:57:30 GMT  
		Size: 42.4 MB (42449498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf02bb6c20cfc307d42493dfa9d2e410a32dde821ac248ed69dd6a7df9d6562`  
		Last Modified: Thu, 19 Oct 2017 16:57:18 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac491d4677a40ab6396a4d562f9bb4868bbf37be3378f57066d9ff744e373888`  
		Last Modified: Thu, 19 Oct 2017 16:57:18 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccc3af7278f5db8e08c2fe132c9e86c0d39929e7831d4786ce45f0fc836a186`  
		Last Modified: Thu, 19 Oct 2017 16:57:18 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee67224a68dabad14949e47b84419539dfca9cf70927d64d056c78a6069626ea`  
		Last Modified: Thu, 19 Oct 2017 16:57:18 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c760aca2ed3fc46dfc8364aa48c8e4e2a922526bc410f825a61514784cd706`  
		Last Modified: Thu, 19 Oct 2017 17:49:56 GMT  
		Size: 5.9 MB (5943028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b675027b088b366164b7a8fca516ad52db46d727f61cebf78dde5d833a60040`  
		Last Modified: Thu, 02 Nov 2017 17:45:01 GMT  
		Size: 53.2 MB (53228832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:artful-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:49e7d002eacbffe217803e9edc605b97d7cc688deea796046fbc32bb0a272577
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89426495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:180cb66cc4f76ab9dabd63413f628de201fde4b33a716188bfb8ec61c1bcd67c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Oct 2017 16:55:44 GMT
ADD file:5c7510b171b1b7d6105fd03e9af0bc57fcf0171317d28a63c042e4bf2893c0d1 in / 
# Thu, 19 Oct 2017 16:55:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Oct 2017 16:55:46 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Oct 2017 16:55:46 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Thu, 19 Oct 2017 16:55:47 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Oct 2017 16:55:47 GMT
CMD ["/bin/bash"]
# Thu, 19 Oct 2017 17:12:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 16:35:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Nov 2017 16:36:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f8cc30fcfbb1531ddada75d028c4f2bd7adf9cbf709aa54d8777eeb284d7727d`  
		Last Modified: Thu, 19 Oct 2017 16:56:28 GMT  
		Size: 38.1 MB (38060264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03157d22d303f87aad86a5467a779446e96962ce972713d0c8101f415a7face`  
		Last Modified: Thu, 19 Oct 2017 16:56:22 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2ade42ec347c6c446d0085493af2f500aabdd8e83933e18d887b10912a045b`  
		Last Modified: Thu, 19 Oct 2017 16:56:21 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b6b0243c9476a6b812fd9d20502bbc1922fa90b44c5fc52d15df1fee6b7ae8`  
		Last Modified: Thu, 19 Oct 2017 16:56:22 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad030e2413b825303bbad9264c02cb00dae6d0bb18819c1247f973e7b16a6c1e`  
		Last Modified: Thu, 19 Oct 2017 16:56:22 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930956f81c68574bc794d5dfee64806cd1a2cc941079361d1fd39c500373bcc7`  
		Last Modified: Thu, 19 Oct 2017 17:15:49 GMT  
		Size: 5.7 MB (5730866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0297405362f10d00149b1277d440993fadbfde91edd27d523e22235520415aa`  
		Last Modified: Thu, 02 Nov 2017 16:52:15 GMT  
		Size: 45.6 MB (45633134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
