<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mono`

-	[`mono:4`](#mono4)
-	[`mono:4.8`](#mono48)
-	[`mono:4.8.0`](#mono480)
-	[`mono:4.8.0.524`](#mono480524)
-	[`mono:5`](#mono5)
-	[`mono:5.2`](#mono52)
-	[`mono:5.2.0`](#mono520)
-	[`mono:5.2.0.224`](#mono520224)
-	[`mono:5.2.0.224-slim`](#mono520224-slim)
-	[`mono:5.2.0-slim`](#mono520-slim)
-	[`mono:5.2-slim`](#mono52-slim)
-	[`mono:5.4`](#mono54)
-	[`mono:5.4.0`](#mono540)
-	[`mono:5.4.0.201`](#mono540201)
-	[`mono:5.4.0.201-slim`](#mono540201-slim)
-	[`mono:5.4.0-slim`](#mono540-slim)
-	[`mono:5.4-slim`](#mono54-slim)
-	[`mono:5-slim`](#mono5-slim)
-	[`mono:latest`](#monolatest)
-	[`mono:slim`](#monoslim)

## `mono:4`

```console
$ docker pull mono@sha256:3f90a8e280fef04a9699bf763ce7740b6560bb19cce78e6afca9d58749e92097
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; 386

### `mono:4` - linux; amd64

```console
$ docker pull mono@sha256:7e112f01b77e0e446befa2481ec400732e0b69615d47368071ed7b07b442d67c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.0 MB (153025157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c63f7a540900076d56a503a7e7e10667d1f91e9bfac66c58143f52f2d524056f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:34:51 GMT
ADD file:4a0b4ab0f637224302bf3f7a7eedc5b75a404bc1188499ef2f98edb7ce44d0ed in / 
# Mon, 09 Oct 2017 21:34:51 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:29:48 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Sat, 04 Nov 2017 02:29:49 GMT
ENV MONO_VERSION=4.8.0.524
# Sat, 04 Nov 2017 02:30:14 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Sat, 04 Nov 2017 02:30:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:32:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:39e552a2b1f74a9985244528219d26fc1c27f1447a3d04e64b63bd70a4e68e2c`  
		Last Modified: Mon, 09 Oct 2017 21:44:19 GMT  
		Size: 38.1 MB (38103127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb49ecabf267887e706e892e8ec4289721ac183c987c2ef251c67c82e246e5b0`  
		Last Modified: Sat, 04 Nov 2017 02:37:19 GMT  
		Size: 7.8 MB (7757014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f831d0d16fed096940542da604332943cf125ccd24e4bbc259e74a97023550f4`  
		Last Modified: Sat, 04 Nov 2017 02:37:15 GMT  
		Size: 29.9 KB (29905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b4ca7020dd4bffa0a4864acd8a24d646c1c3b4f0a7eb0147d3e1a3ff4fc90d`  
		Last Modified: Sat, 04 Nov 2017 02:37:52 GMT  
		Size: 107.1 MB (107135111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:4` - linux; arm variant v7

```console
$ docker pull mono@sha256:c8282c63b0657e85ca373a757d4a850fb0cfe6130a71e8bdf25d4a2f3c74429c
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138941885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6525f935a0b30889a88f34dbc57ef3b51a1808ad464e212dde3c2d792bc7c410`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:47:03 GMT
ADD file:2e5b4a4fc5b75973c1d5baf0c2d71c37c885ed3b7f8aa0b0b9f34ed22cd4b952 in / 
# Mon, 09 Oct 2017 21:47:04 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:42:44 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Mon, 09 Oct 2017 22:42:44 GMT
ENV MONO_VERSION=4.8.0.524
# Mon, 09 Oct 2017 22:43:00 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Mon, 09 Oct 2017 22:43:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:44:12 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:485e828d0b07d98838a9442f5d3a10b1e2bf33bfd798a57660b9133a8fa44228`  
		Last Modified: Mon, 09 Oct 2017 21:55:54 GMT  
		Size: 35.7 MB (35656407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4ba70ddab89634918ba367ef6ac77d5596028f4dc763528650b2c78ed6a23a`  
		Last Modified: Mon, 09 Oct 2017 22:48:15 GMT  
		Size: 7.2 MB (7185219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aceca04ff4a1d3d3f4e6e2cd90d650f727125cc39e1f817ab8f852a68a21ce9`  
		Last Modified: Mon, 09 Oct 2017 22:48:13 GMT  
		Size: 29.9 KB (29906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d2d9df1964d7221d99ece2c0451f48ba27f196b87d09e10707f9d0e3c0979f`  
		Last Modified: Mon, 09 Oct 2017 22:48:49 GMT  
		Size: 96.1 MB (96070353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:4` - linux; 386

```console
$ docker pull mono@sha256:c25f804fcdba6c94aa923cde4cfcbde6242c2fe2b51d4344ed0b22c7fa6d2bce
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.0 MB (153031073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f62f6604e72f7ccc28b7503d620b28645f4d1b70ec087c962189fd756c15ea5`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:46:33 GMT
ADD file:f5171b66c2082a6d1e8b5777fb0292564788effc1338f44ece9dc7b4eccd2374 in / 
# Mon, 09 Oct 2017 21:46:33 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:27:38 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Mon, 09 Oct 2017 22:27:38 GMT
ENV MONO_VERSION=4.8.0.524
# Mon, 09 Oct 2017 22:27:55 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Mon, 09 Oct 2017 22:27:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:29:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:827d66beec7d37d54d975d338834e5a422854c71c84b2ad3b652f85537277bae`  
		Last Modified: Mon, 09 Oct 2017 22:00:34 GMT  
		Size: 37.4 MB (37433248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8070f4756a69574994ccaa2600f91a9a0120f8c4d6abd8b55d4b30c2674c32b1`  
		Last Modified: Mon, 09 Oct 2017 22:41:17 GMT  
		Size: 9.6 MB (9606718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee92c800704e678bd3b210eca76793a8b500af53c626e263ffa41f1017521c72`  
		Last Modified: Mon, 09 Oct 2017 22:41:14 GMT  
		Size: 29.9 KB (29907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeeaa104eb3b78a5310fd9e38ec0e7f86cd3c9018dd91563d05da2bc8ed74ed5`  
		Last Modified: Mon, 09 Oct 2017 22:41:40 GMT  
		Size: 106.0 MB (105961200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:4.8`

```console
$ docker pull mono@sha256:3f90a8e280fef04a9699bf763ce7740b6560bb19cce78e6afca9d58749e92097
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; 386

### `mono:4.8` - linux; amd64

```console
$ docker pull mono@sha256:7e112f01b77e0e446befa2481ec400732e0b69615d47368071ed7b07b442d67c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.0 MB (153025157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c63f7a540900076d56a503a7e7e10667d1f91e9bfac66c58143f52f2d524056f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:34:51 GMT
ADD file:4a0b4ab0f637224302bf3f7a7eedc5b75a404bc1188499ef2f98edb7ce44d0ed in / 
# Mon, 09 Oct 2017 21:34:51 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:29:48 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Sat, 04 Nov 2017 02:29:49 GMT
ENV MONO_VERSION=4.8.0.524
# Sat, 04 Nov 2017 02:30:14 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Sat, 04 Nov 2017 02:30:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:32:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:39e552a2b1f74a9985244528219d26fc1c27f1447a3d04e64b63bd70a4e68e2c`  
		Last Modified: Mon, 09 Oct 2017 21:44:19 GMT  
		Size: 38.1 MB (38103127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb49ecabf267887e706e892e8ec4289721ac183c987c2ef251c67c82e246e5b0`  
		Last Modified: Sat, 04 Nov 2017 02:37:19 GMT  
		Size: 7.8 MB (7757014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f831d0d16fed096940542da604332943cf125ccd24e4bbc259e74a97023550f4`  
		Last Modified: Sat, 04 Nov 2017 02:37:15 GMT  
		Size: 29.9 KB (29905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b4ca7020dd4bffa0a4864acd8a24d646c1c3b4f0a7eb0147d3e1a3ff4fc90d`  
		Last Modified: Sat, 04 Nov 2017 02:37:52 GMT  
		Size: 107.1 MB (107135111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:4.8` - linux; arm variant v7

```console
$ docker pull mono@sha256:c8282c63b0657e85ca373a757d4a850fb0cfe6130a71e8bdf25d4a2f3c74429c
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138941885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6525f935a0b30889a88f34dbc57ef3b51a1808ad464e212dde3c2d792bc7c410`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:47:03 GMT
ADD file:2e5b4a4fc5b75973c1d5baf0c2d71c37c885ed3b7f8aa0b0b9f34ed22cd4b952 in / 
# Mon, 09 Oct 2017 21:47:04 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:42:44 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Mon, 09 Oct 2017 22:42:44 GMT
ENV MONO_VERSION=4.8.0.524
# Mon, 09 Oct 2017 22:43:00 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Mon, 09 Oct 2017 22:43:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:44:12 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:485e828d0b07d98838a9442f5d3a10b1e2bf33bfd798a57660b9133a8fa44228`  
		Last Modified: Mon, 09 Oct 2017 21:55:54 GMT  
		Size: 35.7 MB (35656407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4ba70ddab89634918ba367ef6ac77d5596028f4dc763528650b2c78ed6a23a`  
		Last Modified: Mon, 09 Oct 2017 22:48:15 GMT  
		Size: 7.2 MB (7185219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aceca04ff4a1d3d3f4e6e2cd90d650f727125cc39e1f817ab8f852a68a21ce9`  
		Last Modified: Mon, 09 Oct 2017 22:48:13 GMT  
		Size: 29.9 KB (29906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d2d9df1964d7221d99ece2c0451f48ba27f196b87d09e10707f9d0e3c0979f`  
		Last Modified: Mon, 09 Oct 2017 22:48:49 GMT  
		Size: 96.1 MB (96070353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:4.8` - linux; 386

```console
$ docker pull mono@sha256:c25f804fcdba6c94aa923cde4cfcbde6242c2fe2b51d4344ed0b22c7fa6d2bce
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.0 MB (153031073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f62f6604e72f7ccc28b7503d620b28645f4d1b70ec087c962189fd756c15ea5`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:46:33 GMT
ADD file:f5171b66c2082a6d1e8b5777fb0292564788effc1338f44ece9dc7b4eccd2374 in / 
# Mon, 09 Oct 2017 21:46:33 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:27:38 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Mon, 09 Oct 2017 22:27:38 GMT
ENV MONO_VERSION=4.8.0.524
# Mon, 09 Oct 2017 22:27:55 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Mon, 09 Oct 2017 22:27:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:29:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:827d66beec7d37d54d975d338834e5a422854c71c84b2ad3b652f85537277bae`  
		Last Modified: Mon, 09 Oct 2017 22:00:34 GMT  
		Size: 37.4 MB (37433248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8070f4756a69574994ccaa2600f91a9a0120f8c4d6abd8b55d4b30c2674c32b1`  
		Last Modified: Mon, 09 Oct 2017 22:41:17 GMT  
		Size: 9.6 MB (9606718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee92c800704e678bd3b210eca76793a8b500af53c626e263ffa41f1017521c72`  
		Last Modified: Mon, 09 Oct 2017 22:41:14 GMT  
		Size: 29.9 KB (29907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeeaa104eb3b78a5310fd9e38ec0e7f86cd3c9018dd91563d05da2bc8ed74ed5`  
		Last Modified: Mon, 09 Oct 2017 22:41:40 GMT  
		Size: 106.0 MB (105961200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:4.8.0`

```console
$ docker pull mono@sha256:3f90a8e280fef04a9699bf763ce7740b6560bb19cce78e6afca9d58749e92097
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; 386

### `mono:4.8.0` - linux; amd64

```console
$ docker pull mono@sha256:7e112f01b77e0e446befa2481ec400732e0b69615d47368071ed7b07b442d67c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.0 MB (153025157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c63f7a540900076d56a503a7e7e10667d1f91e9bfac66c58143f52f2d524056f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:34:51 GMT
ADD file:4a0b4ab0f637224302bf3f7a7eedc5b75a404bc1188499ef2f98edb7ce44d0ed in / 
# Mon, 09 Oct 2017 21:34:51 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:29:48 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Sat, 04 Nov 2017 02:29:49 GMT
ENV MONO_VERSION=4.8.0.524
# Sat, 04 Nov 2017 02:30:14 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Sat, 04 Nov 2017 02:30:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:32:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:39e552a2b1f74a9985244528219d26fc1c27f1447a3d04e64b63bd70a4e68e2c`  
		Last Modified: Mon, 09 Oct 2017 21:44:19 GMT  
		Size: 38.1 MB (38103127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb49ecabf267887e706e892e8ec4289721ac183c987c2ef251c67c82e246e5b0`  
		Last Modified: Sat, 04 Nov 2017 02:37:19 GMT  
		Size: 7.8 MB (7757014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f831d0d16fed096940542da604332943cf125ccd24e4bbc259e74a97023550f4`  
		Last Modified: Sat, 04 Nov 2017 02:37:15 GMT  
		Size: 29.9 KB (29905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b4ca7020dd4bffa0a4864acd8a24d646c1c3b4f0a7eb0147d3e1a3ff4fc90d`  
		Last Modified: Sat, 04 Nov 2017 02:37:52 GMT  
		Size: 107.1 MB (107135111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:4.8.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:c8282c63b0657e85ca373a757d4a850fb0cfe6130a71e8bdf25d4a2f3c74429c
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138941885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6525f935a0b30889a88f34dbc57ef3b51a1808ad464e212dde3c2d792bc7c410`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:47:03 GMT
ADD file:2e5b4a4fc5b75973c1d5baf0c2d71c37c885ed3b7f8aa0b0b9f34ed22cd4b952 in / 
# Mon, 09 Oct 2017 21:47:04 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:42:44 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Mon, 09 Oct 2017 22:42:44 GMT
ENV MONO_VERSION=4.8.0.524
# Mon, 09 Oct 2017 22:43:00 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Mon, 09 Oct 2017 22:43:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:44:12 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:485e828d0b07d98838a9442f5d3a10b1e2bf33bfd798a57660b9133a8fa44228`  
		Last Modified: Mon, 09 Oct 2017 21:55:54 GMT  
		Size: 35.7 MB (35656407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4ba70ddab89634918ba367ef6ac77d5596028f4dc763528650b2c78ed6a23a`  
		Last Modified: Mon, 09 Oct 2017 22:48:15 GMT  
		Size: 7.2 MB (7185219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aceca04ff4a1d3d3f4e6e2cd90d650f727125cc39e1f817ab8f852a68a21ce9`  
		Last Modified: Mon, 09 Oct 2017 22:48:13 GMT  
		Size: 29.9 KB (29906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d2d9df1964d7221d99ece2c0451f48ba27f196b87d09e10707f9d0e3c0979f`  
		Last Modified: Mon, 09 Oct 2017 22:48:49 GMT  
		Size: 96.1 MB (96070353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:4.8.0` - linux; 386

```console
$ docker pull mono@sha256:c25f804fcdba6c94aa923cde4cfcbde6242c2fe2b51d4344ed0b22c7fa6d2bce
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.0 MB (153031073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f62f6604e72f7ccc28b7503d620b28645f4d1b70ec087c962189fd756c15ea5`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:46:33 GMT
ADD file:f5171b66c2082a6d1e8b5777fb0292564788effc1338f44ece9dc7b4eccd2374 in / 
# Mon, 09 Oct 2017 21:46:33 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:27:38 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Mon, 09 Oct 2017 22:27:38 GMT
ENV MONO_VERSION=4.8.0.524
# Mon, 09 Oct 2017 22:27:55 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Mon, 09 Oct 2017 22:27:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:29:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:827d66beec7d37d54d975d338834e5a422854c71c84b2ad3b652f85537277bae`  
		Last Modified: Mon, 09 Oct 2017 22:00:34 GMT  
		Size: 37.4 MB (37433248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8070f4756a69574994ccaa2600f91a9a0120f8c4d6abd8b55d4b30c2674c32b1`  
		Last Modified: Mon, 09 Oct 2017 22:41:17 GMT  
		Size: 9.6 MB (9606718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee92c800704e678bd3b210eca76793a8b500af53c626e263ffa41f1017521c72`  
		Last Modified: Mon, 09 Oct 2017 22:41:14 GMT  
		Size: 29.9 KB (29907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeeaa104eb3b78a5310fd9e38ec0e7f86cd3c9018dd91563d05da2bc8ed74ed5`  
		Last Modified: Mon, 09 Oct 2017 22:41:40 GMT  
		Size: 106.0 MB (105961200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:4.8.0.524`

```console
$ docker pull mono@sha256:3f90a8e280fef04a9699bf763ce7740b6560bb19cce78e6afca9d58749e92097
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; 386

### `mono:4.8.0.524` - linux; amd64

```console
$ docker pull mono@sha256:7e112f01b77e0e446befa2481ec400732e0b69615d47368071ed7b07b442d67c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.0 MB (153025157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c63f7a540900076d56a503a7e7e10667d1f91e9bfac66c58143f52f2d524056f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:34:51 GMT
ADD file:4a0b4ab0f637224302bf3f7a7eedc5b75a404bc1188499ef2f98edb7ce44d0ed in / 
# Mon, 09 Oct 2017 21:34:51 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:29:48 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Sat, 04 Nov 2017 02:29:49 GMT
ENV MONO_VERSION=4.8.0.524
# Sat, 04 Nov 2017 02:30:14 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Sat, 04 Nov 2017 02:30:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:32:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:39e552a2b1f74a9985244528219d26fc1c27f1447a3d04e64b63bd70a4e68e2c`  
		Last Modified: Mon, 09 Oct 2017 21:44:19 GMT  
		Size: 38.1 MB (38103127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb49ecabf267887e706e892e8ec4289721ac183c987c2ef251c67c82e246e5b0`  
		Last Modified: Sat, 04 Nov 2017 02:37:19 GMT  
		Size: 7.8 MB (7757014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f831d0d16fed096940542da604332943cf125ccd24e4bbc259e74a97023550f4`  
		Last Modified: Sat, 04 Nov 2017 02:37:15 GMT  
		Size: 29.9 KB (29905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b4ca7020dd4bffa0a4864acd8a24d646c1c3b4f0a7eb0147d3e1a3ff4fc90d`  
		Last Modified: Sat, 04 Nov 2017 02:37:52 GMT  
		Size: 107.1 MB (107135111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:4.8.0.524` - linux; arm variant v7

```console
$ docker pull mono@sha256:c8282c63b0657e85ca373a757d4a850fb0cfe6130a71e8bdf25d4a2f3c74429c
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138941885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6525f935a0b30889a88f34dbc57ef3b51a1808ad464e212dde3c2d792bc7c410`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:47:03 GMT
ADD file:2e5b4a4fc5b75973c1d5baf0c2d71c37c885ed3b7f8aa0b0b9f34ed22cd4b952 in / 
# Mon, 09 Oct 2017 21:47:04 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:42:44 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Mon, 09 Oct 2017 22:42:44 GMT
ENV MONO_VERSION=4.8.0.524
# Mon, 09 Oct 2017 22:43:00 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Mon, 09 Oct 2017 22:43:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:44:12 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:485e828d0b07d98838a9442f5d3a10b1e2bf33bfd798a57660b9133a8fa44228`  
		Last Modified: Mon, 09 Oct 2017 21:55:54 GMT  
		Size: 35.7 MB (35656407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4ba70ddab89634918ba367ef6ac77d5596028f4dc763528650b2c78ed6a23a`  
		Last Modified: Mon, 09 Oct 2017 22:48:15 GMT  
		Size: 7.2 MB (7185219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aceca04ff4a1d3d3f4e6e2cd90d650f727125cc39e1f817ab8f852a68a21ce9`  
		Last Modified: Mon, 09 Oct 2017 22:48:13 GMT  
		Size: 29.9 KB (29906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d2d9df1964d7221d99ece2c0451f48ba27f196b87d09e10707f9d0e3c0979f`  
		Last Modified: Mon, 09 Oct 2017 22:48:49 GMT  
		Size: 96.1 MB (96070353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:4.8.0.524` - linux; 386

```console
$ docker pull mono@sha256:c25f804fcdba6c94aa923cde4cfcbde6242c2fe2b51d4344ed0b22c7fa6d2bce
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.0 MB (153031073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f62f6604e72f7ccc28b7503d620b28645f4d1b70ec087c962189fd756c15ea5`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:46:33 GMT
ADD file:f5171b66c2082a6d1e8b5777fb0292564788effc1338f44ece9dc7b4eccd2374 in / 
# Mon, 09 Oct 2017 21:46:33 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:27:38 GMT
MAINTAINER Jo Shields <jo.shields@xamarin.com>
# Mon, 09 Oct 2017 22:27:38 GMT
ENV MONO_VERSION=4.8.0.524
# Mon, 09 Oct 2017 22:27:55 GMT
RUN apt-get update   && apt-get install -y curl   && rm -rf /var/lib/apt/lists/*
# Mon, 09 Oct 2017 22:27:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:29:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian wheezy/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-xamarin.list   && apt-get update   && apt-get install -y binutils mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:827d66beec7d37d54d975d338834e5a422854c71c84b2ad3b652f85537277bae`  
		Last Modified: Mon, 09 Oct 2017 22:00:34 GMT  
		Size: 37.4 MB (37433248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8070f4756a69574994ccaa2600f91a9a0120f8c4d6abd8b55d4b30c2674c32b1`  
		Last Modified: Mon, 09 Oct 2017 22:41:17 GMT  
		Size: 9.6 MB (9606718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee92c800704e678bd3b210eca76793a8b500af53c626e263ffa41f1017521c72`  
		Last Modified: Mon, 09 Oct 2017 22:41:14 GMT  
		Size: 29.9 KB (29907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeeaa104eb3b78a5310fd9e38ec0e7f86cd3c9018dd91563d05da2bc8ed74ed5`  
		Last Modified: Mon, 09 Oct 2017 22:41:40 GMT  
		Size: 106.0 MB (105961200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5`

```console
$ docker pull mono@sha256:17a2b85ec4c0942e16c4e6499a57e15ae9c09c2b9034b3ec58b0c23171311902
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5` - linux; amd64

```console
$ docker pull mono@sha256:932cd8cc4dfb08336ba3a5bd31feb361afdb82b5d2c203691fc956b3fce22a3d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.3 MB (167259115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d59c2a7018c7acd0024da96ecfcf7f1f778f58db827bb41788608e53494bb94b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:31:06 GMT
ADD file:187fe0df97a4c52984a518a454fb7ab3984ae7b541ede7ff84dd3c5da1ce1a59 in / 
# Mon, 09 Oct 2017 21:31:06 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:27:41 GMT
ENV MONO_VERSION=5.4.0.201
# Sat, 04 Nov 2017 02:27:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:28:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 04 Nov 2017 02:33:42 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d13d02fa248db2b423d6dbc8ec435675d23122f3939b5278b2156b75258e2259`  
		Last Modified: Mon, 09 Oct 2017 21:37:31 GMT  
		Size: 30.1 MB (30113318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8d78a964aa167e2e8dbfd3365f8445ed149628507a2aa9dfaacde4e97c83b3`  
		Last Modified: Sat, 04 Nov 2017 02:36:19 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c98de1760e34ac9792d43e7e171574a9d63a20a7bff3bf03e29ef3fa026362`  
		Last Modified: Sat, 04 Nov 2017 02:36:31 GMT  
		Size: 27.3 MB (27278585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59b45d6dbf7cd29de575aafcd18d219efc175d67692860d0f4b9be03a8efd4d`  
		Last Modified: Sat, 04 Nov 2017 02:38:48 GMT  
		Size: 109.9 MB (109865143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; arm variant v7

```console
$ docker pull mono@sha256:5189f8b756032897bb3d03f9e1d396ae72a70d1c66c6fcdd8e6b65f3d921fdb0
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.0 MB (147049823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff518dee16442d023eb4b88925989b6defdb55141b58851d208299cedff5f3c4`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:41 GMT
ADD file:0cd8ed314febdbf680645d20f346d9bac16fad5654c0b0d6ce2dec7c27c17b9a in / 
# Mon, 09 Oct 2017 21:42:41 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 17:51:32 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 17:51:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 17:52:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 17 Oct 2017 17:54:46 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:02620033936d6cf3514a813f366025a14370f5dfe654e89eaca3a56b357e88c2`  
		Last Modified: Mon, 09 Oct 2017 21:49:15 GMT  
		Size: 26.3 MB (26280982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebc5f99dc26f440db883809cd8379ade7a516c92b91b7d22ae6485b1278ab1f`  
		Last Modified: Tue, 17 Oct 2017 17:55:04 GMT  
		Size: 2.1 KB (2065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dec16e095e6115a08f0f8530cdfde275c707acbc3fbb2fcc735b863a95122c1`  
		Last Modified: Tue, 17 Oct 2017 17:55:12 GMT  
		Size: 22.0 MB (22035038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c10ba59aa47230cfdc9ee37e8f10718b4c017c2b4906920d0a1ff1b75edad`  
		Last Modified: Tue, 17 Oct 2017 17:56:17 GMT  
		Size: 98.7 MB (98731738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:a68c168b05a89256ded341eeebe49ae1ab5b96523ccbac7001c9e317a0dbd754
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161639631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd34d0efd84450956a53481cef2b10afae252d3f095fc8b53c3e142529cb3009`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:43:51 GMT
ADD file:75f5768db078e9eee90676141a2c9faa9ce02768b7c9cd6e588bdd5ffc0f65e3 in / 
# Mon, 09 Oct 2017 21:43:51 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 19:45:44 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 19:45:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 19:47:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 17 Oct 2017 19:53:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f2da27d97c13e9e531eda9577a28eb81b0d9034d7fd7e6575bd92744eed500f6`  
		Last Modified: Mon, 09 Oct 2017 21:53:20 GMT  
		Size: 27.5 MB (27480591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad3574e8978c5cdfc63d800a5b8666c43c9d93519dbe83105d3ffdb6bac9f8a`  
		Last Modified: Tue, 17 Oct 2017 19:53:55 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b32240292f03d8f265e50d58923a86660a5730b335e0dc5eb333ae7890cd921`  
		Last Modified: Tue, 17 Oct 2017 19:54:07 GMT  
		Size: 26.2 MB (26199265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d3f2ac099ead527a80c01317816b1cbcbcbe0d86403a39344baa73cda1baae`  
		Last Modified: Tue, 17 Oct 2017 19:55:50 GMT  
		Size: 108.0 MB (107957711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; 386

```console
$ docker pull mono@sha256:8b249344ca9584956ed7cb4635f29d545514ca86632705311522274cb2122121
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169638409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a8176ed9b7b0401eb795893a084727d27552a6c788477df53e8e54d4dbc386`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:30 GMT
ADD file:169ab3194fd1b25e06359d6eceb655093f44f0255c799ae8a3fc5bf8ba50fd8d in / 
# Mon, 09 Oct 2017 21:42:31 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 00:57:28 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 00:57:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 00:58:35 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 17 Oct 2017 01:00:06 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d8b3cf5f6e0f087738d5589b812e12f5b8781935412c95d15f2f77d68657b006`  
		Last Modified: Mon, 09 Oct 2017 21:48:54 GMT  
		Size: 30.3 MB (30264454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6db9a23ef19b82644ae3cc18a517df0a01579623915a4d0ea810e09c608927`  
		Last Modified: Tue, 17 Oct 2017 01:02:43 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e350d9d1943c6f652c74dd24e15cbdf943755f73fa0942cb0a1d8b12187ece`  
		Last Modified: Tue, 17 Oct 2017 01:02:49 GMT  
		Size: 29.1 MB (29051973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88be8b6ac98f875586bdbda4e5ffcbea6d9d7210c018d5213e75c5a0d6e1dd4a`  
		Last Modified: Tue, 17 Oct 2017 01:05:06 GMT  
		Size: 110.3 MB (110319916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.2`

```console
$ docker pull mono@sha256:e5cab442beb65facb3a1b94e03e2b3be12eb6a01bba10671eabae5119974e06d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.2` - linux; amd64

```console
$ docker pull mono@sha256:2bab2e198c6b2e6709ad099661fee069cf848324909d2117a140b5c94dff321c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.0 MB (170039966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46890077dea7bc77987471185929ac531dedea73b9d84161510e5bc32d64c99`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:31:06 GMT
ADD file:187fe0df97a4c52984a518a454fb7ab3984ae7b541ede7ff84dd3c5da1ce1a59 in / 
# Mon, 09 Oct 2017 21:31:06 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:28:50 GMT
ENV MONO_VERSION=5.2.0.224
# Sat, 04 Nov 2017 02:28:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:29:44 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 04 Nov 2017 02:35:57 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d13d02fa248db2b423d6dbc8ec435675d23122f3939b5278b2156b75258e2259`  
		Last Modified: Mon, 09 Oct 2017 21:37:31 GMT  
		Size: 30.1 MB (30113318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe72810a809a6d1606064b8b8fa821b63e3d0360d817e6ca17620a9e361a3589`  
		Last Modified: Sat, 04 Nov 2017 02:36:51 GMT  
		Size: 2.1 KB (2068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063ab3201702497ddbed07d6a63bb56da0d3b950a461355879b63bc3a0c72858`  
		Last Modified: Sat, 04 Nov 2017 02:37:02 GMT  
		Size: 27.2 MB (27240685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5a7483019efc574d9e22dfb88abff972e4d0fa71a4ff2fc01aec8b1438c081`  
		Last Modified: Sat, 04 Nov 2017 02:39:43 GMT  
		Size: 112.7 MB (112683895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.2` - linux; arm variant v7

```console
$ docker pull mono@sha256:6e9525473bd50383ed051de2684191f7b1fdc3302d5de4427784f167b11308a3
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148926184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fc645b4287b2e09c20b160ab09826ce50340bb8db3154dede723b22c120cf28`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:41 GMT
ADD file:0cd8ed314febdbf680645d20f346d9bac16fad5654c0b0d6ce2dec7c27c17b9a in / 
# Mon, 09 Oct 2017 21:42:41 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:38:16 GMT
ENV MONO_VERSION=5.2.0.224
# Mon, 09 Oct 2017 22:38:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:39:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Mon, 09 Oct 2017 22:46:21 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:02620033936d6cf3514a813f366025a14370f5dfe654e89eaca3a56b357e88c2`  
		Last Modified: Mon, 09 Oct 2017 21:49:15 GMT  
		Size: 26.3 MB (26280982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a56441a0716875f22a9f06959373f0a4996fa3191b02886e369c44e807e3204`  
		Last Modified: Mon, 09 Oct 2017 22:46:44 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9587a8ff6452a2e1fc4be530cee25fb8d71cc6d55058572cb5e8e2646d13518`  
		Last Modified: Mon, 09 Oct 2017 22:46:53 GMT  
		Size: 21.1 MB (21089899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f6ae07749836a1d621d2b4845d6f5933b4e707793cde023a4a9b3bd8b0cc08`  
		Last Modified: Mon, 09 Oct 2017 22:49:47 GMT  
		Size: 101.6 MB (101553239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.2` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:fb7985d24357e4b148439e36383f8bef8d7c1867ef6f7f3cb7d3bc10092f35f9
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.5 MB (163490268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44373cb770a49a7726792c5350bc4d741ecce60d041fd381b1d2c885e9be7abe`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:43:51 GMT
ADD file:75f5768db078e9eee90676141a2c9faa9ce02768b7c9cd6e588bdd5ffc0f65e3 in / 
# Mon, 09 Oct 2017 21:43:51 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 01:32:53 GMT
ENV MONO_VERSION=5.2.0.224
# Tue, 10 Oct 2017 01:33:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 10 Oct 2017 01:38:36 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 10 Oct 2017 01:59:39 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f2da27d97c13e9e531eda9577a28eb81b0d9034d7fd7e6575bd92744eed500f6`  
		Last Modified: Mon, 09 Oct 2017 21:53:20 GMT  
		Size: 27.5 MB (27480591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae39572730019ff3f4db8884b4c1bf3c1de81cdd121dd3ab0475a279d18809fd`  
		Last Modified: Tue, 10 Oct 2017 02:00:19 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be99f966e1dbb256ca4032fbc6388b8507d4fe83692101907a11fad70e6f2f8b`  
		Last Modified: Tue, 10 Oct 2017 02:00:31 GMT  
		Size: 25.2 MB (25220657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996c092fc7ef0fcd0f6dfa55f1bf82a6358092ed832c60269d6de3af2b500098`  
		Last Modified: Tue, 10 Oct 2017 02:04:16 GMT  
		Size: 110.8 MB (110786954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.2` - linux; 386

```console
$ docker pull mono@sha256:e341094d302b3ca4b0b3fca0b96741fdd462e4a2895e76e558b7a91dae5373b2
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.5 MB (172479663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4a529a31f872997045344a825cb70b3a722ab302729ece5432fbafd20ce616b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:30 GMT
ADD file:169ab3194fd1b25e06359d6eceb655093f44f0255c799ae8a3fc5bf8ba50fd8d in / 
# Mon, 09 Oct 2017 21:42:31 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:19:09 GMT
ENV MONO_VERSION=5.2.0.224
# Mon, 09 Oct 2017 22:19:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:20:17 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Mon, 09 Oct 2017 22:32:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d8b3cf5f6e0f087738d5589b812e12f5b8781935412c95d15f2f77d68657b006`  
		Last Modified: Mon, 09 Oct 2017 21:48:54 GMT  
		Size: 30.3 MB (30264454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2c998c1029c632021db5f103d73d3d976670e9b49dc7bfbfd3151098e30ac8`  
		Last Modified: Mon, 09 Oct 2017 22:35:57 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c26cf3f2f75893c1984b2db1156c5e8070ab23332250940e960ba44a5e6440`  
		Last Modified: Mon, 09 Oct 2017 22:36:09 GMT  
		Size: 29.0 MB (29021157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf125317f61dc10c728b70c279d3f98c9a2493524969f7a234838e3fd8312c0f`  
		Last Modified: Mon, 09 Oct 2017 22:42:38 GMT  
		Size: 113.2 MB (113191983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.2.0`

```console
$ docker pull mono@sha256:e5cab442beb65facb3a1b94e03e2b3be12eb6a01bba10671eabae5119974e06d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.2.0` - linux; amd64

```console
$ docker pull mono@sha256:2bab2e198c6b2e6709ad099661fee069cf848324909d2117a140b5c94dff321c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.0 MB (170039966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46890077dea7bc77987471185929ac531dedea73b9d84161510e5bc32d64c99`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:31:06 GMT
ADD file:187fe0df97a4c52984a518a454fb7ab3984ae7b541ede7ff84dd3c5da1ce1a59 in / 
# Mon, 09 Oct 2017 21:31:06 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:28:50 GMT
ENV MONO_VERSION=5.2.0.224
# Sat, 04 Nov 2017 02:28:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:29:44 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 04 Nov 2017 02:35:57 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d13d02fa248db2b423d6dbc8ec435675d23122f3939b5278b2156b75258e2259`  
		Last Modified: Mon, 09 Oct 2017 21:37:31 GMT  
		Size: 30.1 MB (30113318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe72810a809a6d1606064b8b8fa821b63e3d0360d817e6ca17620a9e361a3589`  
		Last Modified: Sat, 04 Nov 2017 02:36:51 GMT  
		Size: 2.1 KB (2068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063ab3201702497ddbed07d6a63bb56da0d3b950a461355879b63bc3a0c72858`  
		Last Modified: Sat, 04 Nov 2017 02:37:02 GMT  
		Size: 27.2 MB (27240685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5a7483019efc574d9e22dfb88abff972e4d0fa71a4ff2fc01aec8b1438c081`  
		Last Modified: Sat, 04 Nov 2017 02:39:43 GMT  
		Size: 112.7 MB (112683895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.2.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:6e9525473bd50383ed051de2684191f7b1fdc3302d5de4427784f167b11308a3
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148926184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fc645b4287b2e09c20b160ab09826ce50340bb8db3154dede723b22c120cf28`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:41 GMT
ADD file:0cd8ed314febdbf680645d20f346d9bac16fad5654c0b0d6ce2dec7c27c17b9a in / 
# Mon, 09 Oct 2017 21:42:41 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:38:16 GMT
ENV MONO_VERSION=5.2.0.224
# Mon, 09 Oct 2017 22:38:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:39:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Mon, 09 Oct 2017 22:46:21 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:02620033936d6cf3514a813f366025a14370f5dfe654e89eaca3a56b357e88c2`  
		Last Modified: Mon, 09 Oct 2017 21:49:15 GMT  
		Size: 26.3 MB (26280982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a56441a0716875f22a9f06959373f0a4996fa3191b02886e369c44e807e3204`  
		Last Modified: Mon, 09 Oct 2017 22:46:44 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9587a8ff6452a2e1fc4be530cee25fb8d71cc6d55058572cb5e8e2646d13518`  
		Last Modified: Mon, 09 Oct 2017 22:46:53 GMT  
		Size: 21.1 MB (21089899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f6ae07749836a1d621d2b4845d6f5933b4e707793cde023a4a9b3bd8b0cc08`  
		Last Modified: Mon, 09 Oct 2017 22:49:47 GMT  
		Size: 101.6 MB (101553239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.2.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:fb7985d24357e4b148439e36383f8bef8d7c1867ef6f7f3cb7d3bc10092f35f9
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.5 MB (163490268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44373cb770a49a7726792c5350bc4d741ecce60d041fd381b1d2c885e9be7abe`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:43:51 GMT
ADD file:75f5768db078e9eee90676141a2c9faa9ce02768b7c9cd6e588bdd5ffc0f65e3 in / 
# Mon, 09 Oct 2017 21:43:51 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 01:32:53 GMT
ENV MONO_VERSION=5.2.0.224
# Tue, 10 Oct 2017 01:33:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 10 Oct 2017 01:38:36 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 10 Oct 2017 01:59:39 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f2da27d97c13e9e531eda9577a28eb81b0d9034d7fd7e6575bd92744eed500f6`  
		Last Modified: Mon, 09 Oct 2017 21:53:20 GMT  
		Size: 27.5 MB (27480591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae39572730019ff3f4db8884b4c1bf3c1de81cdd121dd3ab0475a279d18809fd`  
		Last Modified: Tue, 10 Oct 2017 02:00:19 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be99f966e1dbb256ca4032fbc6388b8507d4fe83692101907a11fad70e6f2f8b`  
		Last Modified: Tue, 10 Oct 2017 02:00:31 GMT  
		Size: 25.2 MB (25220657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996c092fc7ef0fcd0f6dfa55f1bf82a6358092ed832c60269d6de3af2b500098`  
		Last Modified: Tue, 10 Oct 2017 02:04:16 GMT  
		Size: 110.8 MB (110786954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.2.0` - linux; 386

```console
$ docker pull mono@sha256:e341094d302b3ca4b0b3fca0b96741fdd462e4a2895e76e558b7a91dae5373b2
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.5 MB (172479663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4a529a31f872997045344a825cb70b3a722ab302729ece5432fbafd20ce616b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:30 GMT
ADD file:169ab3194fd1b25e06359d6eceb655093f44f0255c799ae8a3fc5bf8ba50fd8d in / 
# Mon, 09 Oct 2017 21:42:31 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:19:09 GMT
ENV MONO_VERSION=5.2.0.224
# Mon, 09 Oct 2017 22:19:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:20:17 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Mon, 09 Oct 2017 22:32:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d8b3cf5f6e0f087738d5589b812e12f5b8781935412c95d15f2f77d68657b006`  
		Last Modified: Mon, 09 Oct 2017 21:48:54 GMT  
		Size: 30.3 MB (30264454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2c998c1029c632021db5f103d73d3d976670e9b49dc7bfbfd3151098e30ac8`  
		Last Modified: Mon, 09 Oct 2017 22:35:57 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c26cf3f2f75893c1984b2db1156c5e8070ab23332250940e960ba44a5e6440`  
		Last Modified: Mon, 09 Oct 2017 22:36:09 GMT  
		Size: 29.0 MB (29021157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf125317f61dc10c728b70c279d3f98c9a2493524969f7a234838e3fd8312c0f`  
		Last Modified: Mon, 09 Oct 2017 22:42:38 GMT  
		Size: 113.2 MB (113191983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.2.0.224`

```console
$ docker pull mono@sha256:e5cab442beb65facb3a1b94e03e2b3be12eb6a01bba10671eabae5119974e06d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.2.0.224` - linux; amd64

```console
$ docker pull mono@sha256:2bab2e198c6b2e6709ad099661fee069cf848324909d2117a140b5c94dff321c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.0 MB (170039966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46890077dea7bc77987471185929ac531dedea73b9d84161510e5bc32d64c99`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:31:06 GMT
ADD file:187fe0df97a4c52984a518a454fb7ab3984ae7b541ede7ff84dd3c5da1ce1a59 in / 
# Mon, 09 Oct 2017 21:31:06 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:28:50 GMT
ENV MONO_VERSION=5.2.0.224
# Sat, 04 Nov 2017 02:28:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:29:44 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 04 Nov 2017 02:35:57 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d13d02fa248db2b423d6dbc8ec435675d23122f3939b5278b2156b75258e2259`  
		Last Modified: Mon, 09 Oct 2017 21:37:31 GMT  
		Size: 30.1 MB (30113318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe72810a809a6d1606064b8b8fa821b63e3d0360d817e6ca17620a9e361a3589`  
		Last Modified: Sat, 04 Nov 2017 02:36:51 GMT  
		Size: 2.1 KB (2068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063ab3201702497ddbed07d6a63bb56da0d3b950a461355879b63bc3a0c72858`  
		Last Modified: Sat, 04 Nov 2017 02:37:02 GMT  
		Size: 27.2 MB (27240685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5a7483019efc574d9e22dfb88abff972e4d0fa71a4ff2fc01aec8b1438c081`  
		Last Modified: Sat, 04 Nov 2017 02:39:43 GMT  
		Size: 112.7 MB (112683895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.2.0.224` - linux; arm variant v7

```console
$ docker pull mono@sha256:6e9525473bd50383ed051de2684191f7b1fdc3302d5de4427784f167b11308a3
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148926184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fc645b4287b2e09c20b160ab09826ce50340bb8db3154dede723b22c120cf28`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:41 GMT
ADD file:0cd8ed314febdbf680645d20f346d9bac16fad5654c0b0d6ce2dec7c27c17b9a in / 
# Mon, 09 Oct 2017 21:42:41 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:38:16 GMT
ENV MONO_VERSION=5.2.0.224
# Mon, 09 Oct 2017 22:38:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:39:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Mon, 09 Oct 2017 22:46:21 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:02620033936d6cf3514a813f366025a14370f5dfe654e89eaca3a56b357e88c2`  
		Last Modified: Mon, 09 Oct 2017 21:49:15 GMT  
		Size: 26.3 MB (26280982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a56441a0716875f22a9f06959373f0a4996fa3191b02886e369c44e807e3204`  
		Last Modified: Mon, 09 Oct 2017 22:46:44 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9587a8ff6452a2e1fc4be530cee25fb8d71cc6d55058572cb5e8e2646d13518`  
		Last Modified: Mon, 09 Oct 2017 22:46:53 GMT  
		Size: 21.1 MB (21089899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f6ae07749836a1d621d2b4845d6f5933b4e707793cde023a4a9b3bd8b0cc08`  
		Last Modified: Mon, 09 Oct 2017 22:49:47 GMT  
		Size: 101.6 MB (101553239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.2.0.224` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:fb7985d24357e4b148439e36383f8bef8d7c1867ef6f7f3cb7d3bc10092f35f9
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.5 MB (163490268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44373cb770a49a7726792c5350bc4d741ecce60d041fd381b1d2c885e9be7abe`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:43:51 GMT
ADD file:75f5768db078e9eee90676141a2c9faa9ce02768b7c9cd6e588bdd5ffc0f65e3 in / 
# Mon, 09 Oct 2017 21:43:51 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 01:32:53 GMT
ENV MONO_VERSION=5.2.0.224
# Tue, 10 Oct 2017 01:33:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 10 Oct 2017 01:38:36 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 10 Oct 2017 01:59:39 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f2da27d97c13e9e531eda9577a28eb81b0d9034d7fd7e6575bd92744eed500f6`  
		Last Modified: Mon, 09 Oct 2017 21:53:20 GMT  
		Size: 27.5 MB (27480591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae39572730019ff3f4db8884b4c1bf3c1de81cdd121dd3ab0475a279d18809fd`  
		Last Modified: Tue, 10 Oct 2017 02:00:19 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be99f966e1dbb256ca4032fbc6388b8507d4fe83692101907a11fad70e6f2f8b`  
		Last Modified: Tue, 10 Oct 2017 02:00:31 GMT  
		Size: 25.2 MB (25220657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996c092fc7ef0fcd0f6dfa55f1bf82a6358092ed832c60269d6de3af2b500098`  
		Last Modified: Tue, 10 Oct 2017 02:04:16 GMT  
		Size: 110.8 MB (110786954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.2.0.224` - linux; 386

```console
$ docker pull mono@sha256:e341094d302b3ca4b0b3fca0b96741fdd462e4a2895e76e558b7a91dae5373b2
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.5 MB (172479663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4a529a31f872997045344a825cb70b3a722ab302729ece5432fbafd20ce616b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:30 GMT
ADD file:169ab3194fd1b25e06359d6eceb655093f44f0255c799ae8a3fc5bf8ba50fd8d in / 
# Mon, 09 Oct 2017 21:42:31 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:19:09 GMT
ENV MONO_VERSION=5.2.0.224
# Mon, 09 Oct 2017 22:19:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:20:17 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Mon, 09 Oct 2017 22:32:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d8b3cf5f6e0f087738d5589b812e12f5b8781935412c95d15f2f77d68657b006`  
		Last Modified: Mon, 09 Oct 2017 21:48:54 GMT  
		Size: 30.3 MB (30264454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2c998c1029c632021db5f103d73d3d976670e9b49dc7bfbfd3151098e30ac8`  
		Last Modified: Mon, 09 Oct 2017 22:35:57 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c26cf3f2f75893c1984b2db1156c5e8070ab23332250940e960ba44a5e6440`  
		Last Modified: Mon, 09 Oct 2017 22:36:09 GMT  
		Size: 29.0 MB (29021157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf125317f61dc10c728b70c279d3f98c9a2493524969f7a234838e3fd8312c0f`  
		Last Modified: Mon, 09 Oct 2017 22:42:38 GMT  
		Size: 113.2 MB (113191983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.2.0.224-slim`

```console
$ docker pull mono@sha256:75da44ed81071185c1fe5af01873b6d44210cd2141ee90da442ee2e51d9c12ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.2.0.224-slim` - linux; amd64

```console
$ docker pull mono@sha256:e57ddf1d54dd38b5f38eb9d8de0cd5149581d588dba1726bf939fc02357bf334
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57356071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0981ce71a1fcd948209e377f3f3ca6bb64a7e55a61fb9dc8b29e18289b2d11c1`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:31:06 GMT
ADD file:187fe0df97a4c52984a518a454fb7ab3984ae7b541ede7ff84dd3c5da1ce1a59 in / 
# Mon, 09 Oct 2017 21:31:06 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:28:50 GMT
ENV MONO_VERSION=5.2.0.224
# Sat, 04 Nov 2017 02:28:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:29:44 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d13d02fa248db2b423d6dbc8ec435675d23122f3939b5278b2156b75258e2259`  
		Last Modified: Mon, 09 Oct 2017 21:37:31 GMT  
		Size: 30.1 MB (30113318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe72810a809a6d1606064b8b8fa821b63e3d0360d817e6ca17620a9e361a3589`  
		Last Modified: Sat, 04 Nov 2017 02:36:51 GMT  
		Size: 2.1 KB (2068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063ab3201702497ddbed07d6a63bb56da0d3b950a461355879b63bc3a0c72858`  
		Last Modified: Sat, 04 Nov 2017 02:37:02 GMT  
		Size: 27.2 MB (27240685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.2.0.224-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:5cd42475948ffa583df52134779351574a036a004860605532c746e9c1af6603
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47372945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9459e53906fc3b55776589c20ce4355955692e915edb8e74156379ddf6b6b027`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:41 GMT
ADD file:0cd8ed314febdbf680645d20f346d9bac16fad5654c0b0d6ce2dec7c27c17b9a in / 
# Mon, 09 Oct 2017 21:42:41 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:38:16 GMT
ENV MONO_VERSION=5.2.0.224
# Mon, 09 Oct 2017 22:38:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:39:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:02620033936d6cf3514a813f366025a14370f5dfe654e89eaca3a56b357e88c2`  
		Last Modified: Mon, 09 Oct 2017 21:49:15 GMT  
		Size: 26.3 MB (26280982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a56441a0716875f22a9f06959373f0a4996fa3191b02886e369c44e807e3204`  
		Last Modified: Mon, 09 Oct 2017 22:46:44 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9587a8ff6452a2e1fc4be530cee25fb8d71cc6d55058572cb5e8e2646d13518`  
		Last Modified: Mon, 09 Oct 2017 22:46:53 GMT  
		Size: 21.1 MB (21089899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.2.0.224-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:b9f8c9e035c0031920173caa133fa2535de70528bede9238cf2ce5d5f227c3c3
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52703314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3e175ff9fc68b50d83c4a18051deaf08e21afcaee3294705d4db39b42c67b96`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:43:51 GMT
ADD file:75f5768db078e9eee90676141a2c9faa9ce02768b7c9cd6e588bdd5ffc0f65e3 in / 
# Mon, 09 Oct 2017 21:43:51 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 01:32:53 GMT
ENV MONO_VERSION=5.2.0.224
# Tue, 10 Oct 2017 01:33:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 10 Oct 2017 01:38:36 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f2da27d97c13e9e531eda9577a28eb81b0d9034d7fd7e6575bd92744eed500f6`  
		Last Modified: Mon, 09 Oct 2017 21:53:20 GMT  
		Size: 27.5 MB (27480591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae39572730019ff3f4db8884b4c1bf3c1de81cdd121dd3ab0475a279d18809fd`  
		Last Modified: Tue, 10 Oct 2017 02:00:19 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be99f966e1dbb256ca4032fbc6388b8507d4fe83692101907a11fad70e6f2f8b`  
		Last Modified: Tue, 10 Oct 2017 02:00:31 GMT  
		Size: 25.2 MB (25220657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.2.0.224-slim` - linux; 386

```console
$ docker pull mono@sha256:3e9f329445756d18b6ef76a0ad5e8464bf0a4865e2aba4cf008fc3c630440740
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59287680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29cf6239b87a6631d10186ab7a3818e9963695977b3c3326242972eddf333ac3`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:30 GMT
ADD file:169ab3194fd1b25e06359d6eceb655093f44f0255c799ae8a3fc5bf8ba50fd8d in / 
# Mon, 09 Oct 2017 21:42:31 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:19:09 GMT
ENV MONO_VERSION=5.2.0.224
# Mon, 09 Oct 2017 22:19:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:20:17 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d8b3cf5f6e0f087738d5589b812e12f5b8781935412c95d15f2f77d68657b006`  
		Last Modified: Mon, 09 Oct 2017 21:48:54 GMT  
		Size: 30.3 MB (30264454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2c998c1029c632021db5f103d73d3d976670e9b49dc7bfbfd3151098e30ac8`  
		Last Modified: Mon, 09 Oct 2017 22:35:57 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c26cf3f2f75893c1984b2db1156c5e8070ab23332250940e960ba44a5e6440`  
		Last Modified: Mon, 09 Oct 2017 22:36:09 GMT  
		Size: 29.0 MB (29021157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.2.0-slim`

```console
$ docker pull mono@sha256:75da44ed81071185c1fe5af01873b6d44210cd2141ee90da442ee2e51d9c12ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.2.0-slim` - linux; amd64

```console
$ docker pull mono@sha256:e57ddf1d54dd38b5f38eb9d8de0cd5149581d588dba1726bf939fc02357bf334
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57356071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0981ce71a1fcd948209e377f3f3ca6bb64a7e55a61fb9dc8b29e18289b2d11c1`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:31:06 GMT
ADD file:187fe0df97a4c52984a518a454fb7ab3984ae7b541ede7ff84dd3c5da1ce1a59 in / 
# Mon, 09 Oct 2017 21:31:06 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:28:50 GMT
ENV MONO_VERSION=5.2.0.224
# Sat, 04 Nov 2017 02:28:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:29:44 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d13d02fa248db2b423d6dbc8ec435675d23122f3939b5278b2156b75258e2259`  
		Last Modified: Mon, 09 Oct 2017 21:37:31 GMT  
		Size: 30.1 MB (30113318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe72810a809a6d1606064b8b8fa821b63e3d0360d817e6ca17620a9e361a3589`  
		Last Modified: Sat, 04 Nov 2017 02:36:51 GMT  
		Size: 2.1 KB (2068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063ab3201702497ddbed07d6a63bb56da0d3b950a461355879b63bc3a0c72858`  
		Last Modified: Sat, 04 Nov 2017 02:37:02 GMT  
		Size: 27.2 MB (27240685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.2.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:5cd42475948ffa583df52134779351574a036a004860605532c746e9c1af6603
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47372945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9459e53906fc3b55776589c20ce4355955692e915edb8e74156379ddf6b6b027`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:41 GMT
ADD file:0cd8ed314febdbf680645d20f346d9bac16fad5654c0b0d6ce2dec7c27c17b9a in / 
# Mon, 09 Oct 2017 21:42:41 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:38:16 GMT
ENV MONO_VERSION=5.2.0.224
# Mon, 09 Oct 2017 22:38:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:39:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:02620033936d6cf3514a813f366025a14370f5dfe654e89eaca3a56b357e88c2`  
		Last Modified: Mon, 09 Oct 2017 21:49:15 GMT  
		Size: 26.3 MB (26280982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a56441a0716875f22a9f06959373f0a4996fa3191b02886e369c44e807e3204`  
		Last Modified: Mon, 09 Oct 2017 22:46:44 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9587a8ff6452a2e1fc4be530cee25fb8d71cc6d55058572cb5e8e2646d13518`  
		Last Modified: Mon, 09 Oct 2017 22:46:53 GMT  
		Size: 21.1 MB (21089899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.2.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:b9f8c9e035c0031920173caa133fa2535de70528bede9238cf2ce5d5f227c3c3
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52703314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3e175ff9fc68b50d83c4a18051deaf08e21afcaee3294705d4db39b42c67b96`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:43:51 GMT
ADD file:75f5768db078e9eee90676141a2c9faa9ce02768b7c9cd6e588bdd5ffc0f65e3 in / 
# Mon, 09 Oct 2017 21:43:51 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 01:32:53 GMT
ENV MONO_VERSION=5.2.0.224
# Tue, 10 Oct 2017 01:33:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 10 Oct 2017 01:38:36 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f2da27d97c13e9e531eda9577a28eb81b0d9034d7fd7e6575bd92744eed500f6`  
		Last Modified: Mon, 09 Oct 2017 21:53:20 GMT  
		Size: 27.5 MB (27480591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae39572730019ff3f4db8884b4c1bf3c1de81cdd121dd3ab0475a279d18809fd`  
		Last Modified: Tue, 10 Oct 2017 02:00:19 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be99f966e1dbb256ca4032fbc6388b8507d4fe83692101907a11fad70e6f2f8b`  
		Last Modified: Tue, 10 Oct 2017 02:00:31 GMT  
		Size: 25.2 MB (25220657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.2.0-slim` - linux; 386

```console
$ docker pull mono@sha256:3e9f329445756d18b6ef76a0ad5e8464bf0a4865e2aba4cf008fc3c630440740
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59287680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29cf6239b87a6631d10186ab7a3818e9963695977b3c3326242972eddf333ac3`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:30 GMT
ADD file:169ab3194fd1b25e06359d6eceb655093f44f0255c799ae8a3fc5bf8ba50fd8d in / 
# Mon, 09 Oct 2017 21:42:31 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:19:09 GMT
ENV MONO_VERSION=5.2.0.224
# Mon, 09 Oct 2017 22:19:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:20:17 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d8b3cf5f6e0f087738d5589b812e12f5b8781935412c95d15f2f77d68657b006`  
		Last Modified: Mon, 09 Oct 2017 21:48:54 GMT  
		Size: 30.3 MB (30264454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2c998c1029c632021db5f103d73d3d976670e9b49dc7bfbfd3151098e30ac8`  
		Last Modified: Mon, 09 Oct 2017 22:35:57 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c26cf3f2f75893c1984b2db1156c5e8070ab23332250940e960ba44a5e6440`  
		Last Modified: Mon, 09 Oct 2017 22:36:09 GMT  
		Size: 29.0 MB (29021157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.2-slim`

```console
$ docker pull mono@sha256:75da44ed81071185c1fe5af01873b6d44210cd2141ee90da442ee2e51d9c12ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.2-slim` - linux; amd64

```console
$ docker pull mono@sha256:e57ddf1d54dd38b5f38eb9d8de0cd5149581d588dba1726bf939fc02357bf334
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57356071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0981ce71a1fcd948209e377f3f3ca6bb64a7e55a61fb9dc8b29e18289b2d11c1`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:31:06 GMT
ADD file:187fe0df97a4c52984a518a454fb7ab3984ae7b541ede7ff84dd3c5da1ce1a59 in / 
# Mon, 09 Oct 2017 21:31:06 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:28:50 GMT
ENV MONO_VERSION=5.2.0.224
# Sat, 04 Nov 2017 02:28:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:29:44 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d13d02fa248db2b423d6dbc8ec435675d23122f3939b5278b2156b75258e2259`  
		Last Modified: Mon, 09 Oct 2017 21:37:31 GMT  
		Size: 30.1 MB (30113318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe72810a809a6d1606064b8b8fa821b63e3d0360d817e6ca17620a9e361a3589`  
		Last Modified: Sat, 04 Nov 2017 02:36:51 GMT  
		Size: 2.1 KB (2068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063ab3201702497ddbed07d6a63bb56da0d3b950a461355879b63bc3a0c72858`  
		Last Modified: Sat, 04 Nov 2017 02:37:02 GMT  
		Size: 27.2 MB (27240685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.2-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:5cd42475948ffa583df52134779351574a036a004860605532c746e9c1af6603
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47372945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9459e53906fc3b55776589c20ce4355955692e915edb8e74156379ddf6b6b027`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:41 GMT
ADD file:0cd8ed314febdbf680645d20f346d9bac16fad5654c0b0d6ce2dec7c27c17b9a in / 
# Mon, 09 Oct 2017 21:42:41 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:38:16 GMT
ENV MONO_VERSION=5.2.0.224
# Mon, 09 Oct 2017 22:38:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:39:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:02620033936d6cf3514a813f366025a14370f5dfe654e89eaca3a56b357e88c2`  
		Last Modified: Mon, 09 Oct 2017 21:49:15 GMT  
		Size: 26.3 MB (26280982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a56441a0716875f22a9f06959373f0a4996fa3191b02886e369c44e807e3204`  
		Last Modified: Mon, 09 Oct 2017 22:46:44 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9587a8ff6452a2e1fc4be530cee25fb8d71cc6d55058572cb5e8e2646d13518`  
		Last Modified: Mon, 09 Oct 2017 22:46:53 GMT  
		Size: 21.1 MB (21089899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.2-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:b9f8c9e035c0031920173caa133fa2535de70528bede9238cf2ce5d5f227c3c3
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52703314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3e175ff9fc68b50d83c4a18051deaf08e21afcaee3294705d4db39b42c67b96`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:43:51 GMT
ADD file:75f5768db078e9eee90676141a2c9faa9ce02768b7c9cd6e588bdd5ffc0f65e3 in / 
# Mon, 09 Oct 2017 21:43:51 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 01:32:53 GMT
ENV MONO_VERSION=5.2.0.224
# Tue, 10 Oct 2017 01:33:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 10 Oct 2017 01:38:36 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f2da27d97c13e9e531eda9577a28eb81b0d9034d7fd7e6575bd92744eed500f6`  
		Last Modified: Mon, 09 Oct 2017 21:53:20 GMT  
		Size: 27.5 MB (27480591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae39572730019ff3f4db8884b4c1bf3c1de81cdd121dd3ab0475a279d18809fd`  
		Last Modified: Tue, 10 Oct 2017 02:00:19 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be99f966e1dbb256ca4032fbc6388b8507d4fe83692101907a11fad70e6f2f8b`  
		Last Modified: Tue, 10 Oct 2017 02:00:31 GMT  
		Size: 25.2 MB (25220657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.2-slim` - linux; 386

```console
$ docker pull mono@sha256:3e9f329445756d18b6ef76a0ad5e8464bf0a4865e2aba4cf008fc3c630440740
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59287680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29cf6239b87a6631d10186ab7a3818e9963695977b3c3326242972eddf333ac3`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:30 GMT
ADD file:169ab3194fd1b25e06359d6eceb655093f44f0255c799ae8a3fc5bf8ba50fd8d in / 
# Mon, 09 Oct 2017 21:42:31 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:19:09 GMT
ENV MONO_VERSION=5.2.0.224
# Mon, 09 Oct 2017 22:19:19 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Mon, 09 Oct 2017 22:20:17 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d8b3cf5f6e0f087738d5589b812e12f5b8781935412c95d15f2f77d68657b006`  
		Last Modified: Mon, 09 Oct 2017 21:48:54 GMT  
		Size: 30.3 MB (30264454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2c998c1029c632021db5f103d73d3d976670e9b49dc7bfbfd3151098e30ac8`  
		Last Modified: Mon, 09 Oct 2017 22:35:57 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c26cf3f2f75893c1984b2db1156c5e8070ab23332250940e960ba44a5e6440`  
		Last Modified: Mon, 09 Oct 2017 22:36:09 GMT  
		Size: 29.0 MB (29021157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.4`

```console
$ docker pull mono@sha256:17a2b85ec4c0942e16c4e6499a57e15ae9c09c2b9034b3ec58b0c23171311902
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.4` - linux; amd64

```console
$ docker pull mono@sha256:932cd8cc4dfb08336ba3a5bd31feb361afdb82b5d2c203691fc956b3fce22a3d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.3 MB (167259115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d59c2a7018c7acd0024da96ecfcf7f1f778f58db827bb41788608e53494bb94b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:31:06 GMT
ADD file:187fe0df97a4c52984a518a454fb7ab3984ae7b541ede7ff84dd3c5da1ce1a59 in / 
# Mon, 09 Oct 2017 21:31:06 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:27:41 GMT
ENV MONO_VERSION=5.4.0.201
# Sat, 04 Nov 2017 02:27:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:28:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 04 Nov 2017 02:33:42 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d13d02fa248db2b423d6dbc8ec435675d23122f3939b5278b2156b75258e2259`  
		Last Modified: Mon, 09 Oct 2017 21:37:31 GMT  
		Size: 30.1 MB (30113318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8d78a964aa167e2e8dbfd3365f8445ed149628507a2aa9dfaacde4e97c83b3`  
		Last Modified: Sat, 04 Nov 2017 02:36:19 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c98de1760e34ac9792d43e7e171574a9d63a20a7bff3bf03e29ef3fa026362`  
		Last Modified: Sat, 04 Nov 2017 02:36:31 GMT  
		Size: 27.3 MB (27278585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59b45d6dbf7cd29de575aafcd18d219efc175d67692860d0f4b9be03a8efd4d`  
		Last Modified: Sat, 04 Nov 2017 02:38:48 GMT  
		Size: 109.9 MB (109865143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4` - linux; arm variant v7

```console
$ docker pull mono@sha256:5189f8b756032897bb3d03f9e1d396ae72a70d1c66c6fcdd8e6b65f3d921fdb0
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.0 MB (147049823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff518dee16442d023eb4b88925989b6defdb55141b58851d208299cedff5f3c4`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:41 GMT
ADD file:0cd8ed314febdbf680645d20f346d9bac16fad5654c0b0d6ce2dec7c27c17b9a in / 
# Mon, 09 Oct 2017 21:42:41 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 17:51:32 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 17:51:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 17:52:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 17 Oct 2017 17:54:46 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:02620033936d6cf3514a813f366025a14370f5dfe654e89eaca3a56b357e88c2`  
		Last Modified: Mon, 09 Oct 2017 21:49:15 GMT  
		Size: 26.3 MB (26280982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebc5f99dc26f440db883809cd8379ade7a516c92b91b7d22ae6485b1278ab1f`  
		Last Modified: Tue, 17 Oct 2017 17:55:04 GMT  
		Size: 2.1 KB (2065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dec16e095e6115a08f0f8530cdfde275c707acbc3fbb2fcc735b863a95122c1`  
		Last Modified: Tue, 17 Oct 2017 17:55:12 GMT  
		Size: 22.0 MB (22035038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c10ba59aa47230cfdc9ee37e8f10718b4c017c2b4906920d0a1ff1b75edad`  
		Last Modified: Tue, 17 Oct 2017 17:56:17 GMT  
		Size: 98.7 MB (98731738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:a68c168b05a89256ded341eeebe49ae1ab5b96523ccbac7001c9e317a0dbd754
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161639631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd34d0efd84450956a53481cef2b10afae252d3f095fc8b53c3e142529cb3009`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:43:51 GMT
ADD file:75f5768db078e9eee90676141a2c9faa9ce02768b7c9cd6e588bdd5ffc0f65e3 in / 
# Mon, 09 Oct 2017 21:43:51 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 19:45:44 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 19:45:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 19:47:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 17 Oct 2017 19:53:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f2da27d97c13e9e531eda9577a28eb81b0d9034d7fd7e6575bd92744eed500f6`  
		Last Modified: Mon, 09 Oct 2017 21:53:20 GMT  
		Size: 27.5 MB (27480591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad3574e8978c5cdfc63d800a5b8666c43c9d93519dbe83105d3ffdb6bac9f8a`  
		Last Modified: Tue, 17 Oct 2017 19:53:55 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b32240292f03d8f265e50d58923a86660a5730b335e0dc5eb333ae7890cd921`  
		Last Modified: Tue, 17 Oct 2017 19:54:07 GMT  
		Size: 26.2 MB (26199265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d3f2ac099ead527a80c01317816b1cbcbcbe0d86403a39344baa73cda1baae`  
		Last Modified: Tue, 17 Oct 2017 19:55:50 GMT  
		Size: 108.0 MB (107957711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4` - linux; 386

```console
$ docker pull mono@sha256:8b249344ca9584956ed7cb4635f29d545514ca86632705311522274cb2122121
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169638409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a8176ed9b7b0401eb795893a084727d27552a6c788477df53e8e54d4dbc386`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:30 GMT
ADD file:169ab3194fd1b25e06359d6eceb655093f44f0255c799ae8a3fc5bf8ba50fd8d in / 
# Mon, 09 Oct 2017 21:42:31 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 00:57:28 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 00:57:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 00:58:35 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 17 Oct 2017 01:00:06 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d8b3cf5f6e0f087738d5589b812e12f5b8781935412c95d15f2f77d68657b006`  
		Last Modified: Mon, 09 Oct 2017 21:48:54 GMT  
		Size: 30.3 MB (30264454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6db9a23ef19b82644ae3cc18a517df0a01579623915a4d0ea810e09c608927`  
		Last Modified: Tue, 17 Oct 2017 01:02:43 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e350d9d1943c6f652c74dd24e15cbdf943755f73fa0942cb0a1d8b12187ece`  
		Last Modified: Tue, 17 Oct 2017 01:02:49 GMT  
		Size: 29.1 MB (29051973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88be8b6ac98f875586bdbda4e5ffcbea6d9d7210c018d5213e75c5a0d6e1dd4a`  
		Last Modified: Tue, 17 Oct 2017 01:05:06 GMT  
		Size: 110.3 MB (110319916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.4.0`

```console
$ docker pull mono@sha256:17a2b85ec4c0942e16c4e6499a57e15ae9c09c2b9034b3ec58b0c23171311902
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.4.0` - linux; amd64

```console
$ docker pull mono@sha256:932cd8cc4dfb08336ba3a5bd31feb361afdb82b5d2c203691fc956b3fce22a3d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.3 MB (167259115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d59c2a7018c7acd0024da96ecfcf7f1f778f58db827bb41788608e53494bb94b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:31:06 GMT
ADD file:187fe0df97a4c52984a518a454fb7ab3984ae7b541ede7ff84dd3c5da1ce1a59 in / 
# Mon, 09 Oct 2017 21:31:06 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:27:41 GMT
ENV MONO_VERSION=5.4.0.201
# Sat, 04 Nov 2017 02:27:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:28:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 04 Nov 2017 02:33:42 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d13d02fa248db2b423d6dbc8ec435675d23122f3939b5278b2156b75258e2259`  
		Last Modified: Mon, 09 Oct 2017 21:37:31 GMT  
		Size: 30.1 MB (30113318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8d78a964aa167e2e8dbfd3365f8445ed149628507a2aa9dfaacde4e97c83b3`  
		Last Modified: Sat, 04 Nov 2017 02:36:19 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c98de1760e34ac9792d43e7e171574a9d63a20a7bff3bf03e29ef3fa026362`  
		Last Modified: Sat, 04 Nov 2017 02:36:31 GMT  
		Size: 27.3 MB (27278585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59b45d6dbf7cd29de575aafcd18d219efc175d67692860d0f4b9be03a8efd4d`  
		Last Modified: Sat, 04 Nov 2017 02:38:48 GMT  
		Size: 109.9 MB (109865143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:5189f8b756032897bb3d03f9e1d396ae72a70d1c66c6fcdd8e6b65f3d921fdb0
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.0 MB (147049823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff518dee16442d023eb4b88925989b6defdb55141b58851d208299cedff5f3c4`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:41 GMT
ADD file:0cd8ed314febdbf680645d20f346d9bac16fad5654c0b0d6ce2dec7c27c17b9a in / 
# Mon, 09 Oct 2017 21:42:41 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 17:51:32 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 17:51:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 17:52:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 17 Oct 2017 17:54:46 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:02620033936d6cf3514a813f366025a14370f5dfe654e89eaca3a56b357e88c2`  
		Last Modified: Mon, 09 Oct 2017 21:49:15 GMT  
		Size: 26.3 MB (26280982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebc5f99dc26f440db883809cd8379ade7a516c92b91b7d22ae6485b1278ab1f`  
		Last Modified: Tue, 17 Oct 2017 17:55:04 GMT  
		Size: 2.1 KB (2065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dec16e095e6115a08f0f8530cdfde275c707acbc3fbb2fcc735b863a95122c1`  
		Last Modified: Tue, 17 Oct 2017 17:55:12 GMT  
		Size: 22.0 MB (22035038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c10ba59aa47230cfdc9ee37e8f10718b4c017c2b4906920d0a1ff1b75edad`  
		Last Modified: Tue, 17 Oct 2017 17:56:17 GMT  
		Size: 98.7 MB (98731738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:a68c168b05a89256ded341eeebe49ae1ab5b96523ccbac7001c9e317a0dbd754
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161639631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd34d0efd84450956a53481cef2b10afae252d3f095fc8b53c3e142529cb3009`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:43:51 GMT
ADD file:75f5768db078e9eee90676141a2c9faa9ce02768b7c9cd6e588bdd5ffc0f65e3 in / 
# Mon, 09 Oct 2017 21:43:51 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 19:45:44 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 19:45:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 19:47:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 17 Oct 2017 19:53:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f2da27d97c13e9e531eda9577a28eb81b0d9034d7fd7e6575bd92744eed500f6`  
		Last Modified: Mon, 09 Oct 2017 21:53:20 GMT  
		Size: 27.5 MB (27480591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad3574e8978c5cdfc63d800a5b8666c43c9d93519dbe83105d3ffdb6bac9f8a`  
		Last Modified: Tue, 17 Oct 2017 19:53:55 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b32240292f03d8f265e50d58923a86660a5730b335e0dc5eb333ae7890cd921`  
		Last Modified: Tue, 17 Oct 2017 19:54:07 GMT  
		Size: 26.2 MB (26199265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d3f2ac099ead527a80c01317816b1cbcbcbe0d86403a39344baa73cda1baae`  
		Last Modified: Tue, 17 Oct 2017 19:55:50 GMT  
		Size: 108.0 MB (107957711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.0` - linux; 386

```console
$ docker pull mono@sha256:8b249344ca9584956ed7cb4635f29d545514ca86632705311522274cb2122121
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169638409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a8176ed9b7b0401eb795893a084727d27552a6c788477df53e8e54d4dbc386`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:30 GMT
ADD file:169ab3194fd1b25e06359d6eceb655093f44f0255c799ae8a3fc5bf8ba50fd8d in / 
# Mon, 09 Oct 2017 21:42:31 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 00:57:28 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 00:57:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 00:58:35 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 17 Oct 2017 01:00:06 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d8b3cf5f6e0f087738d5589b812e12f5b8781935412c95d15f2f77d68657b006`  
		Last Modified: Mon, 09 Oct 2017 21:48:54 GMT  
		Size: 30.3 MB (30264454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6db9a23ef19b82644ae3cc18a517df0a01579623915a4d0ea810e09c608927`  
		Last Modified: Tue, 17 Oct 2017 01:02:43 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e350d9d1943c6f652c74dd24e15cbdf943755f73fa0942cb0a1d8b12187ece`  
		Last Modified: Tue, 17 Oct 2017 01:02:49 GMT  
		Size: 29.1 MB (29051973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88be8b6ac98f875586bdbda4e5ffcbea6d9d7210c018d5213e75c5a0d6e1dd4a`  
		Last Modified: Tue, 17 Oct 2017 01:05:06 GMT  
		Size: 110.3 MB (110319916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.4.0.201`

```console
$ docker pull mono@sha256:17a2b85ec4c0942e16c4e6499a57e15ae9c09c2b9034b3ec58b0c23171311902
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.4.0.201` - linux; amd64

```console
$ docker pull mono@sha256:932cd8cc4dfb08336ba3a5bd31feb361afdb82b5d2c203691fc956b3fce22a3d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.3 MB (167259115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d59c2a7018c7acd0024da96ecfcf7f1f778f58db827bb41788608e53494bb94b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:31:06 GMT
ADD file:187fe0df97a4c52984a518a454fb7ab3984ae7b541ede7ff84dd3c5da1ce1a59 in / 
# Mon, 09 Oct 2017 21:31:06 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:27:41 GMT
ENV MONO_VERSION=5.4.0.201
# Sat, 04 Nov 2017 02:27:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:28:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 04 Nov 2017 02:33:42 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d13d02fa248db2b423d6dbc8ec435675d23122f3939b5278b2156b75258e2259`  
		Last Modified: Mon, 09 Oct 2017 21:37:31 GMT  
		Size: 30.1 MB (30113318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8d78a964aa167e2e8dbfd3365f8445ed149628507a2aa9dfaacde4e97c83b3`  
		Last Modified: Sat, 04 Nov 2017 02:36:19 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c98de1760e34ac9792d43e7e171574a9d63a20a7bff3bf03e29ef3fa026362`  
		Last Modified: Sat, 04 Nov 2017 02:36:31 GMT  
		Size: 27.3 MB (27278585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59b45d6dbf7cd29de575aafcd18d219efc175d67692860d0f4b9be03a8efd4d`  
		Last Modified: Sat, 04 Nov 2017 02:38:48 GMT  
		Size: 109.9 MB (109865143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.0.201` - linux; arm variant v7

```console
$ docker pull mono@sha256:5189f8b756032897bb3d03f9e1d396ae72a70d1c66c6fcdd8e6b65f3d921fdb0
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.0 MB (147049823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff518dee16442d023eb4b88925989b6defdb55141b58851d208299cedff5f3c4`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:41 GMT
ADD file:0cd8ed314febdbf680645d20f346d9bac16fad5654c0b0d6ce2dec7c27c17b9a in / 
# Mon, 09 Oct 2017 21:42:41 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 17:51:32 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 17:51:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 17:52:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 17 Oct 2017 17:54:46 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:02620033936d6cf3514a813f366025a14370f5dfe654e89eaca3a56b357e88c2`  
		Last Modified: Mon, 09 Oct 2017 21:49:15 GMT  
		Size: 26.3 MB (26280982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebc5f99dc26f440db883809cd8379ade7a516c92b91b7d22ae6485b1278ab1f`  
		Last Modified: Tue, 17 Oct 2017 17:55:04 GMT  
		Size: 2.1 KB (2065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dec16e095e6115a08f0f8530cdfde275c707acbc3fbb2fcc735b863a95122c1`  
		Last Modified: Tue, 17 Oct 2017 17:55:12 GMT  
		Size: 22.0 MB (22035038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c10ba59aa47230cfdc9ee37e8f10718b4c017c2b4906920d0a1ff1b75edad`  
		Last Modified: Tue, 17 Oct 2017 17:56:17 GMT  
		Size: 98.7 MB (98731738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.0.201` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:a68c168b05a89256ded341eeebe49ae1ab5b96523ccbac7001c9e317a0dbd754
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161639631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd34d0efd84450956a53481cef2b10afae252d3f095fc8b53c3e142529cb3009`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:43:51 GMT
ADD file:75f5768db078e9eee90676141a2c9faa9ce02768b7c9cd6e588bdd5ffc0f65e3 in / 
# Mon, 09 Oct 2017 21:43:51 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 19:45:44 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 19:45:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 19:47:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 17 Oct 2017 19:53:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f2da27d97c13e9e531eda9577a28eb81b0d9034d7fd7e6575bd92744eed500f6`  
		Last Modified: Mon, 09 Oct 2017 21:53:20 GMT  
		Size: 27.5 MB (27480591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad3574e8978c5cdfc63d800a5b8666c43c9d93519dbe83105d3ffdb6bac9f8a`  
		Last Modified: Tue, 17 Oct 2017 19:53:55 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b32240292f03d8f265e50d58923a86660a5730b335e0dc5eb333ae7890cd921`  
		Last Modified: Tue, 17 Oct 2017 19:54:07 GMT  
		Size: 26.2 MB (26199265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d3f2ac099ead527a80c01317816b1cbcbcbe0d86403a39344baa73cda1baae`  
		Last Modified: Tue, 17 Oct 2017 19:55:50 GMT  
		Size: 108.0 MB (107957711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.0.201` - linux; 386

```console
$ docker pull mono@sha256:8b249344ca9584956ed7cb4635f29d545514ca86632705311522274cb2122121
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169638409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a8176ed9b7b0401eb795893a084727d27552a6c788477df53e8e54d4dbc386`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:30 GMT
ADD file:169ab3194fd1b25e06359d6eceb655093f44f0255c799ae8a3fc5bf8ba50fd8d in / 
# Mon, 09 Oct 2017 21:42:31 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 00:57:28 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 00:57:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 00:58:35 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 17 Oct 2017 01:00:06 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d8b3cf5f6e0f087738d5589b812e12f5b8781935412c95d15f2f77d68657b006`  
		Last Modified: Mon, 09 Oct 2017 21:48:54 GMT  
		Size: 30.3 MB (30264454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6db9a23ef19b82644ae3cc18a517df0a01579623915a4d0ea810e09c608927`  
		Last Modified: Tue, 17 Oct 2017 01:02:43 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e350d9d1943c6f652c74dd24e15cbdf943755f73fa0942cb0a1d8b12187ece`  
		Last Modified: Tue, 17 Oct 2017 01:02:49 GMT  
		Size: 29.1 MB (29051973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88be8b6ac98f875586bdbda4e5ffcbea6d9d7210c018d5213e75c5a0d6e1dd4a`  
		Last Modified: Tue, 17 Oct 2017 01:05:06 GMT  
		Size: 110.3 MB (110319916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.4.0.201-slim`

```console
$ docker pull mono@sha256:8bb8acd652efd1a6f2c35ac9f384d02b010b3db0802b20fdeb1d65444e2d5d9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.4.0.201-slim` - linux; amd64

```console
$ docker pull mono@sha256:6fa11ce8b3e4f282aec74ac5a67b2a9f4870bea61d1d78559e7ee5b214b82d35
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57393972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b1edbbef1ba391ad23c0143f4dcb99071ea629a89326753fb24f7b718efcf8`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:31:06 GMT
ADD file:187fe0df97a4c52984a518a454fb7ab3984ae7b541ede7ff84dd3c5da1ce1a59 in / 
# Mon, 09 Oct 2017 21:31:06 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:27:41 GMT
ENV MONO_VERSION=5.4.0.201
# Sat, 04 Nov 2017 02:27:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:28:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d13d02fa248db2b423d6dbc8ec435675d23122f3939b5278b2156b75258e2259`  
		Last Modified: Mon, 09 Oct 2017 21:37:31 GMT  
		Size: 30.1 MB (30113318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8d78a964aa167e2e8dbfd3365f8445ed149628507a2aa9dfaacde4e97c83b3`  
		Last Modified: Sat, 04 Nov 2017 02:36:19 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c98de1760e34ac9792d43e7e171574a9d63a20a7bff3bf03e29ef3fa026362`  
		Last Modified: Sat, 04 Nov 2017 02:36:31 GMT  
		Size: 27.3 MB (27278585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.0.201-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:5f8055656d4c37b7f31bd06a372376d76050217a4de7975a6a5f637796e3ce37
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48318085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f2e28a554ed459c68d737d67e3d3814f15caaf9dbc2025cd52f59957bfbd37c`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:41 GMT
ADD file:0cd8ed314febdbf680645d20f346d9bac16fad5654c0b0d6ce2dec7c27c17b9a in / 
# Mon, 09 Oct 2017 21:42:41 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 17:51:32 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 17:51:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 17:52:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:02620033936d6cf3514a813f366025a14370f5dfe654e89eaca3a56b357e88c2`  
		Last Modified: Mon, 09 Oct 2017 21:49:15 GMT  
		Size: 26.3 MB (26280982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebc5f99dc26f440db883809cd8379ade7a516c92b91b7d22ae6485b1278ab1f`  
		Last Modified: Tue, 17 Oct 2017 17:55:04 GMT  
		Size: 2.1 KB (2065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dec16e095e6115a08f0f8530cdfde275c707acbc3fbb2fcc735b863a95122c1`  
		Last Modified: Tue, 17 Oct 2017 17:55:12 GMT  
		Size: 22.0 MB (22035038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.0.201-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:7c7acc4cd80b4ceaa4309ce4aed1d02f3b7c7209957ffafee4c7cc4cad16e8af
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53681920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8480909fbc33d90b5dee55a454ea5be52d3f9c8704ed3e60058f7bce5e2d85b4`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:43:51 GMT
ADD file:75f5768db078e9eee90676141a2c9faa9ce02768b7c9cd6e588bdd5ffc0f65e3 in / 
# Mon, 09 Oct 2017 21:43:51 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 19:45:44 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 19:45:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 19:47:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f2da27d97c13e9e531eda9577a28eb81b0d9034d7fd7e6575bd92744eed500f6`  
		Last Modified: Mon, 09 Oct 2017 21:53:20 GMT  
		Size: 27.5 MB (27480591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad3574e8978c5cdfc63d800a5b8666c43c9d93519dbe83105d3ffdb6bac9f8a`  
		Last Modified: Tue, 17 Oct 2017 19:53:55 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b32240292f03d8f265e50d58923a86660a5730b335e0dc5eb333ae7890cd921`  
		Last Modified: Tue, 17 Oct 2017 19:54:07 GMT  
		Size: 26.2 MB (26199265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.0.201-slim` - linux; 386

```console
$ docker pull mono@sha256:1c1e2d0453aa51c38f1a9c5d857326a7d2584187a3d6b97c7d134857b313eaca
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59318493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc39ab72d2a85482d0fb58d096da734fa000dea510d2a2d0f2ef4dcfcf4e9350`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:30 GMT
ADD file:169ab3194fd1b25e06359d6eceb655093f44f0255c799ae8a3fc5bf8ba50fd8d in / 
# Mon, 09 Oct 2017 21:42:31 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 00:57:28 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 00:57:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 00:58:35 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d8b3cf5f6e0f087738d5589b812e12f5b8781935412c95d15f2f77d68657b006`  
		Last Modified: Mon, 09 Oct 2017 21:48:54 GMT  
		Size: 30.3 MB (30264454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6db9a23ef19b82644ae3cc18a517df0a01579623915a4d0ea810e09c608927`  
		Last Modified: Tue, 17 Oct 2017 01:02:43 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e350d9d1943c6f652c74dd24e15cbdf943755f73fa0942cb0a1d8b12187ece`  
		Last Modified: Tue, 17 Oct 2017 01:02:49 GMT  
		Size: 29.1 MB (29051973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.4.0-slim`

```console
$ docker pull mono@sha256:8bb8acd652efd1a6f2c35ac9f384d02b010b3db0802b20fdeb1d65444e2d5d9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.4.0-slim` - linux; amd64

```console
$ docker pull mono@sha256:6fa11ce8b3e4f282aec74ac5a67b2a9f4870bea61d1d78559e7ee5b214b82d35
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57393972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b1edbbef1ba391ad23c0143f4dcb99071ea629a89326753fb24f7b718efcf8`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:31:06 GMT
ADD file:187fe0df97a4c52984a518a454fb7ab3984ae7b541ede7ff84dd3c5da1ce1a59 in / 
# Mon, 09 Oct 2017 21:31:06 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:27:41 GMT
ENV MONO_VERSION=5.4.0.201
# Sat, 04 Nov 2017 02:27:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:28:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d13d02fa248db2b423d6dbc8ec435675d23122f3939b5278b2156b75258e2259`  
		Last Modified: Mon, 09 Oct 2017 21:37:31 GMT  
		Size: 30.1 MB (30113318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8d78a964aa167e2e8dbfd3365f8445ed149628507a2aa9dfaacde4e97c83b3`  
		Last Modified: Sat, 04 Nov 2017 02:36:19 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c98de1760e34ac9792d43e7e171574a9d63a20a7bff3bf03e29ef3fa026362`  
		Last Modified: Sat, 04 Nov 2017 02:36:31 GMT  
		Size: 27.3 MB (27278585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:5f8055656d4c37b7f31bd06a372376d76050217a4de7975a6a5f637796e3ce37
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48318085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f2e28a554ed459c68d737d67e3d3814f15caaf9dbc2025cd52f59957bfbd37c`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:41 GMT
ADD file:0cd8ed314febdbf680645d20f346d9bac16fad5654c0b0d6ce2dec7c27c17b9a in / 
# Mon, 09 Oct 2017 21:42:41 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 17:51:32 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 17:51:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 17:52:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:02620033936d6cf3514a813f366025a14370f5dfe654e89eaca3a56b357e88c2`  
		Last Modified: Mon, 09 Oct 2017 21:49:15 GMT  
		Size: 26.3 MB (26280982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebc5f99dc26f440db883809cd8379ade7a516c92b91b7d22ae6485b1278ab1f`  
		Last Modified: Tue, 17 Oct 2017 17:55:04 GMT  
		Size: 2.1 KB (2065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dec16e095e6115a08f0f8530cdfde275c707acbc3fbb2fcc735b863a95122c1`  
		Last Modified: Tue, 17 Oct 2017 17:55:12 GMT  
		Size: 22.0 MB (22035038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:7c7acc4cd80b4ceaa4309ce4aed1d02f3b7c7209957ffafee4c7cc4cad16e8af
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53681920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8480909fbc33d90b5dee55a454ea5be52d3f9c8704ed3e60058f7bce5e2d85b4`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:43:51 GMT
ADD file:75f5768db078e9eee90676141a2c9faa9ce02768b7c9cd6e588bdd5ffc0f65e3 in / 
# Mon, 09 Oct 2017 21:43:51 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 19:45:44 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 19:45:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 19:47:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f2da27d97c13e9e531eda9577a28eb81b0d9034d7fd7e6575bd92744eed500f6`  
		Last Modified: Mon, 09 Oct 2017 21:53:20 GMT  
		Size: 27.5 MB (27480591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad3574e8978c5cdfc63d800a5b8666c43c9d93519dbe83105d3ffdb6bac9f8a`  
		Last Modified: Tue, 17 Oct 2017 19:53:55 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b32240292f03d8f265e50d58923a86660a5730b335e0dc5eb333ae7890cd921`  
		Last Modified: Tue, 17 Oct 2017 19:54:07 GMT  
		Size: 26.2 MB (26199265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4.0-slim` - linux; 386

```console
$ docker pull mono@sha256:1c1e2d0453aa51c38f1a9c5d857326a7d2584187a3d6b97c7d134857b313eaca
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59318493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc39ab72d2a85482d0fb58d096da734fa000dea510d2a2d0f2ef4dcfcf4e9350`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:30 GMT
ADD file:169ab3194fd1b25e06359d6eceb655093f44f0255c799ae8a3fc5bf8ba50fd8d in / 
# Mon, 09 Oct 2017 21:42:31 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 00:57:28 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 00:57:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 00:58:35 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d8b3cf5f6e0f087738d5589b812e12f5b8781935412c95d15f2f77d68657b006`  
		Last Modified: Mon, 09 Oct 2017 21:48:54 GMT  
		Size: 30.3 MB (30264454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6db9a23ef19b82644ae3cc18a517df0a01579623915a4d0ea810e09c608927`  
		Last Modified: Tue, 17 Oct 2017 01:02:43 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e350d9d1943c6f652c74dd24e15cbdf943755f73fa0942cb0a1d8b12187ece`  
		Last Modified: Tue, 17 Oct 2017 01:02:49 GMT  
		Size: 29.1 MB (29051973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.4-slim`

```console
$ docker pull mono@sha256:8bb8acd652efd1a6f2c35ac9f384d02b010b3db0802b20fdeb1d65444e2d5d9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5.4-slim` - linux; amd64

```console
$ docker pull mono@sha256:6fa11ce8b3e4f282aec74ac5a67b2a9f4870bea61d1d78559e7ee5b214b82d35
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57393972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b1edbbef1ba391ad23c0143f4dcb99071ea629a89326753fb24f7b718efcf8`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:31:06 GMT
ADD file:187fe0df97a4c52984a518a454fb7ab3984ae7b541ede7ff84dd3c5da1ce1a59 in / 
# Mon, 09 Oct 2017 21:31:06 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:27:41 GMT
ENV MONO_VERSION=5.4.0.201
# Sat, 04 Nov 2017 02:27:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:28:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d13d02fa248db2b423d6dbc8ec435675d23122f3939b5278b2156b75258e2259`  
		Last Modified: Mon, 09 Oct 2017 21:37:31 GMT  
		Size: 30.1 MB (30113318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8d78a964aa167e2e8dbfd3365f8445ed149628507a2aa9dfaacde4e97c83b3`  
		Last Modified: Sat, 04 Nov 2017 02:36:19 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c98de1760e34ac9792d43e7e171574a9d63a20a7bff3bf03e29ef3fa026362`  
		Last Modified: Sat, 04 Nov 2017 02:36:31 GMT  
		Size: 27.3 MB (27278585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:5f8055656d4c37b7f31bd06a372376d76050217a4de7975a6a5f637796e3ce37
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48318085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f2e28a554ed459c68d737d67e3d3814f15caaf9dbc2025cd52f59957bfbd37c`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:41 GMT
ADD file:0cd8ed314febdbf680645d20f346d9bac16fad5654c0b0d6ce2dec7c27c17b9a in / 
# Mon, 09 Oct 2017 21:42:41 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 17:51:32 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 17:51:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 17:52:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:02620033936d6cf3514a813f366025a14370f5dfe654e89eaca3a56b357e88c2`  
		Last Modified: Mon, 09 Oct 2017 21:49:15 GMT  
		Size: 26.3 MB (26280982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebc5f99dc26f440db883809cd8379ade7a516c92b91b7d22ae6485b1278ab1f`  
		Last Modified: Tue, 17 Oct 2017 17:55:04 GMT  
		Size: 2.1 KB (2065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dec16e095e6115a08f0f8530cdfde275c707acbc3fbb2fcc735b863a95122c1`  
		Last Modified: Tue, 17 Oct 2017 17:55:12 GMT  
		Size: 22.0 MB (22035038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:7c7acc4cd80b4ceaa4309ce4aed1d02f3b7c7209957ffafee4c7cc4cad16e8af
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53681920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8480909fbc33d90b5dee55a454ea5be52d3f9c8704ed3e60058f7bce5e2d85b4`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:43:51 GMT
ADD file:75f5768db078e9eee90676141a2c9faa9ce02768b7c9cd6e588bdd5ffc0f65e3 in / 
# Mon, 09 Oct 2017 21:43:51 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 19:45:44 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 19:45:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 19:47:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f2da27d97c13e9e531eda9577a28eb81b0d9034d7fd7e6575bd92744eed500f6`  
		Last Modified: Mon, 09 Oct 2017 21:53:20 GMT  
		Size: 27.5 MB (27480591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad3574e8978c5cdfc63d800a5b8666c43c9d93519dbe83105d3ffdb6bac9f8a`  
		Last Modified: Tue, 17 Oct 2017 19:53:55 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b32240292f03d8f265e50d58923a86660a5730b335e0dc5eb333ae7890cd921`  
		Last Modified: Tue, 17 Oct 2017 19:54:07 GMT  
		Size: 26.2 MB (26199265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.4-slim` - linux; 386

```console
$ docker pull mono@sha256:1c1e2d0453aa51c38f1a9c5d857326a7d2584187a3d6b97c7d134857b313eaca
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59318493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc39ab72d2a85482d0fb58d096da734fa000dea510d2a2d0f2ef4dcfcf4e9350`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:30 GMT
ADD file:169ab3194fd1b25e06359d6eceb655093f44f0255c799ae8a3fc5bf8ba50fd8d in / 
# Mon, 09 Oct 2017 21:42:31 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 00:57:28 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 00:57:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 00:58:35 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d8b3cf5f6e0f087738d5589b812e12f5b8781935412c95d15f2f77d68657b006`  
		Last Modified: Mon, 09 Oct 2017 21:48:54 GMT  
		Size: 30.3 MB (30264454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6db9a23ef19b82644ae3cc18a517df0a01579623915a4d0ea810e09c608927`  
		Last Modified: Tue, 17 Oct 2017 01:02:43 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e350d9d1943c6f652c74dd24e15cbdf943755f73fa0942cb0a1d8b12187ece`  
		Last Modified: Tue, 17 Oct 2017 01:02:49 GMT  
		Size: 29.1 MB (29051973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5-slim`

```console
$ docker pull mono@sha256:8bb8acd652efd1a6f2c35ac9f384d02b010b3db0802b20fdeb1d65444e2d5d9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:5-slim` - linux; amd64

```console
$ docker pull mono@sha256:6fa11ce8b3e4f282aec74ac5a67b2a9f4870bea61d1d78559e7ee5b214b82d35
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57393972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b1edbbef1ba391ad23c0143f4dcb99071ea629a89326753fb24f7b718efcf8`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:31:06 GMT
ADD file:187fe0df97a4c52984a518a454fb7ab3984ae7b541ede7ff84dd3c5da1ce1a59 in / 
# Mon, 09 Oct 2017 21:31:06 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:27:41 GMT
ENV MONO_VERSION=5.4.0.201
# Sat, 04 Nov 2017 02:27:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:28:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d13d02fa248db2b423d6dbc8ec435675d23122f3939b5278b2156b75258e2259`  
		Last Modified: Mon, 09 Oct 2017 21:37:31 GMT  
		Size: 30.1 MB (30113318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8d78a964aa167e2e8dbfd3365f8445ed149628507a2aa9dfaacde4e97c83b3`  
		Last Modified: Sat, 04 Nov 2017 02:36:19 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c98de1760e34ac9792d43e7e171574a9d63a20a7bff3bf03e29ef3fa026362`  
		Last Modified: Sat, 04 Nov 2017 02:36:31 GMT  
		Size: 27.3 MB (27278585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:5f8055656d4c37b7f31bd06a372376d76050217a4de7975a6a5f637796e3ce37
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48318085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f2e28a554ed459c68d737d67e3d3814f15caaf9dbc2025cd52f59957bfbd37c`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:41 GMT
ADD file:0cd8ed314febdbf680645d20f346d9bac16fad5654c0b0d6ce2dec7c27c17b9a in / 
# Mon, 09 Oct 2017 21:42:41 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 17:51:32 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 17:51:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 17:52:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:02620033936d6cf3514a813f366025a14370f5dfe654e89eaca3a56b357e88c2`  
		Last Modified: Mon, 09 Oct 2017 21:49:15 GMT  
		Size: 26.3 MB (26280982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebc5f99dc26f440db883809cd8379ade7a516c92b91b7d22ae6485b1278ab1f`  
		Last Modified: Tue, 17 Oct 2017 17:55:04 GMT  
		Size: 2.1 KB (2065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dec16e095e6115a08f0f8530cdfde275c707acbc3fbb2fcc735b863a95122c1`  
		Last Modified: Tue, 17 Oct 2017 17:55:12 GMT  
		Size: 22.0 MB (22035038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:7c7acc4cd80b4ceaa4309ce4aed1d02f3b7c7209957ffafee4c7cc4cad16e8af
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53681920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8480909fbc33d90b5dee55a454ea5be52d3f9c8704ed3e60058f7bce5e2d85b4`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:43:51 GMT
ADD file:75f5768db078e9eee90676141a2c9faa9ce02768b7c9cd6e588bdd5ffc0f65e3 in / 
# Mon, 09 Oct 2017 21:43:51 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 19:45:44 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 19:45:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 19:47:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f2da27d97c13e9e531eda9577a28eb81b0d9034d7fd7e6575bd92744eed500f6`  
		Last Modified: Mon, 09 Oct 2017 21:53:20 GMT  
		Size: 27.5 MB (27480591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad3574e8978c5cdfc63d800a5b8666c43c9d93519dbe83105d3ffdb6bac9f8a`  
		Last Modified: Tue, 17 Oct 2017 19:53:55 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b32240292f03d8f265e50d58923a86660a5730b335e0dc5eb333ae7890cd921`  
		Last Modified: Tue, 17 Oct 2017 19:54:07 GMT  
		Size: 26.2 MB (26199265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; 386

```console
$ docker pull mono@sha256:1c1e2d0453aa51c38f1a9c5d857326a7d2584187a3d6b97c7d134857b313eaca
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59318493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc39ab72d2a85482d0fb58d096da734fa000dea510d2a2d0f2ef4dcfcf4e9350`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:30 GMT
ADD file:169ab3194fd1b25e06359d6eceb655093f44f0255c799ae8a3fc5bf8ba50fd8d in / 
# Mon, 09 Oct 2017 21:42:31 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 00:57:28 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 00:57:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 00:58:35 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d8b3cf5f6e0f087738d5589b812e12f5b8781935412c95d15f2f77d68657b006`  
		Last Modified: Mon, 09 Oct 2017 21:48:54 GMT  
		Size: 30.3 MB (30264454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6db9a23ef19b82644ae3cc18a517df0a01579623915a4d0ea810e09c608927`  
		Last Modified: Tue, 17 Oct 2017 01:02:43 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e350d9d1943c6f652c74dd24e15cbdf943755f73fa0942cb0a1d8b12187ece`  
		Last Modified: Tue, 17 Oct 2017 01:02:49 GMT  
		Size: 29.1 MB (29051973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:latest`

```console
$ docker pull mono@sha256:17a2b85ec4c0942e16c4e6499a57e15ae9c09c2b9034b3ec58b0c23171311902
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:latest` - linux; amd64

```console
$ docker pull mono@sha256:932cd8cc4dfb08336ba3a5bd31feb361afdb82b5d2c203691fc956b3fce22a3d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.3 MB (167259115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d59c2a7018c7acd0024da96ecfcf7f1f778f58db827bb41788608e53494bb94b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:31:06 GMT
ADD file:187fe0df97a4c52984a518a454fb7ab3984ae7b541ede7ff84dd3c5da1ce1a59 in / 
# Mon, 09 Oct 2017 21:31:06 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:27:41 GMT
ENV MONO_VERSION=5.4.0.201
# Sat, 04 Nov 2017 02:27:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:28:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 04 Nov 2017 02:33:42 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d13d02fa248db2b423d6dbc8ec435675d23122f3939b5278b2156b75258e2259`  
		Last Modified: Mon, 09 Oct 2017 21:37:31 GMT  
		Size: 30.1 MB (30113318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8d78a964aa167e2e8dbfd3365f8445ed149628507a2aa9dfaacde4e97c83b3`  
		Last Modified: Sat, 04 Nov 2017 02:36:19 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c98de1760e34ac9792d43e7e171574a9d63a20a7bff3bf03e29ef3fa026362`  
		Last Modified: Sat, 04 Nov 2017 02:36:31 GMT  
		Size: 27.3 MB (27278585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59b45d6dbf7cd29de575aafcd18d219efc175d67692860d0f4b9be03a8efd4d`  
		Last Modified: Sat, 04 Nov 2017 02:38:48 GMT  
		Size: 109.9 MB (109865143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v7

```console
$ docker pull mono@sha256:5189f8b756032897bb3d03f9e1d396ae72a70d1c66c6fcdd8e6b65f3d921fdb0
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.0 MB (147049823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff518dee16442d023eb4b88925989b6defdb55141b58851d208299cedff5f3c4`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:41 GMT
ADD file:0cd8ed314febdbf680645d20f346d9bac16fad5654c0b0d6ce2dec7c27c17b9a in / 
# Mon, 09 Oct 2017 21:42:41 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 17:51:32 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 17:51:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 17:52:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 17 Oct 2017 17:54:46 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:02620033936d6cf3514a813f366025a14370f5dfe654e89eaca3a56b357e88c2`  
		Last Modified: Mon, 09 Oct 2017 21:49:15 GMT  
		Size: 26.3 MB (26280982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebc5f99dc26f440db883809cd8379ade7a516c92b91b7d22ae6485b1278ab1f`  
		Last Modified: Tue, 17 Oct 2017 17:55:04 GMT  
		Size: 2.1 KB (2065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dec16e095e6115a08f0f8530cdfde275c707acbc3fbb2fcc735b863a95122c1`  
		Last Modified: Tue, 17 Oct 2017 17:55:12 GMT  
		Size: 22.0 MB (22035038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c10ba59aa47230cfdc9ee37e8f10718b4c017c2b4906920d0a1ff1b75edad`  
		Last Modified: Tue, 17 Oct 2017 17:56:17 GMT  
		Size: 98.7 MB (98731738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:a68c168b05a89256ded341eeebe49ae1ab5b96523ccbac7001c9e317a0dbd754
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161639631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd34d0efd84450956a53481cef2b10afae252d3f095fc8b53c3e142529cb3009`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:43:51 GMT
ADD file:75f5768db078e9eee90676141a2c9faa9ce02768b7c9cd6e588bdd5ffc0f65e3 in / 
# Mon, 09 Oct 2017 21:43:51 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 19:45:44 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 19:45:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 19:47:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 17 Oct 2017 19:53:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f2da27d97c13e9e531eda9577a28eb81b0d9034d7fd7e6575bd92744eed500f6`  
		Last Modified: Mon, 09 Oct 2017 21:53:20 GMT  
		Size: 27.5 MB (27480591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad3574e8978c5cdfc63d800a5b8666c43c9d93519dbe83105d3ffdb6bac9f8a`  
		Last Modified: Tue, 17 Oct 2017 19:53:55 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b32240292f03d8f265e50d58923a86660a5730b335e0dc5eb333ae7890cd921`  
		Last Modified: Tue, 17 Oct 2017 19:54:07 GMT  
		Size: 26.2 MB (26199265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d3f2ac099ead527a80c01317816b1cbcbcbe0d86403a39344baa73cda1baae`  
		Last Modified: Tue, 17 Oct 2017 19:55:50 GMT  
		Size: 108.0 MB (107957711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; 386

```console
$ docker pull mono@sha256:8b249344ca9584956ed7cb4635f29d545514ca86632705311522274cb2122121
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169638409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a8176ed9b7b0401eb795893a084727d27552a6c788477df53e8e54d4dbc386`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:30 GMT
ADD file:169ab3194fd1b25e06359d6eceb655093f44f0255c799ae8a3fc5bf8ba50fd8d in / 
# Mon, 09 Oct 2017 21:42:31 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 00:57:28 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 00:57:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 00:58:35 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 17 Oct 2017 01:00:06 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d8b3cf5f6e0f087738d5589b812e12f5b8781935412c95d15f2f77d68657b006`  
		Last Modified: Mon, 09 Oct 2017 21:48:54 GMT  
		Size: 30.3 MB (30264454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6db9a23ef19b82644ae3cc18a517df0a01579623915a4d0ea810e09c608927`  
		Last Modified: Tue, 17 Oct 2017 01:02:43 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e350d9d1943c6f652c74dd24e15cbdf943755f73fa0942cb0a1d8b12187ece`  
		Last Modified: Tue, 17 Oct 2017 01:02:49 GMT  
		Size: 29.1 MB (29051973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88be8b6ac98f875586bdbda4e5ffcbea6d9d7210c018d5213e75c5a0d6e1dd4a`  
		Last Modified: Tue, 17 Oct 2017 01:05:06 GMT  
		Size: 110.3 MB (110319916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:slim`

```console
$ docker pull mono@sha256:8bb8acd652efd1a6f2c35ac9f384d02b010b3db0802b20fdeb1d65444e2d5d9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:slim` - linux; amd64

```console
$ docker pull mono@sha256:6fa11ce8b3e4f282aec74ac5a67b2a9f4870bea61d1d78559e7ee5b214b82d35
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57393972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b1edbbef1ba391ad23c0143f4dcb99071ea629a89326753fb24f7b718efcf8`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:31:06 GMT
ADD file:187fe0df97a4c52984a518a454fb7ab3984ae7b541ede7ff84dd3c5da1ce1a59 in / 
# Mon, 09 Oct 2017 21:31:06 GMT
CMD ["bash"]
# Sat, 04 Nov 2017 02:27:41 GMT
ENV MONO_VERSION=5.4.0.201
# Sat, 04 Nov 2017 02:27:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Sat, 04 Nov 2017 02:28:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d13d02fa248db2b423d6dbc8ec435675d23122f3939b5278b2156b75258e2259`  
		Last Modified: Mon, 09 Oct 2017 21:37:31 GMT  
		Size: 30.1 MB (30113318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8d78a964aa167e2e8dbfd3365f8445ed149628507a2aa9dfaacde4e97c83b3`  
		Last Modified: Sat, 04 Nov 2017 02:36:19 GMT  
		Size: 2.1 KB (2069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c98de1760e34ac9792d43e7e171574a9d63a20a7bff3bf03e29ef3fa026362`  
		Last Modified: Sat, 04 Nov 2017 02:36:31 GMT  
		Size: 27.3 MB (27278585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:5f8055656d4c37b7f31bd06a372376d76050217a4de7975a6a5f637796e3ce37
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48318085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f2e28a554ed459c68d737d67e3d3814f15caaf9dbc2025cd52f59957bfbd37c`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:41 GMT
ADD file:0cd8ed314febdbf680645d20f346d9bac16fad5654c0b0d6ce2dec7c27c17b9a in / 
# Mon, 09 Oct 2017 21:42:41 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 17:51:32 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 17:51:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 17:52:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:02620033936d6cf3514a813f366025a14370f5dfe654e89eaca3a56b357e88c2`  
		Last Modified: Mon, 09 Oct 2017 21:49:15 GMT  
		Size: 26.3 MB (26280982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebc5f99dc26f440db883809cd8379ade7a516c92b91b7d22ae6485b1278ab1f`  
		Last Modified: Tue, 17 Oct 2017 17:55:04 GMT  
		Size: 2.1 KB (2065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dec16e095e6115a08f0f8530cdfde275c707acbc3fbb2fcc735b863a95122c1`  
		Last Modified: Tue, 17 Oct 2017 17:55:12 GMT  
		Size: 22.0 MB (22035038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:7c7acc4cd80b4ceaa4309ce4aed1d02f3b7c7209957ffafee4c7cc4cad16e8af
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53681920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8480909fbc33d90b5dee55a454ea5be52d3f9c8704ed3e60058f7bce5e2d85b4`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:43:51 GMT
ADD file:75f5768db078e9eee90676141a2c9faa9ce02768b7c9cd6e588bdd5ffc0f65e3 in / 
# Mon, 09 Oct 2017 21:43:51 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 19:45:44 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 19:45:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 19:47:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f2da27d97c13e9e531eda9577a28eb81b0d9034d7fd7e6575bd92744eed500f6`  
		Last Modified: Mon, 09 Oct 2017 21:53:20 GMT  
		Size: 27.5 MB (27480591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad3574e8978c5cdfc63d800a5b8666c43c9d93519dbe83105d3ffdb6bac9f8a`  
		Last Modified: Tue, 17 Oct 2017 19:53:55 GMT  
		Size: 2.1 KB (2064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b32240292f03d8f265e50d58923a86660a5730b335e0dc5eb333ae7890cd921`  
		Last Modified: Tue, 17 Oct 2017 19:54:07 GMT  
		Size: 26.2 MB (26199265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; 386

```console
$ docker pull mono@sha256:1c1e2d0453aa51c38f1a9c5d857326a7d2584187a3d6b97c7d134857b313eaca
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59318493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc39ab72d2a85482d0fb58d096da734fa000dea510d2a2d0f2ef4dcfcf4e9350`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:42:30 GMT
ADD file:169ab3194fd1b25e06359d6eceb655093f44f0255c799ae8a3fc5bf8ba50fd8d in / 
# Mon, 09 Oct 2017 21:42:31 GMT
CMD ["bash"]
# Tue, 17 Oct 2017 00:57:28 GMT
ENV MONO_VERSION=5.4.0.201
# Tue, 17 Oct 2017 00:57:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 17 Oct 2017 00:58:35 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d8b3cf5f6e0f087738d5589b812e12f5b8781935412c95d15f2f77d68657b006`  
		Last Modified: Mon, 09 Oct 2017 21:48:54 GMT  
		Size: 30.3 MB (30264454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6db9a23ef19b82644ae3cc18a517df0a01579623915a4d0ea810e09c608927`  
		Last Modified: Tue, 17 Oct 2017 01:02:43 GMT  
		Size: 2.1 KB (2066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e350d9d1943c6f652c74dd24e15cbdf943755f73fa0942cb0a1d8b12187ece`  
		Last Modified: Tue, 17 Oct 2017 01:02:49 GMT  
		Size: 29.1 MB (29051973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
