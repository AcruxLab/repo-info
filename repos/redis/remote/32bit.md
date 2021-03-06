## `redis:32bit`

```console
$ docker pull redis@sha256:20c7c63a47aa546a4df86066de4140a60fd2f07c2760f452ee64dc718309e4bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redis:32bit` - linux; amd64

```console
$ docker pull redis@sha256:2ea266fee6996ba25ddd0de5423b55c9e029fd5d0a0af400faea987ced296279
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36539391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08b6d828691a2df62434a28b32f417ddb8cc2866d4f48591e880048ac8d53be1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 28 Apr 2018 07:09:59 GMT
ADD file:ec5be7eec56a749752ca284359ece04f5eb0b981eac08b8855454c6b16e3893c in / 
# Sat, 28 Apr 2018 07:09:59 GMT
CMD ["bash"]
# Wed, 20 Jun 2018 21:22:30 GMT
RUN groupadd -r redis && useradd -r -g redis redis
# Wed, 20 Jun 2018 21:22:30 GMT
ENV GOSU_VERSION=1.10
# Wed, 20 Jun 2018 21:23:00 GMT
RUN set -ex; 		fetchDeps=" 		ca-certificates 		dirmngr 		gnupg 		wget 	"; 	apt-get update; 	apt-get install -y --no-install-recommends $fetchDeps; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		apt-get purge -y --auto-remove $fetchDeps
# Wed, 20 Jun 2018 21:25:02 GMT
ENV REDIS_VERSION=4.0.10
# Wed, 20 Jun 2018 21:25:02 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-4.0.10.tar.gz
# Wed, 20 Jun 2018 21:25:03 GMT
ENV REDIS_DOWNLOAD_SHA=1db67435a704f8d18aec9b9637b373c34aa233d65b6e174bdac4c1b161f38ca4
# Wed, 20 Jun 2018 21:26:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libc6-i386 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Jun 2018 21:26:43 GMT
RUN set -ex; 		buildDeps=' 		wget 				gcc 		gcc-multilib 		libc6-dev-i386 		make 	'; 	apt-get update; 	apt-get install -y $buildDeps --no-install-recommends; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" 32bit; 	make -C /usr/src/redis install; 		rm -r /usr/src/redis; 		apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Jun 2018 21:26:44 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 20 Jun 2018 21:26:44 GMT
VOLUME [/data]
# Wed, 20 Jun 2018 21:26:45 GMT
WORKDIR /data
# Wed, 20 Jun 2018 21:26:45 GMT
COPY file:9c29fbe8374a97f9c2d953c9c8b7224554607eeb7a610a930844f2bec678265c in /usr/local/bin/ 
# Wed, 20 Jun 2018 21:26:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jun 2018 21:26:46 GMT
EXPOSE 6379/tcp
# Wed, 20 Jun 2018 21:26:46 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:f2aa67a397c49232112953088506d02074a1fe577f65dc2052f158a3e5da52e8`  
		Last Modified: Sat, 28 Apr 2018 09:31:20 GMT  
		Size: 22.5 MB (22496029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298c0b953ff5a27bfba2e1103c7270851e1e4763cefcdbb9abb595ac21102be7`  
		Last Modified: Wed, 20 Jun 2018 21:27:09 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54481933a13d25902ded350fecd86e018990b0ec8e38617c79da922f880352eb`  
		Last Modified: Wed, 20 Jun 2018 21:27:09 GMT  
		Size: 941.5 KB (941505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3391f4238d5f784a27fe954cb46429794fbf588e060c8d06432d33165cd36fa5`  
		Last Modified: Wed, 20 Jun 2018 21:28:55 GMT  
		Size: 4.8 MB (4848286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c432e9bd82eaafd55e88dc440983c1a53f4db9fd0b02ddd781004d6e9c938e`  
		Last Modified: Wed, 20 Jun 2018 21:28:57 GMT  
		Size: 8.3 MB (8251320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13aaa4d52b00c77615c85e78ef2844914a0b905fd15a96af15266e76a4f9aa25`  
		Last Modified: Wed, 20 Jun 2018 21:28:54 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5079200d239b79c581cce3b9baaf158303a5ef99ad4d1eea319c57256f359295`  
		Last Modified: Wed, 20 Jun 2018 21:28:54 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
