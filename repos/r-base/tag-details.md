<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:3.4.2`](#r-base342)
-	[`r-base:latest`](#r-baselatest)

## `r-base:3.4.2`

```console
$ docker pull r-base@sha256:2052f0dc09862bd3a3679fb4eea2581a78b2267ad2f55d7dc5c23a6b304bed3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `r-base:3.4.2` - linux; amd64

```console
$ docker pull r-base@sha256:3a6506a6f030ae9971b723b79db29eef5c2abc4ecb040d3f938143667b66cfa3
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.1 MB (270140652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ea165c4d1cc325d835c7fa9ea77a89ff41c2cca5562850c5ac9a57f0a849ea7`
-	Default Command: `["R"]`

```dockerfile
# Mon, 09 Oct 2017 21:33:57 GMT
ADD file:f2155b46067f1955669502cbb14d0fae745f29940234ec173d13f5e1f885f041 in / 
# Mon, 09 Oct 2017 21:33:57 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 02:45:21 GMT
MAINTAINER "Carl Boettiger and Dirk Eddelbuettel" rocker-maintainers@eddelbuettel.com
# Tue, 10 Oct 2017 02:45:22 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 10 Oct 2017 02:45:33 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:45:34 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 10 Oct 2017 02:45:38 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 10 Oct 2017 02:45:38 GMT
ENV LANG=en_US.UTF-8
# Tue, 10 Oct 2017 02:45:39 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list 	&& echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Tue, 10 Oct 2017 02:45:39 GMT
ENV R_BASE_VERSION=3.4.2
# Tue, 10 Oct 2017 02:47:16 GMT
RUN apt-get update 	&& apt-get install -t unstable -y --no-install-recommends 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}* 		r-base-dev=${R_BASE_VERSION}* 		r-recommended=${R_BASE_VERSION}*         && echo 'options(repos = c(CRAN = "https://cran.rstudio.com/"), download.file.method = "libcurl")' >> /etc/R/Rprofile.site         && echo 'source("/etc/R/Rprofile.site")' >> /etc/littler.r 	&& ln -s /usr/share/doc/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/share/doc/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/share/doc/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/share/doc/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:47:16 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:31d9d91516b8b9604769d1dd4a951948cd1fe368ee7cc8b73bc129b37ee9b3d6`  
		Last Modified: Mon, 09 Oct 2017 21:42:49 GMT  
		Size: 47.5 MB (47527284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd4ad4c36766953cb829872d4c2ed795e00ee2dadc122c413025f31bc211838`  
		Last Modified: Tue, 10 Oct 2017 02:47:37 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a973c39349e45bb6f90732a319ed48c56a4c5fb41c0dded13239ff65338d661c`  
		Last Modified: Tue, 10 Oct 2017 02:47:41 GMT  
		Size: 23.4 MB (23409454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f72c7085f127f88af1983832f57e719aa4bbbe56bcf890665ceb20ce138bde8`  
		Last Modified: Tue, 10 Oct 2017 02:47:37 GMT  
		Size: 425.9 KB (425870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4fe3ed5e1b8253abee00cbe26aac87bc3237d413de4d7c15dc426f1ad27132`  
		Last Modified: Tue, 10 Oct 2017 02:47:37 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67246ad3763ed7c4fd0334d081a1a5da80b291f9a5c173e7cfb363c60c4c9b0f`  
		Last Modified: Tue, 10 Oct 2017 02:48:03 GMT  
		Size: 198.8 MB (198775762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:2052f0dc09862bd3a3679fb4eea2581a78b2267ad2f55d7dc5c23a6b304bed3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:3a6506a6f030ae9971b723b79db29eef5c2abc4ecb040d3f938143667b66cfa3
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.1 MB (270140652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ea165c4d1cc325d835c7fa9ea77a89ff41c2cca5562850c5ac9a57f0a849ea7`
-	Default Command: `["R"]`

```dockerfile
# Mon, 09 Oct 2017 21:33:57 GMT
ADD file:f2155b46067f1955669502cbb14d0fae745f29940234ec173d13f5e1f885f041 in / 
# Mon, 09 Oct 2017 21:33:57 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 02:45:21 GMT
MAINTAINER "Carl Boettiger and Dirk Eddelbuettel" rocker-maintainers@eddelbuettel.com
# Tue, 10 Oct 2017 02:45:22 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 10 Oct 2017 02:45:33 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:45:34 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 10 Oct 2017 02:45:38 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 10 Oct 2017 02:45:38 GMT
ENV LANG=en_US.UTF-8
# Tue, 10 Oct 2017 02:45:39 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list 	&& echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Tue, 10 Oct 2017 02:45:39 GMT
ENV R_BASE_VERSION=3.4.2
# Tue, 10 Oct 2017 02:47:16 GMT
RUN apt-get update 	&& apt-get install -t unstable -y --no-install-recommends 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}* 		r-base-dev=${R_BASE_VERSION}* 		r-recommended=${R_BASE_VERSION}*         && echo 'options(repos = c(CRAN = "https://cran.rstudio.com/"), download.file.method = "libcurl")' >> /etc/R/Rprofile.site         && echo 'source("/etc/R/Rprofile.site")' >> /etc/littler.r 	&& ln -s /usr/share/doc/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/share/doc/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/share/doc/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/share/doc/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2017 02:47:16 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:31d9d91516b8b9604769d1dd4a951948cd1fe368ee7cc8b73bc129b37ee9b3d6`  
		Last Modified: Mon, 09 Oct 2017 21:42:49 GMT  
		Size: 47.5 MB (47527284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd4ad4c36766953cb829872d4c2ed795e00ee2dadc122c413025f31bc211838`  
		Last Modified: Tue, 10 Oct 2017 02:47:37 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a973c39349e45bb6f90732a319ed48c56a4c5fb41c0dded13239ff65338d661c`  
		Last Modified: Tue, 10 Oct 2017 02:47:41 GMT  
		Size: 23.4 MB (23409454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f72c7085f127f88af1983832f57e719aa4bbbe56bcf890665ceb20ce138bde8`  
		Last Modified: Tue, 10 Oct 2017 02:47:37 GMT  
		Size: 425.9 KB (425870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4fe3ed5e1b8253abee00cbe26aac87bc3237d413de4d7c15dc426f1ad27132`  
		Last Modified: Tue, 10 Oct 2017 02:47:37 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67246ad3763ed7c4fd0334d081a1a5da80b291f9a5c173e7cfb363c60c4c9b0f`  
		Last Modified: Tue, 10 Oct 2017 02:48:03 GMT  
		Size: 198.8 MB (198775762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
