## `mono:latest`

```console
$ docker pull mono@sha256:d0a58d5b964e7455a3b33d511cf193fb3c5ad6490c20762cfa0ecc10c1623e50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `mono:latest` - linux; amd64

```console
$ docker pull mono@sha256:9a61311f382cca999579d4ceb75015e41f3b1c4aadf3d81d3f6915363c46f114
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.0 MB (170039430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6df13f0b8472f903345aa10b310e849d6e8ee03035895d53a805b4d19ba9ad9`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 09 Oct 2017 21:31:06 GMT
ADD file:187fe0df97a4c52984a518a454fb7ab3984ae7b541ede7ff84dd3c5da1ce1a59 in / 
# Mon, 09 Oct 2017 21:31:06 GMT
CMD ["bash"]
# Tue, 10 Oct 2017 00:10:52 GMT
ENV MONO_VERSION=5.2.0.224
# Tue, 10 Oct 2017 00:10:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
# Tue, 10 Oct 2017 00:11:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 10 Oct 2017 00:20:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d13d02fa248db2b423d6dbc8ec435675d23122f3939b5278b2156b75258e2259`  
		Last Modified: Mon, 09 Oct 2017 21:37:31 GMT  
		Size: 30.1 MB (30113318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752ae4b42e2f5c6231e4c843dd5c8afde29150a1124d4720d9ef641e35b8bf7f`  
		Last Modified: Tue, 10 Oct 2017 00:20:30 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c7865de4a94d89f524c7706d368c9d1695df91cc9cb22d8e08a796f511aaf3`  
		Last Modified: Tue, 10 Oct 2017 00:20:38 GMT  
		Size: 27.2 MB (27240757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b6ed2742ed96eaf012de781ddf0dab03056127a4742536d08659ae4dc5bdf9`  
		Last Modified: Tue, 10 Oct 2017 00:24:57 GMT  
		Size: 112.7 MB (112683295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v7

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

### `mono:latest` - linux; arm64 variant v8

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

### `mono:latest` - linux; 386

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
