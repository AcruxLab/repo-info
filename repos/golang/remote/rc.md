## `golang:rc`

```console
$ docker pull golang@sha256:84b74893325b4e81bc871ecaa5317730c64bc807b29b660443af6fdbc34cf94e
```

-	Platforms:
	-	linux; amd64

### `golang:rc` - linux; amd64

-	Docker Version: 1.12.6
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.0 MB (260998314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f98b82c517dbec9c4ced9edd3ade6d071af27007bd3d2a183607ae9190a1fcbc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 16 Jan 2017 20:35:09 GMT
ADD file:89ecb642d662ee7edbb868340551106d51336c7e589fdaca4111725ec64da957 in / 
# Mon, 16 Jan 2017 20:35:16 GMT
CMD ["/bin/bash"]
# Tue, 17 Jan 2017 00:00:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Jan 2017 00:01:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Jan 2017 00:40:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 27 Jan 2017 22:39:49 GMT
ENV GOLANG_VERSION=1.8rc3
# Fri, 27 Jan 2017 22:39:49 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.8rc3.linux-amd64.tar.gz
# Fri, 27 Jan 2017 22:39:50 GMT
ENV GOLANG_DOWNLOAD_SHA256=0ff3faba02ac83920a65b453785771e75f128fbf9ba4ad1d5e72c044103f9c7a
# Fri, 27 Jan 2017 22:40:00 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 27 Jan 2017 22:40:01 GMT
ENV GOPATH=/go
# Fri, 27 Jan 2017 22:40:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Jan 2017 22:40:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 27 Jan 2017 22:40:03 GMT
WORKDIR /go
# Fri, 27 Jan 2017 22:40:04 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/ 
```

-	Layers:
	-	`sha256:5040bd2983909aa8896b9932438c3f1479d25ae837a5f6220242a264d0221f2d`  
		Last Modified: Mon, 16 Jan 2017 20:43:26 GMT  
		Size: 51.4 MB (51361210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce5728aad85a763fe3c419db16885eb6f7a670a42824ea618414b8fb309ccde`  
		Last Modified: Tue, 17 Jan 2017 00:19:41 GMT  
		Size: 18.5 MB (18535441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76610ec20bf5892e24cebd4153c7668284aa1d1151b7c3b0c7d50c579aa5ce75`  
		Last Modified: Tue, 17 Jan 2017 00:20:34 GMT  
		Size: 42.5 MB (42502406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b681f75ff656775b833d40e824f47d5b46215fd8a2e829b2b9cf89b28a1628`  
		Last Modified: Wed, 18 Jan 2017 03:45:10 GMT  
		Size: 59.7 MB (59661679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617cf8ca49ad3918926c6695ca04e6d4543aeab0ecd727a5a934b3e6d2f6a645`  
		Last Modified: Fri, 27 Jan 2017 22:54:48 GMT  
		Size: 88.9 MB (88936097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc98e8b55734e8dab79bde49da1e07aeee6b40c7b577390f852f0ff67dd3653b`  
		Last Modified: Fri, 27 Jan 2017 22:54:24 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a954461f63a22eed75ee8078607bb8a2efd1d2ec9e2fab17f13c7e5828e2d285`  
		Last Modified: Fri, 27 Jan 2017 22:54:24 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
