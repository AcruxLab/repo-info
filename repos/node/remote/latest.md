## `node:latest`

```console
$ docker pull node@sha256:d5f73a893ea24dcf920d7b15d2a8a006e130dcb98d2b41dd50f2951abcdb5dc8
```

-	Platforms:
	-	linux; amd64

### `node:latest` - linux; amd64

-	Docker Version: 17.04.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.0 MB (259048887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ca756a6578b9134f0ea78fbfb941a385e6837dff66e763509e7a0be161b4d7d`
-	Default Command: `["node"]`

```dockerfile
# Tue, 21 Mar 2017 18:28:51 GMT
ADD file:4eedf861fb567fffb2694b65ebdd58d5e371a2c28c3863f363f333cb34e5eb7b in / 
# Tue, 21 Mar 2017 18:29:05 GMT
CMD ["/bin/bash"]
# Tue, 21 Mar 2017 19:10:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Mar 2017 19:11:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Mar 2017 19:12:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libgeoip-dev 		libglib2.0-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Mar 2017 21:17:40 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 07 Apr 2017 17:07:07 GMT
RUN set -ex   && for key in     9554F04D7259F04124DE6B476D5A82AC7E37093B     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     FD3A5288F042B6850C66B31F09FE44734EB7990E     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     B9AE9905FFD7803F25714661B63B535A4C206CA9     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     56730D5401028683275BD23C23EFEFE93C4CFFFE   ; do     gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --keyserver pgp.mit.edu --recv-keys "$key" ||     gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;   done
# Fri, 07 Apr 2017 17:07:08 GMT
ENV NPM_CONFIG_LOGLEVEL=info
# Wed, 12 Apr 2017 17:11:30 GMT
ENV NODE_VERSION=7.9.0
# Wed, 12 Apr 2017 17:11:37 GMT
RUN curl -SLO "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-x64.tar.xz"   && curl -SLO "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-x64.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-x64.tar.xz" -C /usr/local --strip-components=1   && rm "node-v$NODE_VERSION-linux-x64.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs
# Thu, 20 Apr 2017 14:37:19 GMT
ENV YARN_VERSION=0.23.2
# Thu, 20 Apr 2017 14:37:24 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --keyserver pgp.mit.edu --recv-keys "$key" ||     gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;   done   && curl -fSL -o yarn.js "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-legacy-$YARN_VERSION.js"   && curl -fSL -o yarn.js.asc "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-legacy-$YARN_VERSION.js.asc"   && gpg --batch --verify yarn.js.asc yarn.js   && rm yarn.js.asc   && mv yarn.js /usr/local/bin/yarn   && chmod +x /usr/local/bin/yarn
# Thu, 20 Apr 2017 14:37:25 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:6d827a3ef358f4fa21ef8251f95492e667da826653fd43641cef5a877dc03a70`  
		Last Modified: Tue, 21 Mar 2017 18:38:18 GMT  
		Size: 51.4 MB (51438476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2726297beaf19be957416750338c095ae15b94adc0e8c1306cebbf113f8b9a5c`  
		Last Modified: Tue, 21 Mar 2017 19:58:58 GMT  
		Size: 18.6 MB (18606479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d27bd3d7fecb89d4028f4afa3ee866d2262c5105fc37f57aa82af918dc2f84c`  
		Last Modified: Tue, 21 Mar 2017 19:59:57 GMT  
		Size: 42.6 MB (42571803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ae682c18a31909b5b2e1c0e95d4a05cdf032e983a0e8dc36cc329fc32b53cd`  
		Last Modified: Tue, 21 Mar 2017 20:01:18 GMT  
		Size: 129.9 MB (129934333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c647cd1137d0c98da1d4b091581ddb974387f76d439c675ca19790343b5ae7`  
		Last Modified: Thu, 23 Mar 2017 00:31:07 GMT  
		Size: 4.4 KB (4352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb26c2bc803f2dce2b74ff4a0825bfba4aac156f2dd192f0aed2295f905cb51`  
		Last Modified: Fri, 07 Apr 2017 17:43:40 GMT  
		Size: 119.1 KB (119057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62954f8f2365a774bb07111b1ec57b3a6695e0d8108f3d550a8f065fcf53dfa7`  
		Last Modified: Wed, 12 Apr 2017 17:32:07 GMT  
		Size: 15.5 MB (15488115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a771ee6bc5e26d1e211e037a5dbb706cf672fbba8fea4dd6674c84fd8e18f328`  
		Last Modified: Thu, 20 Apr 2017 14:43:03 GMT  
		Size: 886.3 KB (886272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
