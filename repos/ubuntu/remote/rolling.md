## `ubuntu:rolling`

```console
$ docker pull ubuntu@sha256:571e383ddf851b1a8b9f6dc5d68855a5d23b75dda5b0e40b7649c7f4e023a996
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:rolling` - linux; amd64

```console
$ docker pull ubuntu@sha256:4a75aed1884321e9122bba5ab28b85e0a196415c3fa59b3e799a995d7bb14ae5
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39978688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8ad041f5225c51764dc85024620ce868a584f26699f75ef0d99dfa4664d449f`
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

### `ubuntu:rolling` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:14774326cbc05e13da0dd0f47e93419fb0b37f88bd679dfe2ae9ed2cbbc9ae8d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35788428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c026e9ebc285a716adcd8a4d947946c8b4faa1e596c1ea0d1d740dcf0f8abb`
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

### `ubuntu:rolling` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:e3ebf225382be6ef78303ce419136a71ba19862127a4f48da4bde4e0ebdfd463
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36936628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f10bc681a06f06ddac5781e64738348b9abb37bfab8ad80f8726cbb0394bf790`
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

### `ubuntu:rolling` - linux; 386

```console
$ docker pull ubuntu@sha256:0ded6199174f62d70ff62e6d7510b5e53804e499fbcdda056423f29ff3251174
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40791368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89b15b72ccaf857ce1a99227a21b1544ea3704b9e490590f90515f78a4f8ee78`
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

### `ubuntu:rolling` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:df111273a62a7268234b1b73e7298029a28dd0334798e49b08a46503811086ed
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43181084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7f35d66359d8c5490eaac0439814b44a6d10c8851d7fcc6e8efd6c0e9e29018`
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

### `ubuntu:rolling` - linux; s390x

```console
$ docker pull ubuntu@sha256:54ebca6746b8b0dafef9a287697c6ae8adfa4a604406d3ac432dfb7ad1806b69
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38700173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2819dbf130d6b5531ceff91361fe01744fdfc03fd222d166ea9a95794693fe3e`
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
