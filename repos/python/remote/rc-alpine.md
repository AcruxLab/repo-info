## `python:rc-alpine`

```console
$ docker pull python@sha256:355281694874784795788182ffcbf71f67982ffb0391a39b4204d76ac326f271
```

-	Platforms:
	-	linux; amd64

### `python:rc-alpine` - linux; amd64

-	Docker Version: 1.12.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29014054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d52e7d8de6448ce1e7ed42ff996a191438d8f3b43d425d5482d168e870d502e`
-	Default Command: `["python3"]`

```dockerfile
# Tue, 27 Dec 2016 18:17:13 GMT
ADD file:eeed5f514a35d18fcd9cbfe6c40c582211020bffdd53e4799018d33826fe5067 in / 
# Tue, 27 Dec 2016 21:27:18 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 27 Dec 2016 21:27:18 GMT
ENV LANG=C.UTF-8
# Tue, 27 Dec 2016 21:27:21 GMT
RUN apk add --no-cache ca-certificates
# Tue, 27 Dec 2016 21:39:31 GMT
ENV GPG_KEY=0D96DF4D4110E5C43FBFB17F2D347EA6AA65421D
# Tue, 27 Dec 2016 21:39:32 GMT
ENV PYTHON_VERSION=3.6.0rc2
# Tue, 27 Dec 2016 21:39:32 GMT
ENV PYTHON_PIP_VERSION=9.0.1
# Tue, 27 Dec 2016 21:41:53 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		openssl 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& rm -r "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bzip2-dev 		gcc 		gdbm-dev 		libc-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		xz-dev 		zlib-dev 	&& apk del .fetch-deps 		&& cd /usr/src/python 	&& ./configure 		--enable-loadable-sqlite-extensions 		--enable-shared 	&& make -j$(getconf _NPROCESSORS_ONLN) 	&& make install 		&& if [ ! -e /usr/local/bin/pip3 ]; then : 		&& wget -O /tmp/get-pip.py 'https://bootstrap.pypa.io/get-pip.py' 		&& python3 /tmp/get-pip.py "pip==$PYTHON_PIP_VERSION" 		&& rm /tmp/get-pip.py 	; fi 	&& pip3 install --no-cache-dir --upgrade --force-reinstall "pip==$PYTHON_PIP_VERSION" 	&& [ "$(pip list |tac|tac| awk -F '[ ()]+' '$1 == "pip" { print $2; exit }')" = "$PYTHON_PIP_VERSION" ] 		&& find /usr/local -depth 		\( 			\( -type d -a -name test -o -name tests \) 			-o 			\( -type f -a -name '*.pyc' -o -name '*.pyo' \) 		\) -exec rm -rf '{}' + 	&& runDeps="$( 		scanelf --needed --nobanner --recursive /usr/local 			| awk '{ gsub(/,/, "\nso:", $2); print "so:" $2 }' 			| sort -u 			| xargs -r apk info --installed 			| sort -u 	)" 	&& apk add --virtual .python-rundeps $runDeps 	&& apk del .build-deps 	&& rm -rf /usr/src/python ~/.cache
# Tue, 27 Dec 2016 21:41:55 GMT
RUN cd /usr/local/bin 	&& { [ -e easy_install ] || ln -s easy_install-* easy_install; } 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 27 Dec 2016 21:41:55 GMT
CMD ["python3"]
```

-	Layers:
	-	`sha256:b7f33cc0b48ea4fb2f0745def58c25483a5f6b7aed5b41ce8f1cb6e17f5723cf`  
		Last Modified: Tue, 27 Dec 2016 18:18:49 GMT  
		Size: 2.3 MB (2313090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eda8bb6fee431ab65900ccd84e8a53fca94486e390147914f8604b45e8f8497`  
		Last Modified: Tue, 27 Dec 2016 21:50:48 GMT  
		Size: 343.9 KB (343948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1e30403818df67ba61e6d90a8deffc5a83169abede8fe5b162716ee0b33ea5`  
		Last Modified: Tue, 27 Dec 2016 22:05:19 GMT  
		Size: 26.4 MB (26356756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c928a01f4bbc2630c9bcee5722b020811d716a6e79c24346d107d91610bbab`  
		Last Modified: Tue, 27 Dec 2016 22:05:02 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
