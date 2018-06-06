## `ros:kinetic-ros-base-jessie`

```console
$ docker pull ros@sha256:c930f5a393d88e8e1b7c6d261ff07889d394c6e50b7e82e15b8f0c98f7e212a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:kinetic-ros-base-jessie` - linux; amd64

```console
$ docker pull ros@sha256:9c80c420ddf1a9ee980427e2165157f953faeca6d5971c971da3105f1e88518b
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **375.4 MB (375421783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3807da99d21ac4070af7e36e390b0f9dd7bc29d81c6ff9c3f88a884eb27e3786`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 06:44:15 GMT
ADD file:3e6141c0c9cb74b14a281eb3ab7aaf162a625733e652c3948b323bb2ec8b4343 in / 
# Sat, 28 Apr 2018 06:44:16 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 22:52:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:52:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:52:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu jessie main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:53:44 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:53:45 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:53:45 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:53:58 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 22:53:59 GMT
ENV ROS_DISTRO=kinetic
# Tue, 05 Jun 2018 22:56:22 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:56:23 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 22:56:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 22:56:24 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 22:58:04 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3d77ce4481b119f00e53bee9b4a443469c42c224db954ddaa2e6b74cd73cd5d0`  
		Last Modified: Sat, 28 Apr 2018 08:24:47 GMT  
		Size: 54.3 MB (54262566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0de818aea1f2533d7ef6d3160065d12993606ff97c4d70e430343444981399e`  
		Last Modified: Wed, 06 Jun 2018 00:18:13 GMT  
		Size: 32.1 MB (32066231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c39208530420e35105977b8b32bb32da8ed770705bfebf0d4aab2ced433880`  
		Last Modified: Wed, 06 Jun 2018 00:18:00 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944d79b8f9f4bcbda5b78a51769a86c72a6bee4719386303528e5cff8bc261c7`  
		Last Modified: Wed, 06 Jun 2018 00:17:58 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111625fa0ce31330096d43e574f0fdff966c0856c1d86c2470aa304ff911c119`  
		Last Modified: Wed, 06 Jun 2018 00:18:20 GMT  
		Size: 46.5 MB (46539380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6588d8ef0724c6d923f14a4c171cea8bc1d72b39a239caf77d0276cb23201d0`  
		Last Modified: Wed, 06 Jun 2018 00:17:59 GMT  
		Size: 866.4 KB (866397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9360fd15ef49d1e737bdb24ca2273209a4acc2700770589fba17e39dc0e9f4af`  
		Last Modified: Wed, 06 Jun 2018 00:19:10 GMT  
		Size: 157.5 MB (157475269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9a9946023522cbb4e9728b454120b0bd70d56d2687d55cec70f14655d643a4`  
		Last Modified: Wed, 06 Jun 2018 00:17:58 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c727713a14d01c395ea5e576d5acb271d732668fbeb31d1639fdebfb00e4f6`  
		Last Modified: Wed, 06 Jun 2018 00:19:52 GMT  
		Size: 84.2 MB (84210100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base-jessie` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0a49e8a8c3129024da38559549dac3e7472107f86584de45938d808ac834d59c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.9 MB (326888800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d53b351cdcd5fe0680ac5c28fc53f09ef64b6d95e7ab5bd244f7f10f83d3d313`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 30 Apr 2018 23:21:38 GMT
ADD file:387c83918422a6546379c4d84818ca3949fcd63aec058da562b08c947a9ed571 in / 
# Mon, 30 Apr 2018 23:21:40 GMT
CMD ["bash"]
# Tue, 01 May 2018 02:11:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 02:11:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 02:11:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu jessie main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 02:15:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 02:15:10 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 02:15:11 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 02:15:57 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 02:15:57 GMT
ENV ROS_DISTRO=kinetic
# Tue, 01 May 2018 02:24:22 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 02:24:26 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 02:24:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 02:24:28 GMT
CMD ["bash"]
# Tue, 01 May 2018 02:31:11 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:363cfded2ef3921ef972c85cafc77cf16cdcfddfd49782ad4540cb73fd5e57a2`  
		Last Modified: Mon, 30 Apr 2018 23:41:06 GMT  
		Size: 51.4 MB (51446854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7a2a3cbb8c886cf7c35daf23d56278fc9499b3b84427b815e340c6887de68a`  
		Last Modified: Tue, 01 May 2018 04:26:53 GMT  
		Size: 30.6 MB (30605699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcd199936fb38824d9edb1fe626cd6602c09b30bea28174aea5bef68daa118e`  
		Last Modified: Tue, 01 May 2018 04:26:35 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896aa3393399d42c7b2513ef0a598903572e2881f613996c6b250a420ab18248`  
		Last Modified: Tue, 01 May 2018 04:26:33 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92024a1019d1ee147846532d332bed467cccac21fbb32e68d24a858c64468d9e`  
		Last Modified: Tue, 01 May 2018 04:27:04 GMT  
		Size: 44.2 MB (44200595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd8d64ceeefcdf37e5c25337d971162dc1d26f34b52aea871d3f04801f302ea`  
		Last Modified: Tue, 01 May 2018 04:26:35 GMT  
		Size: 835.1 KB (835089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49e44792201bb6b813560c52bb75d2569453ee19650eca1c9970cc3b17a8035`  
		Last Modified: Tue, 01 May 2018 04:27:54 GMT  
		Size: 130.8 MB (130755608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4126f23fd7e56bb39f16154e0a83877ba1583879e414f01dbe74c40d586a1d27`  
		Last Modified: Tue, 01 May 2018 04:26:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cddf5f34b92669ab45562b8a143a62ff1852daf1351621e1d1ea56fbb3fa806b`  
		Last Modified: Tue, 01 May 2018 04:28:44 GMT  
		Size: 69.0 MB (69043117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
