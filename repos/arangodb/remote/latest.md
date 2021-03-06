## `arangodb:latest`

```console
$ docker pull arangodb@sha256:dce1a2e4ca65f3426a984328d258da47817153c88624ef59e1f79ea60c703d87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:18f209e8619fb6d36f63717318ac85310881ff98b8f64f1091ec57b7bc8ad9f4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116742025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fafb5e993d586ea6f63429a9c655be42d0d558e4e8bf652a709f3ab2ff51702d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 28 Apr 2018 07:08:53 GMT
ADD file:9572fdb59dfbb9b032f3331bbc2a08b31e0aef5fbde44c8f2008d22bf5290cf2 in / 
# Sat, 28 Apr 2018 07:08:53 GMT
CMD ["bash"]
# Wed, 06 Jun 2018 23:52:42 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 06 Jun 2018 23:52:42 GMT
ENV ARCHITECTURE=amd64
# Wed, 06 Jun 2018 23:52:42 GMT
ENV DEB_PACKAGE_VERSION=1
# Wed, 06 Jun 2018 23:53:41 GMT
ENV ARANGO_VERSION=3.3.10
# Wed, 06 Jun 2018 23:53:41 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb33/Debian_9.0
# Wed, 06 Jun 2018 23:53:42 GMT
ENV ARANGO_PACKAGE=arangodb3-3.3.10-1_amd64.deb
# Wed, 06 Jun 2018 23:53:42 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb33/Debian_9.0/amd64/arangodb3-3.3.10-1_amd64.deb
# Wed, 06 Jun 2018 23:53:42 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb33/Debian_9.0/amd64/arangodb3-3.3.10-1_amd64.deb.asc
# Wed, 06 Jun 2018 23:53:50 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gpg dirmngr     &&     rm -rf /var/lib/apt/lists/*
# Wed, 06 Jun 2018 23:53:58 GMT
RUN gpg --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B
# Wed, 06 Jun 2018 23:54:12 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libjemalloc1         ca-certificates         pwgen         curl     &&     rm -rf /var/lib/apt/lists/*
# Wed, 06 Jun 2018 23:54:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 06 Jun 2018 23:54:32 GMT
RUN curl --fail -O ${ARANGO_SIGNATURE_URL} &&           curl --fail -O ${ARANGO_PACKAGE_URL} &&             gpg --verify ${ARANGO_PACKAGE}.asc &&     (echo arangodb3 arangodb3/password password test | debconf-set-selections) &&     (echo arangodb3 arangodb3/password_again password test | debconf-set-selections) &&     DEBIAN_FRONTEND="noninteractive" dpkg -i ${ARANGO_PACKAGE} &&     rm -rf /var/lib/arangodb3/* &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf     && chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps     && chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps     &&     rm -f ${ARANGO_PACKAGE}*
# Wed, 06 Jun 2018 23:54:33 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 06 Jun 2018 23:54:33 GMT
COPY file:f1d7a2da62ae377ee32c18cf950d6507b5184b50e05c06ad6f35243591159860 in /entrypoint.sh 
# Wed, 06 Jun 2018 23:54:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Jun 2018 23:54:34 GMT
EXPOSE 8529/tcp
# Wed, 06 Jun 2018 23:54:34 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:cc1a78bfd46becbfc3abb8a74d9a70a0e0dc7a5809bbd12e814f9382db003707`  
		Last Modified: Sat, 28 Apr 2018 09:27:54 GMT  
		Size: 45.3 MB (45318159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f4b6541914308bd8af18e9854fa4bfd4800daaf960ed37cdfb0134101888844`  
		Last Modified: Wed, 06 Jun 2018 23:56:21 GMT  
		Size: 6.6 MB (6561185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9dbc410a746359cb024a86bce8433fca3c951e61b3885535d82b9e2cfe8650a`  
		Last Modified: Wed, 06 Jun 2018 23:56:14 GMT  
		Size: 3.5 KB (3465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19d7ea1c15378047fd850773a135a268408d66cc6eeb633c2492187c63ef680`  
		Last Modified: Wed, 06 Jun 2018 23:56:18 GMT  
		Size: 7.4 MB (7353480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ef043b241e0a0d1f29db72bbc6009fa1399dac1c6fe3f9c8caea4306b21b16`  
		Last Modified: Wed, 06 Jun 2018 23:56:15 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b65f50ed0255ecf4865a6659c28ee9ad917ccf00c0b6d4cc81b8b53fd2c78`  
		Last Modified: Wed, 06 Jun 2018 23:56:40 GMT  
		Size: 57.5 MB (57503849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65eaa57a94846a9f60a7ce8895135de19247e74a800a924cf72af1b8eace63f2`  
		Last Modified: Wed, 06 Jun 2018 23:56:14 GMT  
		Size: 1.8 KB (1772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
