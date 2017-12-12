## `debian:wheezy-backports`

```console
$ docker pull debian@sha256:47cad617882fd891d816e09d82de23b402298c6940027ff4cdec078b795a3400
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `debian:wheezy-backports` - linux; amd64

```console
$ docker pull debian@sha256:a7f0b8db3c658e818ac2bfbbab75dcfd84ed5cf17ed20b93ef9442e1a2ec9ecc
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38110051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac409e5e5d523c17e46c1b1d6429741fb66976089574e122a41e85db5a1cc54`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 01:46:04 GMT
ADD file:281b987b09ac9b71793de5201331461636a08ec23af27a9e11a14484018993dd in / 
# Tue, 12 Dec 2017 01:46:04 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 01:46:13 GMT
RUN echo 'deb http://deb.debian.org/debian wheezy-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:762ae076e9a326e4eac3b3db9e3afe4b6dc930ec52dbb2aa27a300d1323a52b6`  
		Last Modified: Tue, 12 Dec 2017 01:59:44 GMT  
		Size: 38.1 MB (38109825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e748540136a3141b35832c1333c2290f5ebafb6aa79b7f35646ce81d4586c0`  
		Last Modified: Tue, 12 Dec 2017 02:00:21 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:wheezy-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:449e4f6c028f59067a0eac9186750e242648d0a7c0d7105c604bcb37d4e2b978
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36949219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a94464ffb88610c14cdb4f90d9a7646a16e490446666a81c68cc766356d0b7d0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 21:04:23 GMT
ADD file:dfb8b543feb8007b990cb5a0dc88e61b84ec22ac2c756ad3ab084b5c46f0d66c in / 
# Tue, 12 Dec 2017 21:04:23 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 21:04:36 GMT
RUN echo 'deb http://deb.debian.org/debian wheezy-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8d01839394fae71ab18c6d4fa6e8f5ff303a13afca2fa23b3b65c12fae1b5fd5`  
		Last Modified: Tue, 12 Dec 2017 21:14:56 GMT  
		Size: 36.9 MB (36948993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8675a7f86f83741fef0c0438e27081f725de2338b50a6a5c8d48d8b252c81043`  
		Last Modified: Tue, 12 Dec 2017 21:15:29 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:wheezy-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:be926a66181a06019a73f39251bf69c1e619e190ea3934cb0f51033000f70a0b
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35662033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2db41752f8c5f1d9c607cae147028c9d69f888fe7d94f63ff99dbdfb2460a650`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 13:36:11 GMT
ADD file:9db26feeeebe82707411c8b6a09f22ba8e33fdd8bdf1e1cb3fd179cfc09b850e in / 
# Tue, 12 Dec 2017 13:36:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 13:36:26 GMT
RUN echo 'deb http://deb.debian.org/debian wheezy-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:dd70000a68c40049fa024e9ebecc22bcd8a32b0fb098e9f3edafdbfc872054b4`  
		Last Modified: Tue, 12 Dec 2017 13:47:59 GMT  
		Size: 35.7 MB (35661805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700ed548cd81f1613e88868df3b9ee7ad98c14c976bf702a97dfeeb189f91172`  
		Last Modified: Tue, 12 Dec 2017 13:48:44 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:wheezy-backports` - linux; 386

```console
$ docker pull debian@sha256:863c7919414633de368b5b05c0d342a58f4606100075f98cb4e46ca47078f311
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37439531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed4a242da1ff75c6caae9bf6c174176c8e31c0e9eca1df3443b804330f9cd2d4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 14:43:45 GMT
ADD file:1ef271fafe70405fd17417a29b02b0245708b5a9acd0d979e7c8ed32371cf210 in / 
# Tue, 12 Dec 2017 14:43:45 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:43:58 GMT
RUN echo 'deb http://deb.debian.org/debian wheezy-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:20f7e6bd30947be27e2a6eed841278c2fcff0db722334016a488feae3ae65859`  
		Last Modified: Tue, 12 Dec 2017 15:09:23 GMT  
		Size: 37.4 MB (37439308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda54b0898b001ab6c7fc1807c3ee60cd49894191d604ddb9ed7e244449a8ffa`  
		Last Modified: Tue, 12 Dec 2017 15:10:16 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
