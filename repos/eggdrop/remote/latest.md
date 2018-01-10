## `eggdrop:latest`

```console
$ docker pull eggdrop@sha256:e94857215b0dd17358d381846669cc4b890b2701d47334866999358d8ee4f59e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `eggdrop:latest` - linux; amd64

```console
$ docker pull eggdrop@sha256:7361a6c942bc44bef6d41a7365496a00491f2e34b35f20b9339dcd44de0eba11
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7485731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97eeb0fcd3d4bca97229c90d7bc42077bd712d0e3d480d422d1bf3ab976d8cb2`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 09 Jan 2018 21:12:40 GMT
ADD file:69848cb51056edaf120230b6f218a79968ac797295c2cef6728332e1801357be in / 
# Tue, 09 Jan 2018 21:12:40 GMT
CMD ["/bin/sh"]
# Wed, 10 Jan 2018 03:30:24 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 10 Jan 2018 03:30:25 GMT
RUN adduser -S eggdrop
# Wed, 10 Jan 2018 03:30:28 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 10 Jan 2018 03:30:34 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 10 Jan 2018 03:31:48 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.2.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.8.2.tar.gz.asc eggdrop-1.8.2.tar.gz   && rm eggdrop-1.8.2.tar.gz.asc   && tar -zxvf eggdrop-1.8.2.tar.gz   && rm eggdrop-1.8.2.tar.gz   && ( cd eggdrop-1.8.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.8.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 10 Jan 2018 03:31:49 GMT
ENV NICK=
# Wed, 10 Jan 2018 03:31:49 GMT
ENV SERVER=
# Wed, 10 Jan 2018 03:31:49 GMT
ENV LISTEN=3333
# Wed, 10 Jan 2018 03:31:49 GMT
ENV OWNER=
# Wed, 10 Jan 2018 03:31:50 GMT
ENV USERFILE=eggdrop.user
# Wed, 10 Jan 2018 03:31:50 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 10 Jan 2018 03:31:50 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 10 Jan 2018 03:31:50 GMT
EXPOSE 3333/tcp
# Wed, 10 Jan 2018 03:31:51 GMT
COPY file:d80744926cf822928c4fc2c3f9107364df320eecb3ae407a3a5419a43ae4b872 in /home/eggdrop/eggdrop 
# Wed, 10 Jan 2018 03:31:51 GMT
COPY file:919804e5ddd4c807c178caccfed03e9d75a459fe0f744c3a1ada109817cb44ec in /home/eggdrop/eggdrop/scripts/ 
# Wed, 10 Jan 2018 03:31:51 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 10 Jan 2018 03:31:52 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:81033e7c1d6a5b44a94bb6b40033a6e589f50fd6b61578da6fc809e61f83898d`  
		Last Modified: Tue, 09 Jan 2018 21:15:04 GMT  
		Size: 2.4 MB (2387570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9413c66d316f56ae3bfd7bc12aa1a2c4a82eefd528df4eb85ebdd45fd5b8b792`  
		Last Modified: Wed, 10 Jan 2018 03:42:12 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972f7b58131ab5c128e2b252d614f4d72d3f9ad6c49c9351a8ce8e44dbb12908`  
		Last Modified: Wed, 10 Jan 2018 03:42:10 GMT  
		Size: 8.1 KB (8055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f252f07c5cd093948fad5a7c30c59301392d14c9765aa09f4a2071ab9a52f057`  
		Last Modified: Wed, 10 Jan 2018 03:42:11 GMT  
		Size: 2.9 MB (2938621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac789379e71dbad827ab68a0e9a0807c95e40cea84c00514cfca0664d1f6509e`  
		Last Modified: Wed, 10 Jan 2018 03:42:11 GMT  
		Size: 2.1 MB (2147625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53280f251829b7f5b0f6e9388288802a11695a08739303639fdd161efd409b1f`  
		Last Modified: Wed, 10 Jan 2018 03:42:10 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db391956bd4314325378e8a38e4dd7320a05a77b0348b78e78726a92a653c26`  
		Last Modified: Wed, 10 Jan 2018 03:42:11 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
