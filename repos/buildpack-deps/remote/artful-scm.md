## `buildpack-deps:artful-scm`

```console
$ docker pull buildpack-deps@sha256:2e01ebc0a0b6636562778c6f19fce5180a2874a0513aa5e8077fb2e6a62cd78a
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
$ docker pull buildpack-deps@sha256:d6f828f6ac46d49f85eb83a253287a4971372a08820281623decf0536651a3d3
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.8 MB (91777188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01c512304311446c6aa153c50e8bf8a1b8b65515774f4656f839b239cf1989f0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Jan 2018 18:03:48 GMT
ADD file:ec58ed9c4227aa7839c3472e7f02851c76b81bd0c3e6b946871f919de8a6af99 in / 
# Thu, 25 Jan 2018 18:03:49 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Jan 2018 18:03:50 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 25 Jan 2018 18:03:51 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Thu, 25 Jan 2018 18:03:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Jan 2018 18:03:52 GMT
CMD ["/bin/bash"]
# Thu, 25 Jan 2018 22:47:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 25 Jan 2018 22:47:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 25 Jan 2018 22:49:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:18c8f805be45ea0f336b99a253692a8c974b07369f94f769feaa663e74d62881`  
		Last Modified: Thu, 25 Jan 2018 18:24:28 GMT  
		Size: 40.0 MB (39976211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7869fb3b98c44f3394fd0386abc807b877b34b2b2ba918707fa2729748d45d6`  
		Last Modified: Thu, 25 Jan 2018 18:24:15 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75000414ffb1e6f1b193b08d62d1367e9dff9290dd758f507f4ce88d655af8d`  
		Last Modified: Thu, 25 Jan 2018 18:24:15 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27c5092058d85ad4e9c133a1ce883777890baae684f6f43c8de9cc5650b066c`  
		Last Modified: Thu, 25 Jan 2018 18:24:15 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add65c7404ea79525338412ae724d5b866d1c53cd3ce592cbaac85cef6093f61`  
		Last Modified: Thu, 25 Jan 2018 18:24:15 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077d47163a8169582edd522db971ed5c21ba4b192240f0272cc39b370f3934e1`  
		Last Modified: Thu, 25 Jan 2018 23:37:10 GMT  
		Size: 6.1 MB (6056396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bf7912836d599e5293e050379b55b0f21d709a694d4efc79841212cbcb718d`  
		Last Modified: Thu, 25 Jan 2018 23:37:44 GMT  
		Size: 45.7 MB (45742104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:artful-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:71872350970ccd01f674bb22d3485d52a83472ae977b3b5a962304dab70f6451
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.7 MB (82738659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed30b5b817e91b9f2bd031ca910e483a42d502284c3c87be6b2250d13c6c9a2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Jan 2018 13:50:36 GMT
ADD file:16c5fbf097c774c1aeef960ef6ab8c4ad71fff4f1af49a15c70d17ce943cc9e2 in / 
# Fri, 26 Jan 2018 13:50:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 26 Jan 2018 13:50:38 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 26 Jan 2018 13:50:39 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 26 Jan 2018 13:50:39 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 26 Jan 2018 13:50:40 GMT
CMD ["/bin/bash"]
# Fri, 26 Jan 2018 14:11:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Jan 2018 14:11:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Jan 2018 14:12:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:add171a4aa5d25515d1d289e1042587a541dbe262ff9a116c9384f4022b6b47d`  
		Last Modified: Fri, 26 Jan 2018 13:52:24 GMT  
		Size: 35.8 MB (35785933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d044d57ca34ebbb756fbe9976fc39f04f306c5a1b9398ff9380f76357b38bf45`  
		Last Modified: Fri, 26 Jan 2018 13:52:15 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a5494025075f7dfebcd3582394f74075ec0f49fc54741dd727d0a80e1d7a20`  
		Last Modified: Fri, 26 Jan 2018 13:52:15 GMT  
		Size: 609.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d418e86e1953e34729085053d7de7a8ee0c5b8243cefe81e23fedcc982a0a606`  
		Last Modified: Fri, 26 Jan 2018 13:52:15 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894b58f4939abe46aee4804244663ba60b559b870a54bca8f2bf79dc0681a14c`  
		Last Modified: Fri, 26 Jan 2018 13:52:17 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8223c328ec4de3db1788c3b73043c145f0a63dd9b93165af5aa908bcf151590`  
		Last Modified: Fri, 26 Jan 2018 14:32:20 GMT  
		Size: 5.1 MB (5098961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51defff311edf26960bc66996ebd312a5ef90734d2c519bcc11e6783695e203`  
		Last Modified: Fri, 26 Jan 2018 14:32:44 GMT  
		Size: 41.9 MB (41851270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:artful-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6e7593a26b2580b97099ce8c089762fe735ef776286accfcd1223598327877d3
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.2 MB (86239369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a943ed27f220da42dd4f5caecc65a9aa3445eeb47274373aab72a9cbb9a7b7d4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Jan 2018 15:00:44 GMT
ADD file:c002d9046d272c6248707940fd8ac8c65b8ee95a099767b89f97e4b95fd25b6f in / 
# Fri, 26 Jan 2018 15:00:46 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 26 Jan 2018 15:00:48 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 26 Jan 2018 15:00:49 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 26 Jan 2018 15:00:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 26 Jan 2018 15:00:51 GMT
CMD ["/bin/bash"]
# Fri, 26 Jan 2018 15:29:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Jan 2018 15:29:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Jan 2018 15:30:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:690f5004fed06e103878d2c2d8b6f90554ed3be8107fe2e5695f48db7a52a0f6`  
		Last Modified: Fri, 26 Jan 2018 15:04:44 GMT  
		Size: 36.9 MB (36934229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb35a200b290063eb29af10a46e7f1f4eb9a98c3b653eddf21d8805aa8a8134`  
		Last Modified: Fri, 26 Jan 2018 15:03:06 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19cc0e591b350fb35db8581b7e37cd040456971dd84c3f353f878e572c1ad6b1`  
		Last Modified: Fri, 26 Jan 2018 15:03:05 GMT  
		Size: 536.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f29cb240b064bb1fd5e9d00d857065273d0a08c629d6ac53548d645cdf04ee2`  
		Last Modified: Fri, 26 Jan 2018 15:03:06 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddc4ce4a6378879651cab518130dee0db2b98533db3c7d720ea78a82e46b1ca`  
		Last Modified: Fri, 26 Jan 2018 15:03:06 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3b3d5597a22630a69d8426c01b3f454949ef926204b935995a319270437ad2`  
		Last Modified: Fri, 26 Jan 2018 16:22:28 GMT  
		Size: 5.3 MB (5336517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38db88a02105c2ab3f2b9d8fb3d49528a000c0f52911b3135ef9176638ff7e1f`  
		Last Modified: Fri, 26 Jan 2018 16:23:52 GMT  
		Size: 44.0 MB (43966224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:artful-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:fc7e13426424583b03e766a97be5a3c0637a0407994d898e1e6efa2e68fc2acc
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94250948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c1c47c61d8d9b1709d0cc85fb7b19bd0c7d9fde3ee8883e3ca4e264a0d41870`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Jan 2018 04:46:02 GMT
ADD file:8df5954491d410ef706a7ee9777a43b2b4eb537dab6624991120fffa50dbd4a9 in / 
# Fri, 26 Jan 2018 04:46:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 26 Jan 2018 04:46:04 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 26 Jan 2018 04:46:04 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 26 Jan 2018 04:46:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 26 Jan 2018 04:46:05 GMT
CMD ["/bin/bash"]
# Fri, 26 Jan 2018 07:58:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Jan 2018 07:58:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Jan 2018 07:59:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c72cd87dc0a80e71756a6b7d061f860dc89b03038145ead07a9e1c3297480f23`  
		Last Modified: Fri, 26 Jan 2018 05:38:34 GMT  
		Size: 40.8 MB (40788939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbaf237fa8472491aded309190fd4d39a17ce8528e910286b3f528238973f0f`  
		Last Modified: Fri, 26 Jan 2018 05:38:18 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584e47ac45bfb7676978cd82b88996d676c04fef450d81664b62d1bdd10d612f`  
		Last Modified: Fri, 26 Jan 2018 05:38:18 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88369684dc1e966d2dc8cb45a4207262fff1d61be73eeb1a73149f074aeb59a`  
		Last Modified: Fri, 26 Jan 2018 05:38:18 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d229cb8cf5afa9f212ad5d1af159d811a970e31cb77022568695fa08f529df8`  
		Last Modified: Fri, 26 Jan 2018 05:38:18 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0158c216dafbcda46b9fc6bc5dffdf3cb34345951bb6c960e91ea67d21541957`  
		Last Modified: Fri, 26 Jan 2018 09:39:02 GMT  
		Size: 6.1 MB (6110342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919d61362d63b720d1078e4f35e8cb43a7df14e355d6759ee91d1d3504b07c08`  
		Last Modified: Fri, 26 Jan 2018 09:47:44 GMT  
		Size: 47.3 MB (47349238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:artful-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:cf0fccee56b7503aed2ac7280f8d9e83c11d83dc9573934f2846f3cac431593f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102608939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1216c7491a97735325ffdc65488eacedbfe07e34d9596f3a80eff622b1dc8294`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Jan 2018 03:39:26 GMT
ADD file:dbc41942f2c0a1878986d510a8b356aba5b8c6a2d6bae0382fa95147e158ed91 in / 
# Fri, 26 Jan 2018 03:39:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 26 Jan 2018 03:39:32 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 26 Jan 2018 03:39:37 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 26 Jan 2018 03:39:40 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 26 Jan 2018 03:39:45 GMT
CMD ["/bin/bash"]
# Fri, 26 Jan 2018 04:00:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Jan 2018 04:01:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Jan 2018 04:02:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e46125f5e240ed2ce4b5fc53006238d7841a1ab2302fc8849590378691af042`  
		Last Modified: Fri, 26 Jan 2018 03:41:59 GMT  
		Size: 43.2 MB (43178612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167aa3fa99c6922d4aea0a6f9ffbb37d26c54a83cd1321d1645392f5af1cf269`  
		Last Modified: Fri, 26 Jan 2018 03:41:47 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964fc38588591a61e53b9d7417e2995fff64f41c3503321dcffaf32eb1aaf4b5`  
		Last Modified: Fri, 26 Jan 2018 03:41:47 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca94695917e8f7cc8d237ec1b13915c27342ae8054d33d20a46cf74dee0ffd3`  
		Last Modified: Fri, 26 Jan 2018 03:41:47 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0402bff2b28216dec30e75567ad2177e38571adf301bb746c717b15d353fbaaa`  
		Last Modified: Fri, 26 Jan 2018 03:41:47 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80ea885fbfefc5a5ca3c6ca06ee93c292243618c83e5911fc86a89c61449831`  
		Last Modified: Fri, 26 Jan 2018 04:47:01 GMT  
		Size: 6.1 MB (6129664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be10b54d7f5b434088809ee87e49fbca6fd5160b67a4193a037b78f0bdfef0f8`  
		Last Modified: Fri, 26 Jan 2018 04:47:26 GMT  
		Size: 53.3 MB (53298191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:artful-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:158c7ae51a91341bc029a2b3191bfd9f2f19c0464a96fc35ecc743214f17ca53
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.1 MB (90121582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b05248c941bb5aef523762581b9f0a5c158f56e248f8446e9472a9ec60b8c12`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Jan 2018 14:15:25 GMT
ADD file:ce2fc343ce9ce59bf14e4d01df5ec72b6954323b0e74bab3d608dc7d9aa89494 in / 
# Fri, 26 Jan 2018 14:15:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 26 Jan 2018 14:15:26 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 26 Jan 2018 14:15:26 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 26 Jan 2018 14:15:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 26 Jan 2018 14:15:27 GMT
CMD ["/bin/bash"]
# Fri, 26 Jan 2018 14:32:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Jan 2018 14:32:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Jan 2018 14:32:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e14223442e09c33da04a729961b6efe41dc6c0559a31acc3780a9527b38c288d`  
		Last Modified: Fri, 26 Jan 2018 14:16:07 GMT  
		Size: 38.7 MB (38697775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f0163c96ad8a32651efe3d24296c37e9ac1dacff4f111e16756c1f992d2704`  
		Last Modified: Fri, 26 Jan 2018 14:15:56 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf7eff8d6a6b663f50952f04ebaea184f771a69286fa798355ee3efcc9a7707`  
		Last Modified: Fri, 26 Jan 2018 14:15:56 GMT  
		Size: 539.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223950c60c9c54933018b1dae8b27a2f01f5ff95d286450ac8705e9ef76fe5ff`  
		Last Modified: Fri, 26 Jan 2018 14:15:56 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5e8977386f8286e8ea57d55cf2d68e4593895a741535ae77908b9ec1dcb9d3`  
		Last Modified: Fri, 26 Jan 2018 14:15:56 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a708f96c30c9dfbd1155ffc8e5baa159554c88c62425421945809b25c3a035b2`  
		Last Modified: Fri, 26 Jan 2018 14:37:49 GMT  
		Size: 5.7 MB (5742152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a0314b3e074fdf9383fcd531e3d88a9804fb75fca1abae7bd790114a6f5beb`  
		Last Modified: Fri, 26 Jan 2018 14:38:05 GMT  
		Size: 45.7 MB (45679257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
