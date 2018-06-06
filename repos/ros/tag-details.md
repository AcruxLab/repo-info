<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ros`

-	[`ros:indigo`](#rosindigo)
-	[`ros:indigo-perception`](#rosindigo-perception)
-	[`ros:indigo-perception-trusty`](#rosindigo-perception-trusty)
-	[`ros:indigo-robot`](#rosindigo-robot)
-	[`ros:indigo-robot-trusty`](#rosindigo-robot-trusty)
-	[`ros:indigo-ros-base`](#rosindigo-ros-base)
-	[`ros:indigo-ros-base-trusty`](#rosindigo-ros-base-trusty)
-	[`ros:indigo-ros-core`](#rosindigo-ros-core)
-	[`ros:indigo-ros-core-trusty`](#rosindigo-ros-core-trusty)
-	[`ros:kinetic`](#roskinetic)
-	[`ros:kinetic-perception`](#roskinetic-perception)
-	[`ros:kinetic-perception-jessie`](#roskinetic-perception-jessie)
-	[`ros:kinetic-perception-xenial`](#roskinetic-perception-xenial)
-	[`ros:kinetic-robot`](#roskinetic-robot)
-	[`ros:kinetic-robot-jessie`](#roskinetic-robot-jessie)
-	[`ros:kinetic-robot-xenial`](#roskinetic-robot-xenial)
-	[`ros:kinetic-ros-base`](#roskinetic-ros-base)
-	[`ros:kinetic-ros-base-jessie`](#roskinetic-ros-base-jessie)
-	[`ros:kinetic-ros-base-xenial`](#roskinetic-ros-base-xenial)
-	[`ros:kinetic-ros-core`](#roskinetic-ros-core)
-	[`ros:kinetic-ros-core-jessie`](#roskinetic-ros-core-jessie)
-	[`ros:kinetic-ros-core-xenial`](#roskinetic-ros-core-xenial)
-	[`ros:latest`](#roslatest)
-	[`ros:lunar`](#roslunar)
-	[`ros:lunar-perception`](#roslunar-perception)
-	[`ros:lunar-perception-stretch`](#roslunar-perception-stretch)
-	[`ros:lunar-perception-xenial`](#roslunar-perception-xenial)
-	[`ros:lunar-robot`](#roslunar-robot)
-	[`ros:lunar-robot-stretch`](#roslunar-robot-stretch)
-	[`ros:lunar-robot-xenial`](#roslunar-robot-xenial)
-	[`ros:lunar-ros-base`](#roslunar-ros-base)
-	[`ros:lunar-ros-base-stretch`](#roslunar-ros-base-stretch)
-	[`ros:lunar-ros-base-xenial`](#roslunar-ros-base-xenial)
-	[`ros:lunar-ros-core`](#roslunar-ros-core)
-	[`ros:lunar-ros-core-stretch`](#roslunar-ros-core-stretch)
-	[`ros:lunar-ros-core-xenial`](#roslunar-ros-core-xenial)
-	[`ros:melodic`](#rosmelodic)
-	[`ros:melodic-perception`](#rosmelodic-perception)
-	[`ros:melodic-perception-bionic`](#rosmelodic-perception-bionic)
-	[`ros:melodic-perception-stretch`](#rosmelodic-perception-stretch)
-	[`ros:melodic-robot`](#rosmelodic-robot)
-	[`ros:melodic-robot-bionic`](#rosmelodic-robot-bionic)
-	[`ros:melodic-robot-stretch`](#rosmelodic-robot-stretch)
-	[`ros:melodic-ros-base`](#rosmelodic-ros-base)
-	[`ros:melodic-ros-base-bionic`](#rosmelodic-ros-base-bionic)
-	[`ros:melodic-ros-base-stretch`](#rosmelodic-ros-base-stretch)
-	[`ros:melodic-ros-core`](#rosmelodic-ros-core)
-	[`ros:melodic-ros-core-bionic`](#rosmelodic-ros-core-bionic)
-	[`ros:melodic-ros-core-stretch`](#rosmelodic-ros-core-stretch)

## `ros:indigo`

```console
$ docker pull ros@sha256:e0dcc9d096efa622898d4925e5baad85c27c6c562802c4acec877dabd681560c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7

### `ros:indigo` - linux; amd64

```console
$ docker pull ros@sha256:488673f5b49f8f9ef5d3e21ba56dc0a28724e6f49e5a8c94170a873f02b7926e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.1 MB (319119015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f544b39c6a23d729f4cff090316ba77c0fa795c1f6a883e697958ccdab3db8d6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:33 GMT
ADD file:3c65bdbcf1318520e7af157cb00317c8312ec16bcaf181d0db919c45f0d7a85e in / 
# Tue, 05 Jun 2018 21:21:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:35 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:35 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:36 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:21:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:21:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:21:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:22:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:22:19 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:22:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:22:36 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 22:22:36 GMT
ENV ROS_DISTRO=indigo
# Tue, 05 Jun 2018 22:26:12 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:26:14 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 22:26:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 22:26:14 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 22:27:21 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-base=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:28bfaceaff9b7464b1e768b0af7e1efe7877a34f238f935c36978a1ecf82c9b1`  
		Last Modified: Mon, 04 Jun 2018 14:56:53 GMT  
		Size: 73.2 MB (73162466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac540055f2f8da75b6587a88763021178d876a2b789ff0c696fbdb62485b62cd`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 72.7 KB (72656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2965585ef8b8370dc8c443e35c743ba723ee427c515535e3ff35d898804cacf9`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 631.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2416bb9f3ad2b5b0c700a4412e2ffbb671f001c45b4b7433ecdcc9c352847814`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b55a6a680757144baae1671d00d4328eee63e790ab36b27d8d52ceb62b179f`  
		Last Modified: Tue, 05 Jun 2018 21:24:12 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f4b9cb761b52e80c8c2e22b82482b36acfc6042d6119b9d9c80477b4edf1ca`  
		Last Modified: Wed, 06 Jun 2018 00:07:28 GMT  
		Size: 16.5 MB (16503268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6e76332e567f50c6d9e227ba8742779cc06fd72ae673b92a49b6a837866a82`  
		Last Modified: Wed, 06 Jun 2018 00:07:19 GMT  
		Size: 13.1 KB (13076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d28474ea3552474796c30ef6b460dbf2ac52da334bf3688c4f5c56e2bbf475`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fb2acd341049ac7e805b600f9ae4b75f463f17c4de2e1268990c044af1ecae`  
		Last Modified: Wed, 06 Jun 2018 00:07:33 GMT  
		Size: 31.8 MB (31793558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8917c4b5e4f11dc6fc522a681fbacd7f49ad1595566e16227a88fea7456be049`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 866.4 KB (866395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b658217912538eca0530e8dc87a5b34901694d0cb0c499c8b4002d6e52394a23`  
		Last Modified: Wed, 06 Jun 2018 00:08:23 GMT  
		Size: 149.9 MB (149933655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43f7eb4cfafeec229d90ac1e2b44df59feb5ecea14466ea1ede851e58316091`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c603e2db050724938129eba87866d0b91de67c5e5aea0301704f85b7e3da6b66`  
		Last Modified: Wed, 06 Jun 2018 00:09:01 GMT  
		Size: 46.8 MB (46771882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:indigo` - linux; arm variant v7

```console
$ docker pull ros@sha256:c916ea6cff813d99aa9248a95ec01310f3ee405855ba960985d9eacbef129431
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289160319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6656f451f62cb0f3375b5f617bc9371a0dc1e41ec7df98742d93222823c5c0f5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:04:54 GMT
ADD file:c3b59ed8b3c28caaaafd56091269a82da9739f5b9261593e97ed075cbd489c28 in / 
# Sat, 28 Apr 2018 12:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:04:57 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:04:58 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:04:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:00 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 15:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:39:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 15:39:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 15:40:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:40:47 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 15:40:47 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 15:41:09 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 15:41:14 GMT
ENV ROS_DISTRO=indigo
# Sat, 28 Apr 2018 15:42:56 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:43:02 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 15:43:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 15:43:03 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 15:44:00 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-base=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1083d09df9ce57f9d8407ea0bcf586a3d67a552c0d0a129bbf8fae6e98a57bb3`  
		Last Modified: Sat, 28 Apr 2018 12:08:17 GMT  
		Size: 66.6 MB (66562822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe7ed775a4a6b507a638e9dd1c82afb92bd7b22f7ec72605227d4795cfb6c83`  
		Last Modified: Sat, 28 Apr 2018 12:07:57 GMT  
		Size: 76.8 KB (76764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da37819308e46c748dcc7fa2e59aac052a6b4926860b94cfc51ba0cd0d21f03`  
		Last Modified: Sat, 28 Apr 2018 12:07:56 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261dcad9941dc4e59979650914aff223718b875292bd6dddf3c8162c71d4331d`  
		Last Modified: Sat, 28 Apr 2018 12:07:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27c2c7e7818c4f4766277047e563b1123caf608301541924286654ab562371e`  
		Last Modified: Sat, 28 Apr 2018 12:07:56 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c26680d6a75ec67fadd17a3478a318eac88e39c3585a8a9561aa9508bb4230`  
		Last Modified: Sat, 28 Apr 2018 15:48:41 GMT  
		Size: 14.5 MB (14479359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05db85a2f86e78acc906d8f2c55ae7f5b1d7cd7d6b06421527e1bf4007ef9b9`  
		Last Modified: Sat, 28 Apr 2018 15:48:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9365fb4da02f26f67cbec4b7d2c0884dbd0286efcbde973c83dae7e4f3aed68d`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4f46c9cbb0b31db49d5073dbab6da69e078dffc865c97d36e4cf84550ff595`  
		Last Modified: Sat, 28 Apr 2018 15:48:47 GMT  
		Size: 29.2 MB (29231895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8128638104464efe80c506388fd9f18ad6adf02b48f0f683787c4573714f518`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 833.5 KB (833478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ca631fefba3ca92616904d017dd021542c1d2d3b76abea5475776baed78ed6`  
		Last Modified: Sat, 28 Apr 2018 15:49:19 GMT  
		Size: 137.6 MB (137578575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f186d161062b0ebd3ef3b9d1fe858d5728d0f29f96a65c2fe82f255d8af43b39`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab989ea1342c8f50876e7603139226a5673f0c0ec4830ce93437e9652924ab2`  
		Last Modified: Sat, 28 Apr 2018 15:49:57 GMT  
		Size: 40.4 MB (40382261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:indigo-perception`

```console
$ docker pull ros@sha256:ca9ef6ab11ac2dfcbe790495adb4549b1bdb5fcf2a480e97487d36bd170116f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7

### `ros:indigo-perception` - linux; amd64

```console
$ docker pull ros@sha256:9d6c87f3fc31200a4d0e6159248651f73da2f63c1bd1985bc372761ac3923259
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **555.5 MB (555465265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dd477cbd376bd2a4a011076375acc11dcfd1968e94ff6858d143e514b6c8ba3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:33 GMT
ADD file:3c65bdbcf1318520e7af157cb00317c8312ec16bcaf181d0db919c45f0d7a85e in / 
# Tue, 05 Jun 2018 21:21:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:35 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:35 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:36 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:21:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:21:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:21:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:22:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:22:19 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:22:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:22:36 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 22:22:36 GMT
ENV ROS_DISTRO=indigo
# Tue, 05 Jun 2018 22:26:12 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:26:14 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 22:26:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 22:26:14 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 22:27:21 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-base=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:34:55 GMT
RUN apt-get update && apt-get install -y     ros-indigo-perception=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:28bfaceaff9b7464b1e768b0af7e1efe7877a34f238f935c36978a1ecf82c9b1`  
		Last Modified: Mon, 04 Jun 2018 14:56:53 GMT  
		Size: 73.2 MB (73162466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac540055f2f8da75b6587a88763021178d876a2b789ff0c696fbdb62485b62cd`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 72.7 KB (72656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2965585ef8b8370dc8c443e35c743ba723ee427c515535e3ff35d898804cacf9`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 631.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2416bb9f3ad2b5b0c700a4412e2ffbb671f001c45b4b7433ecdcc9c352847814`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b55a6a680757144baae1671d00d4328eee63e790ab36b27d8d52ceb62b179f`  
		Last Modified: Tue, 05 Jun 2018 21:24:12 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f4b9cb761b52e80c8c2e22b82482b36acfc6042d6119b9d9c80477b4edf1ca`  
		Last Modified: Wed, 06 Jun 2018 00:07:28 GMT  
		Size: 16.5 MB (16503268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6e76332e567f50c6d9e227ba8742779cc06fd72ae673b92a49b6a837866a82`  
		Last Modified: Wed, 06 Jun 2018 00:07:19 GMT  
		Size: 13.1 KB (13076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d28474ea3552474796c30ef6b460dbf2ac52da334bf3688c4f5c56e2bbf475`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fb2acd341049ac7e805b600f9ae4b75f463f17c4de2e1268990c044af1ecae`  
		Last Modified: Wed, 06 Jun 2018 00:07:33 GMT  
		Size: 31.8 MB (31793558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8917c4b5e4f11dc6fc522a681fbacd7f49ad1595566e16227a88fea7456be049`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 866.4 KB (866395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b658217912538eca0530e8dc87a5b34901694d0cb0c499c8b4002d6e52394a23`  
		Last Modified: Wed, 06 Jun 2018 00:08:23 GMT  
		Size: 149.9 MB (149933655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43f7eb4cfafeec229d90ac1e2b44df59feb5ecea14466ea1ede851e58316091`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c603e2db050724938129eba87866d0b91de67c5e5aea0301704f85b7e3da6b66`  
		Last Modified: Wed, 06 Jun 2018 00:09:01 GMT  
		Size: 46.8 MB (46771882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad02942aea92c9d9dd15d1aae9ffa8ff08bf7cc9913936728d1b1bdbb5a343a`  
		Last Modified: Wed, 06 Jun 2018 00:11:08 GMT  
		Size: 236.3 MB (236346250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:indigo-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:06b22ea7b6d0cc68117cd490497e8a63fb165019d678783ea6d3e53d6af35aa6
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **501.0 MB (501042118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70cc258f00d3dd838ac1bfb0def797789dc3c8a8d749f71f36fca8f2a8ea5cfe`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:04:54 GMT
ADD file:c3b59ed8b3c28caaaafd56091269a82da9739f5b9261593e97ed075cbd489c28 in / 
# Sat, 28 Apr 2018 12:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:04:57 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:04:58 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:04:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:00 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 15:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:39:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 15:39:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 15:40:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:40:47 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 15:40:47 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 15:41:09 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 15:41:14 GMT
ENV ROS_DISTRO=indigo
# Sat, 28 Apr 2018 15:42:56 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:43:02 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 15:43:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 15:43:03 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 15:44:00 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-base=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:47:53 GMT
RUN apt-get update && apt-get install -y     ros-indigo-perception=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1083d09df9ce57f9d8407ea0bcf586a3d67a552c0d0a129bbf8fae6e98a57bb3`  
		Last Modified: Sat, 28 Apr 2018 12:08:17 GMT  
		Size: 66.6 MB (66562822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe7ed775a4a6b507a638e9dd1c82afb92bd7b22f7ec72605227d4795cfb6c83`  
		Last Modified: Sat, 28 Apr 2018 12:07:57 GMT  
		Size: 76.8 KB (76764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da37819308e46c748dcc7fa2e59aac052a6b4926860b94cfc51ba0cd0d21f03`  
		Last Modified: Sat, 28 Apr 2018 12:07:56 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261dcad9941dc4e59979650914aff223718b875292bd6dddf3c8162c71d4331d`  
		Last Modified: Sat, 28 Apr 2018 12:07:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27c2c7e7818c4f4766277047e563b1123caf608301541924286654ab562371e`  
		Last Modified: Sat, 28 Apr 2018 12:07:56 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c26680d6a75ec67fadd17a3478a318eac88e39c3585a8a9561aa9508bb4230`  
		Last Modified: Sat, 28 Apr 2018 15:48:41 GMT  
		Size: 14.5 MB (14479359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05db85a2f86e78acc906d8f2c55ae7f5b1d7cd7d6b06421527e1bf4007ef9b9`  
		Last Modified: Sat, 28 Apr 2018 15:48:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9365fb4da02f26f67cbec4b7d2c0884dbd0286efcbde973c83dae7e4f3aed68d`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4f46c9cbb0b31db49d5073dbab6da69e078dffc865c97d36e4cf84550ff595`  
		Last Modified: Sat, 28 Apr 2018 15:48:47 GMT  
		Size: 29.2 MB (29231895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8128638104464efe80c506388fd9f18ad6adf02b48f0f683787c4573714f518`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 833.5 KB (833478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ca631fefba3ca92616904d017dd021542c1d2d3b76abea5475776baed78ed6`  
		Last Modified: Sat, 28 Apr 2018 15:49:19 GMT  
		Size: 137.6 MB (137578575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f186d161062b0ebd3ef3b9d1fe858d5728d0f29f96a65c2fe82f255d8af43b39`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab989ea1342c8f50876e7603139226a5673f0c0ec4830ce93437e9652924ab2`  
		Last Modified: Sat, 28 Apr 2018 15:49:57 GMT  
		Size: 40.4 MB (40382261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b03f074f91cf9fad5ff4c2899b7830209cce247a02518955b39171e3b523db`  
		Last Modified: Sat, 28 Apr 2018 15:52:08 GMT  
		Size: 211.9 MB (211881799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:indigo-perception-trusty`

```console
$ docker pull ros@sha256:ca9ef6ab11ac2dfcbe790495adb4549b1bdb5fcf2a480e97487d36bd170116f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7

### `ros:indigo-perception-trusty` - linux; amd64

```console
$ docker pull ros@sha256:9d6c87f3fc31200a4d0e6159248651f73da2f63c1bd1985bc372761ac3923259
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **555.5 MB (555465265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dd477cbd376bd2a4a011076375acc11dcfd1968e94ff6858d143e514b6c8ba3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:33 GMT
ADD file:3c65bdbcf1318520e7af157cb00317c8312ec16bcaf181d0db919c45f0d7a85e in / 
# Tue, 05 Jun 2018 21:21:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:35 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:35 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:36 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:21:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:21:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:21:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:22:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:22:19 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:22:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:22:36 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 22:22:36 GMT
ENV ROS_DISTRO=indigo
# Tue, 05 Jun 2018 22:26:12 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:26:14 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 22:26:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 22:26:14 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 22:27:21 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-base=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:34:55 GMT
RUN apt-get update && apt-get install -y     ros-indigo-perception=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:28bfaceaff9b7464b1e768b0af7e1efe7877a34f238f935c36978a1ecf82c9b1`  
		Last Modified: Mon, 04 Jun 2018 14:56:53 GMT  
		Size: 73.2 MB (73162466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac540055f2f8da75b6587a88763021178d876a2b789ff0c696fbdb62485b62cd`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 72.7 KB (72656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2965585ef8b8370dc8c443e35c743ba723ee427c515535e3ff35d898804cacf9`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 631.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2416bb9f3ad2b5b0c700a4412e2ffbb671f001c45b4b7433ecdcc9c352847814`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b55a6a680757144baae1671d00d4328eee63e790ab36b27d8d52ceb62b179f`  
		Last Modified: Tue, 05 Jun 2018 21:24:12 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f4b9cb761b52e80c8c2e22b82482b36acfc6042d6119b9d9c80477b4edf1ca`  
		Last Modified: Wed, 06 Jun 2018 00:07:28 GMT  
		Size: 16.5 MB (16503268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6e76332e567f50c6d9e227ba8742779cc06fd72ae673b92a49b6a837866a82`  
		Last Modified: Wed, 06 Jun 2018 00:07:19 GMT  
		Size: 13.1 KB (13076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d28474ea3552474796c30ef6b460dbf2ac52da334bf3688c4f5c56e2bbf475`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fb2acd341049ac7e805b600f9ae4b75f463f17c4de2e1268990c044af1ecae`  
		Last Modified: Wed, 06 Jun 2018 00:07:33 GMT  
		Size: 31.8 MB (31793558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8917c4b5e4f11dc6fc522a681fbacd7f49ad1595566e16227a88fea7456be049`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 866.4 KB (866395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b658217912538eca0530e8dc87a5b34901694d0cb0c499c8b4002d6e52394a23`  
		Last Modified: Wed, 06 Jun 2018 00:08:23 GMT  
		Size: 149.9 MB (149933655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43f7eb4cfafeec229d90ac1e2b44df59feb5ecea14466ea1ede851e58316091`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c603e2db050724938129eba87866d0b91de67c5e5aea0301704f85b7e3da6b66`  
		Last Modified: Wed, 06 Jun 2018 00:09:01 GMT  
		Size: 46.8 MB (46771882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad02942aea92c9d9dd15d1aae9ffa8ff08bf7cc9913936728d1b1bdbb5a343a`  
		Last Modified: Wed, 06 Jun 2018 00:11:08 GMT  
		Size: 236.3 MB (236346250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:indigo-perception-trusty` - linux; arm variant v7

```console
$ docker pull ros@sha256:06b22ea7b6d0cc68117cd490497e8a63fb165019d678783ea6d3e53d6af35aa6
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **501.0 MB (501042118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70cc258f00d3dd838ac1bfb0def797789dc3c8a8d749f71f36fca8f2a8ea5cfe`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:04:54 GMT
ADD file:c3b59ed8b3c28caaaafd56091269a82da9739f5b9261593e97ed075cbd489c28 in / 
# Sat, 28 Apr 2018 12:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:04:57 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:04:58 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:04:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:00 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 15:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:39:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 15:39:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 15:40:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:40:47 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 15:40:47 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 15:41:09 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 15:41:14 GMT
ENV ROS_DISTRO=indigo
# Sat, 28 Apr 2018 15:42:56 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:43:02 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 15:43:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 15:43:03 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 15:44:00 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-base=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:47:53 GMT
RUN apt-get update && apt-get install -y     ros-indigo-perception=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1083d09df9ce57f9d8407ea0bcf586a3d67a552c0d0a129bbf8fae6e98a57bb3`  
		Last Modified: Sat, 28 Apr 2018 12:08:17 GMT  
		Size: 66.6 MB (66562822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe7ed775a4a6b507a638e9dd1c82afb92bd7b22f7ec72605227d4795cfb6c83`  
		Last Modified: Sat, 28 Apr 2018 12:07:57 GMT  
		Size: 76.8 KB (76764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da37819308e46c748dcc7fa2e59aac052a6b4926860b94cfc51ba0cd0d21f03`  
		Last Modified: Sat, 28 Apr 2018 12:07:56 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261dcad9941dc4e59979650914aff223718b875292bd6dddf3c8162c71d4331d`  
		Last Modified: Sat, 28 Apr 2018 12:07:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27c2c7e7818c4f4766277047e563b1123caf608301541924286654ab562371e`  
		Last Modified: Sat, 28 Apr 2018 12:07:56 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c26680d6a75ec67fadd17a3478a318eac88e39c3585a8a9561aa9508bb4230`  
		Last Modified: Sat, 28 Apr 2018 15:48:41 GMT  
		Size: 14.5 MB (14479359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05db85a2f86e78acc906d8f2c55ae7f5b1d7cd7d6b06421527e1bf4007ef9b9`  
		Last Modified: Sat, 28 Apr 2018 15:48:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9365fb4da02f26f67cbec4b7d2c0884dbd0286efcbde973c83dae7e4f3aed68d`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4f46c9cbb0b31db49d5073dbab6da69e078dffc865c97d36e4cf84550ff595`  
		Last Modified: Sat, 28 Apr 2018 15:48:47 GMT  
		Size: 29.2 MB (29231895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8128638104464efe80c506388fd9f18ad6adf02b48f0f683787c4573714f518`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 833.5 KB (833478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ca631fefba3ca92616904d017dd021542c1d2d3b76abea5475776baed78ed6`  
		Last Modified: Sat, 28 Apr 2018 15:49:19 GMT  
		Size: 137.6 MB (137578575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f186d161062b0ebd3ef3b9d1fe858d5728d0f29f96a65c2fe82f255d8af43b39`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab989ea1342c8f50876e7603139226a5673f0c0ec4830ce93437e9652924ab2`  
		Last Modified: Sat, 28 Apr 2018 15:49:57 GMT  
		Size: 40.4 MB (40382261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b03f074f91cf9fad5ff4c2899b7830209cce247a02518955b39171e3b523db`  
		Last Modified: Sat, 28 Apr 2018 15:52:08 GMT  
		Size: 211.9 MB (211881799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:indigo-robot`

```console
$ docker pull ros@sha256:e6542fb7518c040288cf4f074aa6f3cbca9b3eca57819c73b306e042d3b38cf1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7

### `ros:indigo-robot` - linux; amd64

```console
$ docker pull ros@sha256:f2cc9faf99ce471882b5842f043eded77920a09cc70baf4b2c8e78c2eb6ed2b5
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.1 MB (338145173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a309b89388202250ee192a1dbb06c57602d4d41c895a20316baf10bf64ce8110`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:33 GMT
ADD file:3c65bdbcf1318520e7af157cb00317c8312ec16bcaf181d0db919c45f0d7a85e in / 
# Tue, 05 Jun 2018 21:21:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:35 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:35 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:36 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:21:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:21:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:21:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:22:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:22:19 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:22:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:22:36 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 22:22:36 GMT
ENV ROS_DISTRO=indigo
# Tue, 05 Jun 2018 22:26:12 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:26:14 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 22:26:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 22:26:14 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 22:27:21 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-base=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:28:29 GMT
RUN apt-get update && apt-get install -y     ros-indigo-robot=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:28bfaceaff9b7464b1e768b0af7e1efe7877a34f238f935c36978a1ecf82c9b1`  
		Last Modified: Mon, 04 Jun 2018 14:56:53 GMT  
		Size: 73.2 MB (73162466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac540055f2f8da75b6587a88763021178d876a2b789ff0c696fbdb62485b62cd`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 72.7 KB (72656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2965585ef8b8370dc8c443e35c743ba723ee427c515535e3ff35d898804cacf9`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 631.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2416bb9f3ad2b5b0c700a4412e2ffbb671f001c45b4b7433ecdcc9c352847814`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b55a6a680757144baae1671d00d4328eee63e790ab36b27d8d52ceb62b179f`  
		Last Modified: Tue, 05 Jun 2018 21:24:12 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f4b9cb761b52e80c8c2e22b82482b36acfc6042d6119b9d9c80477b4edf1ca`  
		Last Modified: Wed, 06 Jun 2018 00:07:28 GMT  
		Size: 16.5 MB (16503268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6e76332e567f50c6d9e227ba8742779cc06fd72ae673b92a49b6a837866a82`  
		Last Modified: Wed, 06 Jun 2018 00:07:19 GMT  
		Size: 13.1 KB (13076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d28474ea3552474796c30ef6b460dbf2ac52da334bf3688c4f5c56e2bbf475`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fb2acd341049ac7e805b600f9ae4b75f463f17c4de2e1268990c044af1ecae`  
		Last Modified: Wed, 06 Jun 2018 00:07:33 GMT  
		Size: 31.8 MB (31793558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8917c4b5e4f11dc6fc522a681fbacd7f49ad1595566e16227a88fea7456be049`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 866.4 KB (866395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b658217912538eca0530e8dc87a5b34901694d0cb0c499c8b4002d6e52394a23`  
		Last Modified: Wed, 06 Jun 2018 00:08:23 GMT  
		Size: 149.9 MB (149933655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43f7eb4cfafeec229d90ac1e2b44df59feb5ecea14466ea1ede851e58316091`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c603e2db050724938129eba87866d0b91de67c5e5aea0301704f85b7e3da6b66`  
		Last Modified: Wed, 06 Jun 2018 00:09:01 GMT  
		Size: 46.8 MB (46771882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaac867b2b2218179046afb6e893257b76f4861049b598cdd417d862740dc1b7`  
		Last Modified: Wed, 06 Jun 2018 00:09:25 GMT  
		Size: 19.0 MB (19026158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:indigo-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:ea78f4ac1e47238dfafab6c53f2cf2da4f7a2a294b8061a87a0b0a55a42c5cf4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.8 MB (306839431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f36dffccb69e094849cddbc952a12ffe2cdb1ec08ac61e01ed9d74d3405f6a6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:04:54 GMT
ADD file:c3b59ed8b3c28caaaafd56091269a82da9739f5b9261593e97ed075cbd489c28 in / 
# Sat, 28 Apr 2018 12:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:04:57 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:04:58 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:04:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:00 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 15:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:39:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 15:39:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 15:40:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:40:47 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 15:40:47 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 15:41:09 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 15:41:14 GMT
ENV ROS_DISTRO=indigo
# Sat, 28 Apr 2018 15:42:56 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:43:02 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 15:43:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 15:43:03 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 15:44:00 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-base=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:45:00 GMT
RUN apt-get update && apt-get install -y     ros-indigo-robot=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1083d09df9ce57f9d8407ea0bcf586a3d67a552c0d0a129bbf8fae6e98a57bb3`  
		Last Modified: Sat, 28 Apr 2018 12:08:17 GMT  
		Size: 66.6 MB (66562822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe7ed775a4a6b507a638e9dd1c82afb92bd7b22f7ec72605227d4795cfb6c83`  
		Last Modified: Sat, 28 Apr 2018 12:07:57 GMT  
		Size: 76.8 KB (76764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da37819308e46c748dcc7fa2e59aac052a6b4926860b94cfc51ba0cd0d21f03`  
		Last Modified: Sat, 28 Apr 2018 12:07:56 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261dcad9941dc4e59979650914aff223718b875292bd6dddf3c8162c71d4331d`  
		Last Modified: Sat, 28 Apr 2018 12:07:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27c2c7e7818c4f4766277047e563b1123caf608301541924286654ab562371e`  
		Last Modified: Sat, 28 Apr 2018 12:07:56 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c26680d6a75ec67fadd17a3478a318eac88e39c3585a8a9561aa9508bb4230`  
		Last Modified: Sat, 28 Apr 2018 15:48:41 GMT  
		Size: 14.5 MB (14479359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05db85a2f86e78acc906d8f2c55ae7f5b1d7cd7d6b06421527e1bf4007ef9b9`  
		Last Modified: Sat, 28 Apr 2018 15:48:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9365fb4da02f26f67cbec4b7d2c0884dbd0286efcbde973c83dae7e4f3aed68d`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4f46c9cbb0b31db49d5073dbab6da69e078dffc865c97d36e4cf84550ff595`  
		Last Modified: Sat, 28 Apr 2018 15:48:47 GMT  
		Size: 29.2 MB (29231895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8128638104464efe80c506388fd9f18ad6adf02b48f0f683787c4573714f518`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 833.5 KB (833478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ca631fefba3ca92616904d017dd021542c1d2d3b76abea5475776baed78ed6`  
		Last Modified: Sat, 28 Apr 2018 15:49:19 GMT  
		Size: 137.6 MB (137578575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f186d161062b0ebd3ef3b9d1fe858d5728d0f29f96a65c2fe82f255d8af43b39`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab989ea1342c8f50876e7603139226a5673f0c0ec4830ce93437e9652924ab2`  
		Last Modified: Sat, 28 Apr 2018 15:49:57 GMT  
		Size: 40.4 MB (40382261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47007e480980a01b78d07442ce599521de555e4b0dab771631446969c3b48996`  
		Last Modified: Sat, 28 Apr 2018 15:50:38 GMT  
		Size: 17.7 MB (17679112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:indigo-robot-trusty`

```console
$ docker pull ros@sha256:e6542fb7518c040288cf4f074aa6f3cbca9b3eca57819c73b306e042d3b38cf1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7

### `ros:indigo-robot-trusty` - linux; amd64

```console
$ docker pull ros@sha256:f2cc9faf99ce471882b5842f043eded77920a09cc70baf4b2c8e78c2eb6ed2b5
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.1 MB (338145173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a309b89388202250ee192a1dbb06c57602d4d41c895a20316baf10bf64ce8110`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:33 GMT
ADD file:3c65bdbcf1318520e7af157cb00317c8312ec16bcaf181d0db919c45f0d7a85e in / 
# Tue, 05 Jun 2018 21:21:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:35 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:35 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:36 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:21:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:21:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:21:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:22:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:22:19 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:22:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:22:36 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 22:22:36 GMT
ENV ROS_DISTRO=indigo
# Tue, 05 Jun 2018 22:26:12 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:26:14 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 22:26:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 22:26:14 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 22:27:21 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-base=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:28:29 GMT
RUN apt-get update && apt-get install -y     ros-indigo-robot=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:28bfaceaff9b7464b1e768b0af7e1efe7877a34f238f935c36978a1ecf82c9b1`  
		Last Modified: Mon, 04 Jun 2018 14:56:53 GMT  
		Size: 73.2 MB (73162466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac540055f2f8da75b6587a88763021178d876a2b789ff0c696fbdb62485b62cd`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 72.7 KB (72656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2965585ef8b8370dc8c443e35c743ba723ee427c515535e3ff35d898804cacf9`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 631.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2416bb9f3ad2b5b0c700a4412e2ffbb671f001c45b4b7433ecdcc9c352847814`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b55a6a680757144baae1671d00d4328eee63e790ab36b27d8d52ceb62b179f`  
		Last Modified: Tue, 05 Jun 2018 21:24:12 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f4b9cb761b52e80c8c2e22b82482b36acfc6042d6119b9d9c80477b4edf1ca`  
		Last Modified: Wed, 06 Jun 2018 00:07:28 GMT  
		Size: 16.5 MB (16503268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6e76332e567f50c6d9e227ba8742779cc06fd72ae673b92a49b6a837866a82`  
		Last Modified: Wed, 06 Jun 2018 00:07:19 GMT  
		Size: 13.1 KB (13076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d28474ea3552474796c30ef6b460dbf2ac52da334bf3688c4f5c56e2bbf475`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fb2acd341049ac7e805b600f9ae4b75f463f17c4de2e1268990c044af1ecae`  
		Last Modified: Wed, 06 Jun 2018 00:07:33 GMT  
		Size: 31.8 MB (31793558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8917c4b5e4f11dc6fc522a681fbacd7f49ad1595566e16227a88fea7456be049`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 866.4 KB (866395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b658217912538eca0530e8dc87a5b34901694d0cb0c499c8b4002d6e52394a23`  
		Last Modified: Wed, 06 Jun 2018 00:08:23 GMT  
		Size: 149.9 MB (149933655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43f7eb4cfafeec229d90ac1e2b44df59feb5ecea14466ea1ede851e58316091`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c603e2db050724938129eba87866d0b91de67c5e5aea0301704f85b7e3da6b66`  
		Last Modified: Wed, 06 Jun 2018 00:09:01 GMT  
		Size: 46.8 MB (46771882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaac867b2b2218179046afb6e893257b76f4861049b598cdd417d862740dc1b7`  
		Last Modified: Wed, 06 Jun 2018 00:09:25 GMT  
		Size: 19.0 MB (19026158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:indigo-robot-trusty` - linux; arm variant v7

```console
$ docker pull ros@sha256:ea78f4ac1e47238dfafab6c53f2cf2da4f7a2a294b8061a87a0b0a55a42c5cf4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.8 MB (306839431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f36dffccb69e094849cddbc952a12ffe2cdb1ec08ac61e01ed9d74d3405f6a6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:04:54 GMT
ADD file:c3b59ed8b3c28caaaafd56091269a82da9739f5b9261593e97ed075cbd489c28 in / 
# Sat, 28 Apr 2018 12:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:04:57 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:04:58 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:04:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:00 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 15:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:39:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 15:39:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 15:40:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:40:47 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 15:40:47 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 15:41:09 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 15:41:14 GMT
ENV ROS_DISTRO=indigo
# Sat, 28 Apr 2018 15:42:56 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:43:02 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 15:43:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 15:43:03 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 15:44:00 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-base=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:45:00 GMT
RUN apt-get update && apt-get install -y     ros-indigo-robot=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1083d09df9ce57f9d8407ea0bcf586a3d67a552c0d0a129bbf8fae6e98a57bb3`  
		Last Modified: Sat, 28 Apr 2018 12:08:17 GMT  
		Size: 66.6 MB (66562822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe7ed775a4a6b507a638e9dd1c82afb92bd7b22f7ec72605227d4795cfb6c83`  
		Last Modified: Sat, 28 Apr 2018 12:07:57 GMT  
		Size: 76.8 KB (76764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da37819308e46c748dcc7fa2e59aac052a6b4926860b94cfc51ba0cd0d21f03`  
		Last Modified: Sat, 28 Apr 2018 12:07:56 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261dcad9941dc4e59979650914aff223718b875292bd6dddf3c8162c71d4331d`  
		Last Modified: Sat, 28 Apr 2018 12:07:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27c2c7e7818c4f4766277047e563b1123caf608301541924286654ab562371e`  
		Last Modified: Sat, 28 Apr 2018 12:07:56 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c26680d6a75ec67fadd17a3478a318eac88e39c3585a8a9561aa9508bb4230`  
		Last Modified: Sat, 28 Apr 2018 15:48:41 GMT  
		Size: 14.5 MB (14479359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05db85a2f86e78acc906d8f2c55ae7f5b1d7cd7d6b06421527e1bf4007ef9b9`  
		Last Modified: Sat, 28 Apr 2018 15:48:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9365fb4da02f26f67cbec4b7d2c0884dbd0286efcbde973c83dae7e4f3aed68d`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4f46c9cbb0b31db49d5073dbab6da69e078dffc865c97d36e4cf84550ff595`  
		Last Modified: Sat, 28 Apr 2018 15:48:47 GMT  
		Size: 29.2 MB (29231895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8128638104464efe80c506388fd9f18ad6adf02b48f0f683787c4573714f518`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 833.5 KB (833478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ca631fefba3ca92616904d017dd021542c1d2d3b76abea5475776baed78ed6`  
		Last Modified: Sat, 28 Apr 2018 15:49:19 GMT  
		Size: 137.6 MB (137578575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f186d161062b0ebd3ef3b9d1fe858d5728d0f29f96a65c2fe82f255d8af43b39`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab989ea1342c8f50876e7603139226a5673f0c0ec4830ce93437e9652924ab2`  
		Last Modified: Sat, 28 Apr 2018 15:49:57 GMT  
		Size: 40.4 MB (40382261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47007e480980a01b78d07442ce599521de555e4b0dab771631446969c3b48996`  
		Last Modified: Sat, 28 Apr 2018 15:50:38 GMT  
		Size: 17.7 MB (17679112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:indigo-ros-base`

```console
$ docker pull ros@sha256:e0dcc9d096efa622898d4925e5baad85c27c6c562802c4acec877dabd681560c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7

### `ros:indigo-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:488673f5b49f8f9ef5d3e21ba56dc0a28724e6f49e5a8c94170a873f02b7926e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.1 MB (319119015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f544b39c6a23d729f4cff090316ba77c0fa795c1f6a883e697958ccdab3db8d6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:33 GMT
ADD file:3c65bdbcf1318520e7af157cb00317c8312ec16bcaf181d0db919c45f0d7a85e in / 
# Tue, 05 Jun 2018 21:21:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:35 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:35 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:36 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:21:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:21:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:21:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:22:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:22:19 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:22:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:22:36 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 22:22:36 GMT
ENV ROS_DISTRO=indigo
# Tue, 05 Jun 2018 22:26:12 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:26:14 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 22:26:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 22:26:14 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 22:27:21 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-base=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:28bfaceaff9b7464b1e768b0af7e1efe7877a34f238f935c36978a1ecf82c9b1`  
		Last Modified: Mon, 04 Jun 2018 14:56:53 GMT  
		Size: 73.2 MB (73162466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac540055f2f8da75b6587a88763021178d876a2b789ff0c696fbdb62485b62cd`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 72.7 KB (72656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2965585ef8b8370dc8c443e35c743ba723ee427c515535e3ff35d898804cacf9`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 631.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2416bb9f3ad2b5b0c700a4412e2ffbb671f001c45b4b7433ecdcc9c352847814`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b55a6a680757144baae1671d00d4328eee63e790ab36b27d8d52ceb62b179f`  
		Last Modified: Tue, 05 Jun 2018 21:24:12 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f4b9cb761b52e80c8c2e22b82482b36acfc6042d6119b9d9c80477b4edf1ca`  
		Last Modified: Wed, 06 Jun 2018 00:07:28 GMT  
		Size: 16.5 MB (16503268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6e76332e567f50c6d9e227ba8742779cc06fd72ae673b92a49b6a837866a82`  
		Last Modified: Wed, 06 Jun 2018 00:07:19 GMT  
		Size: 13.1 KB (13076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d28474ea3552474796c30ef6b460dbf2ac52da334bf3688c4f5c56e2bbf475`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fb2acd341049ac7e805b600f9ae4b75f463f17c4de2e1268990c044af1ecae`  
		Last Modified: Wed, 06 Jun 2018 00:07:33 GMT  
		Size: 31.8 MB (31793558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8917c4b5e4f11dc6fc522a681fbacd7f49ad1595566e16227a88fea7456be049`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 866.4 KB (866395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b658217912538eca0530e8dc87a5b34901694d0cb0c499c8b4002d6e52394a23`  
		Last Modified: Wed, 06 Jun 2018 00:08:23 GMT  
		Size: 149.9 MB (149933655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43f7eb4cfafeec229d90ac1e2b44df59feb5ecea14466ea1ede851e58316091`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c603e2db050724938129eba87866d0b91de67c5e5aea0301704f85b7e3da6b66`  
		Last Modified: Wed, 06 Jun 2018 00:09:01 GMT  
		Size: 46.8 MB (46771882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:indigo-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:c916ea6cff813d99aa9248a95ec01310f3ee405855ba960985d9eacbef129431
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289160319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6656f451f62cb0f3375b5f617bc9371a0dc1e41ec7df98742d93222823c5c0f5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:04:54 GMT
ADD file:c3b59ed8b3c28caaaafd56091269a82da9739f5b9261593e97ed075cbd489c28 in / 
# Sat, 28 Apr 2018 12:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:04:57 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:04:58 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:04:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:00 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 15:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:39:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 15:39:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 15:40:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:40:47 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 15:40:47 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 15:41:09 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 15:41:14 GMT
ENV ROS_DISTRO=indigo
# Sat, 28 Apr 2018 15:42:56 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:43:02 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 15:43:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 15:43:03 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 15:44:00 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-base=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1083d09df9ce57f9d8407ea0bcf586a3d67a552c0d0a129bbf8fae6e98a57bb3`  
		Last Modified: Sat, 28 Apr 2018 12:08:17 GMT  
		Size: 66.6 MB (66562822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe7ed775a4a6b507a638e9dd1c82afb92bd7b22f7ec72605227d4795cfb6c83`  
		Last Modified: Sat, 28 Apr 2018 12:07:57 GMT  
		Size: 76.8 KB (76764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da37819308e46c748dcc7fa2e59aac052a6b4926860b94cfc51ba0cd0d21f03`  
		Last Modified: Sat, 28 Apr 2018 12:07:56 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261dcad9941dc4e59979650914aff223718b875292bd6dddf3c8162c71d4331d`  
		Last Modified: Sat, 28 Apr 2018 12:07:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27c2c7e7818c4f4766277047e563b1123caf608301541924286654ab562371e`  
		Last Modified: Sat, 28 Apr 2018 12:07:56 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c26680d6a75ec67fadd17a3478a318eac88e39c3585a8a9561aa9508bb4230`  
		Last Modified: Sat, 28 Apr 2018 15:48:41 GMT  
		Size: 14.5 MB (14479359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05db85a2f86e78acc906d8f2c55ae7f5b1d7cd7d6b06421527e1bf4007ef9b9`  
		Last Modified: Sat, 28 Apr 2018 15:48:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9365fb4da02f26f67cbec4b7d2c0884dbd0286efcbde973c83dae7e4f3aed68d`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4f46c9cbb0b31db49d5073dbab6da69e078dffc865c97d36e4cf84550ff595`  
		Last Modified: Sat, 28 Apr 2018 15:48:47 GMT  
		Size: 29.2 MB (29231895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8128638104464efe80c506388fd9f18ad6adf02b48f0f683787c4573714f518`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 833.5 KB (833478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ca631fefba3ca92616904d017dd021542c1d2d3b76abea5475776baed78ed6`  
		Last Modified: Sat, 28 Apr 2018 15:49:19 GMT  
		Size: 137.6 MB (137578575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f186d161062b0ebd3ef3b9d1fe858d5728d0f29f96a65c2fe82f255d8af43b39`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab989ea1342c8f50876e7603139226a5673f0c0ec4830ce93437e9652924ab2`  
		Last Modified: Sat, 28 Apr 2018 15:49:57 GMT  
		Size: 40.4 MB (40382261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:indigo-ros-base-trusty`

```console
$ docker pull ros@sha256:e0dcc9d096efa622898d4925e5baad85c27c6c562802c4acec877dabd681560c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7

### `ros:indigo-ros-base-trusty` - linux; amd64

```console
$ docker pull ros@sha256:488673f5b49f8f9ef5d3e21ba56dc0a28724e6f49e5a8c94170a873f02b7926e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.1 MB (319119015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f544b39c6a23d729f4cff090316ba77c0fa795c1f6a883e697958ccdab3db8d6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:33 GMT
ADD file:3c65bdbcf1318520e7af157cb00317c8312ec16bcaf181d0db919c45f0d7a85e in / 
# Tue, 05 Jun 2018 21:21:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:35 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:35 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:36 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:21:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:21:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:21:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:22:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:22:19 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:22:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:22:36 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 22:22:36 GMT
ENV ROS_DISTRO=indigo
# Tue, 05 Jun 2018 22:26:12 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:26:14 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 22:26:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 22:26:14 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 22:27:21 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-base=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:28bfaceaff9b7464b1e768b0af7e1efe7877a34f238f935c36978a1ecf82c9b1`  
		Last Modified: Mon, 04 Jun 2018 14:56:53 GMT  
		Size: 73.2 MB (73162466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac540055f2f8da75b6587a88763021178d876a2b789ff0c696fbdb62485b62cd`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 72.7 KB (72656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2965585ef8b8370dc8c443e35c743ba723ee427c515535e3ff35d898804cacf9`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 631.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2416bb9f3ad2b5b0c700a4412e2ffbb671f001c45b4b7433ecdcc9c352847814`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b55a6a680757144baae1671d00d4328eee63e790ab36b27d8d52ceb62b179f`  
		Last Modified: Tue, 05 Jun 2018 21:24:12 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f4b9cb761b52e80c8c2e22b82482b36acfc6042d6119b9d9c80477b4edf1ca`  
		Last Modified: Wed, 06 Jun 2018 00:07:28 GMT  
		Size: 16.5 MB (16503268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6e76332e567f50c6d9e227ba8742779cc06fd72ae673b92a49b6a837866a82`  
		Last Modified: Wed, 06 Jun 2018 00:07:19 GMT  
		Size: 13.1 KB (13076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d28474ea3552474796c30ef6b460dbf2ac52da334bf3688c4f5c56e2bbf475`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fb2acd341049ac7e805b600f9ae4b75f463f17c4de2e1268990c044af1ecae`  
		Last Modified: Wed, 06 Jun 2018 00:07:33 GMT  
		Size: 31.8 MB (31793558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8917c4b5e4f11dc6fc522a681fbacd7f49ad1595566e16227a88fea7456be049`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 866.4 KB (866395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b658217912538eca0530e8dc87a5b34901694d0cb0c499c8b4002d6e52394a23`  
		Last Modified: Wed, 06 Jun 2018 00:08:23 GMT  
		Size: 149.9 MB (149933655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43f7eb4cfafeec229d90ac1e2b44df59feb5ecea14466ea1ede851e58316091`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c603e2db050724938129eba87866d0b91de67c5e5aea0301704f85b7e3da6b66`  
		Last Modified: Wed, 06 Jun 2018 00:09:01 GMT  
		Size: 46.8 MB (46771882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:indigo-ros-base-trusty` - linux; arm variant v7

```console
$ docker pull ros@sha256:c916ea6cff813d99aa9248a95ec01310f3ee405855ba960985d9eacbef129431
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289160319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6656f451f62cb0f3375b5f617bc9371a0dc1e41ec7df98742d93222823c5c0f5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:04:54 GMT
ADD file:c3b59ed8b3c28caaaafd56091269a82da9739f5b9261593e97ed075cbd489c28 in / 
# Sat, 28 Apr 2018 12:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:04:57 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:04:58 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:04:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:00 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 15:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:39:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 15:39:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 15:40:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:40:47 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 15:40:47 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 15:41:09 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 15:41:14 GMT
ENV ROS_DISTRO=indigo
# Sat, 28 Apr 2018 15:42:56 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:43:02 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 15:43:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 15:43:03 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 15:44:00 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-base=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1083d09df9ce57f9d8407ea0bcf586a3d67a552c0d0a129bbf8fae6e98a57bb3`  
		Last Modified: Sat, 28 Apr 2018 12:08:17 GMT  
		Size: 66.6 MB (66562822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe7ed775a4a6b507a638e9dd1c82afb92bd7b22f7ec72605227d4795cfb6c83`  
		Last Modified: Sat, 28 Apr 2018 12:07:57 GMT  
		Size: 76.8 KB (76764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da37819308e46c748dcc7fa2e59aac052a6b4926860b94cfc51ba0cd0d21f03`  
		Last Modified: Sat, 28 Apr 2018 12:07:56 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261dcad9941dc4e59979650914aff223718b875292bd6dddf3c8162c71d4331d`  
		Last Modified: Sat, 28 Apr 2018 12:07:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27c2c7e7818c4f4766277047e563b1123caf608301541924286654ab562371e`  
		Last Modified: Sat, 28 Apr 2018 12:07:56 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c26680d6a75ec67fadd17a3478a318eac88e39c3585a8a9561aa9508bb4230`  
		Last Modified: Sat, 28 Apr 2018 15:48:41 GMT  
		Size: 14.5 MB (14479359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05db85a2f86e78acc906d8f2c55ae7f5b1d7cd7d6b06421527e1bf4007ef9b9`  
		Last Modified: Sat, 28 Apr 2018 15:48:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9365fb4da02f26f67cbec4b7d2c0884dbd0286efcbde973c83dae7e4f3aed68d`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4f46c9cbb0b31db49d5073dbab6da69e078dffc865c97d36e4cf84550ff595`  
		Last Modified: Sat, 28 Apr 2018 15:48:47 GMT  
		Size: 29.2 MB (29231895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8128638104464efe80c506388fd9f18ad6adf02b48f0f683787c4573714f518`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 833.5 KB (833478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ca631fefba3ca92616904d017dd021542c1d2d3b76abea5475776baed78ed6`  
		Last Modified: Sat, 28 Apr 2018 15:49:19 GMT  
		Size: 137.6 MB (137578575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f186d161062b0ebd3ef3b9d1fe858d5728d0f29f96a65c2fe82f255d8af43b39`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab989ea1342c8f50876e7603139226a5673f0c0ec4830ce93437e9652924ab2`  
		Last Modified: Sat, 28 Apr 2018 15:49:57 GMT  
		Size: 40.4 MB (40382261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:indigo-ros-core`

```console
$ docker pull ros@sha256:8dd37d8cb02f907f2b0cf04201f0499edc0384e81918d95f6971ca462f2fc782
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7

### `ros:indigo-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:506624053c2c0c7506df085875af338626d1e616e11e3772745163ce102d214e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.3 MB (272347133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae83cd08ab20c37a584d81ea7a01db0dee9c787c4a698ea57ebaddc38dfe6ca4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:33 GMT
ADD file:3c65bdbcf1318520e7af157cb00317c8312ec16bcaf181d0db919c45f0d7a85e in / 
# Tue, 05 Jun 2018 21:21:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:35 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:35 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:36 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:21:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:21:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:21:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:22:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:22:19 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:22:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:22:36 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 22:22:36 GMT
ENV ROS_DISTRO=indigo
# Tue, 05 Jun 2018 22:26:12 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:26:14 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 22:26:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 22:26:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:28bfaceaff9b7464b1e768b0af7e1efe7877a34f238f935c36978a1ecf82c9b1`  
		Last Modified: Mon, 04 Jun 2018 14:56:53 GMT  
		Size: 73.2 MB (73162466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac540055f2f8da75b6587a88763021178d876a2b789ff0c696fbdb62485b62cd`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 72.7 KB (72656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2965585ef8b8370dc8c443e35c743ba723ee427c515535e3ff35d898804cacf9`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 631.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2416bb9f3ad2b5b0c700a4412e2ffbb671f001c45b4b7433ecdcc9c352847814`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b55a6a680757144baae1671d00d4328eee63e790ab36b27d8d52ceb62b179f`  
		Last Modified: Tue, 05 Jun 2018 21:24:12 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f4b9cb761b52e80c8c2e22b82482b36acfc6042d6119b9d9c80477b4edf1ca`  
		Last Modified: Wed, 06 Jun 2018 00:07:28 GMT  
		Size: 16.5 MB (16503268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6e76332e567f50c6d9e227ba8742779cc06fd72ae673b92a49b6a837866a82`  
		Last Modified: Wed, 06 Jun 2018 00:07:19 GMT  
		Size: 13.1 KB (13076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d28474ea3552474796c30ef6b460dbf2ac52da334bf3688c4f5c56e2bbf475`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fb2acd341049ac7e805b600f9ae4b75f463f17c4de2e1268990c044af1ecae`  
		Last Modified: Wed, 06 Jun 2018 00:07:33 GMT  
		Size: 31.8 MB (31793558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8917c4b5e4f11dc6fc522a681fbacd7f49ad1595566e16227a88fea7456be049`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 866.4 KB (866395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b658217912538eca0530e8dc87a5b34901694d0cb0c499c8b4002d6e52394a23`  
		Last Modified: Wed, 06 Jun 2018 00:08:23 GMT  
		Size: 149.9 MB (149933655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43f7eb4cfafeec229d90ac1e2b44df59feb5ecea14466ea1ede851e58316091`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:indigo-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:69bb62ec259532111b92496645ef138a2ba374d2b85b5ec6ce05bf445f4b17fc
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248778058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54f2f3f28fc74bbab0a6e4a63015b8f92e784a012251a0611d4f208add949714`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:04:54 GMT
ADD file:c3b59ed8b3c28caaaafd56091269a82da9739f5b9261593e97ed075cbd489c28 in / 
# Sat, 28 Apr 2018 12:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:04:57 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:04:58 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:04:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:00 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 15:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:39:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 15:39:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 15:40:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:40:47 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 15:40:47 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 15:41:09 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 15:41:14 GMT
ENV ROS_DISTRO=indigo
# Sat, 28 Apr 2018 15:42:56 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:43:02 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 15:43:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 15:43:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1083d09df9ce57f9d8407ea0bcf586a3d67a552c0d0a129bbf8fae6e98a57bb3`  
		Last Modified: Sat, 28 Apr 2018 12:08:17 GMT  
		Size: 66.6 MB (66562822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe7ed775a4a6b507a638e9dd1c82afb92bd7b22f7ec72605227d4795cfb6c83`  
		Last Modified: Sat, 28 Apr 2018 12:07:57 GMT  
		Size: 76.8 KB (76764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da37819308e46c748dcc7fa2e59aac052a6b4926860b94cfc51ba0cd0d21f03`  
		Last Modified: Sat, 28 Apr 2018 12:07:56 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261dcad9941dc4e59979650914aff223718b875292bd6dddf3c8162c71d4331d`  
		Last Modified: Sat, 28 Apr 2018 12:07:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27c2c7e7818c4f4766277047e563b1123caf608301541924286654ab562371e`  
		Last Modified: Sat, 28 Apr 2018 12:07:56 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c26680d6a75ec67fadd17a3478a318eac88e39c3585a8a9561aa9508bb4230`  
		Last Modified: Sat, 28 Apr 2018 15:48:41 GMT  
		Size: 14.5 MB (14479359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05db85a2f86e78acc906d8f2c55ae7f5b1d7cd7d6b06421527e1bf4007ef9b9`  
		Last Modified: Sat, 28 Apr 2018 15:48:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9365fb4da02f26f67cbec4b7d2c0884dbd0286efcbde973c83dae7e4f3aed68d`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4f46c9cbb0b31db49d5073dbab6da69e078dffc865c97d36e4cf84550ff595`  
		Last Modified: Sat, 28 Apr 2018 15:48:47 GMT  
		Size: 29.2 MB (29231895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8128638104464efe80c506388fd9f18ad6adf02b48f0f683787c4573714f518`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 833.5 KB (833478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ca631fefba3ca92616904d017dd021542c1d2d3b76abea5475776baed78ed6`  
		Last Modified: Sat, 28 Apr 2018 15:49:19 GMT  
		Size: 137.6 MB (137578575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f186d161062b0ebd3ef3b9d1fe858d5728d0f29f96a65c2fe82f255d8af43b39`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:indigo-ros-core-trusty`

```console
$ docker pull ros@sha256:8dd37d8cb02f907f2b0cf04201f0499edc0384e81918d95f6971ca462f2fc782
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7

### `ros:indigo-ros-core-trusty` - linux; amd64

```console
$ docker pull ros@sha256:506624053c2c0c7506df085875af338626d1e616e11e3772745163ce102d214e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.3 MB (272347133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae83cd08ab20c37a584d81ea7a01db0dee9c787c4a698ea57ebaddc38dfe6ca4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:33 GMT
ADD file:3c65bdbcf1318520e7af157cb00317c8312ec16bcaf181d0db919c45f0d7a85e in / 
# Tue, 05 Jun 2018 21:21:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:35 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:35 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:36 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:21:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:21:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:21:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:22:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:22:19 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:22:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:22:36 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 22:22:36 GMT
ENV ROS_DISTRO=indigo
# Tue, 05 Jun 2018 22:26:12 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:26:14 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 22:26:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 22:26:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:28bfaceaff9b7464b1e768b0af7e1efe7877a34f238f935c36978a1ecf82c9b1`  
		Last Modified: Mon, 04 Jun 2018 14:56:53 GMT  
		Size: 73.2 MB (73162466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac540055f2f8da75b6587a88763021178d876a2b789ff0c696fbdb62485b62cd`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 72.7 KB (72656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2965585ef8b8370dc8c443e35c743ba723ee427c515535e3ff35d898804cacf9`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 631.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2416bb9f3ad2b5b0c700a4412e2ffbb671f001c45b4b7433ecdcc9c352847814`  
		Last Modified: Tue, 05 Jun 2018 21:24:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b55a6a680757144baae1671d00d4328eee63e790ab36b27d8d52ceb62b179f`  
		Last Modified: Tue, 05 Jun 2018 21:24:12 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f4b9cb761b52e80c8c2e22b82482b36acfc6042d6119b9d9c80477b4edf1ca`  
		Last Modified: Wed, 06 Jun 2018 00:07:28 GMT  
		Size: 16.5 MB (16503268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6e76332e567f50c6d9e227ba8742779cc06fd72ae673b92a49b6a837866a82`  
		Last Modified: Wed, 06 Jun 2018 00:07:19 GMT  
		Size: 13.1 KB (13076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d28474ea3552474796c30ef6b460dbf2ac52da334bf3688c4f5c56e2bbf475`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fb2acd341049ac7e805b600f9ae4b75f463f17c4de2e1268990c044af1ecae`  
		Last Modified: Wed, 06 Jun 2018 00:07:33 GMT  
		Size: 31.8 MB (31793558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8917c4b5e4f11dc6fc522a681fbacd7f49ad1595566e16227a88fea7456be049`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 866.4 KB (866395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b658217912538eca0530e8dc87a5b34901694d0cb0c499c8b4002d6e52394a23`  
		Last Modified: Wed, 06 Jun 2018 00:08:23 GMT  
		Size: 149.9 MB (149933655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43f7eb4cfafeec229d90ac1e2b44df59feb5ecea14466ea1ede851e58316091`  
		Last Modified: Wed, 06 Jun 2018 00:07:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:indigo-ros-core-trusty` - linux; arm variant v7

```console
$ docker pull ros@sha256:69bb62ec259532111b92496645ef138a2ba374d2b85b5ec6ce05bf445f4b17fc
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248778058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54f2f3f28fc74bbab0a6e4a63015b8f92e784a012251a0611d4f208add949714`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:04:54 GMT
ADD file:c3b59ed8b3c28caaaafd56091269a82da9739f5b9261593e97ed075cbd489c28 in / 
# Sat, 28 Apr 2018 12:04:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:04:57 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:04:58 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:04:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:00 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 15:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:39:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 15:39:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 15:40:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:40:47 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 15:40:47 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 15:41:09 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 15:41:14 GMT
ENV ROS_DISTRO=indigo
# Sat, 28 Apr 2018 15:42:56 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.6-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 15:43:02 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 15:43:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 15:43:03 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1083d09df9ce57f9d8407ea0bcf586a3d67a552c0d0a129bbf8fae6e98a57bb3`  
		Last Modified: Sat, 28 Apr 2018 12:08:17 GMT  
		Size: 66.6 MB (66562822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe7ed775a4a6b507a638e9dd1c82afb92bd7b22f7ec72605227d4795cfb6c83`  
		Last Modified: Sat, 28 Apr 2018 12:07:57 GMT  
		Size: 76.8 KB (76764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da37819308e46c748dcc7fa2e59aac052a6b4926860b94cfc51ba0cd0d21f03`  
		Last Modified: Sat, 28 Apr 2018 12:07:56 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261dcad9941dc4e59979650914aff223718b875292bd6dddf3c8162c71d4331d`  
		Last Modified: Sat, 28 Apr 2018 12:07:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27c2c7e7818c4f4766277047e563b1123caf608301541924286654ab562371e`  
		Last Modified: Sat, 28 Apr 2018 12:07:56 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c26680d6a75ec67fadd17a3478a318eac88e39c3585a8a9561aa9508bb4230`  
		Last Modified: Sat, 28 Apr 2018 15:48:41 GMT  
		Size: 14.5 MB (14479359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05db85a2f86e78acc906d8f2c55ae7f5b1d7cd7d6b06421527e1bf4007ef9b9`  
		Last Modified: Sat, 28 Apr 2018 15:48:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9365fb4da02f26f67cbec4b7d2c0884dbd0286efcbde973c83dae7e4f3aed68d`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4f46c9cbb0b31db49d5073dbab6da69e078dffc865c97d36e4cf84550ff595`  
		Last Modified: Sat, 28 Apr 2018 15:48:47 GMT  
		Size: 29.2 MB (29231895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8128638104464efe80c506388fd9f18ad6adf02b48f0f683787c4573714f518`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 833.5 KB (833478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ca631fefba3ca92616904d017dd021542c1d2d3b76abea5475776baed78ed6`  
		Last Modified: Sat, 28 Apr 2018 15:49:19 GMT  
		Size: 137.6 MB (137578575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f186d161062b0ebd3ef3b9d1fe858d5728d0f29f96a65c2fe82f255d8af43b39`  
		Last Modified: Sat, 28 Apr 2018 15:48:36 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic`

```console
$ docker pull ros@sha256:514dc64b38c39328168451af72407209a0deb168674ffb23bc63ef90f33797ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic` - linux; amd64

```console
$ docker pull ros@sha256:a2983a9a10f8d57c674ce7a3a522d52bafadb0916b95f8f64053eae0a0878b09
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **382.5 MB (382492888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c95770be708eaf6d9552544c42ad44df548bbb2995b19d17be5a75cbb9fabf55`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:52 GMT
ADD file:d37ff24540ea7700d0fc053e1996b234428a88f3a324d7fcbd83d8ef95318040 in / 
# Tue, 05 Jun 2018 21:21:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:54 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:55 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:35:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:35:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:35:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:36:43 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 22:36:43 GMT
ENV ROS_DISTRO=kinetic
# Tue, 05 Jun 2018 22:39:54 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:39:55 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 22:39:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 22:39:56 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 22:42:13 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b234f539f7a1d65eabae1617e63c81ac01768abffd48b5cbbf7166efca6a3429`  
		Last Modified: Mon, 28 May 2018 14:57:20 GMT  
		Size: 43.1 MB (43122477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55172d420b43cf03feeec11bcc917c7ddfc192036102e065ab57aa9abb95311e`  
		Last Modified: Tue, 05 Jun 2018 21:24:52 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba5bbeb6b91e2676c98255c6babc66d7b05cac40185eeba4b3773199c701da0`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ae2841ad7a7fd1aeae30028105cac7f6ee0ec955e5229e52b3333fea3c17b5`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c9c6de41905e9a66f2bc2c4a19858c8dc5b0a94f01e03eafc719afe25888aa`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22c30eae0b9363cecd2e5ac27a92dd1bc354e2e16a3ee82b70932814b4c12a`  
		Last Modified: Wed, 06 Jun 2018 00:11:32 GMT  
		Size: 5.4 MB (5362202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fce58d2960dc3a1265e5bc18474d652795940cafde67d662929605c9e3b1c44`  
		Last Modified: Wed, 06 Jun 2018 00:11:29 GMT  
		Size: 13.1 KB (13081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a8410e99e70f8971b54ce991fecd04014ef363a7dde349dd255d6358a6893d`  
		Last Modified: Wed, 06 Jun 2018 00:11:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3037b7978826369126bbe26cbb5d642f59ccd31d96e28044f872cd3eac55ab`  
		Last Modified: Wed, 06 Jun 2018 00:11:55 GMT  
		Size: 55.6 MB (55571338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cfa8aa4c1f7b161f88b862221bacc540052abfa4f8a11884d0090ebcd55cf9`  
		Last Modified: Wed, 06 Jun 2018 00:11:27 GMT  
		Size: 866.4 KB (866393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16efe7b0a2f0d3cc997ef3ea8c9ed2f3a888fbba64f18ae15c76824cc3fb268d`  
		Last Modified: Wed, 06 Jun 2018 00:12:49 GMT  
		Size: 193.6 MB (193645836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4305ed9cccd0e188c6305b22e2947c513b38a205a8c2fa4ab93825b1ab5d3873`  
		Last Modified: Wed, 06 Jun 2018 00:11:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cce0e73a68108059c9c4433d0c94134a0326a293063d40ac9e2106b50b0b18`  
		Last Modified: Wed, 06 Jun 2018 00:13:42 GMT  
		Size: 83.9 MB (83908652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic` - linux; arm variant v7

```console
$ docker pull ros@sha256:354195f78c404ff1fa6cae0f5970cf95e49dfb2879055aeeebd14bd4d2ca3232
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.2 MB (334248273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1b693d5d950e5bec2c9bc8928434570a2e2c180e7306444f9e5ac0cf0be8352`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:05:33 GMT
ADD file:1e3efdebaf133af6b22e61da056500ff8cf5292f051296f69abd35f44da5625c in / 
# Sat, 28 Apr 2018 12:05:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:05:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:05:37 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:05:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:50 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 12:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:08:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 12:08:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 12:09:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 12:09:57 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 12:09:58 GMT
ENV ROS_DISTRO=kinetic
# Sat, 28 Apr 2018 12:11:17 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:11:18 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 12:11:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 12:11:19 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 12:12:30 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f68dc00194f474ccfe395953a935f0a65f37edc5e218b6f310f432b3866f9bac`  
		Last Modified: Sat, 28 Apr 2018 12:09:03 GMT  
		Size: 38.1 MB (38126697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281b914f46e3b5e9fac0f9436525399186a66cb5abb5403eed9940d4207e15b4`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b205ebc944011540b5d7c371fe39a5cb49890d018253fcd39db61040dfed3`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418c61fca2a7e383833d9b12bd7adf62e311bf6350037e68503fbbbdfb8cc2b`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b471dd10511e8664a33e00815086f40bdfd8c30a16f93b190084bb5bb8a993f`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5050587be2fd4accc805402daed25e9344bd052ced481a6ecd1a5754102cb84`  
		Last Modified: Sat, 28 Apr 2018 12:27:40 GMT  
		Size: 4.6 MB (4614906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334ce8d248512220d545aecf150f8b8172bbd3e4c62f9cdc4c1e814053440912`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d06c2ef1c00b3cb66443790e82ae98882427dfc78b0009b2b801bdd0387146`  
		Last Modified: Sat, 28 Apr 2018 12:27:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b97dba49af961b21651a5255033ef01a2c0100029e05207d73befd0c45f6d85`  
		Last Modified: Sat, 28 Apr 2018 12:27:55 GMT  
		Size: 50.7 MB (50671071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1310601b6139b280f88b623eeaef6873b2ed293d2e09bc94346f6a444ab9973`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 833.2 KB (833166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a715f7dcd6ee641ea9e85cf6349780799f1e5d41a2a378290058db5c5cd28cb9`  
		Last Modified: Sat, 28 Apr 2018 12:28:25 GMT  
		Size: 164.9 MB (164896280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4e27b5b65dc6b6f87f9c3ae1918a2f334a2f06d1f6ef92a7cfcbabf5871c03`  
		Last Modified: Sat, 28 Apr 2018 12:27:37 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af540861d5e6d956c803433ef96efdb49e6b8d0585b05bc5a5fa810807687f22`  
		Last Modified: Sat, 28 Apr 2018 12:29:03 GMT  
		Size: 75.1 MB (75090166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:89c95b9f4fac10565324dc86c8386555a757b1cd15cc3c33a345b946b3592dc9
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.0 MB (348048555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab8e7598dc15d5e6be4962d16faeeb44bb7d27153a3744202cf92b978b8bf1b1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:12:52 GMT
ADD file:fef3655a03a1c7f1533148016797b982955b3d5556f32c777214b8426028509b in / 
# Tue, 01 May 2018 01:12:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:13:04 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:13:10 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:13:20 GMT
CMD ["/bin/bash"]
# Tue, 01 May 2018 01:19:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:19:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 01:19:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 01:23:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:23:33 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 01:23:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 01:24:25 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 01:24:27 GMT
ENV ROS_DISTRO=kinetic
# Tue, 01 May 2018 01:36:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:37:08 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 01:37:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 01:37:33 GMT
CMD ["bash"]
# Tue, 01 May 2018 01:48:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c016a9a148a71d05469a3994d54eb7eb9c3d40a65e07bf68788018a71d951b`  
		Last Modified: Mon, 23 Apr 2018 14:56:07 GMT  
		Size: 39.2 MB (39223827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1976297de94ed1f5c4c0f13b0b25199c6d6ca003ddfc3e873938aa2f8e86b`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d83417bbef32ed4713f4224bcb9f9573597ee6d91174dc7403ce457f145d2`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2544c5c45beca34c948aca9c981d56b587a973354727e4c97dc99d88227fb6a`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92ef1d410a96b276ec1425b000d80d5c1d914688aae8bce3e6f20d8a5a7a5f`  
		Last Modified: Tue, 01 May 2018 01:17:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3a2ac905d0d30502b9bf9736c755da2e7a05465764ff1fb14a45f067faa71c`  
		Last Modified: Tue, 01 May 2018 04:17:49 GMT  
		Size: 4.8 MB (4819486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31df2d860f2dc7f931faa244a38a740a44c732fd7ab480a29daf8999b5fb7fcd`  
		Last Modified: Tue, 01 May 2018 04:17:40 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a06299e2df93eba22547e7bbfaf291225cb3e1d85dcd160f7080d0d65647a`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ce03745d3f424b139a80266262e70dfefbda981c88ae34eac7b56df3120657`  
		Last Modified: Tue, 01 May 2018 04:18:42 GMT  
		Size: 52.4 MB (52441627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360b2687112930e2c2a443c4f89ecbdda5be0103c5b840e39840d3aca65352a`  
		Last Modified: Tue, 01 May 2018 04:17:41 GMT  
		Size: 835.1 KB (835081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf20cb73de898c810a3ce03d3d4ac43ca405c527b42e21244058ec4bdbf204b`  
		Last Modified: Tue, 01 May 2018 04:19:47 GMT  
		Size: 174.2 MB (174167620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede09c9013f1c95beb0aee3d89bc517d63df382e40d6e2e506b200c897ebc627`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31090de9e5f5a2759e0e667f1d0e72efbb5354d84bd5084b225053079926d2d7`  
		Last Modified: Tue, 01 May 2018 04:20:58 GMT  
		Size: 76.5 MB (76544918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-perception`

```console
$ docker pull ros@sha256:7a45f5242e95496f6354b554bf29cc68145b4a3fcfc03b36316f474de1c29c8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:aff3077aa97bc8dba5be25ad84921aa7676b201946fbf2946e4557a6be88b180
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **722.8 MB (722753235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a556929a861a67d340eb4abda14ffd731567256fb98d262ac059549c69c3422`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:52 GMT
ADD file:d37ff24540ea7700d0fc053e1996b234428a88f3a324d7fcbd83d8ef95318040 in / 
# Tue, 05 Jun 2018 21:21:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:54 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:55 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:35:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:35:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:35:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:36:43 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 22:36:43 GMT
ENV ROS_DISTRO=kinetic
# Tue, 05 Jun 2018 22:39:54 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:39:55 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 22:39:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 22:39:56 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 22:42:13 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:50:55 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b234f539f7a1d65eabae1617e63c81ac01768abffd48b5cbbf7166efca6a3429`  
		Last Modified: Mon, 28 May 2018 14:57:20 GMT  
		Size: 43.1 MB (43122477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55172d420b43cf03feeec11bcc917c7ddfc192036102e065ab57aa9abb95311e`  
		Last Modified: Tue, 05 Jun 2018 21:24:52 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba5bbeb6b91e2676c98255c6babc66d7b05cac40185eeba4b3773199c701da0`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ae2841ad7a7fd1aeae30028105cac7f6ee0ec955e5229e52b3333fea3c17b5`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c9c6de41905e9a66f2bc2c4a19858c8dc5b0a94f01e03eafc719afe25888aa`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22c30eae0b9363cecd2e5ac27a92dd1bc354e2e16a3ee82b70932814b4c12a`  
		Last Modified: Wed, 06 Jun 2018 00:11:32 GMT  
		Size: 5.4 MB (5362202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fce58d2960dc3a1265e5bc18474d652795940cafde67d662929605c9e3b1c44`  
		Last Modified: Wed, 06 Jun 2018 00:11:29 GMT  
		Size: 13.1 KB (13081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a8410e99e70f8971b54ce991fecd04014ef363a7dde349dd255d6358a6893d`  
		Last Modified: Wed, 06 Jun 2018 00:11:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3037b7978826369126bbe26cbb5d642f59ccd31d96e28044f872cd3eac55ab`  
		Last Modified: Wed, 06 Jun 2018 00:11:55 GMT  
		Size: 55.6 MB (55571338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cfa8aa4c1f7b161f88b862221bacc540052abfa4f8a11884d0090ebcd55cf9`  
		Last Modified: Wed, 06 Jun 2018 00:11:27 GMT  
		Size: 866.4 KB (866393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16efe7b0a2f0d3cc997ef3ea8c9ed2f3a888fbba64f18ae15c76824cc3fb268d`  
		Last Modified: Wed, 06 Jun 2018 00:12:49 GMT  
		Size: 193.6 MB (193645836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4305ed9cccd0e188c6305b22e2947c513b38a205a8c2fa4ab93825b1ab5d3873`  
		Last Modified: Wed, 06 Jun 2018 00:11:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cce0e73a68108059c9c4433d0c94134a0326a293063d40ac9e2106b50b0b18`  
		Last Modified: Wed, 06 Jun 2018 00:13:42 GMT  
		Size: 83.9 MB (83908652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6718e843943fa578dab87cf7688bcb66a376f6fbb6b8bb626794b9cf7ad4aa`  
		Last Modified: Wed, 06 Jun 2018 00:17:41 GMT  
		Size: 340.3 MB (340260347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:f7890e7493bb6f2cc5d575fce15154e6a080e5d201414027f82fa4c16e11eb83
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **614.6 MB (614612392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03f84f4251b4aca5d0a4b17af712b114ee10fe82f233bd280b1d45004a8d5de4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:05:33 GMT
ADD file:1e3efdebaf133af6b22e61da056500ff8cf5292f051296f69abd35f44da5625c in / 
# Sat, 28 Apr 2018 12:05:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:05:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:05:37 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:05:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:50 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 12:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:08:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 12:08:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 12:09:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 12:09:57 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 12:09:58 GMT
ENV ROS_DISTRO=kinetic
# Sat, 28 Apr 2018 12:11:17 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:11:18 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 12:11:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 12:11:19 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 12:12:30 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:16:25 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f68dc00194f474ccfe395953a935f0a65f37edc5e218b6f310f432b3866f9bac`  
		Last Modified: Sat, 28 Apr 2018 12:09:03 GMT  
		Size: 38.1 MB (38126697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281b914f46e3b5e9fac0f9436525399186a66cb5abb5403eed9940d4207e15b4`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b205ebc944011540b5d7c371fe39a5cb49890d018253fcd39db61040dfed3`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418c61fca2a7e383833d9b12bd7adf62e311bf6350037e68503fbbbdfb8cc2b`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b471dd10511e8664a33e00815086f40bdfd8c30a16f93b190084bb5bb8a993f`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5050587be2fd4accc805402daed25e9344bd052ced481a6ecd1a5754102cb84`  
		Last Modified: Sat, 28 Apr 2018 12:27:40 GMT  
		Size: 4.6 MB (4614906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334ce8d248512220d545aecf150f8b8172bbd3e4c62f9cdc4c1e814053440912`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d06c2ef1c00b3cb66443790e82ae98882427dfc78b0009b2b801bdd0387146`  
		Last Modified: Sat, 28 Apr 2018 12:27:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b97dba49af961b21651a5255033ef01a2c0100029e05207d73befd0c45f6d85`  
		Last Modified: Sat, 28 Apr 2018 12:27:55 GMT  
		Size: 50.7 MB (50671071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1310601b6139b280f88b623eeaef6873b2ed293d2e09bc94346f6a444ab9973`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 833.2 KB (833166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a715f7dcd6ee641ea9e85cf6349780799f1e5d41a2a378290058db5c5cd28cb9`  
		Last Modified: Sat, 28 Apr 2018 12:28:25 GMT  
		Size: 164.9 MB (164896280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4e27b5b65dc6b6f87f9c3ae1918a2f334a2f06d1f6ef92a7cfcbabf5871c03`  
		Last Modified: Sat, 28 Apr 2018 12:27:37 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af540861d5e6d956c803433ef96efdb49e6b8d0585b05bc5a5fa810807687f22`  
		Last Modified: Sat, 28 Apr 2018 12:29:03 GMT  
		Size: 75.1 MB (75090166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461ef1127a6358d0391e19225c9244833973907958057913babdf0d2b722e0f2`  
		Last Modified: Sat, 28 Apr 2018 12:31:41 GMT  
		Size: 280.4 MB (280364119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0ef4dd6ebd43a736cef4d9ccd3af0c0dede98d17c857d2e2f296a3ac25cda0c5
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **638.9 MB (638877793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2abe895a522e8a7b2fd45e528f65ffdfd6e46dca6f0f979b016f053f5e4b5ec1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:12:52 GMT
ADD file:fef3655a03a1c7f1533148016797b982955b3d5556f32c777214b8426028509b in / 
# Tue, 01 May 2018 01:12:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:13:04 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:13:10 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:13:20 GMT
CMD ["/bin/bash"]
# Tue, 01 May 2018 01:19:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:19:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 01:19:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 01:23:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:23:33 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 01:23:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 01:24:25 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 01:24:27 GMT
ENV ROS_DISTRO=kinetic
# Tue, 01 May 2018 01:36:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:37:08 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 01:37:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 01:37:33 GMT
CMD ["bash"]
# Tue, 01 May 2018 01:48:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 02:08:20 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c016a9a148a71d05469a3994d54eb7eb9c3d40a65e07bf68788018a71d951b`  
		Last Modified: Mon, 23 Apr 2018 14:56:07 GMT  
		Size: 39.2 MB (39223827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1976297de94ed1f5c4c0f13b0b25199c6d6ca003ddfc3e873938aa2f8e86b`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d83417bbef32ed4713f4224bcb9f9573597ee6d91174dc7403ce457f145d2`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2544c5c45beca34c948aca9c981d56b587a973354727e4c97dc99d88227fb6a`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92ef1d410a96b276ec1425b000d80d5c1d914688aae8bce3e6f20d8a5a7a5f`  
		Last Modified: Tue, 01 May 2018 01:17:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3a2ac905d0d30502b9bf9736c755da2e7a05465764ff1fb14a45f067faa71c`  
		Last Modified: Tue, 01 May 2018 04:17:49 GMT  
		Size: 4.8 MB (4819486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31df2d860f2dc7f931faa244a38a740a44c732fd7ab480a29daf8999b5fb7fcd`  
		Last Modified: Tue, 01 May 2018 04:17:40 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a06299e2df93eba22547e7bbfaf291225cb3e1d85dcd160f7080d0d65647a`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ce03745d3f424b139a80266262e70dfefbda981c88ae34eac7b56df3120657`  
		Last Modified: Tue, 01 May 2018 04:18:42 GMT  
		Size: 52.4 MB (52441627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360b2687112930e2c2a443c4f89ecbdda5be0103c5b840e39840d3aca65352a`  
		Last Modified: Tue, 01 May 2018 04:17:41 GMT  
		Size: 835.1 KB (835081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf20cb73de898c810a3ce03d3d4ac43ca405c527b42e21244058ec4bdbf204b`  
		Last Modified: Tue, 01 May 2018 04:19:47 GMT  
		Size: 174.2 MB (174167620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede09c9013f1c95beb0aee3d89bc517d63df382e40d6e2e506b200c897ebc627`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31090de9e5f5a2759e0e667f1d0e72efbb5354d84bd5084b225053079926d2d7`  
		Last Modified: Tue, 01 May 2018 04:20:58 GMT  
		Size: 76.5 MB (76544918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3979a12b0fda2321282b7685908c8a70e7c6c23b2ec74747e3643d7a8879e71d`  
		Last Modified: Tue, 01 May 2018 04:26:15 GMT  
		Size: 290.8 MB (290829238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-perception-jessie`

```console
$ docker pull ros@sha256:316a994d613b78c38543cd485f52dcc568018bfb226f3e083af14a1ac6f1dbb8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:kinetic-perception-jessie` - linux; amd64

```console
$ docker pull ros@sha256:ac0e7ec3085397143751aa8e63697e0a9fdba717cf86b3d401e7a4674ccd148a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.0 MB (641009477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63310c6e836ee0f0161deb4dcefa020ff97fc6dfbac9e04b67b20a999465c7cc`
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
# Tue, 05 Jun 2018 23:04:01 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:02a387a3e0a5d46341d49f1eeb6a4fb8b04f64714acca651b626d76790280273`  
		Last Modified: Wed, 06 Jun 2018 00:22:18 GMT  
		Size: 265.6 MB (265587694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception-jessie` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fb3319fd70ccbef7d0c51296256eaf21cda176e61e40063e8d73edd27f172bcf
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **557.8 MB (557829113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42a79943c0674ac386999fe672a9e0ef47dd189e0d95982615224d97c7442951`
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
# Tue, 01 May 2018 02:51:14 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:a60973845366075406dcfeb715d4dc8b438b8ba7d157c72822e0d618e03ca8cb`  
		Last Modified: Tue, 01 May 2018 04:32:31 GMT  
		Size: 230.9 MB (230940313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-perception-xenial`

```console
$ docker pull ros@sha256:7a45f5242e95496f6354b554bf29cc68145b4a3fcfc03b36316f474de1c29c8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-perception-xenial` - linux; amd64

```console
$ docker pull ros@sha256:aff3077aa97bc8dba5be25ad84921aa7676b201946fbf2946e4557a6be88b180
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **722.8 MB (722753235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a556929a861a67d340eb4abda14ffd731567256fb98d262ac059549c69c3422`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:52 GMT
ADD file:d37ff24540ea7700d0fc053e1996b234428a88f3a324d7fcbd83d8ef95318040 in / 
# Tue, 05 Jun 2018 21:21:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:54 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:55 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:35:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:35:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:35:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:36:43 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 22:36:43 GMT
ENV ROS_DISTRO=kinetic
# Tue, 05 Jun 2018 22:39:54 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:39:55 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 22:39:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 22:39:56 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 22:42:13 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:50:55 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b234f539f7a1d65eabae1617e63c81ac01768abffd48b5cbbf7166efca6a3429`  
		Last Modified: Mon, 28 May 2018 14:57:20 GMT  
		Size: 43.1 MB (43122477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55172d420b43cf03feeec11bcc917c7ddfc192036102e065ab57aa9abb95311e`  
		Last Modified: Tue, 05 Jun 2018 21:24:52 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba5bbeb6b91e2676c98255c6babc66d7b05cac40185eeba4b3773199c701da0`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ae2841ad7a7fd1aeae30028105cac7f6ee0ec955e5229e52b3333fea3c17b5`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c9c6de41905e9a66f2bc2c4a19858c8dc5b0a94f01e03eafc719afe25888aa`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22c30eae0b9363cecd2e5ac27a92dd1bc354e2e16a3ee82b70932814b4c12a`  
		Last Modified: Wed, 06 Jun 2018 00:11:32 GMT  
		Size: 5.4 MB (5362202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fce58d2960dc3a1265e5bc18474d652795940cafde67d662929605c9e3b1c44`  
		Last Modified: Wed, 06 Jun 2018 00:11:29 GMT  
		Size: 13.1 KB (13081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a8410e99e70f8971b54ce991fecd04014ef363a7dde349dd255d6358a6893d`  
		Last Modified: Wed, 06 Jun 2018 00:11:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3037b7978826369126bbe26cbb5d642f59ccd31d96e28044f872cd3eac55ab`  
		Last Modified: Wed, 06 Jun 2018 00:11:55 GMT  
		Size: 55.6 MB (55571338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cfa8aa4c1f7b161f88b862221bacc540052abfa4f8a11884d0090ebcd55cf9`  
		Last Modified: Wed, 06 Jun 2018 00:11:27 GMT  
		Size: 866.4 KB (866393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16efe7b0a2f0d3cc997ef3ea8c9ed2f3a888fbba64f18ae15c76824cc3fb268d`  
		Last Modified: Wed, 06 Jun 2018 00:12:49 GMT  
		Size: 193.6 MB (193645836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4305ed9cccd0e188c6305b22e2947c513b38a205a8c2fa4ab93825b1ab5d3873`  
		Last Modified: Wed, 06 Jun 2018 00:11:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cce0e73a68108059c9c4433d0c94134a0326a293063d40ac9e2106b50b0b18`  
		Last Modified: Wed, 06 Jun 2018 00:13:42 GMT  
		Size: 83.9 MB (83908652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6718e843943fa578dab87cf7688bcb66a376f6fbb6b8bb626794b9cf7ad4aa`  
		Last Modified: Wed, 06 Jun 2018 00:17:41 GMT  
		Size: 340.3 MB (340260347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:f7890e7493bb6f2cc5d575fce15154e6a080e5d201414027f82fa4c16e11eb83
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **614.6 MB (614612392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03f84f4251b4aca5d0a4b17af712b114ee10fe82f233bd280b1d45004a8d5de4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:05:33 GMT
ADD file:1e3efdebaf133af6b22e61da056500ff8cf5292f051296f69abd35f44da5625c in / 
# Sat, 28 Apr 2018 12:05:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:05:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:05:37 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:05:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:50 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 12:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:08:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 12:08:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 12:09:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 12:09:57 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 12:09:58 GMT
ENV ROS_DISTRO=kinetic
# Sat, 28 Apr 2018 12:11:17 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:11:18 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 12:11:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 12:11:19 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 12:12:30 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:16:25 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f68dc00194f474ccfe395953a935f0a65f37edc5e218b6f310f432b3866f9bac`  
		Last Modified: Sat, 28 Apr 2018 12:09:03 GMT  
		Size: 38.1 MB (38126697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281b914f46e3b5e9fac0f9436525399186a66cb5abb5403eed9940d4207e15b4`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b205ebc944011540b5d7c371fe39a5cb49890d018253fcd39db61040dfed3`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418c61fca2a7e383833d9b12bd7adf62e311bf6350037e68503fbbbdfb8cc2b`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b471dd10511e8664a33e00815086f40bdfd8c30a16f93b190084bb5bb8a993f`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5050587be2fd4accc805402daed25e9344bd052ced481a6ecd1a5754102cb84`  
		Last Modified: Sat, 28 Apr 2018 12:27:40 GMT  
		Size: 4.6 MB (4614906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334ce8d248512220d545aecf150f8b8172bbd3e4c62f9cdc4c1e814053440912`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d06c2ef1c00b3cb66443790e82ae98882427dfc78b0009b2b801bdd0387146`  
		Last Modified: Sat, 28 Apr 2018 12:27:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b97dba49af961b21651a5255033ef01a2c0100029e05207d73befd0c45f6d85`  
		Last Modified: Sat, 28 Apr 2018 12:27:55 GMT  
		Size: 50.7 MB (50671071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1310601b6139b280f88b623eeaef6873b2ed293d2e09bc94346f6a444ab9973`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 833.2 KB (833166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a715f7dcd6ee641ea9e85cf6349780799f1e5d41a2a378290058db5c5cd28cb9`  
		Last Modified: Sat, 28 Apr 2018 12:28:25 GMT  
		Size: 164.9 MB (164896280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4e27b5b65dc6b6f87f9c3ae1918a2f334a2f06d1f6ef92a7cfcbabf5871c03`  
		Last Modified: Sat, 28 Apr 2018 12:27:37 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af540861d5e6d956c803433ef96efdb49e6b8d0585b05bc5a5fa810807687f22`  
		Last Modified: Sat, 28 Apr 2018 12:29:03 GMT  
		Size: 75.1 MB (75090166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461ef1127a6358d0391e19225c9244833973907958057913babdf0d2b722e0f2`  
		Last Modified: Sat, 28 Apr 2018 12:31:41 GMT  
		Size: 280.4 MB (280364119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-perception-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0ef4dd6ebd43a736cef4d9ccd3af0c0dede98d17c857d2e2f296a3ac25cda0c5
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **638.9 MB (638877793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2abe895a522e8a7b2fd45e528f65ffdfd6e46dca6f0f979b016f053f5e4b5ec1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:12:52 GMT
ADD file:fef3655a03a1c7f1533148016797b982955b3d5556f32c777214b8426028509b in / 
# Tue, 01 May 2018 01:12:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:13:04 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:13:10 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:13:20 GMT
CMD ["/bin/bash"]
# Tue, 01 May 2018 01:19:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:19:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 01:19:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 01:23:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:23:33 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 01:23:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 01:24:25 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 01:24:27 GMT
ENV ROS_DISTRO=kinetic
# Tue, 01 May 2018 01:36:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:37:08 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 01:37:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 01:37:33 GMT
CMD ["bash"]
# Tue, 01 May 2018 01:48:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 02:08:20 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c016a9a148a71d05469a3994d54eb7eb9c3d40a65e07bf68788018a71d951b`  
		Last Modified: Mon, 23 Apr 2018 14:56:07 GMT  
		Size: 39.2 MB (39223827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1976297de94ed1f5c4c0f13b0b25199c6d6ca003ddfc3e873938aa2f8e86b`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d83417bbef32ed4713f4224bcb9f9573597ee6d91174dc7403ce457f145d2`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2544c5c45beca34c948aca9c981d56b587a973354727e4c97dc99d88227fb6a`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92ef1d410a96b276ec1425b000d80d5c1d914688aae8bce3e6f20d8a5a7a5f`  
		Last Modified: Tue, 01 May 2018 01:17:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3a2ac905d0d30502b9bf9736c755da2e7a05465764ff1fb14a45f067faa71c`  
		Last Modified: Tue, 01 May 2018 04:17:49 GMT  
		Size: 4.8 MB (4819486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31df2d860f2dc7f931faa244a38a740a44c732fd7ab480a29daf8999b5fb7fcd`  
		Last Modified: Tue, 01 May 2018 04:17:40 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a06299e2df93eba22547e7bbfaf291225cb3e1d85dcd160f7080d0d65647a`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ce03745d3f424b139a80266262e70dfefbda981c88ae34eac7b56df3120657`  
		Last Modified: Tue, 01 May 2018 04:18:42 GMT  
		Size: 52.4 MB (52441627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360b2687112930e2c2a443c4f89ecbdda5be0103c5b840e39840d3aca65352a`  
		Last Modified: Tue, 01 May 2018 04:17:41 GMT  
		Size: 835.1 KB (835081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf20cb73de898c810a3ce03d3d4ac43ca405c527b42e21244058ec4bdbf204b`  
		Last Modified: Tue, 01 May 2018 04:19:47 GMT  
		Size: 174.2 MB (174167620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede09c9013f1c95beb0aee3d89bc517d63df382e40d6e2e506b200c897ebc627`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31090de9e5f5a2759e0e667f1d0e72efbb5354d84bd5084b225053079926d2d7`  
		Last Modified: Tue, 01 May 2018 04:20:58 GMT  
		Size: 76.5 MB (76544918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3979a12b0fda2321282b7685908c8a70e7c6c23b2ec74747e3643d7a8879e71d`  
		Last Modified: Tue, 01 May 2018 04:26:15 GMT  
		Size: 290.8 MB (290829238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-robot`

```console
$ docker pull ros@sha256:93ff528ca028fbbbecad73f65c9c089c08fcaafb2bc34de368ee640e74164f84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:7de0e8b7e50972c78db4d562a30a52c36bbbf8b4b6dfff9deb6145953151f33a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.1 MB (486079279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd7fc7c1c617f7d9e63a4af3925cb04ad45728fd626c176190a2f7eedb56d2a1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:52 GMT
ADD file:d37ff24540ea7700d0fc053e1996b234428a88f3a324d7fcbd83d8ef95318040 in / 
# Tue, 05 Jun 2018 21:21:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:54 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:55 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:35:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:35:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:35:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:36:43 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 22:36:43 GMT
ENV ROS_DISTRO=kinetic
# Tue, 05 Jun 2018 22:39:54 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:39:55 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 22:39:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 22:39:56 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 22:42:13 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:45:10 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b234f539f7a1d65eabae1617e63c81ac01768abffd48b5cbbf7166efca6a3429`  
		Last Modified: Mon, 28 May 2018 14:57:20 GMT  
		Size: 43.1 MB (43122477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55172d420b43cf03feeec11bcc917c7ddfc192036102e065ab57aa9abb95311e`  
		Last Modified: Tue, 05 Jun 2018 21:24:52 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba5bbeb6b91e2676c98255c6babc66d7b05cac40185eeba4b3773199c701da0`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ae2841ad7a7fd1aeae30028105cac7f6ee0ec955e5229e52b3333fea3c17b5`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c9c6de41905e9a66f2bc2c4a19858c8dc5b0a94f01e03eafc719afe25888aa`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22c30eae0b9363cecd2e5ac27a92dd1bc354e2e16a3ee82b70932814b4c12a`  
		Last Modified: Wed, 06 Jun 2018 00:11:32 GMT  
		Size: 5.4 MB (5362202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fce58d2960dc3a1265e5bc18474d652795940cafde67d662929605c9e3b1c44`  
		Last Modified: Wed, 06 Jun 2018 00:11:29 GMT  
		Size: 13.1 KB (13081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a8410e99e70f8971b54ce991fecd04014ef363a7dde349dd255d6358a6893d`  
		Last Modified: Wed, 06 Jun 2018 00:11:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3037b7978826369126bbe26cbb5d642f59ccd31d96e28044f872cd3eac55ab`  
		Last Modified: Wed, 06 Jun 2018 00:11:55 GMT  
		Size: 55.6 MB (55571338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cfa8aa4c1f7b161f88b862221bacc540052abfa4f8a11884d0090ebcd55cf9`  
		Last Modified: Wed, 06 Jun 2018 00:11:27 GMT  
		Size: 866.4 KB (866393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16efe7b0a2f0d3cc997ef3ea8c9ed2f3a888fbba64f18ae15c76824cc3fb268d`  
		Last Modified: Wed, 06 Jun 2018 00:12:49 GMT  
		Size: 193.6 MB (193645836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4305ed9cccd0e188c6305b22e2947c513b38a205a8c2fa4ab93825b1ab5d3873`  
		Last Modified: Wed, 06 Jun 2018 00:11:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cce0e73a68108059c9c4433d0c94134a0326a293063d40ac9e2106b50b0b18`  
		Last Modified: Wed, 06 Jun 2018 00:13:42 GMT  
		Size: 83.9 MB (83908652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4567c5bb30132628370213c4a90199c467537c4ba627b16f7df6268b75c20b9d`  
		Last Modified: Wed, 06 Jun 2018 00:14:53 GMT  
		Size: 103.6 MB (103586391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:b290fc09f313cdbddd5ff0676eee22a455c2be81edaab85f1888f6df6f400716
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.3 MB (424265942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f8bb432561fb6800361614853012463ff48a4e04c28b4cae78f897d8371bb0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:05:33 GMT
ADD file:1e3efdebaf133af6b22e61da056500ff8cf5292f051296f69abd35f44da5625c in / 
# Sat, 28 Apr 2018 12:05:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:05:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:05:37 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:05:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:50 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 12:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:08:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 12:08:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 12:09:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 12:09:57 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 12:09:58 GMT
ENV ROS_DISTRO=kinetic
# Sat, 28 Apr 2018 12:11:17 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:11:18 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 12:11:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 12:11:19 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 12:12:30 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:13:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f68dc00194f474ccfe395953a935f0a65f37edc5e218b6f310f432b3866f9bac`  
		Last Modified: Sat, 28 Apr 2018 12:09:03 GMT  
		Size: 38.1 MB (38126697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281b914f46e3b5e9fac0f9436525399186a66cb5abb5403eed9940d4207e15b4`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b205ebc944011540b5d7c371fe39a5cb49890d018253fcd39db61040dfed3`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418c61fca2a7e383833d9b12bd7adf62e311bf6350037e68503fbbbdfb8cc2b`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b471dd10511e8664a33e00815086f40bdfd8c30a16f93b190084bb5bb8a993f`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5050587be2fd4accc805402daed25e9344bd052ced481a6ecd1a5754102cb84`  
		Last Modified: Sat, 28 Apr 2018 12:27:40 GMT  
		Size: 4.6 MB (4614906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334ce8d248512220d545aecf150f8b8172bbd3e4c62f9cdc4c1e814053440912`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d06c2ef1c00b3cb66443790e82ae98882427dfc78b0009b2b801bdd0387146`  
		Last Modified: Sat, 28 Apr 2018 12:27:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b97dba49af961b21651a5255033ef01a2c0100029e05207d73befd0c45f6d85`  
		Last Modified: Sat, 28 Apr 2018 12:27:55 GMT  
		Size: 50.7 MB (50671071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1310601b6139b280f88b623eeaef6873b2ed293d2e09bc94346f6a444ab9973`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 833.2 KB (833166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a715f7dcd6ee641ea9e85cf6349780799f1e5d41a2a378290058db5c5cd28cb9`  
		Last Modified: Sat, 28 Apr 2018 12:28:25 GMT  
		Size: 164.9 MB (164896280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4e27b5b65dc6b6f87f9c3ae1918a2f334a2f06d1f6ef92a7cfcbabf5871c03`  
		Last Modified: Sat, 28 Apr 2018 12:27:37 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af540861d5e6d956c803433ef96efdb49e6b8d0585b05bc5a5fa810807687f22`  
		Last Modified: Sat, 28 Apr 2018 12:29:03 GMT  
		Size: 75.1 MB (75090166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd65ecc77f71757905503ccfcd7f8c02bfdf34adb53dc0877a39a234f1124a70`  
		Last Modified: Sat, 28 Apr 2018 12:30:03 GMT  
		Size: 90.0 MB (90017669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4ab543ea35ef8d478988773fe3a0e9a81d5fb101e20977a6130afbf1b1ca1d9c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.9 MB (441920257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0fc39746fa0b336c4e2992ee81f6f735469c1004a4f4b6622a163f2c96d9993`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:12:52 GMT
ADD file:fef3655a03a1c7f1533148016797b982955b3d5556f32c777214b8426028509b in / 
# Tue, 01 May 2018 01:12:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:13:04 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:13:10 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:13:20 GMT
CMD ["/bin/bash"]
# Tue, 01 May 2018 01:19:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:19:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 01:19:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 01:23:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:23:33 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 01:23:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 01:24:25 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 01:24:27 GMT
ENV ROS_DISTRO=kinetic
# Tue, 01 May 2018 01:36:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:37:08 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 01:37:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 01:37:33 GMT
CMD ["bash"]
# Tue, 01 May 2018 01:48:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:56:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c016a9a148a71d05469a3994d54eb7eb9c3d40a65e07bf68788018a71d951b`  
		Last Modified: Mon, 23 Apr 2018 14:56:07 GMT  
		Size: 39.2 MB (39223827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1976297de94ed1f5c4c0f13b0b25199c6d6ca003ddfc3e873938aa2f8e86b`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d83417bbef32ed4713f4224bcb9f9573597ee6d91174dc7403ce457f145d2`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2544c5c45beca34c948aca9c981d56b587a973354727e4c97dc99d88227fb6a`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92ef1d410a96b276ec1425b000d80d5c1d914688aae8bce3e6f20d8a5a7a5f`  
		Last Modified: Tue, 01 May 2018 01:17:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3a2ac905d0d30502b9bf9736c755da2e7a05465764ff1fb14a45f067faa71c`  
		Last Modified: Tue, 01 May 2018 04:17:49 GMT  
		Size: 4.8 MB (4819486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31df2d860f2dc7f931faa244a38a740a44c732fd7ab480a29daf8999b5fb7fcd`  
		Last Modified: Tue, 01 May 2018 04:17:40 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a06299e2df93eba22547e7bbfaf291225cb3e1d85dcd160f7080d0d65647a`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ce03745d3f424b139a80266262e70dfefbda981c88ae34eac7b56df3120657`  
		Last Modified: Tue, 01 May 2018 04:18:42 GMT  
		Size: 52.4 MB (52441627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360b2687112930e2c2a443c4f89ecbdda5be0103c5b840e39840d3aca65352a`  
		Last Modified: Tue, 01 May 2018 04:17:41 GMT  
		Size: 835.1 KB (835081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf20cb73de898c810a3ce03d3d4ac43ca405c527b42e21244058ec4bdbf204b`  
		Last Modified: Tue, 01 May 2018 04:19:47 GMT  
		Size: 174.2 MB (174167620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede09c9013f1c95beb0aee3d89bc517d63df382e40d6e2e506b200c897ebc627`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31090de9e5f5a2759e0e667f1d0e72efbb5354d84bd5084b225053079926d2d7`  
		Last Modified: Tue, 01 May 2018 04:20:58 GMT  
		Size: 76.5 MB (76544918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa91dd06c82bffc284c967344bb609d266c569c0b79bae67355033f559ec1c54`  
		Last Modified: Tue, 01 May 2018 04:22:49 GMT  
		Size: 93.9 MB (93871702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-robot-jessie`

```console
$ docker pull ros@sha256:a6b173144606faf8aa7f475ee90cc7c7760426b2582f6327c4485b96507d10f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:kinetic-robot-jessie` - linux; amd64

```console
$ docker pull ros@sha256:f598724fc925646d90866c01d02401c1f5ec015cca1c76d1862019c3c55daaae
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **436.9 MB (436933564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d23e1a232dec16706be35514146058a836f597dde6d531b3b5a7497a79245cba`
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
# Tue, 05 Jun 2018 23:00:01 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:4e39db2b17cd5ec2d221b8b09b55aac1e7997ee388935ad529136f4142e926dd`  
		Last Modified: Wed, 06 Jun 2018 00:20:27 GMT  
		Size: 61.5 MB (61511781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot-jessie` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e6029559ede3a90cf6091f5f0e5d6b176c00e4138e20201db2e9ae07e1a7e441
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.3 MB (384270996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:575980fa886343279bcabb46ec3e135f388fc7cbd7dcb8ff26793a0bf8bbf6cb`
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
# Tue, 01 May 2018 02:38:40 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:ddfde1469dea58d63f670ef36e63b83b5974e5d0b5d51a449962da364d32a33a`  
		Last Modified: Tue, 01 May 2018 04:29:34 GMT  
		Size: 57.4 MB (57382196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-robot-xenial`

```console
$ docker pull ros@sha256:93ff528ca028fbbbecad73f65c9c089c08fcaafb2bc34de368ee640e74164f84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-robot-xenial` - linux; amd64

```console
$ docker pull ros@sha256:7de0e8b7e50972c78db4d562a30a52c36bbbf8b4b6dfff9deb6145953151f33a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.1 MB (486079279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd7fc7c1c617f7d9e63a4af3925cb04ad45728fd626c176190a2f7eedb56d2a1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:52 GMT
ADD file:d37ff24540ea7700d0fc053e1996b234428a88f3a324d7fcbd83d8ef95318040 in / 
# Tue, 05 Jun 2018 21:21:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:54 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:55 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:35:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:35:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:35:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:36:43 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 22:36:43 GMT
ENV ROS_DISTRO=kinetic
# Tue, 05 Jun 2018 22:39:54 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:39:55 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 22:39:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 22:39:56 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 22:42:13 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:45:10 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b234f539f7a1d65eabae1617e63c81ac01768abffd48b5cbbf7166efca6a3429`  
		Last Modified: Mon, 28 May 2018 14:57:20 GMT  
		Size: 43.1 MB (43122477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55172d420b43cf03feeec11bcc917c7ddfc192036102e065ab57aa9abb95311e`  
		Last Modified: Tue, 05 Jun 2018 21:24:52 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba5bbeb6b91e2676c98255c6babc66d7b05cac40185eeba4b3773199c701da0`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ae2841ad7a7fd1aeae30028105cac7f6ee0ec955e5229e52b3333fea3c17b5`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c9c6de41905e9a66f2bc2c4a19858c8dc5b0a94f01e03eafc719afe25888aa`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22c30eae0b9363cecd2e5ac27a92dd1bc354e2e16a3ee82b70932814b4c12a`  
		Last Modified: Wed, 06 Jun 2018 00:11:32 GMT  
		Size: 5.4 MB (5362202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fce58d2960dc3a1265e5bc18474d652795940cafde67d662929605c9e3b1c44`  
		Last Modified: Wed, 06 Jun 2018 00:11:29 GMT  
		Size: 13.1 KB (13081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a8410e99e70f8971b54ce991fecd04014ef363a7dde349dd255d6358a6893d`  
		Last Modified: Wed, 06 Jun 2018 00:11:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3037b7978826369126bbe26cbb5d642f59ccd31d96e28044f872cd3eac55ab`  
		Last Modified: Wed, 06 Jun 2018 00:11:55 GMT  
		Size: 55.6 MB (55571338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cfa8aa4c1f7b161f88b862221bacc540052abfa4f8a11884d0090ebcd55cf9`  
		Last Modified: Wed, 06 Jun 2018 00:11:27 GMT  
		Size: 866.4 KB (866393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16efe7b0a2f0d3cc997ef3ea8c9ed2f3a888fbba64f18ae15c76824cc3fb268d`  
		Last Modified: Wed, 06 Jun 2018 00:12:49 GMT  
		Size: 193.6 MB (193645836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4305ed9cccd0e188c6305b22e2947c513b38a205a8c2fa4ab93825b1ab5d3873`  
		Last Modified: Wed, 06 Jun 2018 00:11:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cce0e73a68108059c9c4433d0c94134a0326a293063d40ac9e2106b50b0b18`  
		Last Modified: Wed, 06 Jun 2018 00:13:42 GMT  
		Size: 83.9 MB (83908652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4567c5bb30132628370213c4a90199c467537c4ba627b16f7df6268b75c20b9d`  
		Last Modified: Wed, 06 Jun 2018 00:14:53 GMT  
		Size: 103.6 MB (103586391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:b290fc09f313cdbddd5ff0676eee22a455c2be81edaab85f1888f6df6f400716
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.3 MB (424265942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f8bb432561fb6800361614853012463ff48a4e04c28b4cae78f897d8371bb0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:05:33 GMT
ADD file:1e3efdebaf133af6b22e61da056500ff8cf5292f051296f69abd35f44da5625c in / 
# Sat, 28 Apr 2018 12:05:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:05:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:05:37 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:05:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:50 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 12:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:08:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 12:08:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 12:09:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 12:09:57 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 12:09:58 GMT
ENV ROS_DISTRO=kinetic
# Sat, 28 Apr 2018 12:11:17 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:11:18 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 12:11:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 12:11:19 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 12:12:30 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:13:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f68dc00194f474ccfe395953a935f0a65f37edc5e218b6f310f432b3866f9bac`  
		Last Modified: Sat, 28 Apr 2018 12:09:03 GMT  
		Size: 38.1 MB (38126697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281b914f46e3b5e9fac0f9436525399186a66cb5abb5403eed9940d4207e15b4`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b205ebc944011540b5d7c371fe39a5cb49890d018253fcd39db61040dfed3`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418c61fca2a7e383833d9b12bd7adf62e311bf6350037e68503fbbbdfb8cc2b`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b471dd10511e8664a33e00815086f40bdfd8c30a16f93b190084bb5bb8a993f`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5050587be2fd4accc805402daed25e9344bd052ced481a6ecd1a5754102cb84`  
		Last Modified: Sat, 28 Apr 2018 12:27:40 GMT  
		Size: 4.6 MB (4614906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334ce8d248512220d545aecf150f8b8172bbd3e4c62f9cdc4c1e814053440912`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d06c2ef1c00b3cb66443790e82ae98882427dfc78b0009b2b801bdd0387146`  
		Last Modified: Sat, 28 Apr 2018 12:27:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b97dba49af961b21651a5255033ef01a2c0100029e05207d73befd0c45f6d85`  
		Last Modified: Sat, 28 Apr 2018 12:27:55 GMT  
		Size: 50.7 MB (50671071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1310601b6139b280f88b623eeaef6873b2ed293d2e09bc94346f6a444ab9973`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 833.2 KB (833166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a715f7dcd6ee641ea9e85cf6349780799f1e5d41a2a378290058db5c5cd28cb9`  
		Last Modified: Sat, 28 Apr 2018 12:28:25 GMT  
		Size: 164.9 MB (164896280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4e27b5b65dc6b6f87f9c3ae1918a2f334a2f06d1f6ef92a7cfcbabf5871c03`  
		Last Modified: Sat, 28 Apr 2018 12:27:37 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af540861d5e6d956c803433ef96efdb49e6b8d0585b05bc5a5fa810807687f22`  
		Last Modified: Sat, 28 Apr 2018 12:29:03 GMT  
		Size: 75.1 MB (75090166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd65ecc77f71757905503ccfcd7f8c02bfdf34adb53dc0877a39a234f1124a70`  
		Last Modified: Sat, 28 Apr 2018 12:30:03 GMT  
		Size: 90.0 MB (90017669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-robot-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4ab543ea35ef8d478988773fe3a0e9a81d5fb101e20977a6130afbf1b1ca1d9c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.9 MB (441920257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0fc39746fa0b336c4e2992ee81f6f735469c1004a4f4b6622a163f2c96d9993`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:12:52 GMT
ADD file:fef3655a03a1c7f1533148016797b982955b3d5556f32c777214b8426028509b in / 
# Tue, 01 May 2018 01:12:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:13:04 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:13:10 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:13:20 GMT
CMD ["/bin/bash"]
# Tue, 01 May 2018 01:19:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:19:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 01:19:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 01:23:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:23:33 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 01:23:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 01:24:25 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 01:24:27 GMT
ENV ROS_DISTRO=kinetic
# Tue, 01 May 2018 01:36:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:37:08 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 01:37:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 01:37:33 GMT
CMD ["bash"]
# Tue, 01 May 2018 01:48:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:56:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c016a9a148a71d05469a3994d54eb7eb9c3d40a65e07bf68788018a71d951b`  
		Last Modified: Mon, 23 Apr 2018 14:56:07 GMT  
		Size: 39.2 MB (39223827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1976297de94ed1f5c4c0f13b0b25199c6d6ca003ddfc3e873938aa2f8e86b`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d83417bbef32ed4713f4224bcb9f9573597ee6d91174dc7403ce457f145d2`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2544c5c45beca34c948aca9c981d56b587a973354727e4c97dc99d88227fb6a`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92ef1d410a96b276ec1425b000d80d5c1d914688aae8bce3e6f20d8a5a7a5f`  
		Last Modified: Tue, 01 May 2018 01:17:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3a2ac905d0d30502b9bf9736c755da2e7a05465764ff1fb14a45f067faa71c`  
		Last Modified: Tue, 01 May 2018 04:17:49 GMT  
		Size: 4.8 MB (4819486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31df2d860f2dc7f931faa244a38a740a44c732fd7ab480a29daf8999b5fb7fcd`  
		Last Modified: Tue, 01 May 2018 04:17:40 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a06299e2df93eba22547e7bbfaf291225cb3e1d85dcd160f7080d0d65647a`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ce03745d3f424b139a80266262e70dfefbda981c88ae34eac7b56df3120657`  
		Last Modified: Tue, 01 May 2018 04:18:42 GMT  
		Size: 52.4 MB (52441627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360b2687112930e2c2a443c4f89ecbdda5be0103c5b840e39840d3aca65352a`  
		Last Modified: Tue, 01 May 2018 04:17:41 GMT  
		Size: 835.1 KB (835081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf20cb73de898c810a3ce03d3d4ac43ca405c527b42e21244058ec4bdbf204b`  
		Last Modified: Tue, 01 May 2018 04:19:47 GMT  
		Size: 174.2 MB (174167620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede09c9013f1c95beb0aee3d89bc517d63df382e40d6e2e506b200c897ebc627`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31090de9e5f5a2759e0e667f1d0e72efbb5354d84bd5084b225053079926d2d7`  
		Last Modified: Tue, 01 May 2018 04:20:58 GMT  
		Size: 76.5 MB (76544918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa91dd06c82bffc284c967344bb609d266c569c0b79bae67355033f559ec1c54`  
		Last Modified: Tue, 01 May 2018 04:22:49 GMT  
		Size: 93.9 MB (93871702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-base`

```console
$ docker pull ros@sha256:514dc64b38c39328168451af72407209a0deb168674ffb23bc63ef90f33797ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:a2983a9a10f8d57c674ce7a3a522d52bafadb0916b95f8f64053eae0a0878b09
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **382.5 MB (382492888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c95770be708eaf6d9552544c42ad44df548bbb2995b19d17be5a75cbb9fabf55`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:52 GMT
ADD file:d37ff24540ea7700d0fc053e1996b234428a88f3a324d7fcbd83d8ef95318040 in / 
# Tue, 05 Jun 2018 21:21:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:54 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:55 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:35:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:35:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:35:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:36:43 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 22:36:43 GMT
ENV ROS_DISTRO=kinetic
# Tue, 05 Jun 2018 22:39:54 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:39:55 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 22:39:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 22:39:56 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 22:42:13 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b234f539f7a1d65eabae1617e63c81ac01768abffd48b5cbbf7166efca6a3429`  
		Last Modified: Mon, 28 May 2018 14:57:20 GMT  
		Size: 43.1 MB (43122477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55172d420b43cf03feeec11bcc917c7ddfc192036102e065ab57aa9abb95311e`  
		Last Modified: Tue, 05 Jun 2018 21:24:52 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba5bbeb6b91e2676c98255c6babc66d7b05cac40185eeba4b3773199c701da0`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ae2841ad7a7fd1aeae30028105cac7f6ee0ec955e5229e52b3333fea3c17b5`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c9c6de41905e9a66f2bc2c4a19858c8dc5b0a94f01e03eafc719afe25888aa`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22c30eae0b9363cecd2e5ac27a92dd1bc354e2e16a3ee82b70932814b4c12a`  
		Last Modified: Wed, 06 Jun 2018 00:11:32 GMT  
		Size: 5.4 MB (5362202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fce58d2960dc3a1265e5bc18474d652795940cafde67d662929605c9e3b1c44`  
		Last Modified: Wed, 06 Jun 2018 00:11:29 GMT  
		Size: 13.1 KB (13081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a8410e99e70f8971b54ce991fecd04014ef363a7dde349dd255d6358a6893d`  
		Last Modified: Wed, 06 Jun 2018 00:11:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3037b7978826369126bbe26cbb5d642f59ccd31d96e28044f872cd3eac55ab`  
		Last Modified: Wed, 06 Jun 2018 00:11:55 GMT  
		Size: 55.6 MB (55571338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cfa8aa4c1f7b161f88b862221bacc540052abfa4f8a11884d0090ebcd55cf9`  
		Last Modified: Wed, 06 Jun 2018 00:11:27 GMT  
		Size: 866.4 KB (866393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16efe7b0a2f0d3cc997ef3ea8c9ed2f3a888fbba64f18ae15c76824cc3fb268d`  
		Last Modified: Wed, 06 Jun 2018 00:12:49 GMT  
		Size: 193.6 MB (193645836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4305ed9cccd0e188c6305b22e2947c513b38a205a8c2fa4ab93825b1ab5d3873`  
		Last Modified: Wed, 06 Jun 2018 00:11:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cce0e73a68108059c9c4433d0c94134a0326a293063d40ac9e2106b50b0b18`  
		Last Modified: Wed, 06 Jun 2018 00:13:42 GMT  
		Size: 83.9 MB (83908652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:354195f78c404ff1fa6cae0f5970cf95e49dfb2879055aeeebd14bd4d2ca3232
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.2 MB (334248273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1b693d5d950e5bec2c9bc8928434570a2e2c180e7306444f9e5ac0cf0be8352`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:05:33 GMT
ADD file:1e3efdebaf133af6b22e61da056500ff8cf5292f051296f69abd35f44da5625c in / 
# Sat, 28 Apr 2018 12:05:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:05:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:05:37 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:05:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:50 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 12:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:08:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 12:08:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 12:09:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 12:09:57 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 12:09:58 GMT
ENV ROS_DISTRO=kinetic
# Sat, 28 Apr 2018 12:11:17 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:11:18 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 12:11:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 12:11:19 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 12:12:30 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f68dc00194f474ccfe395953a935f0a65f37edc5e218b6f310f432b3866f9bac`  
		Last Modified: Sat, 28 Apr 2018 12:09:03 GMT  
		Size: 38.1 MB (38126697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281b914f46e3b5e9fac0f9436525399186a66cb5abb5403eed9940d4207e15b4`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b205ebc944011540b5d7c371fe39a5cb49890d018253fcd39db61040dfed3`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418c61fca2a7e383833d9b12bd7adf62e311bf6350037e68503fbbbdfb8cc2b`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b471dd10511e8664a33e00815086f40bdfd8c30a16f93b190084bb5bb8a993f`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5050587be2fd4accc805402daed25e9344bd052ced481a6ecd1a5754102cb84`  
		Last Modified: Sat, 28 Apr 2018 12:27:40 GMT  
		Size: 4.6 MB (4614906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334ce8d248512220d545aecf150f8b8172bbd3e4c62f9cdc4c1e814053440912`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d06c2ef1c00b3cb66443790e82ae98882427dfc78b0009b2b801bdd0387146`  
		Last Modified: Sat, 28 Apr 2018 12:27:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b97dba49af961b21651a5255033ef01a2c0100029e05207d73befd0c45f6d85`  
		Last Modified: Sat, 28 Apr 2018 12:27:55 GMT  
		Size: 50.7 MB (50671071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1310601b6139b280f88b623eeaef6873b2ed293d2e09bc94346f6a444ab9973`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 833.2 KB (833166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a715f7dcd6ee641ea9e85cf6349780799f1e5d41a2a378290058db5c5cd28cb9`  
		Last Modified: Sat, 28 Apr 2018 12:28:25 GMT  
		Size: 164.9 MB (164896280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4e27b5b65dc6b6f87f9c3ae1918a2f334a2f06d1f6ef92a7cfcbabf5871c03`  
		Last Modified: Sat, 28 Apr 2018 12:27:37 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af540861d5e6d956c803433ef96efdb49e6b8d0585b05bc5a5fa810807687f22`  
		Last Modified: Sat, 28 Apr 2018 12:29:03 GMT  
		Size: 75.1 MB (75090166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:89c95b9f4fac10565324dc86c8386555a757b1cd15cc3c33a345b946b3592dc9
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.0 MB (348048555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab8e7598dc15d5e6be4962d16faeeb44bb7d27153a3744202cf92b978b8bf1b1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:12:52 GMT
ADD file:fef3655a03a1c7f1533148016797b982955b3d5556f32c777214b8426028509b in / 
# Tue, 01 May 2018 01:12:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:13:04 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:13:10 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:13:20 GMT
CMD ["/bin/bash"]
# Tue, 01 May 2018 01:19:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:19:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 01:19:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 01:23:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:23:33 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 01:23:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 01:24:25 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 01:24:27 GMT
ENV ROS_DISTRO=kinetic
# Tue, 01 May 2018 01:36:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:37:08 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 01:37:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 01:37:33 GMT
CMD ["bash"]
# Tue, 01 May 2018 01:48:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c016a9a148a71d05469a3994d54eb7eb9c3d40a65e07bf68788018a71d951b`  
		Last Modified: Mon, 23 Apr 2018 14:56:07 GMT  
		Size: 39.2 MB (39223827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1976297de94ed1f5c4c0f13b0b25199c6d6ca003ddfc3e873938aa2f8e86b`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d83417bbef32ed4713f4224bcb9f9573597ee6d91174dc7403ce457f145d2`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2544c5c45beca34c948aca9c981d56b587a973354727e4c97dc99d88227fb6a`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92ef1d410a96b276ec1425b000d80d5c1d914688aae8bce3e6f20d8a5a7a5f`  
		Last Modified: Tue, 01 May 2018 01:17:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3a2ac905d0d30502b9bf9736c755da2e7a05465764ff1fb14a45f067faa71c`  
		Last Modified: Tue, 01 May 2018 04:17:49 GMT  
		Size: 4.8 MB (4819486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31df2d860f2dc7f931faa244a38a740a44c732fd7ab480a29daf8999b5fb7fcd`  
		Last Modified: Tue, 01 May 2018 04:17:40 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a06299e2df93eba22547e7bbfaf291225cb3e1d85dcd160f7080d0d65647a`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ce03745d3f424b139a80266262e70dfefbda981c88ae34eac7b56df3120657`  
		Last Modified: Tue, 01 May 2018 04:18:42 GMT  
		Size: 52.4 MB (52441627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360b2687112930e2c2a443c4f89ecbdda5be0103c5b840e39840d3aca65352a`  
		Last Modified: Tue, 01 May 2018 04:17:41 GMT  
		Size: 835.1 KB (835081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf20cb73de898c810a3ce03d3d4ac43ca405c527b42e21244058ec4bdbf204b`  
		Last Modified: Tue, 01 May 2018 04:19:47 GMT  
		Size: 174.2 MB (174167620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede09c9013f1c95beb0aee3d89bc517d63df382e40d6e2e506b200c897ebc627`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31090de9e5f5a2759e0e667f1d0e72efbb5354d84bd5084b225053079926d2d7`  
		Last Modified: Tue, 01 May 2018 04:20:58 GMT  
		Size: 76.5 MB (76544918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `ros:kinetic-ros-base-xenial`

```console
$ docker pull ros@sha256:514dc64b38c39328168451af72407209a0deb168674ffb23bc63ef90f33797ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-base-xenial` - linux; amd64

```console
$ docker pull ros@sha256:a2983a9a10f8d57c674ce7a3a522d52bafadb0916b95f8f64053eae0a0878b09
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **382.5 MB (382492888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c95770be708eaf6d9552544c42ad44df548bbb2995b19d17be5a75cbb9fabf55`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:52 GMT
ADD file:d37ff24540ea7700d0fc053e1996b234428a88f3a324d7fcbd83d8ef95318040 in / 
# Tue, 05 Jun 2018 21:21:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:54 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:55 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:35:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:35:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:35:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:36:43 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 22:36:43 GMT
ENV ROS_DISTRO=kinetic
# Tue, 05 Jun 2018 22:39:54 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:39:55 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 22:39:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 22:39:56 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 22:42:13 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b234f539f7a1d65eabae1617e63c81ac01768abffd48b5cbbf7166efca6a3429`  
		Last Modified: Mon, 28 May 2018 14:57:20 GMT  
		Size: 43.1 MB (43122477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55172d420b43cf03feeec11bcc917c7ddfc192036102e065ab57aa9abb95311e`  
		Last Modified: Tue, 05 Jun 2018 21:24:52 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba5bbeb6b91e2676c98255c6babc66d7b05cac40185eeba4b3773199c701da0`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ae2841ad7a7fd1aeae30028105cac7f6ee0ec955e5229e52b3333fea3c17b5`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c9c6de41905e9a66f2bc2c4a19858c8dc5b0a94f01e03eafc719afe25888aa`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22c30eae0b9363cecd2e5ac27a92dd1bc354e2e16a3ee82b70932814b4c12a`  
		Last Modified: Wed, 06 Jun 2018 00:11:32 GMT  
		Size: 5.4 MB (5362202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fce58d2960dc3a1265e5bc18474d652795940cafde67d662929605c9e3b1c44`  
		Last Modified: Wed, 06 Jun 2018 00:11:29 GMT  
		Size: 13.1 KB (13081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a8410e99e70f8971b54ce991fecd04014ef363a7dde349dd255d6358a6893d`  
		Last Modified: Wed, 06 Jun 2018 00:11:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3037b7978826369126bbe26cbb5d642f59ccd31d96e28044f872cd3eac55ab`  
		Last Modified: Wed, 06 Jun 2018 00:11:55 GMT  
		Size: 55.6 MB (55571338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cfa8aa4c1f7b161f88b862221bacc540052abfa4f8a11884d0090ebcd55cf9`  
		Last Modified: Wed, 06 Jun 2018 00:11:27 GMT  
		Size: 866.4 KB (866393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16efe7b0a2f0d3cc997ef3ea8c9ed2f3a888fbba64f18ae15c76824cc3fb268d`  
		Last Modified: Wed, 06 Jun 2018 00:12:49 GMT  
		Size: 193.6 MB (193645836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4305ed9cccd0e188c6305b22e2947c513b38a205a8c2fa4ab93825b1ab5d3873`  
		Last Modified: Wed, 06 Jun 2018 00:11:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cce0e73a68108059c9c4433d0c94134a0326a293063d40ac9e2106b50b0b18`  
		Last Modified: Wed, 06 Jun 2018 00:13:42 GMT  
		Size: 83.9 MB (83908652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:354195f78c404ff1fa6cae0f5970cf95e49dfb2879055aeeebd14bd4d2ca3232
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.2 MB (334248273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1b693d5d950e5bec2c9bc8928434570a2e2c180e7306444f9e5ac0cf0be8352`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:05:33 GMT
ADD file:1e3efdebaf133af6b22e61da056500ff8cf5292f051296f69abd35f44da5625c in / 
# Sat, 28 Apr 2018 12:05:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:05:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:05:37 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:05:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:50 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 12:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:08:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 12:08:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 12:09:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 12:09:57 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 12:09:58 GMT
ENV ROS_DISTRO=kinetic
# Sat, 28 Apr 2018 12:11:17 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:11:18 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 12:11:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 12:11:19 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 12:12:30 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f68dc00194f474ccfe395953a935f0a65f37edc5e218b6f310f432b3866f9bac`  
		Last Modified: Sat, 28 Apr 2018 12:09:03 GMT  
		Size: 38.1 MB (38126697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281b914f46e3b5e9fac0f9436525399186a66cb5abb5403eed9940d4207e15b4`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b205ebc944011540b5d7c371fe39a5cb49890d018253fcd39db61040dfed3`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418c61fca2a7e383833d9b12bd7adf62e311bf6350037e68503fbbbdfb8cc2b`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b471dd10511e8664a33e00815086f40bdfd8c30a16f93b190084bb5bb8a993f`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5050587be2fd4accc805402daed25e9344bd052ced481a6ecd1a5754102cb84`  
		Last Modified: Sat, 28 Apr 2018 12:27:40 GMT  
		Size: 4.6 MB (4614906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334ce8d248512220d545aecf150f8b8172bbd3e4c62f9cdc4c1e814053440912`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d06c2ef1c00b3cb66443790e82ae98882427dfc78b0009b2b801bdd0387146`  
		Last Modified: Sat, 28 Apr 2018 12:27:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b97dba49af961b21651a5255033ef01a2c0100029e05207d73befd0c45f6d85`  
		Last Modified: Sat, 28 Apr 2018 12:27:55 GMT  
		Size: 50.7 MB (50671071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1310601b6139b280f88b623eeaef6873b2ed293d2e09bc94346f6a444ab9973`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 833.2 KB (833166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a715f7dcd6ee641ea9e85cf6349780799f1e5d41a2a378290058db5c5cd28cb9`  
		Last Modified: Sat, 28 Apr 2018 12:28:25 GMT  
		Size: 164.9 MB (164896280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4e27b5b65dc6b6f87f9c3ae1918a2f334a2f06d1f6ef92a7cfcbabf5871c03`  
		Last Modified: Sat, 28 Apr 2018 12:27:37 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af540861d5e6d956c803433ef96efdb49e6b8d0585b05bc5a5fa810807687f22`  
		Last Modified: Sat, 28 Apr 2018 12:29:03 GMT  
		Size: 75.1 MB (75090166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-base-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:89c95b9f4fac10565324dc86c8386555a757b1cd15cc3c33a345b946b3592dc9
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.0 MB (348048555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab8e7598dc15d5e6be4962d16faeeb44bb7d27153a3744202cf92b978b8bf1b1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:12:52 GMT
ADD file:fef3655a03a1c7f1533148016797b982955b3d5556f32c777214b8426028509b in / 
# Tue, 01 May 2018 01:12:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:13:04 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:13:10 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:13:20 GMT
CMD ["/bin/bash"]
# Tue, 01 May 2018 01:19:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:19:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 01:19:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 01:23:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:23:33 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 01:23:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 01:24:25 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 01:24:27 GMT
ENV ROS_DISTRO=kinetic
# Tue, 01 May 2018 01:36:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:37:08 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 01:37:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 01:37:33 GMT
CMD ["bash"]
# Tue, 01 May 2018 01:48:51 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c016a9a148a71d05469a3994d54eb7eb9c3d40a65e07bf68788018a71d951b`  
		Last Modified: Mon, 23 Apr 2018 14:56:07 GMT  
		Size: 39.2 MB (39223827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1976297de94ed1f5c4c0f13b0b25199c6d6ca003ddfc3e873938aa2f8e86b`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d83417bbef32ed4713f4224bcb9f9573597ee6d91174dc7403ce457f145d2`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2544c5c45beca34c948aca9c981d56b587a973354727e4c97dc99d88227fb6a`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92ef1d410a96b276ec1425b000d80d5c1d914688aae8bce3e6f20d8a5a7a5f`  
		Last Modified: Tue, 01 May 2018 01:17:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3a2ac905d0d30502b9bf9736c755da2e7a05465764ff1fb14a45f067faa71c`  
		Last Modified: Tue, 01 May 2018 04:17:49 GMT  
		Size: 4.8 MB (4819486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31df2d860f2dc7f931faa244a38a740a44c732fd7ab480a29daf8999b5fb7fcd`  
		Last Modified: Tue, 01 May 2018 04:17:40 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a06299e2df93eba22547e7bbfaf291225cb3e1d85dcd160f7080d0d65647a`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ce03745d3f424b139a80266262e70dfefbda981c88ae34eac7b56df3120657`  
		Last Modified: Tue, 01 May 2018 04:18:42 GMT  
		Size: 52.4 MB (52441627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360b2687112930e2c2a443c4f89ecbdda5be0103c5b840e39840d3aca65352a`  
		Last Modified: Tue, 01 May 2018 04:17:41 GMT  
		Size: 835.1 KB (835081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf20cb73de898c810a3ce03d3d4ac43ca405c527b42e21244058ec4bdbf204b`  
		Last Modified: Tue, 01 May 2018 04:19:47 GMT  
		Size: 174.2 MB (174167620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede09c9013f1c95beb0aee3d89bc517d63df382e40d6e2e506b200c897ebc627`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31090de9e5f5a2759e0e667f1d0e72efbb5354d84bd5084b225053079926d2d7`  
		Last Modified: Tue, 01 May 2018 04:20:58 GMT  
		Size: 76.5 MB (76544918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-core`

```console
$ docker pull ros@sha256:e98a0d9080747dfdd6e67142c532f823ec7039787e20df3dda8458e0af58b865
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:3d73b80e1ce481e56a1ae2a8722acc94b032ff34eff9ab01faa7711b9a6a095c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298584236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0840dad96a1709dfbbbe7d0c478910a01994f783ba310d10c7edc0a9679ae296`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:52 GMT
ADD file:d37ff24540ea7700d0fc053e1996b234428a88f3a324d7fcbd83d8ef95318040 in / 
# Tue, 05 Jun 2018 21:21:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:54 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:55 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:35:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:35:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:35:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:36:43 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 22:36:43 GMT
ENV ROS_DISTRO=kinetic
# Tue, 05 Jun 2018 22:39:54 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:39:55 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 22:39:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 22:39:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b234f539f7a1d65eabae1617e63c81ac01768abffd48b5cbbf7166efca6a3429`  
		Last Modified: Mon, 28 May 2018 14:57:20 GMT  
		Size: 43.1 MB (43122477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55172d420b43cf03feeec11bcc917c7ddfc192036102e065ab57aa9abb95311e`  
		Last Modified: Tue, 05 Jun 2018 21:24:52 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba5bbeb6b91e2676c98255c6babc66d7b05cac40185eeba4b3773199c701da0`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ae2841ad7a7fd1aeae30028105cac7f6ee0ec955e5229e52b3333fea3c17b5`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c9c6de41905e9a66f2bc2c4a19858c8dc5b0a94f01e03eafc719afe25888aa`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22c30eae0b9363cecd2e5ac27a92dd1bc354e2e16a3ee82b70932814b4c12a`  
		Last Modified: Wed, 06 Jun 2018 00:11:32 GMT  
		Size: 5.4 MB (5362202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fce58d2960dc3a1265e5bc18474d652795940cafde67d662929605c9e3b1c44`  
		Last Modified: Wed, 06 Jun 2018 00:11:29 GMT  
		Size: 13.1 KB (13081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a8410e99e70f8971b54ce991fecd04014ef363a7dde349dd255d6358a6893d`  
		Last Modified: Wed, 06 Jun 2018 00:11:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3037b7978826369126bbe26cbb5d642f59ccd31d96e28044f872cd3eac55ab`  
		Last Modified: Wed, 06 Jun 2018 00:11:55 GMT  
		Size: 55.6 MB (55571338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cfa8aa4c1f7b161f88b862221bacc540052abfa4f8a11884d0090ebcd55cf9`  
		Last Modified: Wed, 06 Jun 2018 00:11:27 GMT  
		Size: 866.4 KB (866393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16efe7b0a2f0d3cc997ef3ea8c9ed2f3a888fbba64f18ae15c76824cc3fb268d`  
		Last Modified: Wed, 06 Jun 2018 00:12:49 GMT  
		Size: 193.6 MB (193645836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4305ed9cccd0e188c6305b22e2947c513b38a205a8c2fa4ab93825b1ab5d3873`  
		Last Modified: Wed, 06 Jun 2018 00:11:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:e86ab4b2f7f7378b581b999d35444718336159fd41cf756114d44353d800666a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.2 MB (259158107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fe3f27b5794dbb5f454eefaa6d922552d0a302fde9100e0af40bdb0aaa96836`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:05:33 GMT
ADD file:1e3efdebaf133af6b22e61da056500ff8cf5292f051296f69abd35f44da5625c in / 
# Sat, 28 Apr 2018 12:05:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:05:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:05:37 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:05:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:50 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 12:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:08:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 12:08:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 12:09:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 12:09:57 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 12:09:58 GMT
ENV ROS_DISTRO=kinetic
# Sat, 28 Apr 2018 12:11:17 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:11:18 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 12:11:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 12:11:19 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f68dc00194f474ccfe395953a935f0a65f37edc5e218b6f310f432b3866f9bac`  
		Last Modified: Sat, 28 Apr 2018 12:09:03 GMT  
		Size: 38.1 MB (38126697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281b914f46e3b5e9fac0f9436525399186a66cb5abb5403eed9940d4207e15b4`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b205ebc944011540b5d7c371fe39a5cb49890d018253fcd39db61040dfed3`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418c61fca2a7e383833d9b12bd7adf62e311bf6350037e68503fbbbdfb8cc2b`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b471dd10511e8664a33e00815086f40bdfd8c30a16f93b190084bb5bb8a993f`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5050587be2fd4accc805402daed25e9344bd052ced481a6ecd1a5754102cb84`  
		Last Modified: Sat, 28 Apr 2018 12:27:40 GMT  
		Size: 4.6 MB (4614906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334ce8d248512220d545aecf150f8b8172bbd3e4c62f9cdc4c1e814053440912`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d06c2ef1c00b3cb66443790e82ae98882427dfc78b0009b2b801bdd0387146`  
		Last Modified: Sat, 28 Apr 2018 12:27:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b97dba49af961b21651a5255033ef01a2c0100029e05207d73befd0c45f6d85`  
		Last Modified: Sat, 28 Apr 2018 12:27:55 GMT  
		Size: 50.7 MB (50671071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1310601b6139b280f88b623eeaef6873b2ed293d2e09bc94346f6a444ab9973`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 833.2 KB (833166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a715f7dcd6ee641ea9e85cf6349780799f1e5d41a2a378290058db5c5cd28cb9`  
		Last Modified: Sat, 28 Apr 2018 12:28:25 GMT  
		Size: 164.9 MB (164896280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4e27b5b65dc6b6f87f9c3ae1918a2f334a2f06d1f6ef92a7cfcbabf5871c03`  
		Last Modified: Sat, 28 Apr 2018 12:27:37 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0652ecdf8815c70f36813883b78db8cbaf47231575736f7c9bf93b0754b342b6
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.5 MB (271503637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4480a36445fbfe35a16b5f976d5fc00c07542b0890ada0554e2304e0f96492a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:12:52 GMT
ADD file:fef3655a03a1c7f1533148016797b982955b3d5556f32c777214b8426028509b in / 
# Tue, 01 May 2018 01:12:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:13:04 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:13:10 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:13:20 GMT
CMD ["/bin/bash"]
# Tue, 01 May 2018 01:19:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:19:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 01:19:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 01:23:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:23:33 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 01:23:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 01:24:25 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 01:24:27 GMT
ENV ROS_DISTRO=kinetic
# Tue, 01 May 2018 01:36:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:37:08 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 01:37:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 01:37:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:83c016a9a148a71d05469a3994d54eb7eb9c3d40a65e07bf68788018a71d951b`  
		Last Modified: Mon, 23 Apr 2018 14:56:07 GMT  
		Size: 39.2 MB (39223827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1976297de94ed1f5c4c0f13b0b25199c6d6ca003ddfc3e873938aa2f8e86b`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d83417bbef32ed4713f4224bcb9f9573597ee6d91174dc7403ce457f145d2`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2544c5c45beca34c948aca9c981d56b587a973354727e4c97dc99d88227fb6a`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92ef1d410a96b276ec1425b000d80d5c1d914688aae8bce3e6f20d8a5a7a5f`  
		Last Modified: Tue, 01 May 2018 01:17:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3a2ac905d0d30502b9bf9736c755da2e7a05465764ff1fb14a45f067faa71c`  
		Last Modified: Tue, 01 May 2018 04:17:49 GMT  
		Size: 4.8 MB (4819486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31df2d860f2dc7f931faa244a38a740a44c732fd7ab480a29daf8999b5fb7fcd`  
		Last Modified: Tue, 01 May 2018 04:17:40 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a06299e2df93eba22547e7bbfaf291225cb3e1d85dcd160f7080d0d65647a`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ce03745d3f424b139a80266262e70dfefbda981c88ae34eac7b56df3120657`  
		Last Modified: Tue, 01 May 2018 04:18:42 GMT  
		Size: 52.4 MB (52441627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360b2687112930e2c2a443c4f89ecbdda5be0103c5b840e39840d3aca65352a`  
		Last Modified: Tue, 01 May 2018 04:17:41 GMT  
		Size: 835.1 KB (835081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf20cb73de898c810a3ce03d3d4ac43ca405c527b42e21244058ec4bdbf204b`  
		Last Modified: Tue, 01 May 2018 04:19:47 GMT  
		Size: 174.2 MB (174167620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede09c9013f1c95beb0aee3d89bc517d63df382e40d6e2e506b200c897ebc627`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-core-jessie`

```console
$ docker pull ros@sha256:b3c5cec29d7fea5a4887e32bae9ec5dde200a47ba1a634b72d37bc3eab11833f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core-jessie` - linux; amd64

```console
$ docker pull ros@sha256:051339f475727546f747e20eb35f26fb6cae42f902c4480360caf9d1c31818f9
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.2 MB (291211683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b195d928adb0f15bcf1ba9f004de4696b14ca4b0ec752a7deaf676128725724d`
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

### `ros:kinetic-ros-core-jessie` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:654c526bac7f2cf6c5dd14b04d0b7794260864aaa5a9b30bf2f7ec229ee7fa09
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.8 MB (257845683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c1f0bd372d819b12ab182fc642e444bdf014c88ada5218dde83167dd5fc5d2f`
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

## `ros:kinetic-ros-core-xenial`

```console
$ docker pull ros@sha256:e98a0d9080747dfdd6e67142c532f823ec7039787e20df3dda8458e0af58b865
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:kinetic-ros-core-xenial` - linux; amd64

```console
$ docker pull ros@sha256:3d73b80e1ce481e56a1ae2a8722acc94b032ff34eff9ab01faa7711b9a6a095c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298584236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0840dad96a1709dfbbbe7d0c478910a01994f783ba310d10c7edc0a9679ae296`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:52 GMT
ADD file:d37ff24540ea7700d0fc053e1996b234428a88f3a324d7fcbd83d8ef95318040 in / 
# Tue, 05 Jun 2018 21:21:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:54 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:55 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:35:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:35:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:35:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:36:43 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 22:36:43 GMT
ENV ROS_DISTRO=kinetic
# Tue, 05 Jun 2018 22:39:54 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:39:55 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 22:39:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 22:39:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b234f539f7a1d65eabae1617e63c81ac01768abffd48b5cbbf7166efca6a3429`  
		Last Modified: Mon, 28 May 2018 14:57:20 GMT  
		Size: 43.1 MB (43122477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55172d420b43cf03feeec11bcc917c7ddfc192036102e065ab57aa9abb95311e`  
		Last Modified: Tue, 05 Jun 2018 21:24:52 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba5bbeb6b91e2676c98255c6babc66d7b05cac40185eeba4b3773199c701da0`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ae2841ad7a7fd1aeae30028105cac7f6ee0ec955e5229e52b3333fea3c17b5`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c9c6de41905e9a66f2bc2c4a19858c8dc5b0a94f01e03eafc719afe25888aa`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22c30eae0b9363cecd2e5ac27a92dd1bc354e2e16a3ee82b70932814b4c12a`  
		Last Modified: Wed, 06 Jun 2018 00:11:32 GMT  
		Size: 5.4 MB (5362202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fce58d2960dc3a1265e5bc18474d652795940cafde67d662929605c9e3b1c44`  
		Last Modified: Wed, 06 Jun 2018 00:11:29 GMT  
		Size: 13.1 KB (13081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a8410e99e70f8971b54ce991fecd04014ef363a7dde349dd255d6358a6893d`  
		Last Modified: Wed, 06 Jun 2018 00:11:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3037b7978826369126bbe26cbb5d642f59ccd31d96e28044f872cd3eac55ab`  
		Last Modified: Wed, 06 Jun 2018 00:11:55 GMT  
		Size: 55.6 MB (55571338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cfa8aa4c1f7b161f88b862221bacc540052abfa4f8a11884d0090ebcd55cf9`  
		Last Modified: Wed, 06 Jun 2018 00:11:27 GMT  
		Size: 866.4 KB (866393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16efe7b0a2f0d3cc997ef3ea8c9ed2f3a888fbba64f18ae15c76824cc3fb268d`  
		Last Modified: Wed, 06 Jun 2018 00:12:49 GMT  
		Size: 193.6 MB (193645836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4305ed9cccd0e188c6305b22e2947c513b38a205a8c2fa4ab93825b1ab5d3873`  
		Last Modified: Wed, 06 Jun 2018 00:11:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:e86ab4b2f7f7378b581b999d35444718336159fd41cf756114d44353d800666a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.2 MB (259158107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fe3f27b5794dbb5f454eefaa6d922552d0a302fde9100e0af40bdb0aaa96836`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:05:33 GMT
ADD file:1e3efdebaf133af6b22e61da056500ff8cf5292f051296f69abd35f44da5625c in / 
# Sat, 28 Apr 2018 12:05:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:05:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:05:37 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:05:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:50 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 12:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:08:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 12:08:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 12:09:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 12:09:57 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 12:09:58 GMT
ENV ROS_DISTRO=kinetic
# Sat, 28 Apr 2018 12:11:17 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:11:18 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 12:11:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 12:11:19 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f68dc00194f474ccfe395953a935f0a65f37edc5e218b6f310f432b3866f9bac`  
		Last Modified: Sat, 28 Apr 2018 12:09:03 GMT  
		Size: 38.1 MB (38126697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281b914f46e3b5e9fac0f9436525399186a66cb5abb5403eed9940d4207e15b4`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b205ebc944011540b5d7c371fe39a5cb49890d018253fcd39db61040dfed3`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418c61fca2a7e383833d9b12bd7adf62e311bf6350037e68503fbbbdfb8cc2b`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b471dd10511e8664a33e00815086f40bdfd8c30a16f93b190084bb5bb8a993f`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5050587be2fd4accc805402daed25e9344bd052ced481a6ecd1a5754102cb84`  
		Last Modified: Sat, 28 Apr 2018 12:27:40 GMT  
		Size: 4.6 MB (4614906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334ce8d248512220d545aecf150f8b8172bbd3e4c62f9cdc4c1e814053440912`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d06c2ef1c00b3cb66443790e82ae98882427dfc78b0009b2b801bdd0387146`  
		Last Modified: Sat, 28 Apr 2018 12:27:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b97dba49af961b21651a5255033ef01a2c0100029e05207d73befd0c45f6d85`  
		Last Modified: Sat, 28 Apr 2018 12:27:55 GMT  
		Size: 50.7 MB (50671071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1310601b6139b280f88b623eeaef6873b2ed293d2e09bc94346f6a444ab9973`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 833.2 KB (833166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a715f7dcd6ee641ea9e85cf6349780799f1e5d41a2a378290058db5c5cd28cb9`  
		Last Modified: Sat, 28 Apr 2018 12:28:25 GMT  
		Size: 164.9 MB (164896280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4e27b5b65dc6b6f87f9c3ae1918a2f334a2f06d1f6ef92a7cfcbabf5871c03`  
		Last Modified: Sat, 28 Apr 2018 12:27:37 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:kinetic-ros-core-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0652ecdf8815c70f36813883b78db8cbaf47231575736f7c9bf93b0754b342b6
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.5 MB (271503637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4480a36445fbfe35a16b5f976d5fc00c07542b0890ada0554e2304e0f96492a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:12:52 GMT
ADD file:fef3655a03a1c7f1533148016797b982955b3d5556f32c777214b8426028509b in / 
# Tue, 01 May 2018 01:12:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:13:04 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:13:10 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:13:20 GMT
CMD ["/bin/bash"]
# Tue, 01 May 2018 01:19:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:19:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 01:19:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 01:23:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:23:33 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 01:23:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 01:24:25 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 01:24:27 GMT
ENV ROS_DISTRO=kinetic
# Tue, 01 May 2018 01:36:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:37:08 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 01:37:16 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 01:37:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:83c016a9a148a71d05469a3994d54eb7eb9c3d40a65e07bf68788018a71d951b`  
		Last Modified: Mon, 23 Apr 2018 14:56:07 GMT  
		Size: 39.2 MB (39223827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1976297de94ed1f5c4c0f13b0b25199c6d6ca003ddfc3e873938aa2f8e86b`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d83417bbef32ed4713f4224bcb9f9573597ee6d91174dc7403ce457f145d2`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2544c5c45beca34c948aca9c981d56b587a973354727e4c97dc99d88227fb6a`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92ef1d410a96b276ec1425b000d80d5c1d914688aae8bce3e6f20d8a5a7a5f`  
		Last Modified: Tue, 01 May 2018 01:17:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3a2ac905d0d30502b9bf9736c755da2e7a05465764ff1fb14a45f067faa71c`  
		Last Modified: Tue, 01 May 2018 04:17:49 GMT  
		Size: 4.8 MB (4819486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31df2d860f2dc7f931faa244a38a740a44c732fd7ab480a29daf8999b5fb7fcd`  
		Last Modified: Tue, 01 May 2018 04:17:40 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a06299e2df93eba22547e7bbfaf291225cb3e1d85dcd160f7080d0d65647a`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ce03745d3f424b139a80266262e70dfefbda981c88ae34eac7b56df3120657`  
		Last Modified: Tue, 01 May 2018 04:18:42 GMT  
		Size: 52.4 MB (52441627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360b2687112930e2c2a443c4f89ecbdda5be0103c5b840e39840d3aca65352a`  
		Last Modified: Tue, 01 May 2018 04:17:41 GMT  
		Size: 835.1 KB (835081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf20cb73de898c810a3ce03d3d4ac43ca405c527b42e21244058ec4bdbf204b`  
		Last Modified: Tue, 01 May 2018 04:19:47 GMT  
		Size: 174.2 MB (174167620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede09c9013f1c95beb0aee3d89bc517d63df382e40d6e2e506b200c897ebc627`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:65fa1c573112741d9bf457a4c01de50f383ce57281f3d196e79a02e7cba3e354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:latest` - linux; amd64

```console
$ docker pull ros@sha256:6cb9d04fe705668a8939f8d24b67370ec79cba45750cff9a3b4ac549dcf8c592
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **379.8 MB (379836490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8141688e843965dabe1111f59e049862a0c270b10da0cc85efa9beff999898f3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 27 Apr 2018 23:28:32 GMT
ADD file:81813d6023adb66b80fe163bc7db464004673838d17195b9d84aade4f8961b71 in / 
# Fri, 27 Apr 2018 23:28:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 27 Apr 2018 23:28:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 27 Apr 2018 23:28:35 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 27 Apr 2018 23:28:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 27 Apr 2018 23:28:36 GMT
CMD ["/bin/bash"]
# Tue, 15 May 2018 17:22:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 15 May 2018 17:22:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 15 May 2018 17:24:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:24:08 GMT
ENV LANG=C.UTF-8
# Tue, 15 May 2018 17:24:09 GMT
ENV LC_ALL=C.UTF-8
# Tue, 15 May 2018 17:24:19 GMT
RUN rosdep init     && rosdep update
# Tue, 15 May 2018 17:24:19 GMT
ENV ROS_DISTRO=melodic
# Thu, 24 May 2018 21:26:28 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:26:29 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Thu, 24 May 2018 21:26:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 24 May 2018 21:26:29 GMT
CMD ["bash"]
# Thu, 24 May 2018 21:29:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a48c500ed24e62926cb079df35f964c57d8bb08159b1d29c6a3b0a58dc365dc1`  
		Last Modified: Fri, 27 Apr 2018 22:14:33 GMT  
		Size: 31.0 MB (30957448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1de00ff7e1fea0858b6a4b5ca208eeca970607ea9a6eb5fc972494e7a0cdde`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0330ca45a200e1fcef05ae97f434366d262a1c50b3dc053e7928b58dd37211dd`  
		Last Modified: Fri, 27 Apr 2018 23:32:05 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471db38bcfbf0f5bac78012b9d458dfd37309d5cbb99d4e95310321a60a0cfdf`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4aba487617ca27519745ae722b8ea1917474c495b91b3c4887728a3f2ee7db`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8456edf85c693828820f7381dde166ac747f2cd8e10610d4c51120bc668379f`  
		Last Modified: Tue, 15 May 2018 18:06:38 GMT  
		Size: 831.1 KB (831054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2122c178c47e334cadb90a80317c074c9ab5b4ad3c03bd385e7b1cd3e348aa`  
		Last Modified: Tue, 15 May 2018 18:06:39 GMT  
		Size: 4.9 MB (4859414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d31beaa42936003685a0b05665d5767eeeddc4c318aaadc6fca1bba5debf2b`  
		Last Modified: Tue, 15 May 2018 18:06:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4b733826c103e038eda6e27b5f02bd3d2399d9c5c0a1af66b687989888289`  
		Last Modified: Tue, 15 May 2018 18:06:33 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c0ecb640b5f315f0d1dfa938e893872008c4f9a375a74e3c04c718e57bf3a5`  
		Last Modified: Tue, 15 May 2018 18:06:53 GMT  
		Size: 58.4 MB (58398228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae98d14520da6037aa61bc4046566731135de07187c4ea0f29030924bdcedb9`  
		Last Modified: Tue, 15 May 2018 18:06:35 GMT  
		Size: 848.9 KB (848891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5010f265d43daa5e2b9fbbbd090b2aa10b524945743a39cfd845a82379bd2f`  
		Last Modified: Thu, 24 May 2018 22:02:00 GMT  
		Size: 215.8 MB (215752594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0876834886b1318e9ec6eea07a901cde589827dacaef6c6179af7bb73bff5ea9`  
		Last Modified: Thu, 24 May 2018 22:01:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f4d2a0227e9474ba6418c71791baf644b56f14e7b6ab2389c7c9b071db5331`  
		Last Modified: Thu, 24 May 2018 22:02:53 GMT  
		Size: 68.2 MB (68184788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm variant v7

```console
$ docker pull ros@sha256:f46872e2c7c6a4cd2d6cf52a79b0ff955df4dc892b30856465400b371df39cd4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.9 MB (333902303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37417f98d377f368a74e8f07277aac34c9f2115dbd17839aed2f3494cdaeece`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:03:57 GMT
ADD file:5b2d516c09b4419925efe09e1b5c861cbd3a2d48ed47d6b2c7e571ec6d9ead64 in / 
# Sat, 28 Apr 2018 12:03:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:03:59 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:04:05 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:04:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:04:18 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 11:58:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 11:58:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 11:59:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:59:16 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 11:59:16 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 11:59:39 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 11:59:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 12:23:42 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 12:23:45 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 12:23:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 12:23:55 GMT
CMD ["bash"]
# Fri, 25 May 2018 12:25:08 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c68b3181adc7da3b2a5c9be4e228fe5b958ebee478e094e17cf4a61c60a75190`  
		Last Modified: Sat, 28 Apr 2018 12:06:55 GMT  
		Size: 26.5 MB (26487045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91be1119609b1847ebcb9f2621129540bc1fb01ca2c914cc9d03985f48513d24`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605e73e7288ab8c0b45ebed929576b45d7e024077e0f2ae8b1bfabc549e22b0f`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843bab014c7a7d380f7e5c7b7c205da6050bb6e3411217ebae052fae49a97708`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebf53478b460975ab3dc0b245e93b5121d21e03232fcef2d94cd838e034c3af`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ad074d342b779241149fc3fd8ca37e75b9985c3c0c75194f0baa6457643bc9`  
		Last Modified: Wed, 16 May 2018 12:07:02 GMT  
		Size: 831.2 KB (831191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2563139b45010cd554b552642217d24a54e56e1348796c0e156c8b1da6cb10`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 4.1 MB (4077205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a670c1a3040793070164343ff80a5fe224179f0542e8caa26ffdd706fc9a8f`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46573ec96640100c935e1de546d8e484aba5795ae4a439d06a5fce5ceb7bab17`  
		Last Modified: Wed, 16 May 2018 12:06:58 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c0d825eae387d208e3db5a3d2c211d2da64e3b8d2dd2eec5c4c4d33531d312`  
		Last Modified: Wed, 16 May 2018 12:07:17 GMT  
		Size: 53.3 MB (53260829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43be66fa479508bd5da868d645d6ac16277dab0c314790a1a45868b46042f4fd`  
		Last Modified: Wed, 16 May 2018 12:06:59 GMT  
		Size: 849.5 KB (849453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b73a800962eaa799f32d90e55a98ff0d75b6ec5f28b22a5e7a230c076eb77c`  
		Last Modified: Fri, 25 May 2018 12:31:35 GMT  
		Size: 188.4 MB (188390821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fff307b7b5e5b8f708310d05f17e3b91e9e87dff16e5e389a8efdf56ecbc62`  
		Last Modified: Fri, 25 May 2018 12:30:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fab2540810360b8fa43551847a14f4816b8a9d4a0e79958f8a8950a0079161`  
		Last Modified: Fri, 25 May 2018 12:32:35 GMT  
		Size: 60.0 MB (60001666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:latest` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:421fe69542b69504d5185c436ab23bece33ea046c086ae3c6a28cd1b1416f87d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.0 MB (356993267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7a933463e40d905ead1f8ad4f817bbcd68225be7dd2476192fff9dc0d4ca2a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:10:30 GMT
ADD file:2738a1f35ded405c55bf8578757cc7a8a559fecd00a693b443369262b6dd3127 in / 
# Tue, 01 May 2018 01:10:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:10:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:11:00 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:11:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:11:09 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 09:17:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 09:18:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 09:20:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:20:22 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 09:20:23 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 09:21:02 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 09:21:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 14:59:45 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 14:59:50 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 14:59:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 14:59:51 GMT
CMD ["bash"]
# Fri, 25 May 2018 15:02:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5b73461db237fc125ed4bbd267b3cd588b6d3957c33cf7fc1d7f9aaf6dcd23fd`  
		Last Modified: Fri, 27 Apr 2018 22:48:27 GMT  
		Size: 27.9 MB (27906574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c642ceb6d4dae80623e35056b3672b999504c5a0cb5dfdd4017f3ff74c6613d8`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6b10168e4f59716c9bf42ae4d202df59f2177923f5e0c6a10228be5c719a2e`  
		Last Modified: Tue, 01 May 2018 01:15:00 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0393063bd61dd94962711e03eb55999a0f821b5939d53509bd5aaf041018dfd`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7da53af2791e4570af9528b9ac2c4487a67026625b4de48184810193f3aa76f`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c156a4d1ad7cd59ce110f77b00214890cbe16b288cc38dfddfe83e9a4cbf4c6`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 831.0 KB (830976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be34a6338091a5e6c7b3336a3410157dd78d861793b54433ff7d219681b4cd95`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 4.4 MB (4438186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17243111bd7f4cc4a686835d4f7d86a2a8a0f4e9cd0db83d23b3b13069bad744`  
		Last Modified: Wed, 16 May 2018 10:26:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e446f86bbda79f1e1d14edd48864be9d560d0705f48166af8f8275833fe37b2e`  
		Last Modified: Wed, 16 May 2018 10:26:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6301719156835f879808d742b36f8b71f5f44741b3081e6516c61a3165608e4`  
		Last Modified: Wed, 16 May 2018 10:26:28 GMT  
		Size: 56.3 MB (56321857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92cb898705c424115a56cd1f955c61c5731211890c95409572b1b64666e60af`  
		Last Modified: Wed, 16 May 2018 10:26:01 GMT  
		Size: 849.4 KB (849389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa2f2edfc54bc83efbb1aecee4ad233c58a7b6f678c0f27f5c95ec2d241795`  
		Last Modified: Fri, 25 May 2018 15:49:15 GMT  
		Size: 203.3 MB (203260535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a862ae50eb668fd467dd0529f7a65222c885a20ef8d430ae67c1ef80d6211e20`  
		Last Modified: Fri, 25 May 2018 15:48:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b4a39407c12801335afb2e67bf30ec79318c34459ca9c277d0fcc3b4d3aa22`  
		Last Modified: Fri, 25 May 2018 15:50:07 GMT  
		Size: 63.4 MB (63381662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:lunar`

```console
$ docker pull ros@sha256:de7b5f5cc43ffc2c0ea47e21715056b81fe5fa914250cef9164b2fba61854a0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:lunar` - linux; amd64

```console
$ docker pull ros@sha256:090aa9b43c5825561a3a278153b6f7c14a68fe3065977fba9cf139c6f7f05c80
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **382.4 MB (382411487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a1e78d62416346ebef2833ea5ce2c0959c49f9a1fa314be34ea503322ccf28c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:52 GMT
ADD file:d37ff24540ea7700d0fc053e1996b234428a88f3a324d7fcbd83d8ef95318040 in / 
# Tue, 05 Jun 2018 21:21:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:54 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:55 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:35:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:35:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:35:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:36:43 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 23:04:04 GMT
ENV ROS_DISTRO=lunar
# Tue, 05 Jun 2018 23:08:25 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 23:08:27 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 23:08:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 23:08:27 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 23:11:38 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b234f539f7a1d65eabae1617e63c81ac01768abffd48b5cbbf7166efca6a3429`  
		Last Modified: Mon, 28 May 2018 14:57:20 GMT  
		Size: 43.1 MB (43122477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55172d420b43cf03feeec11bcc917c7ddfc192036102e065ab57aa9abb95311e`  
		Last Modified: Tue, 05 Jun 2018 21:24:52 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba5bbeb6b91e2676c98255c6babc66d7b05cac40185eeba4b3773199c701da0`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ae2841ad7a7fd1aeae30028105cac7f6ee0ec955e5229e52b3333fea3c17b5`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c9c6de41905e9a66f2bc2c4a19858c8dc5b0a94f01e03eafc719afe25888aa`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22c30eae0b9363cecd2e5ac27a92dd1bc354e2e16a3ee82b70932814b4c12a`  
		Last Modified: Wed, 06 Jun 2018 00:11:32 GMT  
		Size: 5.4 MB (5362202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fce58d2960dc3a1265e5bc18474d652795940cafde67d662929605c9e3b1c44`  
		Last Modified: Wed, 06 Jun 2018 00:11:29 GMT  
		Size: 13.1 KB (13081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a8410e99e70f8971b54ce991fecd04014ef363a7dde349dd255d6358a6893d`  
		Last Modified: Wed, 06 Jun 2018 00:11:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3037b7978826369126bbe26cbb5d642f59ccd31d96e28044f872cd3eac55ab`  
		Last Modified: Wed, 06 Jun 2018 00:11:55 GMT  
		Size: 55.6 MB (55571338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cfa8aa4c1f7b161f88b862221bacc540052abfa4f8a11884d0090ebcd55cf9`  
		Last Modified: Wed, 06 Jun 2018 00:11:27 GMT  
		Size: 866.4 KB (866393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f170ce1e7cb1fdb2828bd6d23958f58b3be2174117f4f6e52d753d4c1422755d`  
		Last Modified: Wed, 06 Jun 2018 00:23:44 GMT  
		Size: 193.6 MB (193641819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0eb07e8e7dea220978bd30a26bf318649bf3cef13901c943bee38ed05afbede`  
		Last Modified: Wed, 06 Jun 2018 00:22:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dec063ced0219e39083dbd6fe65cc6f033c293b408910fcd3495c0928558874`  
		Last Modified: Wed, 06 Jun 2018 00:24:38 GMT  
		Size: 83.8 MB (83831267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar` - linux; arm variant v7

```console
$ docker pull ros@sha256:9bd1c7651a0551f4d2b7d6c5638e12a4087b3474e25d9e506469f0cf79c38e2a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.2 MB (334192284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b670e98de88ae0afdba3403479590682d0375233bc241fc2fab02c5ec3ef6e6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:05:33 GMT
ADD file:1e3efdebaf133af6b22e61da056500ff8cf5292f051296f69abd35f44da5625c in / 
# Sat, 28 Apr 2018 12:05:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:05:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:05:37 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:05:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:50 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 12:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:08:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 12:08:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 12:09:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 12:09:57 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 12:16:42 GMT
ENV ROS_DISTRO=lunar
# Sat, 28 Apr 2018 12:18:04 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:18:11 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 12:18:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 12:18:15 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 12:19:38 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f68dc00194f474ccfe395953a935f0a65f37edc5e218b6f310f432b3866f9bac`  
		Last Modified: Sat, 28 Apr 2018 12:09:03 GMT  
		Size: 38.1 MB (38126697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281b914f46e3b5e9fac0f9436525399186a66cb5abb5403eed9940d4207e15b4`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b205ebc944011540b5d7c371fe39a5cb49890d018253fcd39db61040dfed3`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418c61fca2a7e383833d9b12bd7adf62e311bf6350037e68503fbbbdfb8cc2b`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b471dd10511e8664a33e00815086f40bdfd8c30a16f93b190084bb5bb8a993f`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5050587be2fd4accc805402daed25e9344bd052ced481a6ecd1a5754102cb84`  
		Last Modified: Sat, 28 Apr 2018 12:27:40 GMT  
		Size: 4.6 MB (4614906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334ce8d248512220d545aecf150f8b8172bbd3e4c62f9cdc4c1e814053440912`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d06c2ef1c00b3cb66443790e82ae98882427dfc78b0009b2b801bdd0387146`  
		Last Modified: Sat, 28 Apr 2018 12:27:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b97dba49af961b21651a5255033ef01a2c0100029e05207d73befd0c45f6d85`  
		Last Modified: Sat, 28 Apr 2018 12:27:55 GMT  
		Size: 50.7 MB (50671071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1310601b6139b280f88b623eeaef6873b2ed293d2e09bc94346f6a444ab9973`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 833.2 KB (833166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08118158eff956ccf6049e24b2f4fdc1f4450a505d85654be6726518a4e26b48`  
		Last Modified: Sat, 28 Apr 2018 12:32:52 GMT  
		Size: 164.9 MB (164914641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333082bc4516b0aeb21520abb86eecc31f08b6ed0c020598e2f0191242f3d8b9`  
		Last Modified: Sat, 28 Apr 2018 12:32:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d4a1cce90475c4e7ac57ddbdc2d54c1fbd714cd01ad340f7065323a3f662fe`  
		Last Modified: Sat, 28 Apr 2018 12:33:30 GMT  
		Size: 75.0 MB (75015814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0f7b9fee47153280362bb4ace6bd74e1f1665c93dca0b781f3e23c455898a742
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.0 MB (347963461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:911262005503e580de950c25cbe41b95752296011e4448d98d3bed828f5bd96c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:12:52 GMT
ADD file:fef3655a03a1c7f1533148016797b982955b3d5556f32c777214b8426028509b in / 
# Tue, 01 May 2018 01:12:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:13:04 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:13:10 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:13:20 GMT
CMD ["/bin/bash"]
# Tue, 01 May 2018 01:19:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:19:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 01:19:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 01:23:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:23:33 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 01:23:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 01:24:25 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 02:51:26 GMT
ENV ROS_DISTRO=lunar
# Tue, 01 May 2018 02:59:44 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 02:59:49 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 02:59:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 02:59:52 GMT
CMD ["bash"]
# Tue, 01 May 2018 03:06:57 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c016a9a148a71d05469a3994d54eb7eb9c3d40a65e07bf68788018a71d951b`  
		Last Modified: Mon, 23 Apr 2018 14:56:07 GMT  
		Size: 39.2 MB (39223827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1976297de94ed1f5c4c0f13b0b25199c6d6ca003ddfc3e873938aa2f8e86b`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d83417bbef32ed4713f4224bcb9f9573597ee6d91174dc7403ce457f145d2`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2544c5c45beca34c948aca9c981d56b587a973354727e4c97dc99d88227fb6a`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92ef1d410a96b276ec1425b000d80d5c1d914688aae8bce3e6f20d8a5a7a5f`  
		Last Modified: Tue, 01 May 2018 01:17:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3a2ac905d0d30502b9bf9736c755da2e7a05465764ff1fb14a45f067faa71c`  
		Last Modified: Tue, 01 May 2018 04:17:49 GMT  
		Size: 4.8 MB (4819486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31df2d860f2dc7f931faa244a38a740a44c732fd7ab480a29daf8999b5fb7fcd`  
		Last Modified: Tue, 01 May 2018 04:17:40 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a06299e2df93eba22547e7bbfaf291225cb3e1d85dcd160f7080d0d65647a`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ce03745d3f424b139a80266262e70dfefbda981c88ae34eac7b56df3120657`  
		Last Modified: Tue, 01 May 2018 04:18:42 GMT  
		Size: 52.4 MB (52441627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360b2687112930e2c2a443c4f89ecbdda5be0103c5b840e39840d3aca65352a`  
		Last Modified: Tue, 01 May 2018 04:17:41 GMT  
		Size: 835.1 KB (835081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dbca386e5c6b5ffe323554a2f8bf12b018dace7d69b3b4ba8c6f9e99ac97c8`  
		Last Modified: Tue, 01 May 2018 04:34:53 GMT  
		Size: 174.2 MB (174164133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6170ad5544fce2d65ed25da27444eaad1efb07f3af011b076ca66e054d4895a`  
		Last Modified: Tue, 01 May 2018 04:32:45 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973fc8cb4ca9d12fc8aabae8747ce1911197af7de290fe386c7de3d47da65d05`  
		Last Modified: Tue, 01 May 2018 04:35:43 GMT  
		Size: 76.5 MB (76463310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:lunar-perception`

```console
$ docker pull ros@sha256:eb0bc35d8f700135d3ad8e67f063d8a77c184cb7c4128bbe61e3596c4b6659b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:lunar-perception` - linux; amd64

```console
$ docker pull ros@sha256:96f63f5329e6b6658971f48d81ebf69e09fef58c56bc69cc441fbe9d7dea8fc5
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **720.9 MB (720947904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5203c1869087b207731ade9ef00f398e32d744b7424e4986f69ffea4e95e02a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 27 Apr 2018 23:30:17 GMT
ADD file:592c2540de1c707636622213ee30ff5b6f8be0a48bb25c97edc7204ea4df1a81 in / 
# Fri, 27 Apr 2018 23:30:18 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 27 Apr 2018 23:30:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 27 Apr 2018 23:30:19 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 27 Apr 2018 23:30:20 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 27 Apr 2018 23:30:21 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 00:29:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 00:29:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 00:29:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 00:30:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 00:30:23 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 00:30:23 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 00:30:39 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 01:42:30 GMT
ENV ROS_DISTRO=lunar
# Sat, 28 Apr 2018 01:45:34 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 01:45:35 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 01:45:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 01:45:36 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 02:02:31 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 02:10:53 GMT
RUN apt-get update && apt-get install -y     ros-lunar-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:297061f60c367c17cfd016c97a8cb24f5308db2c913def0f85d7a6848c0a17fa`  
		Last Modified: Fri, 20 Apr 2018 22:11:58 GMT  
		Size: 43.0 MB (43026850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ccef17b516e916aa8abe7817876211000c27150b908bdffcdeeba938cd004c`  
		Last Modified: Fri, 27 Apr 2018 23:35:41 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc33716854d9e2ef2de9769422f498f5320ffa41cb79336e7a88fbb6c3ef844`  
		Last Modified: Fri, 27 Apr 2018 23:35:41 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe36b178d25214195af42254bc7d5d64a269f654ef8801bbeb0b6a70a618353`  
		Last Modified: Fri, 27 Apr 2018 23:35:41 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686596545a94a0f0bf822e442cfd28fbd8a769f28e5f4018d7c24576dc6c3aac`  
		Last Modified: Fri, 27 Apr 2018 23:35:41 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a541c4d9d1f7e445180393cf16198af675a3551e79073ba1b43a73563971942`  
		Last Modified: Sat, 28 Apr 2018 04:01:44 GMT  
		Size: 5.4 MB (5362303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54d52e8e263dd82140fc98a624fd354e428b5919518bba02a6552ec088c00a9`  
		Last Modified: Sat, 28 Apr 2018 04:01:41 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15c6b1f100d8f680278d97ed3b2dbfeced8829d1375a6daee70d2875ce49c37`  
		Last Modified: Sat, 28 Apr 2018 04:01:38 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ecfc254e5e4899b87aa39bab7c2b82b075a419770e15c3e8b37438f6230416`  
		Last Modified: Sat, 28 Apr 2018 04:02:00 GMT  
		Size: 55.6 MB (55565364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9871000b426da10d8c74f5351b8a44cc41c9f6fa115985ca5e078b56bd005ea2`  
		Last Modified: Sat, 28 Apr 2018 04:01:40 GMT  
		Size: 833.1 KB (833115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994abacad26ee6e24559fc8ff7124e6c51a17d0d60ab0761fcb010c46be2fd19`  
		Last Modified: Sat, 28 Apr 2018 05:15:46 GMT  
		Size: 193.6 MB (193612569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60b2aedcd93a1dac29bd2f719525f6dc8f752aaaa99655da2b43c8d208540f2`  
		Last Modified: Sat, 28 Apr 2018 05:14:50 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b258a2815634b1c35a5da26216e0217fbeca65eefbd8f0bd29d29445d92fba76`  
		Last Modified: Sat, 28 Apr 2018 05:33:31 GMT  
		Size: 83.8 MB (83830688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d640b74a6683b7ed02b18e544c280ad2579a6f7f47bec1f9be30342ad43261`  
		Last Modified: Sat, 28 Apr 2018 05:37:27 GMT  
		Size: 338.7 MB (338701025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:bbd01496fb33dcd2a30c753db0c55e71ab633e6bd418faf4339f0b6598d1ac06
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **614.1 MB (614120576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e476a506ac63062b861410fd4caa7606a895e1400735d1b944f3affb9232a8d3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:05:33 GMT
ADD file:1e3efdebaf133af6b22e61da056500ff8cf5292f051296f69abd35f44da5625c in / 
# Sat, 28 Apr 2018 12:05:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:05:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:05:37 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:05:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:50 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 12:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:08:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 12:08:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 12:09:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 12:09:57 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 12:16:42 GMT
ENV ROS_DISTRO=lunar
# Sat, 28 Apr 2018 12:18:04 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:18:11 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 12:18:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 12:18:15 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 12:19:38 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:23:53 GMT
RUN apt-get update && apt-get install -y     ros-lunar-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f68dc00194f474ccfe395953a935f0a65f37edc5e218b6f310f432b3866f9bac`  
		Last Modified: Sat, 28 Apr 2018 12:09:03 GMT  
		Size: 38.1 MB (38126697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281b914f46e3b5e9fac0f9436525399186a66cb5abb5403eed9940d4207e15b4`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b205ebc944011540b5d7c371fe39a5cb49890d018253fcd39db61040dfed3`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418c61fca2a7e383833d9b12bd7adf62e311bf6350037e68503fbbbdfb8cc2b`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b471dd10511e8664a33e00815086f40bdfd8c30a16f93b190084bb5bb8a993f`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5050587be2fd4accc805402daed25e9344bd052ced481a6ecd1a5754102cb84`  
		Last Modified: Sat, 28 Apr 2018 12:27:40 GMT  
		Size: 4.6 MB (4614906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334ce8d248512220d545aecf150f8b8172bbd3e4c62f9cdc4c1e814053440912`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d06c2ef1c00b3cb66443790e82ae98882427dfc78b0009b2b801bdd0387146`  
		Last Modified: Sat, 28 Apr 2018 12:27:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b97dba49af961b21651a5255033ef01a2c0100029e05207d73befd0c45f6d85`  
		Last Modified: Sat, 28 Apr 2018 12:27:55 GMT  
		Size: 50.7 MB (50671071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1310601b6139b280f88b623eeaef6873b2ed293d2e09bc94346f6a444ab9973`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 833.2 KB (833166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08118158eff956ccf6049e24b2f4fdc1f4450a505d85654be6726518a4e26b48`  
		Last Modified: Sat, 28 Apr 2018 12:32:52 GMT  
		Size: 164.9 MB (164914641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333082bc4516b0aeb21520abb86eecc31f08b6ed0c020598e2f0191242f3d8b9`  
		Last Modified: Sat, 28 Apr 2018 12:32:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d4a1cce90475c4e7ac57ddbdc2d54c1fbd714cd01ad340f7065323a3f662fe`  
		Last Modified: Sat, 28 Apr 2018 12:33:30 GMT  
		Size: 75.0 MB (75015814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0559e165b507c7a1783781fe0803a506284232f32f85f74bd12146b18be058a`  
		Last Modified: Sat, 28 Apr 2018 12:35:59 GMT  
		Size: 279.9 MB (279928292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d0a57292bbb93ea1ded113e80c55fec11d991383819dca0772ed7467e2d4395e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **637.6 MB (637554752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b0072f112be5eb51fe251af0608804a2640c4c7919e4ca710e747c14f90435a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:12:52 GMT
ADD file:fef3655a03a1c7f1533148016797b982955b3d5556f32c777214b8426028509b in / 
# Tue, 01 May 2018 01:12:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:13:04 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:13:10 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:13:20 GMT
CMD ["/bin/bash"]
# Tue, 01 May 2018 01:19:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:19:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 01:19:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 01:23:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:23:33 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 01:23:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 01:24:25 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 02:51:26 GMT
ENV ROS_DISTRO=lunar
# Tue, 01 May 2018 02:59:44 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 02:59:49 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 02:59:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 02:59:52 GMT
CMD ["bash"]
# Tue, 01 May 2018 03:06:57 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:29:08 GMT
RUN apt-get update && apt-get install -y     ros-lunar-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c016a9a148a71d05469a3994d54eb7eb9c3d40a65e07bf68788018a71d951b`  
		Last Modified: Mon, 23 Apr 2018 14:56:07 GMT  
		Size: 39.2 MB (39223827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1976297de94ed1f5c4c0f13b0b25199c6d6ca003ddfc3e873938aa2f8e86b`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d83417bbef32ed4713f4224bcb9f9573597ee6d91174dc7403ce457f145d2`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2544c5c45beca34c948aca9c981d56b587a973354727e4c97dc99d88227fb6a`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92ef1d410a96b276ec1425b000d80d5c1d914688aae8bce3e6f20d8a5a7a5f`  
		Last Modified: Tue, 01 May 2018 01:17:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3a2ac905d0d30502b9bf9736c755da2e7a05465764ff1fb14a45f067faa71c`  
		Last Modified: Tue, 01 May 2018 04:17:49 GMT  
		Size: 4.8 MB (4819486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31df2d860f2dc7f931faa244a38a740a44c732fd7ab480a29daf8999b5fb7fcd`  
		Last Modified: Tue, 01 May 2018 04:17:40 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a06299e2df93eba22547e7bbfaf291225cb3e1d85dcd160f7080d0d65647a`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ce03745d3f424b139a80266262e70dfefbda981c88ae34eac7b56df3120657`  
		Last Modified: Tue, 01 May 2018 04:18:42 GMT  
		Size: 52.4 MB (52441627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360b2687112930e2c2a443c4f89ecbdda5be0103c5b840e39840d3aca65352a`  
		Last Modified: Tue, 01 May 2018 04:17:41 GMT  
		Size: 835.1 KB (835081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dbca386e5c6b5ffe323554a2f8bf12b018dace7d69b3b4ba8c6f9e99ac97c8`  
		Last Modified: Tue, 01 May 2018 04:34:53 GMT  
		Size: 174.2 MB (174164133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6170ad5544fce2d65ed25da27444eaad1efb07f3af011b076ca66e054d4895a`  
		Last Modified: Tue, 01 May 2018 04:32:45 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973fc8cb4ca9d12fc8aabae8747ce1911197af7de290fe386c7de3d47da65d05`  
		Last Modified: Tue, 01 May 2018 04:35:43 GMT  
		Size: 76.5 MB (76463310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ef85a414da412179c1de9ee6598df88056712c18c9233e1271aaebc4da5135`  
		Last Modified: Tue, 01 May 2018 04:40:36 GMT  
		Size: 289.6 MB (289591291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:lunar-perception-stretch`

```console
$ docker pull ros@sha256:36c8e84aea138c2c67b64b4ee3ccc5226c92bd9c9c80716faf3704e66f391aae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:lunar-perception-stretch` - linux; amd64

```console
$ docker pull ros@sha256:72c488eae32b14ac277e37c683b9b9af63e8f5f552187201ad3f21892404afe9
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **930.4 MB (930399304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ffe0c89abdde569ecbff27937d9ac158f4bad18082ccd2cdb6cbb253240432`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 07:08:53 GMT
ADD file:9572fdb59dfbb9b032f3331bbc2a08b31e0aef5fbde44c8f2008d22bf5290cf2 in / 
# Sat, 28 Apr 2018 07:08:53 GMT
CMD ["bash"]
# Sun, 29 Apr 2018 12:52:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:52:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sun, 29 Apr 2018 12:52:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros-latest.list
# Sun, 29 Apr 2018 12:52:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:52:42 GMT
ENV LANG=C.UTF-8
# Sun, 29 Apr 2018 12:52:42 GMT
ENV LC_ALL=C.UTF-8
# Sun, 29 Apr 2018 12:52:54 GMT
RUN rosdep init     && rosdep update
# Sun, 29 Apr 2018 12:52:54 GMT
ENV ROS_DISTRO=lunar
# Sun, 29 Apr 2018 12:54:28 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:54:29 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sun, 29 Apr 2018 12:54:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 29 Apr 2018 12:54:29 GMT
CMD ["bash"]
# Sun, 29 Apr 2018 13:15:48 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 13:37:13 GMT
RUN apt-get update && apt-get install -y     ros-lunar-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc1a78bfd46becbfc3abb8a74d9a70a0e0dc7a5809bbd12e814f9382db003707`  
		Last Modified: Sat, 28 Apr 2018 09:27:54 GMT  
		Size: 45.3 MB (45318159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080d14fa56ef128c193fd94edf1e5eb031d02ae97b680588c7248e5e84304f13`  
		Last Modified: Sun, 29 Apr 2018 14:48:05 GMT  
		Size: 6.9 MB (6859072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604921583c4f613ebee4eb24564ca607566b8b48206868b48c018443567dd0b2`  
		Last Modified: Sun, 29 Apr 2018 14:48:03 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631afcce8e2d86cf9596b3823955679a3e770120d1da140a494003c85bf577b7`  
		Last Modified: Sun, 29 Apr 2018 14:48:00 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b0b4ce522ec73ddd931386acbe825b6203543509a3d76c51e649cb124d5ca1`  
		Last Modified: Sun, 29 Apr 2018 14:48:25 GMT  
		Size: 64.9 MB (64857453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea215428a3b38a4f7bc2be7aad6084d16a82bb84f706aebde2d34120ffc5190`  
		Last Modified: Sun, 29 Apr 2018 14:48:01 GMT  
		Size: 833.5 KB (833530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26629a9af11703b4ed3e40e78cb5403156db690083566f39f679a55e75c6fb67`  
		Last Modified: Sun, 29 Apr 2018 14:49:00 GMT  
		Size: 251.9 MB (251873129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b853450ebbc6b17d4b77840bb123c679eebd84b027b38915296bef615ae43600`  
		Last Modified: Sun, 29 Apr 2018 14:48:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63863f0fc73e348d8df8c2777a8ca0d09df3991f247fd340c53ae4264056544d`  
		Last Modified: Sun, 29 Apr 2018 15:01:25 GMT  
		Size: 122.2 MB (122225868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360a56f8c15d012898db23f317d404c8f3ec80017f316412817583dae0cebf53`  
		Last Modified: Sun, 29 Apr 2018 15:28:38 GMT  
		Size: 438.4 MB (438430302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-perception-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:46bd33abe2f4717e1fba6ba648cbfb6b49b3b46c709288228fdff9b017c30014
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **813.6 MB (813636567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8b38e413db4441f342f3285c5722bb42480620ee78caebdbfba48919b6f5d72`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 30 Apr 2018 23:31:58 GMT
ADD file:245a8cfe59ea071e4e215a722e0d4b4b14fa95dd6ffd03739fe048433cfaf523 in / 
# Mon, 30 Apr 2018 23:32:00 GMT
CMD ["bash"]
# Tue, 01 May 2018 03:30:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:30:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 03:30:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 03:35:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:35:21 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 03:35:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 03:36:07 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 03:36:07 GMT
ENV ROS_DISTRO=lunar
# Tue, 01 May 2018 03:46:08 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:46:13 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 03:46:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 03:46:14 GMT
CMD ["bash"]
# Tue, 01 May 2018 03:51:28 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 04:16:59 GMT
RUN apt-get update && apt-get install -y     ros-lunar-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:142bf25d8d1b3ebc9dfbedd586e70a011594690acf48b2695bfce01e3a2cf0d5`  
		Last Modified: Mon, 30 Apr 2018 23:52:13 GMT  
		Size: 43.1 MB (43109349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994bacc3e1c11e50065156c511f0c11e001707e55b61e361b8dc44d236c76f24`  
		Last Modified: Tue, 01 May 2018 04:41:15 GMT  
		Size: 6.4 MB (6427112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663899231a010cf1e857473d7203c7e5f109b38379d2d822c31dba98a7f8af10`  
		Last Modified: Tue, 01 May 2018 04:41:09 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d68d9781734de3f7c1ce451752978a14ba285ad3c63d5ab58034a2008cd25ef`  
		Last Modified: Tue, 01 May 2018 04:41:06 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678cb4b8d2f95bf400236eedd95783c53081503a2ed2b39f51e57a6062cd18c7`  
		Last Modified: Tue, 01 May 2018 04:42:23 GMT  
		Size: 61.9 MB (61938600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0225d679802c170200a58607e1e5a805065659ce28bdec6f9cc91f1c5f6ac461`  
		Last Modified: Tue, 01 May 2018 04:41:08 GMT  
		Size: 835.1 KB (835084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8018c896d8c469869af751ab6dedae7d929c8c1eecd50bd607c44492245c688`  
		Last Modified: Tue, 01 May 2018 04:44:18 GMT  
		Size: 206.8 MB (206795100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4f80d568803a6e955c93890cfbb1629933a150a5d0a54e78f081bf2731b724`  
		Last Modified: Tue, 01 May 2018 04:41:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f59bacdd92efa26460f246475e05ca8c1d323676766477354f6c57571d53fa9`  
		Last Modified: Tue, 01 May 2018 04:45:14 GMT  
		Size: 116.0 MB (116022523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f244582c1aa41867d976d5391b8287d6b4dbcb917782000331ad8cb2cdff0290`  
		Last Modified: Tue, 01 May 2018 04:49:00 GMT  
		Size: 378.5 MB (378507002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:lunar-perception-xenial`

```console
$ docker pull ros@sha256:eb0bc35d8f700135d3ad8e67f063d8a77c184cb7c4128bbe61e3596c4b6659b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:lunar-perception-xenial` - linux; amd64

```console
$ docker pull ros@sha256:96f63f5329e6b6658971f48d81ebf69e09fef58c56bc69cc441fbe9d7dea8fc5
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **720.9 MB (720947904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5203c1869087b207731ade9ef00f398e32d744b7424e4986f69ffea4e95e02a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 27 Apr 2018 23:30:17 GMT
ADD file:592c2540de1c707636622213ee30ff5b6f8be0a48bb25c97edc7204ea4df1a81 in / 
# Fri, 27 Apr 2018 23:30:18 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 27 Apr 2018 23:30:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 27 Apr 2018 23:30:19 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 27 Apr 2018 23:30:20 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 27 Apr 2018 23:30:21 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 00:29:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 00:29:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 00:29:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 00:30:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 00:30:23 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 00:30:23 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 00:30:39 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 01:42:30 GMT
ENV ROS_DISTRO=lunar
# Sat, 28 Apr 2018 01:45:34 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 01:45:35 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 01:45:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 01:45:36 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 02:02:31 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 02:10:53 GMT
RUN apt-get update && apt-get install -y     ros-lunar-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:297061f60c367c17cfd016c97a8cb24f5308db2c913def0f85d7a6848c0a17fa`  
		Last Modified: Fri, 20 Apr 2018 22:11:58 GMT  
		Size: 43.0 MB (43026850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ccef17b516e916aa8abe7817876211000c27150b908bdffcdeeba938cd004c`  
		Last Modified: Fri, 27 Apr 2018 23:35:41 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc33716854d9e2ef2de9769422f498f5320ffa41cb79336e7a88fbb6c3ef844`  
		Last Modified: Fri, 27 Apr 2018 23:35:41 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe36b178d25214195af42254bc7d5d64a269f654ef8801bbeb0b6a70a618353`  
		Last Modified: Fri, 27 Apr 2018 23:35:41 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686596545a94a0f0bf822e442cfd28fbd8a769f28e5f4018d7c24576dc6c3aac`  
		Last Modified: Fri, 27 Apr 2018 23:35:41 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a541c4d9d1f7e445180393cf16198af675a3551e79073ba1b43a73563971942`  
		Last Modified: Sat, 28 Apr 2018 04:01:44 GMT  
		Size: 5.4 MB (5362303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54d52e8e263dd82140fc98a624fd354e428b5919518bba02a6552ec088c00a9`  
		Last Modified: Sat, 28 Apr 2018 04:01:41 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15c6b1f100d8f680278d97ed3b2dbfeced8829d1375a6daee70d2875ce49c37`  
		Last Modified: Sat, 28 Apr 2018 04:01:38 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ecfc254e5e4899b87aa39bab7c2b82b075a419770e15c3e8b37438f6230416`  
		Last Modified: Sat, 28 Apr 2018 04:02:00 GMT  
		Size: 55.6 MB (55565364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9871000b426da10d8c74f5351b8a44cc41c9f6fa115985ca5e078b56bd005ea2`  
		Last Modified: Sat, 28 Apr 2018 04:01:40 GMT  
		Size: 833.1 KB (833115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994abacad26ee6e24559fc8ff7124e6c51a17d0d60ab0761fcb010c46be2fd19`  
		Last Modified: Sat, 28 Apr 2018 05:15:46 GMT  
		Size: 193.6 MB (193612569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60b2aedcd93a1dac29bd2f719525f6dc8f752aaaa99655da2b43c8d208540f2`  
		Last Modified: Sat, 28 Apr 2018 05:14:50 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b258a2815634b1c35a5da26216e0217fbeca65eefbd8f0bd29d29445d92fba76`  
		Last Modified: Sat, 28 Apr 2018 05:33:31 GMT  
		Size: 83.8 MB (83830688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d640b74a6683b7ed02b18e544c280ad2579a6f7f47bec1f9be30342ad43261`  
		Last Modified: Sat, 28 Apr 2018 05:37:27 GMT  
		Size: 338.7 MB (338701025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-perception-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:bbd01496fb33dcd2a30c753db0c55e71ab633e6bd418faf4339f0b6598d1ac06
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **614.1 MB (614120576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e476a506ac63062b861410fd4caa7606a895e1400735d1b944f3affb9232a8d3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:05:33 GMT
ADD file:1e3efdebaf133af6b22e61da056500ff8cf5292f051296f69abd35f44da5625c in / 
# Sat, 28 Apr 2018 12:05:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:05:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:05:37 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:05:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:50 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 12:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:08:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 12:08:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 12:09:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 12:09:57 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 12:16:42 GMT
ENV ROS_DISTRO=lunar
# Sat, 28 Apr 2018 12:18:04 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:18:11 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 12:18:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 12:18:15 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 12:19:38 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:23:53 GMT
RUN apt-get update && apt-get install -y     ros-lunar-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f68dc00194f474ccfe395953a935f0a65f37edc5e218b6f310f432b3866f9bac`  
		Last Modified: Sat, 28 Apr 2018 12:09:03 GMT  
		Size: 38.1 MB (38126697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281b914f46e3b5e9fac0f9436525399186a66cb5abb5403eed9940d4207e15b4`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b205ebc944011540b5d7c371fe39a5cb49890d018253fcd39db61040dfed3`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418c61fca2a7e383833d9b12bd7adf62e311bf6350037e68503fbbbdfb8cc2b`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b471dd10511e8664a33e00815086f40bdfd8c30a16f93b190084bb5bb8a993f`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5050587be2fd4accc805402daed25e9344bd052ced481a6ecd1a5754102cb84`  
		Last Modified: Sat, 28 Apr 2018 12:27:40 GMT  
		Size: 4.6 MB (4614906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334ce8d248512220d545aecf150f8b8172bbd3e4c62f9cdc4c1e814053440912`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d06c2ef1c00b3cb66443790e82ae98882427dfc78b0009b2b801bdd0387146`  
		Last Modified: Sat, 28 Apr 2018 12:27:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b97dba49af961b21651a5255033ef01a2c0100029e05207d73befd0c45f6d85`  
		Last Modified: Sat, 28 Apr 2018 12:27:55 GMT  
		Size: 50.7 MB (50671071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1310601b6139b280f88b623eeaef6873b2ed293d2e09bc94346f6a444ab9973`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 833.2 KB (833166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08118158eff956ccf6049e24b2f4fdc1f4450a505d85654be6726518a4e26b48`  
		Last Modified: Sat, 28 Apr 2018 12:32:52 GMT  
		Size: 164.9 MB (164914641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333082bc4516b0aeb21520abb86eecc31f08b6ed0c020598e2f0191242f3d8b9`  
		Last Modified: Sat, 28 Apr 2018 12:32:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d4a1cce90475c4e7ac57ddbdc2d54c1fbd714cd01ad340f7065323a3f662fe`  
		Last Modified: Sat, 28 Apr 2018 12:33:30 GMT  
		Size: 75.0 MB (75015814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0559e165b507c7a1783781fe0803a506284232f32f85f74bd12146b18be058a`  
		Last Modified: Sat, 28 Apr 2018 12:35:59 GMT  
		Size: 279.9 MB (279928292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-perception-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d0a57292bbb93ea1ded113e80c55fec11d991383819dca0772ed7467e2d4395e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **637.6 MB (637554752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b0072f112be5eb51fe251af0608804a2640c4c7919e4ca710e747c14f90435a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:12:52 GMT
ADD file:fef3655a03a1c7f1533148016797b982955b3d5556f32c777214b8426028509b in / 
# Tue, 01 May 2018 01:12:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:13:04 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:13:10 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:13:20 GMT
CMD ["/bin/bash"]
# Tue, 01 May 2018 01:19:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:19:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 01:19:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 01:23:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:23:33 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 01:23:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 01:24:25 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 02:51:26 GMT
ENV ROS_DISTRO=lunar
# Tue, 01 May 2018 02:59:44 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 02:59:49 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 02:59:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 02:59:52 GMT
CMD ["bash"]
# Tue, 01 May 2018 03:06:57 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:29:08 GMT
RUN apt-get update && apt-get install -y     ros-lunar-perception=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c016a9a148a71d05469a3994d54eb7eb9c3d40a65e07bf68788018a71d951b`  
		Last Modified: Mon, 23 Apr 2018 14:56:07 GMT  
		Size: 39.2 MB (39223827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1976297de94ed1f5c4c0f13b0b25199c6d6ca003ddfc3e873938aa2f8e86b`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d83417bbef32ed4713f4224bcb9f9573597ee6d91174dc7403ce457f145d2`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2544c5c45beca34c948aca9c981d56b587a973354727e4c97dc99d88227fb6a`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92ef1d410a96b276ec1425b000d80d5c1d914688aae8bce3e6f20d8a5a7a5f`  
		Last Modified: Tue, 01 May 2018 01:17:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3a2ac905d0d30502b9bf9736c755da2e7a05465764ff1fb14a45f067faa71c`  
		Last Modified: Tue, 01 May 2018 04:17:49 GMT  
		Size: 4.8 MB (4819486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31df2d860f2dc7f931faa244a38a740a44c732fd7ab480a29daf8999b5fb7fcd`  
		Last Modified: Tue, 01 May 2018 04:17:40 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a06299e2df93eba22547e7bbfaf291225cb3e1d85dcd160f7080d0d65647a`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ce03745d3f424b139a80266262e70dfefbda981c88ae34eac7b56df3120657`  
		Last Modified: Tue, 01 May 2018 04:18:42 GMT  
		Size: 52.4 MB (52441627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360b2687112930e2c2a443c4f89ecbdda5be0103c5b840e39840d3aca65352a`  
		Last Modified: Tue, 01 May 2018 04:17:41 GMT  
		Size: 835.1 KB (835081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dbca386e5c6b5ffe323554a2f8bf12b018dace7d69b3b4ba8c6f9e99ac97c8`  
		Last Modified: Tue, 01 May 2018 04:34:53 GMT  
		Size: 174.2 MB (174164133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6170ad5544fce2d65ed25da27444eaad1efb07f3af011b076ca66e054d4895a`  
		Last Modified: Tue, 01 May 2018 04:32:45 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973fc8cb4ca9d12fc8aabae8747ce1911197af7de290fe386c7de3d47da65d05`  
		Last Modified: Tue, 01 May 2018 04:35:43 GMT  
		Size: 76.5 MB (76463310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ef85a414da412179c1de9ee6598df88056712c18c9233e1271aaebc4da5135`  
		Last Modified: Tue, 01 May 2018 04:40:36 GMT  
		Size: 289.6 MB (289591291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:lunar-robot`

```console
$ docker pull ros@sha256:69b2e29d5d7ec660c57522300747daea0937dddc050eea2d3317a700b3685241
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:lunar-robot` - linux; amd64

```console
$ docker pull ros@sha256:67bbd8b9d2b95750069eb00dcab46db78a34f8232502a12f2d9108855ed6f844
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.9 MB (485948756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab5592dc8bb6e38efff0a59d5cd3de7c50574d54f3184302fd87cf7a784fd2a6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 27 Apr 2018 23:30:17 GMT
ADD file:592c2540de1c707636622213ee30ff5b6f8be0a48bb25c97edc7204ea4df1a81 in / 
# Fri, 27 Apr 2018 23:30:18 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 27 Apr 2018 23:30:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 27 Apr 2018 23:30:19 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 27 Apr 2018 23:30:20 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 27 Apr 2018 23:30:21 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 00:29:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 00:29:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 00:29:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 00:30:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 00:30:23 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 00:30:23 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 00:30:39 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 01:42:30 GMT
ENV ROS_DISTRO=lunar
# Sat, 28 Apr 2018 01:45:34 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 01:45:35 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 01:45:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 01:45:36 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 02:02:31 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 02:05:39 GMT
RUN apt-get update && apt-get install -y     ros-lunar-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:297061f60c367c17cfd016c97a8cb24f5308db2c913def0f85d7a6848c0a17fa`  
		Last Modified: Fri, 20 Apr 2018 22:11:58 GMT  
		Size: 43.0 MB (43026850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ccef17b516e916aa8abe7817876211000c27150b908bdffcdeeba938cd004c`  
		Last Modified: Fri, 27 Apr 2018 23:35:41 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc33716854d9e2ef2de9769422f498f5320ffa41cb79336e7a88fbb6c3ef844`  
		Last Modified: Fri, 27 Apr 2018 23:35:41 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe36b178d25214195af42254bc7d5d64a269f654ef8801bbeb0b6a70a618353`  
		Last Modified: Fri, 27 Apr 2018 23:35:41 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686596545a94a0f0bf822e442cfd28fbd8a769f28e5f4018d7c24576dc6c3aac`  
		Last Modified: Fri, 27 Apr 2018 23:35:41 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a541c4d9d1f7e445180393cf16198af675a3551e79073ba1b43a73563971942`  
		Last Modified: Sat, 28 Apr 2018 04:01:44 GMT  
		Size: 5.4 MB (5362303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54d52e8e263dd82140fc98a624fd354e428b5919518bba02a6552ec088c00a9`  
		Last Modified: Sat, 28 Apr 2018 04:01:41 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15c6b1f100d8f680278d97ed3b2dbfeced8829d1375a6daee70d2875ce49c37`  
		Last Modified: Sat, 28 Apr 2018 04:01:38 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ecfc254e5e4899b87aa39bab7c2b82b075a419770e15c3e8b37438f6230416`  
		Last Modified: Sat, 28 Apr 2018 04:02:00 GMT  
		Size: 55.6 MB (55565364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9871000b426da10d8c74f5351b8a44cc41c9f6fa115985ca5e078b56bd005ea2`  
		Last Modified: Sat, 28 Apr 2018 04:01:40 GMT  
		Size: 833.1 KB (833115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994abacad26ee6e24559fc8ff7124e6c51a17d0d60ab0761fcb010c46be2fd19`  
		Last Modified: Sat, 28 Apr 2018 05:15:46 GMT  
		Size: 193.6 MB (193612569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60b2aedcd93a1dac29bd2f719525f6dc8f752aaaa99655da2b43c8d208540f2`  
		Last Modified: Sat, 28 Apr 2018 05:14:50 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b258a2815634b1c35a5da26216e0217fbeca65eefbd8f0bd29d29445d92fba76`  
		Last Modified: Sat, 28 Apr 2018 05:33:31 GMT  
		Size: 83.8 MB (83830688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2074ddf0af0e25ca6bf03fd58bf97b12f19996430eec4952f4fca64ebb1e4700`  
		Last Modified: Sat, 28 Apr 2018 05:35:10 GMT  
		Size: 103.7 MB (103701877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:9e6990e048830256c118a19211b536e2af527a0b9da5fb87762b4c6f38daee20
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.3 MB (424302453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ba70bc2cba67eeb3f8573b220f02ea090993d654caf73990944bdeaa0d96794`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:05:33 GMT
ADD file:1e3efdebaf133af6b22e61da056500ff8cf5292f051296f69abd35f44da5625c in / 
# Sat, 28 Apr 2018 12:05:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:05:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:05:37 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:05:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:50 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 12:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:08:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 12:08:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 12:09:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 12:09:57 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 12:16:42 GMT
ENV ROS_DISTRO=lunar
# Sat, 28 Apr 2018 12:18:04 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:18:11 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 12:18:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 12:18:15 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 12:19:38 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:20:57 GMT
RUN apt-get update && apt-get install -y     ros-lunar-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f68dc00194f474ccfe395953a935f0a65f37edc5e218b6f310f432b3866f9bac`  
		Last Modified: Sat, 28 Apr 2018 12:09:03 GMT  
		Size: 38.1 MB (38126697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281b914f46e3b5e9fac0f9436525399186a66cb5abb5403eed9940d4207e15b4`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b205ebc944011540b5d7c371fe39a5cb49890d018253fcd39db61040dfed3`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418c61fca2a7e383833d9b12bd7adf62e311bf6350037e68503fbbbdfb8cc2b`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b471dd10511e8664a33e00815086f40bdfd8c30a16f93b190084bb5bb8a993f`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5050587be2fd4accc805402daed25e9344bd052ced481a6ecd1a5754102cb84`  
		Last Modified: Sat, 28 Apr 2018 12:27:40 GMT  
		Size: 4.6 MB (4614906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334ce8d248512220d545aecf150f8b8172bbd3e4c62f9cdc4c1e814053440912`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d06c2ef1c00b3cb66443790e82ae98882427dfc78b0009b2b801bdd0387146`  
		Last Modified: Sat, 28 Apr 2018 12:27:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b97dba49af961b21651a5255033ef01a2c0100029e05207d73befd0c45f6d85`  
		Last Modified: Sat, 28 Apr 2018 12:27:55 GMT  
		Size: 50.7 MB (50671071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1310601b6139b280f88b623eeaef6873b2ed293d2e09bc94346f6a444ab9973`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 833.2 KB (833166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08118158eff956ccf6049e24b2f4fdc1f4450a505d85654be6726518a4e26b48`  
		Last Modified: Sat, 28 Apr 2018 12:32:52 GMT  
		Size: 164.9 MB (164914641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333082bc4516b0aeb21520abb86eecc31f08b6ed0c020598e2f0191242f3d8b9`  
		Last Modified: Sat, 28 Apr 2018 12:32:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d4a1cce90475c4e7ac57ddbdc2d54c1fbd714cd01ad340f7065323a3f662fe`  
		Last Modified: Sat, 28 Apr 2018 12:33:30 GMT  
		Size: 75.0 MB (75015814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb61f4ccbddf9c3823a976204bb5d71ff8ed2690dc38057cb10bdbe67356ab27`  
		Last Modified: Sat, 28 Apr 2018 12:34:23 GMT  
		Size: 90.1 MB (90110169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1406b2505b86dc04d203f950a67786e4ff95ca61a27c93ddcd3f818c53dae411
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.9 MB (441906391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:113e9c3ad6de7730a8cb8bf5b2270141d7d11cc32d391002104b0a50f8bcd208`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:12:52 GMT
ADD file:fef3655a03a1c7f1533148016797b982955b3d5556f32c777214b8426028509b in / 
# Tue, 01 May 2018 01:12:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:13:04 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:13:10 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:13:20 GMT
CMD ["/bin/bash"]
# Tue, 01 May 2018 01:19:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:19:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 01:19:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 01:23:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:23:33 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 01:23:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 01:24:25 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 02:51:26 GMT
ENV ROS_DISTRO=lunar
# Tue, 01 May 2018 02:59:44 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 02:59:49 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 02:59:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 02:59:52 GMT
CMD ["bash"]
# Tue, 01 May 2018 03:06:57 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:12:40 GMT
RUN apt-get update && apt-get install -y     ros-lunar-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c016a9a148a71d05469a3994d54eb7eb9c3d40a65e07bf68788018a71d951b`  
		Last Modified: Mon, 23 Apr 2018 14:56:07 GMT  
		Size: 39.2 MB (39223827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1976297de94ed1f5c4c0f13b0b25199c6d6ca003ddfc3e873938aa2f8e86b`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d83417bbef32ed4713f4224bcb9f9573597ee6d91174dc7403ce457f145d2`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2544c5c45beca34c948aca9c981d56b587a973354727e4c97dc99d88227fb6a`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92ef1d410a96b276ec1425b000d80d5c1d914688aae8bce3e6f20d8a5a7a5f`  
		Last Modified: Tue, 01 May 2018 01:17:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3a2ac905d0d30502b9bf9736c755da2e7a05465764ff1fb14a45f067faa71c`  
		Last Modified: Tue, 01 May 2018 04:17:49 GMT  
		Size: 4.8 MB (4819486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31df2d860f2dc7f931faa244a38a740a44c732fd7ab480a29daf8999b5fb7fcd`  
		Last Modified: Tue, 01 May 2018 04:17:40 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a06299e2df93eba22547e7bbfaf291225cb3e1d85dcd160f7080d0d65647a`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ce03745d3f424b139a80266262e70dfefbda981c88ae34eac7b56df3120657`  
		Last Modified: Tue, 01 May 2018 04:18:42 GMT  
		Size: 52.4 MB (52441627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360b2687112930e2c2a443c4f89ecbdda5be0103c5b840e39840d3aca65352a`  
		Last Modified: Tue, 01 May 2018 04:17:41 GMT  
		Size: 835.1 KB (835081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dbca386e5c6b5ffe323554a2f8bf12b018dace7d69b3b4ba8c6f9e99ac97c8`  
		Last Modified: Tue, 01 May 2018 04:34:53 GMT  
		Size: 174.2 MB (174164133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6170ad5544fce2d65ed25da27444eaad1efb07f3af011b076ca66e054d4895a`  
		Last Modified: Tue, 01 May 2018 04:32:45 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973fc8cb4ca9d12fc8aabae8747ce1911197af7de290fe386c7de3d47da65d05`  
		Last Modified: Tue, 01 May 2018 04:35:43 GMT  
		Size: 76.5 MB (76463310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e290a4f1bb794592b6e89122c4e277c35382fbe5ac2f9f64e6d3acf783fe03`  
		Last Modified: Tue, 01 May 2018 04:37:04 GMT  
		Size: 93.9 MB (93942930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:lunar-robot-stretch`

```console
$ docker pull ros@sha256:15c8a7c3b0f5cb7d99d658240d4f34e39aa45fc2f4cde67dfb526b3efb2924ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:lunar-robot-stretch` - linux; amd64

```console
$ docker pull ros@sha256:afdfd0657c73db187be089954a1b58221634077d60dfa2f01994ae1c72a13c4b
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **552.4 MB (552408250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ab832c7ec1493131ffe7b9ccd1104d1de7fdd04901aa05b8806a632ebd204b9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 07:08:53 GMT
ADD file:9572fdb59dfbb9b032f3331bbc2a08b31e0aef5fbde44c8f2008d22bf5290cf2 in / 
# Sat, 28 Apr 2018 07:08:53 GMT
CMD ["bash"]
# Sun, 29 Apr 2018 12:52:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:52:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sun, 29 Apr 2018 12:52:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros-latest.list
# Sun, 29 Apr 2018 12:52:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:52:42 GMT
ENV LANG=C.UTF-8
# Sun, 29 Apr 2018 12:52:42 GMT
ENV LC_ALL=C.UTF-8
# Sun, 29 Apr 2018 12:52:54 GMT
RUN rosdep init     && rosdep update
# Sun, 29 Apr 2018 12:52:54 GMT
ENV ROS_DISTRO=lunar
# Sun, 29 Apr 2018 12:54:28 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:54:29 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sun, 29 Apr 2018 12:54:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 29 Apr 2018 12:54:29 GMT
CMD ["bash"]
# Sun, 29 Apr 2018 13:15:48 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 13:20:08 GMT
RUN apt-get update && apt-get install -y     ros-lunar-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc1a78bfd46becbfc3abb8a74d9a70a0e0dc7a5809bbd12e814f9382db003707`  
		Last Modified: Sat, 28 Apr 2018 09:27:54 GMT  
		Size: 45.3 MB (45318159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080d14fa56ef128c193fd94edf1e5eb031d02ae97b680588c7248e5e84304f13`  
		Last Modified: Sun, 29 Apr 2018 14:48:05 GMT  
		Size: 6.9 MB (6859072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604921583c4f613ebee4eb24564ca607566b8b48206868b48c018443567dd0b2`  
		Last Modified: Sun, 29 Apr 2018 14:48:03 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631afcce8e2d86cf9596b3823955679a3e770120d1da140a494003c85bf577b7`  
		Last Modified: Sun, 29 Apr 2018 14:48:00 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b0b4ce522ec73ddd931386acbe825b6203543509a3d76c51e649cb124d5ca1`  
		Last Modified: Sun, 29 Apr 2018 14:48:25 GMT  
		Size: 64.9 MB (64857453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea215428a3b38a4f7bc2be7aad6084d16a82bb84f706aebde2d34120ffc5190`  
		Last Modified: Sun, 29 Apr 2018 14:48:01 GMT  
		Size: 833.5 KB (833530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26629a9af11703b4ed3e40e78cb5403156db690083566f39f679a55e75c6fb67`  
		Last Modified: Sun, 29 Apr 2018 14:49:00 GMT  
		Size: 251.9 MB (251873129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b853450ebbc6b17d4b77840bb123c679eebd84b027b38915296bef615ae43600`  
		Last Modified: Sun, 29 Apr 2018 14:48:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63863f0fc73e348d8df8c2777a8ca0d09df3991f247fd340c53ae4264056544d`  
		Last Modified: Sun, 29 Apr 2018 15:01:25 GMT  
		Size: 122.2 MB (122225868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b60d7ece16e3465f3c214a315b792cdfd175a2d44e17883d36de528f44c9ab0`  
		Last Modified: Sun, 29 Apr 2018 15:09:33 GMT  
		Size: 60.4 MB (60439248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-robot-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:894f11683856b6ba206078297eb02f05e3fea4ecf06ba96e6dbaa47ac3269cf5
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.6 MB (492646713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c4aba1fb2d7e94c22fabf73e1e0a28fcb4b3c11028bb0772b9613fe1afcae30`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 30 Apr 2018 23:31:58 GMT
ADD file:245a8cfe59ea071e4e215a722e0d4b4b14fa95dd6ffd03739fe048433cfaf523 in / 
# Mon, 30 Apr 2018 23:32:00 GMT
CMD ["bash"]
# Tue, 01 May 2018 03:30:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:30:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 03:30:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 03:35:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:35:21 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 03:35:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 03:36:07 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 03:36:07 GMT
ENV ROS_DISTRO=lunar
# Tue, 01 May 2018 03:46:08 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:46:13 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 03:46:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 03:46:14 GMT
CMD ["bash"]
# Tue, 01 May 2018 03:51:28 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:57:30 GMT
RUN apt-get update && apt-get install -y     ros-lunar-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:142bf25d8d1b3ebc9dfbedd586e70a011594690acf48b2695bfce01e3a2cf0d5`  
		Last Modified: Mon, 30 Apr 2018 23:52:13 GMT  
		Size: 43.1 MB (43109349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994bacc3e1c11e50065156c511f0c11e001707e55b61e361b8dc44d236c76f24`  
		Last Modified: Tue, 01 May 2018 04:41:15 GMT  
		Size: 6.4 MB (6427112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663899231a010cf1e857473d7203c7e5f109b38379d2d822c31dba98a7f8af10`  
		Last Modified: Tue, 01 May 2018 04:41:09 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d68d9781734de3f7c1ce451752978a14ba285ad3c63d5ab58034a2008cd25ef`  
		Last Modified: Tue, 01 May 2018 04:41:06 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678cb4b8d2f95bf400236eedd95783c53081503a2ed2b39f51e57a6062cd18c7`  
		Last Modified: Tue, 01 May 2018 04:42:23 GMT  
		Size: 61.9 MB (61938600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0225d679802c170200a58607e1e5a805065659ce28bdec6f9cc91f1c5f6ac461`  
		Last Modified: Tue, 01 May 2018 04:41:08 GMT  
		Size: 835.1 KB (835084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8018c896d8c469869af751ab6dedae7d929c8c1eecd50bd607c44492245c688`  
		Last Modified: Tue, 01 May 2018 04:44:18 GMT  
		Size: 206.8 MB (206795100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4f80d568803a6e955c93890cfbb1629933a150a5d0a54e78f081bf2731b724`  
		Last Modified: Tue, 01 May 2018 04:41:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f59bacdd92efa26460f246475e05ca8c1d323676766477354f6c57571d53fa9`  
		Last Modified: Tue, 01 May 2018 04:45:14 GMT  
		Size: 116.0 MB (116022523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a10db811d6be31f3fd2565254776071b854565d4874d53a986fc12b15f011f`  
		Last Modified: Tue, 01 May 2018 04:45:50 GMT  
		Size: 57.5 MB (57517148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:lunar-robot-xenial`

```console
$ docker pull ros@sha256:69b2e29d5d7ec660c57522300747daea0937dddc050eea2d3317a700b3685241
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:lunar-robot-xenial` - linux; amd64

```console
$ docker pull ros@sha256:67bbd8b9d2b95750069eb00dcab46db78a34f8232502a12f2d9108855ed6f844
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.9 MB (485948756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab5592dc8bb6e38efff0a59d5cd3de7c50574d54f3184302fd87cf7a784fd2a6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 27 Apr 2018 23:30:17 GMT
ADD file:592c2540de1c707636622213ee30ff5b6f8be0a48bb25c97edc7204ea4df1a81 in / 
# Fri, 27 Apr 2018 23:30:18 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 27 Apr 2018 23:30:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 27 Apr 2018 23:30:19 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 27 Apr 2018 23:30:20 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 27 Apr 2018 23:30:21 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 00:29:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 00:29:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 00:29:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 00:30:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 00:30:23 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 00:30:23 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 00:30:39 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 01:42:30 GMT
ENV ROS_DISTRO=lunar
# Sat, 28 Apr 2018 01:45:34 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 01:45:35 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 01:45:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 01:45:36 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 02:02:31 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 02:05:39 GMT
RUN apt-get update && apt-get install -y     ros-lunar-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:297061f60c367c17cfd016c97a8cb24f5308db2c913def0f85d7a6848c0a17fa`  
		Last Modified: Fri, 20 Apr 2018 22:11:58 GMT  
		Size: 43.0 MB (43026850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ccef17b516e916aa8abe7817876211000c27150b908bdffcdeeba938cd004c`  
		Last Modified: Fri, 27 Apr 2018 23:35:41 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc33716854d9e2ef2de9769422f498f5320ffa41cb79336e7a88fbb6c3ef844`  
		Last Modified: Fri, 27 Apr 2018 23:35:41 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe36b178d25214195af42254bc7d5d64a269f654ef8801bbeb0b6a70a618353`  
		Last Modified: Fri, 27 Apr 2018 23:35:41 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686596545a94a0f0bf822e442cfd28fbd8a769f28e5f4018d7c24576dc6c3aac`  
		Last Modified: Fri, 27 Apr 2018 23:35:41 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a541c4d9d1f7e445180393cf16198af675a3551e79073ba1b43a73563971942`  
		Last Modified: Sat, 28 Apr 2018 04:01:44 GMT  
		Size: 5.4 MB (5362303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54d52e8e263dd82140fc98a624fd354e428b5919518bba02a6552ec088c00a9`  
		Last Modified: Sat, 28 Apr 2018 04:01:41 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15c6b1f100d8f680278d97ed3b2dbfeced8829d1375a6daee70d2875ce49c37`  
		Last Modified: Sat, 28 Apr 2018 04:01:38 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ecfc254e5e4899b87aa39bab7c2b82b075a419770e15c3e8b37438f6230416`  
		Last Modified: Sat, 28 Apr 2018 04:02:00 GMT  
		Size: 55.6 MB (55565364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9871000b426da10d8c74f5351b8a44cc41c9f6fa115985ca5e078b56bd005ea2`  
		Last Modified: Sat, 28 Apr 2018 04:01:40 GMT  
		Size: 833.1 KB (833115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994abacad26ee6e24559fc8ff7124e6c51a17d0d60ab0761fcb010c46be2fd19`  
		Last Modified: Sat, 28 Apr 2018 05:15:46 GMT  
		Size: 193.6 MB (193612569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60b2aedcd93a1dac29bd2f719525f6dc8f752aaaa99655da2b43c8d208540f2`  
		Last Modified: Sat, 28 Apr 2018 05:14:50 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b258a2815634b1c35a5da26216e0217fbeca65eefbd8f0bd29d29445d92fba76`  
		Last Modified: Sat, 28 Apr 2018 05:33:31 GMT  
		Size: 83.8 MB (83830688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2074ddf0af0e25ca6bf03fd58bf97b12f19996430eec4952f4fca64ebb1e4700`  
		Last Modified: Sat, 28 Apr 2018 05:35:10 GMT  
		Size: 103.7 MB (103701877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-robot-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:9e6990e048830256c118a19211b536e2af527a0b9da5fb87762b4c6f38daee20
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.3 MB (424302453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ba70bc2cba67eeb3f8573b220f02ea090993d654caf73990944bdeaa0d96794`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:05:33 GMT
ADD file:1e3efdebaf133af6b22e61da056500ff8cf5292f051296f69abd35f44da5625c in / 
# Sat, 28 Apr 2018 12:05:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:05:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:05:37 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:05:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:50 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 12:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:08:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 12:08:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 12:09:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 12:09:57 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 12:16:42 GMT
ENV ROS_DISTRO=lunar
# Sat, 28 Apr 2018 12:18:04 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:18:11 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 12:18:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 12:18:15 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 12:19:38 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:20:57 GMT
RUN apt-get update && apt-get install -y     ros-lunar-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f68dc00194f474ccfe395953a935f0a65f37edc5e218b6f310f432b3866f9bac`  
		Last Modified: Sat, 28 Apr 2018 12:09:03 GMT  
		Size: 38.1 MB (38126697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281b914f46e3b5e9fac0f9436525399186a66cb5abb5403eed9940d4207e15b4`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b205ebc944011540b5d7c371fe39a5cb49890d018253fcd39db61040dfed3`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418c61fca2a7e383833d9b12bd7adf62e311bf6350037e68503fbbbdfb8cc2b`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b471dd10511e8664a33e00815086f40bdfd8c30a16f93b190084bb5bb8a993f`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5050587be2fd4accc805402daed25e9344bd052ced481a6ecd1a5754102cb84`  
		Last Modified: Sat, 28 Apr 2018 12:27:40 GMT  
		Size: 4.6 MB (4614906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334ce8d248512220d545aecf150f8b8172bbd3e4c62f9cdc4c1e814053440912`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d06c2ef1c00b3cb66443790e82ae98882427dfc78b0009b2b801bdd0387146`  
		Last Modified: Sat, 28 Apr 2018 12:27:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b97dba49af961b21651a5255033ef01a2c0100029e05207d73befd0c45f6d85`  
		Last Modified: Sat, 28 Apr 2018 12:27:55 GMT  
		Size: 50.7 MB (50671071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1310601b6139b280f88b623eeaef6873b2ed293d2e09bc94346f6a444ab9973`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 833.2 KB (833166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08118158eff956ccf6049e24b2f4fdc1f4450a505d85654be6726518a4e26b48`  
		Last Modified: Sat, 28 Apr 2018 12:32:52 GMT  
		Size: 164.9 MB (164914641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333082bc4516b0aeb21520abb86eecc31f08b6ed0c020598e2f0191242f3d8b9`  
		Last Modified: Sat, 28 Apr 2018 12:32:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d4a1cce90475c4e7ac57ddbdc2d54c1fbd714cd01ad340f7065323a3f662fe`  
		Last Modified: Sat, 28 Apr 2018 12:33:30 GMT  
		Size: 75.0 MB (75015814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb61f4ccbddf9c3823a976204bb5d71ff8ed2690dc38057cb10bdbe67356ab27`  
		Last Modified: Sat, 28 Apr 2018 12:34:23 GMT  
		Size: 90.1 MB (90110169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-robot-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1406b2505b86dc04d203f950a67786e4ff95ca61a27c93ddcd3f818c53dae411
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.9 MB (441906391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:113e9c3ad6de7730a8cb8bf5b2270141d7d11cc32d391002104b0a50f8bcd208`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:12:52 GMT
ADD file:fef3655a03a1c7f1533148016797b982955b3d5556f32c777214b8426028509b in / 
# Tue, 01 May 2018 01:12:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:13:04 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:13:10 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:13:20 GMT
CMD ["/bin/bash"]
# Tue, 01 May 2018 01:19:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:19:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 01:19:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 01:23:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:23:33 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 01:23:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 01:24:25 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 02:51:26 GMT
ENV ROS_DISTRO=lunar
# Tue, 01 May 2018 02:59:44 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 02:59:49 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 02:59:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 02:59:52 GMT
CMD ["bash"]
# Tue, 01 May 2018 03:06:57 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:12:40 GMT
RUN apt-get update && apt-get install -y     ros-lunar-robot=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c016a9a148a71d05469a3994d54eb7eb9c3d40a65e07bf68788018a71d951b`  
		Last Modified: Mon, 23 Apr 2018 14:56:07 GMT  
		Size: 39.2 MB (39223827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1976297de94ed1f5c4c0f13b0b25199c6d6ca003ddfc3e873938aa2f8e86b`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d83417bbef32ed4713f4224bcb9f9573597ee6d91174dc7403ce457f145d2`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2544c5c45beca34c948aca9c981d56b587a973354727e4c97dc99d88227fb6a`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92ef1d410a96b276ec1425b000d80d5c1d914688aae8bce3e6f20d8a5a7a5f`  
		Last Modified: Tue, 01 May 2018 01:17:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3a2ac905d0d30502b9bf9736c755da2e7a05465764ff1fb14a45f067faa71c`  
		Last Modified: Tue, 01 May 2018 04:17:49 GMT  
		Size: 4.8 MB (4819486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31df2d860f2dc7f931faa244a38a740a44c732fd7ab480a29daf8999b5fb7fcd`  
		Last Modified: Tue, 01 May 2018 04:17:40 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a06299e2df93eba22547e7bbfaf291225cb3e1d85dcd160f7080d0d65647a`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ce03745d3f424b139a80266262e70dfefbda981c88ae34eac7b56df3120657`  
		Last Modified: Tue, 01 May 2018 04:18:42 GMT  
		Size: 52.4 MB (52441627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360b2687112930e2c2a443c4f89ecbdda5be0103c5b840e39840d3aca65352a`  
		Last Modified: Tue, 01 May 2018 04:17:41 GMT  
		Size: 835.1 KB (835081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dbca386e5c6b5ffe323554a2f8bf12b018dace7d69b3b4ba8c6f9e99ac97c8`  
		Last Modified: Tue, 01 May 2018 04:34:53 GMT  
		Size: 174.2 MB (174164133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6170ad5544fce2d65ed25da27444eaad1efb07f3af011b076ca66e054d4895a`  
		Last Modified: Tue, 01 May 2018 04:32:45 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973fc8cb4ca9d12fc8aabae8747ce1911197af7de290fe386c7de3d47da65d05`  
		Last Modified: Tue, 01 May 2018 04:35:43 GMT  
		Size: 76.5 MB (76463310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e290a4f1bb794592b6e89122c4e277c35382fbe5ac2f9f64e6d3acf783fe03`  
		Last Modified: Tue, 01 May 2018 04:37:04 GMT  
		Size: 93.9 MB (93942930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:lunar-ros-base`

```console
$ docker pull ros@sha256:de7b5f5cc43ffc2c0ea47e21715056b81fe5fa914250cef9164b2fba61854a0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:lunar-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:090aa9b43c5825561a3a278153b6f7c14a68fe3065977fba9cf139c6f7f05c80
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **382.4 MB (382411487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a1e78d62416346ebef2833ea5ce2c0959c49f9a1fa314be34ea503322ccf28c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:52 GMT
ADD file:d37ff24540ea7700d0fc053e1996b234428a88f3a324d7fcbd83d8ef95318040 in / 
# Tue, 05 Jun 2018 21:21:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:54 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:55 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:35:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:35:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:35:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:36:43 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 23:04:04 GMT
ENV ROS_DISTRO=lunar
# Tue, 05 Jun 2018 23:08:25 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 23:08:27 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 23:08:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 23:08:27 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 23:11:38 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b234f539f7a1d65eabae1617e63c81ac01768abffd48b5cbbf7166efca6a3429`  
		Last Modified: Mon, 28 May 2018 14:57:20 GMT  
		Size: 43.1 MB (43122477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55172d420b43cf03feeec11bcc917c7ddfc192036102e065ab57aa9abb95311e`  
		Last Modified: Tue, 05 Jun 2018 21:24:52 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba5bbeb6b91e2676c98255c6babc66d7b05cac40185eeba4b3773199c701da0`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ae2841ad7a7fd1aeae30028105cac7f6ee0ec955e5229e52b3333fea3c17b5`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c9c6de41905e9a66f2bc2c4a19858c8dc5b0a94f01e03eafc719afe25888aa`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22c30eae0b9363cecd2e5ac27a92dd1bc354e2e16a3ee82b70932814b4c12a`  
		Last Modified: Wed, 06 Jun 2018 00:11:32 GMT  
		Size: 5.4 MB (5362202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fce58d2960dc3a1265e5bc18474d652795940cafde67d662929605c9e3b1c44`  
		Last Modified: Wed, 06 Jun 2018 00:11:29 GMT  
		Size: 13.1 KB (13081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a8410e99e70f8971b54ce991fecd04014ef363a7dde349dd255d6358a6893d`  
		Last Modified: Wed, 06 Jun 2018 00:11:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3037b7978826369126bbe26cbb5d642f59ccd31d96e28044f872cd3eac55ab`  
		Last Modified: Wed, 06 Jun 2018 00:11:55 GMT  
		Size: 55.6 MB (55571338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cfa8aa4c1f7b161f88b862221bacc540052abfa4f8a11884d0090ebcd55cf9`  
		Last Modified: Wed, 06 Jun 2018 00:11:27 GMT  
		Size: 866.4 KB (866393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f170ce1e7cb1fdb2828bd6d23958f58b3be2174117f4f6e52d753d4c1422755d`  
		Last Modified: Wed, 06 Jun 2018 00:23:44 GMT  
		Size: 193.6 MB (193641819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0eb07e8e7dea220978bd30a26bf318649bf3cef13901c943bee38ed05afbede`  
		Last Modified: Wed, 06 Jun 2018 00:22:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dec063ced0219e39083dbd6fe65cc6f033c293b408910fcd3495c0928558874`  
		Last Modified: Wed, 06 Jun 2018 00:24:38 GMT  
		Size: 83.8 MB (83831267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:9bd1c7651a0551f4d2b7d6c5638e12a4087b3474e25d9e506469f0cf79c38e2a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.2 MB (334192284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b670e98de88ae0afdba3403479590682d0375233bc241fc2fab02c5ec3ef6e6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:05:33 GMT
ADD file:1e3efdebaf133af6b22e61da056500ff8cf5292f051296f69abd35f44da5625c in / 
# Sat, 28 Apr 2018 12:05:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:05:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:05:37 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:05:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:50 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 12:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:08:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 12:08:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 12:09:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 12:09:57 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 12:16:42 GMT
ENV ROS_DISTRO=lunar
# Sat, 28 Apr 2018 12:18:04 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:18:11 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 12:18:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 12:18:15 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 12:19:38 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f68dc00194f474ccfe395953a935f0a65f37edc5e218b6f310f432b3866f9bac`  
		Last Modified: Sat, 28 Apr 2018 12:09:03 GMT  
		Size: 38.1 MB (38126697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281b914f46e3b5e9fac0f9436525399186a66cb5abb5403eed9940d4207e15b4`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b205ebc944011540b5d7c371fe39a5cb49890d018253fcd39db61040dfed3`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418c61fca2a7e383833d9b12bd7adf62e311bf6350037e68503fbbbdfb8cc2b`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b471dd10511e8664a33e00815086f40bdfd8c30a16f93b190084bb5bb8a993f`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5050587be2fd4accc805402daed25e9344bd052ced481a6ecd1a5754102cb84`  
		Last Modified: Sat, 28 Apr 2018 12:27:40 GMT  
		Size: 4.6 MB (4614906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334ce8d248512220d545aecf150f8b8172bbd3e4c62f9cdc4c1e814053440912`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d06c2ef1c00b3cb66443790e82ae98882427dfc78b0009b2b801bdd0387146`  
		Last Modified: Sat, 28 Apr 2018 12:27:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b97dba49af961b21651a5255033ef01a2c0100029e05207d73befd0c45f6d85`  
		Last Modified: Sat, 28 Apr 2018 12:27:55 GMT  
		Size: 50.7 MB (50671071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1310601b6139b280f88b623eeaef6873b2ed293d2e09bc94346f6a444ab9973`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 833.2 KB (833166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08118158eff956ccf6049e24b2f4fdc1f4450a505d85654be6726518a4e26b48`  
		Last Modified: Sat, 28 Apr 2018 12:32:52 GMT  
		Size: 164.9 MB (164914641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333082bc4516b0aeb21520abb86eecc31f08b6ed0c020598e2f0191242f3d8b9`  
		Last Modified: Sat, 28 Apr 2018 12:32:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d4a1cce90475c4e7ac57ddbdc2d54c1fbd714cd01ad340f7065323a3f662fe`  
		Last Modified: Sat, 28 Apr 2018 12:33:30 GMT  
		Size: 75.0 MB (75015814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0f7b9fee47153280362bb4ace6bd74e1f1665c93dca0b781f3e23c455898a742
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.0 MB (347963461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:911262005503e580de950c25cbe41b95752296011e4448d98d3bed828f5bd96c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:12:52 GMT
ADD file:fef3655a03a1c7f1533148016797b982955b3d5556f32c777214b8426028509b in / 
# Tue, 01 May 2018 01:12:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:13:04 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:13:10 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:13:20 GMT
CMD ["/bin/bash"]
# Tue, 01 May 2018 01:19:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:19:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 01:19:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 01:23:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:23:33 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 01:23:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 01:24:25 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 02:51:26 GMT
ENV ROS_DISTRO=lunar
# Tue, 01 May 2018 02:59:44 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 02:59:49 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 02:59:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 02:59:52 GMT
CMD ["bash"]
# Tue, 01 May 2018 03:06:57 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c016a9a148a71d05469a3994d54eb7eb9c3d40a65e07bf68788018a71d951b`  
		Last Modified: Mon, 23 Apr 2018 14:56:07 GMT  
		Size: 39.2 MB (39223827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1976297de94ed1f5c4c0f13b0b25199c6d6ca003ddfc3e873938aa2f8e86b`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d83417bbef32ed4713f4224bcb9f9573597ee6d91174dc7403ce457f145d2`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2544c5c45beca34c948aca9c981d56b587a973354727e4c97dc99d88227fb6a`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92ef1d410a96b276ec1425b000d80d5c1d914688aae8bce3e6f20d8a5a7a5f`  
		Last Modified: Tue, 01 May 2018 01:17:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3a2ac905d0d30502b9bf9736c755da2e7a05465764ff1fb14a45f067faa71c`  
		Last Modified: Tue, 01 May 2018 04:17:49 GMT  
		Size: 4.8 MB (4819486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31df2d860f2dc7f931faa244a38a740a44c732fd7ab480a29daf8999b5fb7fcd`  
		Last Modified: Tue, 01 May 2018 04:17:40 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a06299e2df93eba22547e7bbfaf291225cb3e1d85dcd160f7080d0d65647a`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ce03745d3f424b139a80266262e70dfefbda981c88ae34eac7b56df3120657`  
		Last Modified: Tue, 01 May 2018 04:18:42 GMT  
		Size: 52.4 MB (52441627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360b2687112930e2c2a443c4f89ecbdda5be0103c5b840e39840d3aca65352a`  
		Last Modified: Tue, 01 May 2018 04:17:41 GMT  
		Size: 835.1 KB (835081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dbca386e5c6b5ffe323554a2f8bf12b018dace7d69b3b4ba8c6f9e99ac97c8`  
		Last Modified: Tue, 01 May 2018 04:34:53 GMT  
		Size: 174.2 MB (174164133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6170ad5544fce2d65ed25da27444eaad1efb07f3af011b076ca66e054d4895a`  
		Last Modified: Tue, 01 May 2018 04:32:45 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973fc8cb4ca9d12fc8aabae8747ce1911197af7de290fe386c7de3d47da65d05`  
		Last Modified: Tue, 01 May 2018 04:35:43 GMT  
		Size: 76.5 MB (76463310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:lunar-ros-base-stretch`

```console
$ docker pull ros@sha256:f4a4592e6693181c1c47307dd1fd35bd6e5174e1eeabc384bfbd1ee854f3e373
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:lunar-ros-base-stretch` - linux; amd64

```console
$ docker pull ros@sha256:45a539a5d18ca807de75e9a35cf313adc05225550e76377efaa5d2e16b678cd4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.0 MB (491969002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:294bd4c567a407d2c90504775146545cb7a829292f9976e9db901da7d875c136`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 07:08:53 GMT
ADD file:9572fdb59dfbb9b032f3331bbc2a08b31e0aef5fbde44c8f2008d22bf5290cf2 in / 
# Sat, 28 Apr 2018 07:08:53 GMT
CMD ["bash"]
# Sun, 29 Apr 2018 12:52:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:52:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sun, 29 Apr 2018 12:52:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros-latest.list
# Sun, 29 Apr 2018 12:52:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:52:42 GMT
ENV LANG=C.UTF-8
# Sun, 29 Apr 2018 12:52:42 GMT
ENV LC_ALL=C.UTF-8
# Sun, 29 Apr 2018 12:52:54 GMT
RUN rosdep init     && rosdep update
# Sun, 29 Apr 2018 12:52:54 GMT
ENV ROS_DISTRO=lunar
# Sun, 29 Apr 2018 12:54:28 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:54:29 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sun, 29 Apr 2018 12:54:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 29 Apr 2018 12:54:29 GMT
CMD ["bash"]
# Sun, 29 Apr 2018 13:15:48 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc1a78bfd46becbfc3abb8a74d9a70a0e0dc7a5809bbd12e814f9382db003707`  
		Last Modified: Sat, 28 Apr 2018 09:27:54 GMT  
		Size: 45.3 MB (45318159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080d14fa56ef128c193fd94edf1e5eb031d02ae97b680588c7248e5e84304f13`  
		Last Modified: Sun, 29 Apr 2018 14:48:05 GMT  
		Size: 6.9 MB (6859072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604921583c4f613ebee4eb24564ca607566b8b48206868b48c018443567dd0b2`  
		Last Modified: Sun, 29 Apr 2018 14:48:03 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631afcce8e2d86cf9596b3823955679a3e770120d1da140a494003c85bf577b7`  
		Last Modified: Sun, 29 Apr 2018 14:48:00 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b0b4ce522ec73ddd931386acbe825b6203543509a3d76c51e649cb124d5ca1`  
		Last Modified: Sun, 29 Apr 2018 14:48:25 GMT  
		Size: 64.9 MB (64857453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea215428a3b38a4f7bc2be7aad6084d16a82bb84f706aebde2d34120ffc5190`  
		Last Modified: Sun, 29 Apr 2018 14:48:01 GMT  
		Size: 833.5 KB (833530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26629a9af11703b4ed3e40e78cb5403156db690083566f39f679a55e75c6fb67`  
		Last Modified: Sun, 29 Apr 2018 14:49:00 GMT  
		Size: 251.9 MB (251873129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b853450ebbc6b17d4b77840bb123c679eebd84b027b38915296bef615ae43600`  
		Last Modified: Sun, 29 Apr 2018 14:48:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63863f0fc73e348d8df8c2777a8ca0d09df3991f247fd340c53ae4264056544d`  
		Last Modified: Sun, 29 Apr 2018 15:01:25 GMT  
		Size: 122.2 MB (122225868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-ros-base-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4d3c94bfb1fa3bb8b5e046ba2f8a4806561d8a61ef561caf4cf0e5ff1f191996
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **435.1 MB (435129565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b95d94a4fe9849a429cc3cc742e4f8cbff789953b9cacda1b0c3cc38391902`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 30 Apr 2018 23:31:58 GMT
ADD file:245a8cfe59ea071e4e215a722e0d4b4b14fa95dd6ffd03739fe048433cfaf523 in / 
# Mon, 30 Apr 2018 23:32:00 GMT
CMD ["bash"]
# Tue, 01 May 2018 03:30:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:30:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 03:30:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 03:35:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:35:21 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 03:35:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 03:36:07 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 03:36:07 GMT
ENV ROS_DISTRO=lunar
# Tue, 01 May 2018 03:46:08 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:46:13 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 03:46:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 03:46:14 GMT
CMD ["bash"]
# Tue, 01 May 2018 03:51:28 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:142bf25d8d1b3ebc9dfbedd586e70a011594690acf48b2695bfce01e3a2cf0d5`  
		Last Modified: Mon, 30 Apr 2018 23:52:13 GMT  
		Size: 43.1 MB (43109349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994bacc3e1c11e50065156c511f0c11e001707e55b61e361b8dc44d236c76f24`  
		Last Modified: Tue, 01 May 2018 04:41:15 GMT  
		Size: 6.4 MB (6427112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663899231a010cf1e857473d7203c7e5f109b38379d2d822c31dba98a7f8af10`  
		Last Modified: Tue, 01 May 2018 04:41:09 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d68d9781734de3f7c1ce451752978a14ba285ad3c63d5ab58034a2008cd25ef`  
		Last Modified: Tue, 01 May 2018 04:41:06 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678cb4b8d2f95bf400236eedd95783c53081503a2ed2b39f51e57a6062cd18c7`  
		Last Modified: Tue, 01 May 2018 04:42:23 GMT  
		Size: 61.9 MB (61938600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0225d679802c170200a58607e1e5a805065659ce28bdec6f9cc91f1c5f6ac461`  
		Last Modified: Tue, 01 May 2018 04:41:08 GMT  
		Size: 835.1 KB (835084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8018c896d8c469869af751ab6dedae7d929c8c1eecd50bd607c44492245c688`  
		Last Modified: Tue, 01 May 2018 04:44:18 GMT  
		Size: 206.8 MB (206795100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4f80d568803a6e955c93890cfbb1629933a150a5d0a54e78f081bf2731b724`  
		Last Modified: Tue, 01 May 2018 04:41:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f59bacdd92efa26460f246475e05ca8c1d323676766477354f6c57571d53fa9`  
		Last Modified: Tue, 01 May 2018 04:45:14 GMT  
		Size: 116.0 MB (116022523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:lunar-ros-base-xenial`

```console
$ docker pull ros@sha256:de7b5f5cc43ffc2c0ea47e21715056b81fe5fa914250cef9164b2fba61854a0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:lunar-ros-base-xenial` - linux; amd64

```console
$ docker pull ros@sha256:090aa9b43c5825561a3a278153b6f7c14a68fe3065977fba9cf139c6f7f05c80
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **382.4 MB (382411487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a1e78d62416346ebef2833ea5ce2c0959c49f9a1fa314be34ea503322ccf28c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:52 GMT
ADD file:d37ff24540ea7700d0fc053e1996b234428a88f3a324d7fcbd83d8ef95318040 in / 
# Tue, 05 Jun 2018 21:21:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:54 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:55 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:35:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:35:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:35:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:36:43 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 23:04:04 GMT
ENV ROS_DISTRO=lunar
# Tue, 05 Jun 2018 23:08:25 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 23:08:27 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 23:08:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 23:08:27 GMT
CMD ["bash"]
# Tue, 05 Jun 2018 23:11:38 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b234f539f7a1d65eabae1617e63c81ac01768abffd48b5cbbf7166efca6a3429`  
		Last Modified: Mon, 28 May 2018 14:57:20 GMT  
		Size: 43.1 MB (43122477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55172d420b43cf03feeec11bcc917c7ddfc192036102e065ab57aa9abb95311e`  
		Last Modified: Tue, 05 Jun 2018 21:24:52 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba5bbeb6b91e2676c98255c6babc66d7b05cac40185eeba4b3773199c701da0`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ae2841ad7a7fd1aeae30028105cac7f6ee0ec955e5229e52b3333fea3c17b5`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c9c6de41905e9a66f2bc2c4a19858c8dc5b0a94f01e03eafc719afe25888aa`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22c30eae0b9363cecd2e5ac27a92dd1bc354e2e16a3ee82b70932814b4c12a`  
		Last Modified: Wed, 06 Jun 2018 00:11:32 GMT  
		Size: 5.4 MB (5362202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fce58d2960dc3a1265e5bc18474d652795940cafde67d662929605c9e3b1c44`  
		Last Modified: Wed, 06 Jun 2018 00:11:29 GMT  
		Size: 13.1 KB (13081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a8410e99e70f8971b54ce991fecd04014ef363a7dde349dd255d6358a6893d`  
		Last Modified: Wed, 06 Jun 2018 00:11:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3037b7978826369126bbe26cbb5d642f59ccd31d96e28044f872cd3eac55ab`  
		Last Modified: Wed, 06 Jun 2018 00:11:55 GMT  
		Size: 55.6 MB (55571338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cfa8aa4c1f7b161f88b862221bacc540052abfa4f8a11884d0090ebcd55cf9`  
		Last Modified: Wed, 06 Jun 2018 00:11:27 GMT  
		Size: 866.4 KB (866393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f170ce1e7cb1fdb2828bd6d23958f58b3be2174117f4f6e52d753d4c1422755d`  
		Last Modified: Wed, 06 Jun 2018 00:23:44 GMT  
		Size: 193.6 MB (193641819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0eb07e8e7dea220978bd30a26bf318649bf3cef13901c943bee38ed05afbede`  
		Last Modified: Wed, 06 Jun 2018 00:22:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dec063ced0219e39083dbd6fe65cc6f033c293b408910fcd3495c0928558874`  
		Last Modified: Wed, 06 Jun 2018 00:24:38 GMT  
		Size: 83.8 MB (83831267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-ros-base-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:9bd1c7651a0551f4d2b7d6c5638e12a4087b3474e25d9e506469f0cf79c38e2a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.2 MB (334192284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b670e98de88ae0afdba3403479590682d0375233bc241fc2fab02c5ec3ef6e6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:05:33 GMT
ADD file:1e3efdebaf133af6b22e61da056500ff8cf5292f051296f69abd35f44da5625c in / 
# Sat, 28 Apr 2018 12:05:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:05:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:05:37 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:05:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:50 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 12:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:08:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 12:08:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 12:09:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 12:09:57 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 12:16:42 GMT
ENV ROS_DISTRO=lunar
# Sat, 28 Apr 2018 12:18:04 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:18:11 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 12:18:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 12:18:15 GMT
CMD ["bash"]
# Sat, 28 Apr 2018 12:19:38 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f68dc00194f474ccfe395953a935f0a65f37edc5e218b6f310f432b3866f9bac`  
		Last Modified: Sat, 28 Apr 2018 12:09:03 GMT  
		Size: 38.1 MB (38126697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281b914f46e3b5e9fac0f9436525399186a66cb5abb5403eed9940d4207e15b4`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b205ebc944011540b5d7c371fe39a5cb49890d018253fcd39db61040dfed3`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418c61fca2a7e383833d9b12bd7adf62e311bf6350037e68503fbbbdfb8cc2b`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b471dd10511e8664a33e00815086f40bdfd8c30a16f93b190084bb5bb8a993f`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5050587be2fd4accc805402daed25e9344bd052ced481a6ecd1a5754102cb84`  
		Last Modified: Sat, 28 Apr 2018 12:27:40 GMT  
		Size: 4.6 MB (4614906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334ce8d248512220d545aecf150f8b8172bbd3e4c62f9cdc4c1e814053440912`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d06c2ef1c00b3cb66443790e82ae98882427dfc78b0009b2b801bdd0387146`  
		Last Modified: Sat, 28 Apr 2018 12:27:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b97dba49af961b21651a5255033ef01a2c0100029e05207d73befd0c45f6d85`  
		Last Modified: Sat, 28 Apr 2018 12:27:55 GMT  
		Size: 50.7 MB (50671071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1310601b6139b280f88b623eeaef6873b2ed293d2e09bc94346f6a444ab9973`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 833.2 KB (833166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08118158eff956ccf6049e24b2f4fdc1f4450a505d85654be6726518a4e26b48`  
		Last Modified: Sat, 28 Apr 2018 12:32:52 GMT  
		Size: 164.9 MB (164914641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333082bc4516b0aeb21520abb86eecc31f08b6ed0c020598e2f0191242f3d8b9`  
		Last Modified: Sat, 28 Apr 2018 12:32:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d4a1cce90475c4e7ac57ddbdc2d54c1fbd714cd01ad340f7065323a3f662fe`  
		Last Modified: Sat, 28 Apr 2018 12:33:30 GMT  
		Size: 75.0 MB (75015814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-ros-base-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0f7b9fee47153280362bb4ace6bd74e1f1665c93dca0b781f3e23c455898a742
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.0 MB (347963461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:911262005503e580de950c25cbe41b95752296011e4448d98d3bed828f5bd96c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:12:52 GMT
ADD file:fef3655a03a1c7f1533148016797b982955b3d5556f32c777214b8426028509b in / 
# Tue, 01 May 2018 01:12:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:13:04 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:13:10 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:13:20 GMT
CMD ["/bin/bash"]
# Tue, 01 May 2018 01:19:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:19:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 01:19:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 01:23:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:23:33 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 01:23:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 01:24:25 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 02:51:26 GMT
ENV ROS_DISTRO=lunar
# Tue, 01 May 2018 02:59:44 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 02:59:49 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 02:59:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 02:59:52 GMT
CMD ["bash"]
# Tue, 01 May 2018 03:06:57 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-base=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c016a9a148a71d05469a3994d54eb7eb9c3d40a65e07bf68788018a71d951b`  
		Last Modified: Mon, 23 Apr 2018 14:56:07 GMT  
		Size: 39.2 MB (39223827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1976297de94ed1f5c4c0f13b0b25199c6d6ca003ddfc3e873938aa2f8e86b`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d83417bbef32ed4713f4224bcb9f9573597ee6d91174dc7403ce457f145d2`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2544c5c45beca34c948aca9c981d56b587a973354727e4c97dc99d88227fb6a`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92ef1d410a96b276ec1425b000d80d5c1d914688aae8bce3e6f20d8a5a7a5f`  
		Last Modified: Tue, 01 May 2018 01:17:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3a2ac905d0d30502b9bf9736c755da2e7a05465764ff1fb14a45f067faa71c`  
		Last Modified: Tue, 01 May 2018 04:17:49 GMT  
		Size: 4.8 MB (4819486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31df2d860f2dc7f931faa244a38a740a44c732fd7ab480a29daf8999b5fb7fcd`  
		Last Modified: Tue, 01 May 2018 04:17:40 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a06299e2df93eba22547e7bbfaf291225cb3e1d85dcd160f7080d0d65647a`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ce03745d3f424b139a80266262e70dfefbda981c88ae34eac7b56df3120657`  
		Last Modified: Tue, 01 May 2018 04:18:42 GMT  
		Size: 52.4 MB (52441627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360b2687112930e2c2a443c4f89ecbdda5be0103c5b840e39840d3aca65352a`  
		Last Modified: Tue, 01 May 2018 04:17:41 GMT  
		Size: 835.1 KB (835081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dbca386e5c6b5ffe323554a2f8bf12b018dace7d69b3b4ba8c6f9e99ac97c8`  
		Last Modified: Tue, 01 May 2018 04:34:53 GMT  
		Size: 174.2 MB (174164133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6170ad5544fce2d65ed25da27444eaad1efb07f3af011b076ca66e054d4895a`  
		Last Modified: Tue, 01 May 2018 04:32:45 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973fc8cb4ca9d12fc8aabae8747ce1911197af7de290fe386c7de3d47da65d05`  
		Last Modified: Tue, 01 May 2018 04:35:43 GMT  
		Size: 76.5 MB (76463310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:lunar-ros-core`

```console
$ docker pull ros@sha256:90ed8159c6dfdf67a48851449d820980144792598c3a75e89924278052b7e3dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:lunar-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:ddd78cea959d25b627f8c661fa3661e4a2e3c41df305b8a6ee6f98abaf56ebed
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298580220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fbc082f8d2fc6e6e60ec9bf8f3043a960d82e777f495bffb648712cb68663eb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:52 GMT
ADD file:d37ff24540ea7700d0fc053e1996b234428a88f3a324d7fcbd83d8ef95318040 in / 
# Tue, 05 Jun 2018 21:21:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:54 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:55 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:35:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:35:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:35:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:36:43 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 23:04:04 GMT
ENV ROS_DISTRO=lunar
# Tue, 05 Jun 2018 23:08:25 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 23:08:27 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 23:08:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 23:08:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b234f539f7a1d65eabae1617e63c81ac01768abffd48b5cbbf7166efca6a3429`  
		Last Modified: Mon, 28 May 2018 14:57:20 GMT  
		Size: 43.1 MB (43122477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55172d420b43cf03feeec11bcc917c7ddfc192036102e065ab57aa9abb95311e`  
		Last Modified: Tue, 05 Jun 2018 21:24:52 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba5bbeb6b91e2676c98255c6babc66d7b05cac40185eeba4b3773199c701da0`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ae2841ad7a7fd1aeae30028105cac7f6ee0ec955e5229e52b3333fea3c17b5`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c9c6de41905e9a66f2bc2c4a19858c8dc5b0a94f01e03eafc719afe25888aa`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22c30eae0b9363cecd2e5ac27a92dd1bc354e2e16a3ee82b70932814b4c12a`  
		Last Modified: Wed, 06 Jun 2018 00:11:32 GMT  
		Size: 5.4 MB (5362202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fce58d2960dc3a1265e5bc18474d652795940cafde67d662929605c9e3b1c44`  
		Last Modified: Wed, 06 Jun 2018 00:11:29 GMT  
		Size: 13.1 KB (13081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a8410e99e70f8971b54ce991fecd04014ef363a7dde349dd255d6358a6893d`  
		Last Modified: Wed, 06 Jun 2018 00:11:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3037b7978826369126bbe26cbb5d642f59ccd31d96e28044f872cd3eac55ab`  
		Last Modified: Wed, 06 Jun 2018 00:11:55 GMT  
		Size: 55.6 MB (55571338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cfa8aa4c1f7b161f88b862221bacc540052abfa4f8a11884d0090ebcd55cf9`  
		Last Modified: Wed, 06 Jun 2018 00:11:27 GMT  
		Size: 866.4 KB (866393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f170ce1e7cb1fdb2828bd6d23958f58b3be2174117f4f6e52d753d4c1422755d`  
		Last Modified: Wed, 06 Jun 2018 00:23:44 GMT  
		Size: 193.6 MB (193641819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0eb07e8e7dea220978bd30a26bf318649bf3cef13901c943bee38ed05afbede`  
		Last Modified: Wed, 06 Jun 2018 00:22:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:3c47dc7b22cc9c60001de030f86b0c0af97fcd393de5d48bca688896dbc368ea
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.2 MB (259176470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:964265330a93de83d8633f39951f21cd92fd2c55969d17a6d02fd68c7b08974d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:05:33 GMT
ADD file:1e3efdebaf133af6b22e61da056500ff8cf5292f051296f69abd35f44da5625c in / 
# Sat, 28 Apr 2018 12:05:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:05:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:05:37 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:05:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:50 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 12:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:08:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 12:08:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 12:09:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 12:09:57 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 12:16:42 GMT
ENV ROS_DISTRO=lunar
# Sat, 28 Apr 2018 12:18:04 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:18:11 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 12:18:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 12:18:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f68dc00194f474ccfe395953a935f0a65f37edc5e218b6f310f432b3866f9bac`  
		Last Modified: Sat, 28 Apr 2018 12:09:03 GMT  
		Size: 38.1 MB (38126697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281b914f46e3b5e9fac0f9436525399186a66cb5abb5403eed9940d4207e15b4`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b205ebc944011540b5d7c371fe39a5cb49890d018253fcd39db61040dfed3`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418c61fca2a7e383833d9b12bd7adf62e311bf6350037e68503fbbbdfb8cc2b`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b471dd10511e8664a33e00815086f40bdfd8c30a16f93b190084bb5bb8a993f`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5050587be2fd4accc805402daed25e9344bd052ced481a6ecd1a5754102cb84`  
		Last Modified: Sat, 28 Apr 2018 12:27:40 GMT  
		Size: 4.6 MB (4614906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334ce8d248512220d545aecf150f8b8172bbd3e4c62f9cdc4c1e814053440912`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d06c2ef1c00b3cb66443790e82ae98882427dfc78b0009b2b801bdd0387146`  
		Last Modified: Sat, 28 Apr 2018 12:27:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b97dba49af961b21651a5255033ef01a2c0100029e05207d73befd0c45f6d85`  
		Last Modified: Sat, 28 Apr 2018 12:27:55 GMT  
		Size: 50.7 MB (50671071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1310601b6139b280f88b623eeaef6873b2ed293d2e09bc94346f6a444ab9973`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 833.2 KB (833166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08118158eff956ccf6049e24b2f4fdc1f4450a505d85654be6726518a4e26b48`  
		Last Modified: Sat, 28 Apr 2018 12:32:52 GMT  
		Size: 164.9 MB (164914641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333082bc4516b0aeb21520abb86eecc31f08b6ed0c020598e2f0191242f3d8b9`  
		Last Modified: Sat, 28 Apr 2018 12:32:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c34f3c534626da603a4aedb738054f9c1b1a260d5252abdba36a7483700ee4b6
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.5 MB (271500151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00f3beabbd3352eb950cd66ccd82c08ff362a84ad32bc7d9cd302c8c2b4f9003`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:12:52 GMT
ADD file:fef3655a03a1c7f1533148016797b982955b3d5556f32c777214b8426028509b in / 
# Tue, 01 May 2018 01:12:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:13:04 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:13:10 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:13:20 GMT
CMD ["/bin/bash"]
# Tue, 01 May 2018 01:19:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:19:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 01:19:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 01:23:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:23:33 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 01:23:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 01:24:25 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 02:51:26 GMT
ENV ROS_DISTRO=lunar
# Tue, 01 May 2018 02:59:44 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 02:59:49 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 02:59:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 02:59:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:83c016a9a148a71d05469a3994d54eb7eb9c3d40a65e07bf68788018a71d951b`  
		Last Modified: Mon, 23 Apr 2018 14:56:07 GMT  
		Size: 39.2 MB (39223827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1976297de94ed1f5c4c0f13b0b25199c6d6ca003ddfc3e873938aa2f8e86b`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d83417bbef32ed4713f4224bcb9f9573597ee6d91174dc7403ce457f145d2`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2544c5c45beca34c948aca9c981d56b587a973354727e4c97dc99d88227fb6a`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92ef1d410a96b276ec1425b000d80d5c1d914688aae8bce3e6f20d8a5a7a5f`  
		Last Modified: Tue, 01 May 2018 01:17:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3a2ac905d0d30502b9bf9736c755da2e7a05465764ff1fb14a45f067faa71c`  
		Last Modified: Tue, 01 May 2018 04:17:49 GMT  
		Size: 4.8 MB (4819486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31df2d860f2dc7f931faa244a38a740a44c732fd7ab480a29daf8999b5fb7fcd`  
		Last Modified: Tue, 01 May 2018 04:17:40 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a06299e2df93eba22547e7bbfaf291225cb3e1d85dcd160f7080d0d65647a`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ce03745d3f424b139a80266262e70dfefbda981c88ae34eac7b56df3120657`  
		Last Modified: Tue, 01 May 2018 04:18:42 GMT  
		Size: 52.4 MB (52441627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360b2687112930e2c2a443c4f89ecbdda5be0103c5b840e39840d3aca65352a`  
		Last Modified: Tue, 01 May 2018 04:17:41 GMT  
		Size: 835.1 KB (835081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dbca386e5c6b5ffe323554a2f8bf12b018dace7d69b3b4ba8c6f9e99ac97c8`  
		Last Modified: Tue, 01 May 2018 04:34:53 GMT  
		Size: 174.2 MB (174164133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6170ad5544fce2d65ed25da27444eaad1efb07f3af011b076ca66e054d4895a`  
		Last Modified: Tue, 01 May 2018 04:32:45 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:lunar-ros-core-stretch`

```console
$ docker pull ros@sha256:2d8321ec420d7d308be029a09d610c49e842b037ccc89c2f19a99b49d3e94c50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:lunar-ros-core-stretch` - linux; amd64

```console
$ docker pull ros@sha256:1f8533233a6195c7c277b297b2746b45bc6df511812fe11ecab1be7901d7422d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **369.7 MB (369743134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24e7719ce8e79b2d6c2240399d87dc3ff8b047f95e5c342b4403e865632236b5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 07:08:53 GMT
ADD file:9572fdb59dfbb9b032f3331bbc2a08b31e0aef5fbde44c8f2008d22bf5290cf2 in / 
# Sat, 28 Apr 2018 07:08:53 GMT
CMD ["bash"]
# Sun, 29 Apr 2018 12:52:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:52:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sun, 29 Apr 2018 12:52:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros-latest.list
# Sun, 29 Apr 2018 12:52:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:52:42 GMT
ENV LANG=C.UTF-8
# Sun, 29 Apr 2018 12:52:42 GMT
ENV LC_ALL=C.UTF-8
# Sun, 29 Apr 2018 12:52:54 GMT
RUN rosdep init     && rosdep update
# Sun, 29 Apr 2018 12:52:54 GMT
ENV ROS_DISTRO=lunar
# Sun, 29 Apr 2018 12:54:28 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:54:29 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sun, 29 Apr 2018 12:54:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 29 Apr 2018 12:54:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cc1a78bfd46becbfc3abb8a74d9a70a0e0dc7a5809bbd12e814f9382db003707`  
		Last Modified: Sat, 28 Apr 2018 09:27:54 GMT  
		Size: 45.3 MB (45318159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080d14fa56ef128c193fd94edf1e5eb031d02ae97b680588c7248e5e84304f13`  
		Last Modified: Sun, 29 Apr 2018 14:48:05 GMT  
		Size: 6.9 MB (6859072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604921583c4f613ebee4eb24564ca607566b8b48206868b48c018443567dd0b2`  
		Last Modified: Sun, 29 Apr 2018 14:48:03 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631afcce8e2d86cf9596b3823955679a3e770120d1da140a494003c85bf577b7`  
		Last Modified: Sun, 29 Apr 2018 14:48:00 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b0b4ce522ec73ddd931386acbe825b6203543509a3d76c51e649cb124d5ca1`  
		Last Modified: Sun, 29 Apr 2018 14:48:25 GMT  
		Size: 64.9 MB (64857453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea215428a3b38a4f7bc2be7aad6084d16a82bb84f706aebde2d34120ffc5190`  
		Last Modified: Sun, 29 Apr 2018 14:48:01 GMT  
		Size: 833.5 KB (833530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26629a9af11703b4ed3e40e78cb5403156db690083566f39f679a55e75c6fb67`  
		Last Modified: Sun, 29 Apr 2018 14:49:00 GMT  
		Size: 251.9 MB (251873129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b853450ebbc6b17d4b77840bb123c679eebd84b027b38915296bef615ae43600`  
		Last Modified: Sun, 29 Apr 2018 14:48:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-ros-core-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:bee0b4e7b2ccf0f9ccc2e80e8bec9ea7b9a93cf70d2b08823e95809c4419a0c2
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.1 MB (319107042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5552bf8cdb65a4245d25f47103086b24fe08888c954267191d57784f923ef9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 30 Apr 2018 23:31:58 GMT
ADD file:245a8cfe59ea071e4e215a722e0d4b4b14fa95dd6ffd03739fe048433cfaf523 in / 
# Mon, 30 Apr 2018 23:32:00 GMT
CMD ["bash"]
# Tue, 01 May 2018 03:30:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:30:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 03:30:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 03:35:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:35:21 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 03:35:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 03:36:07 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 03:36:07 GMT
ENV ROS_DISTRO=lunar
# Tue, 01 May 2018 03:46:08 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:46:13 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 03:46:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 03:46:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:142bf25d8d1b3ebc9dfbedd586e70a011594690acf48b2695bfce01e3a2cf0d5`  
		Last Modified: Mon, 30 Apr 2018 23:52:13 GMT  
		Size: 43.1 MB (43109349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994bacc3e1c11e50065156c511f0c11e001707e55b61e361b8dc44d236c76f24`  
		Last Modified: Tue, 01 May 2018 04:41:15 GMT  
		Size: 6.4 MB (6427112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663899231a010cf1e857473d7203c7e5f109b38379d2d822c31dba98a7f8af10`  
		Last Modified: Tue, 01 May 2018 04:41:09 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d68d9781734de3f7c1ce451752978a14ba285ad3c63d5ab58034a2008cd25ef`  
		Last Modified: Tue, 01 May 2018 04:41:06 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678cb4b8d2f95bf400236eedd95783c53081503a2ed2b39f51e57a6062cd18c7`  
		Last Modified: Tue, 01 May 2018 04:42:23 GMT  
		Size: 61.9 MB (61938600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0225d679802c170200a58607e1e5a805065659ce28bdec6f9cc91f1c5f6ac461`  
		Last Modified: Tue, 01 May 2018 04:41:08 GMT  
		Size: 835.1 KB (835084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8018c896d8c469869af751ab6dedae7d929c8c1eecd50bd607c44492245c688`  
		Last Modified: Tue, 01 May 2018 04:44:18 GMT  
		Size: 206.8 MB (206795100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4f80d568803a6e955c93890cfbb1629933a150a5d0a54e78f081bf2731b724`  
		Last Modified: Tue, 01 May 2018 04:41:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:lunar-ros-core-xenial`

```console
$ docker pull ros@sha256:90ed8159c6dfdf67a48851449d820980144792598c3a75e89924278052b7e3dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:lunar-ros-core-xenial` - linux; amd64

```console
$ docker pull ros@sha256:ddd78cea959d25b627f8c661fa3661e4a2e3c41df305b8a6ee6f98abaf56ebed
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298580220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fbc082f8d2fc6e6e60ec9bf8f3043a960d82e777f495bffb648712cb68663eb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Jun 2018 21:21:52 GMT
ADD file:d37ff24540ea7700d0fc053e1996b234428a88f3a324d7fcbd83d8ef95318040 in / 
# Tue, 05 Jun 2018 21:21:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 05 Jun 2018 21:21:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 21:21:54 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 05 Jun 2018 21:21:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 05 Jun 2018 21:21:55 GMT
CMD ["/bin/bash"]
# Tue, 05 Jun 2018 22:35:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:35:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 05 Jun 2018 22:35:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 05 Jun 2018 22:36:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jun 2018 22:36:25 GMT
ENV LC_ALL=C.UTF-8
# Tue, 05 Jun 2018 22:36:43 GMT
RUN rosdep init     && rosdep update
# Tue, 05 Jun 2018 23:04:04 GMT
ENV ROS_DISTRO=lunar
# Tue, 05 Jun 2018 23:08:25 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Jun 2018 23:08:27 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 05 Jun 2018 23:08:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 05 Jun 2018 23:08:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b234f539f7a1d65eabae1617e63c81ac01768abffd48b5cbbf7166efca6a3429`  
		Last Modified: Mon, 28 May 2018 14:57:20 GMT  
		Size: 43.1 MB (43122477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55172d420b43cf03feeec11bcc917c7ddfc192036102e065ab57aa9abb95311e`  
		Last Modified: Tue, 05 Jun 2018 21:24:52 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba5bbeb6b91e2676c98255c6babc66d7b05cac40185eeba4b3773199c701da0`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ae2841ad7a7fd1aeae30028105cac7f6ee0ec955e5229e52b3333fea3c17b5`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c9c6de41905e9a66f2bc2c4a19858c8dc5b0a94f01e03eafc719afe25888aa`  
		Last Modified: Tue, 05 Jun 2018 21:24:50 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d22c30eae0b9363cecd2e5ac27a92dd1bc354e2e16a3ee82b70932814b4c12a`  
		Last Modified: Wed, 06 Jun 2018 00:11:32 GMT  
		Size: 5.4 MB (5362202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fce58d2960dc3a1265e5bc18474d652795940cafde67d662929605c9e3b1c44`  
		Last Modified: Wed, 06 Jun 2018 00:11:29 GMT  
		Size: 13.1 KB (13081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a8410e99e70f8971b54ce991fecd04014ef363a7dde349dd255d6358a6893d`  
		Last Modified: Wed, 06 Jun 2018 00:11:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3037b7978826369126bbe26cbb5d642f59ccd31d96e28044f872cd3eac55ab`  
		Last Modified: Wed, 06 Jun 2018 00:11:55 GMT  
		Size: 55.6 MB (55571338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cfa8aa4c1f7b161f88b862221bacc540052abfa4f8a11884d0090ebcd55cf9`  
		Last Modified: Wed, 06 Jun 2018 00:11:27 GMT  
		Size: 866.4 KB (866393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f170ce1e7cb1fdb2828bd6d23958f58b3be2174117f4f6e52d753d4c1422755d`  
		Last Modified: Wed, 06 Jun 2018 00:23:44 GMT  
		Size: 193.6 MB (193641819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0eb07e8e7dea220978bd30a26bf318649bf3cef13901c943bee38ed05afbede`  
		Last Modified: Wed, 06 Jun 2018 00:22:27 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-ros-core-xenial` - linux; arm variant v7

```console
$ docker pull ros@sha256:3c47dc7b22cc9c60001de030f86b0c0af97fcd393de5d48bca688896dbc368ea
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.2 MB (259176470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:964265330a93de83d8633f39951f21cd92fd2c55969d17a6d02fd68c7b08974d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:05:33 GMT
ADD file:1e3efdebaf133af6b22e61da056500ff8cf5292f051296f69abd35f44da5625c in / 
# Sat, 28 Apr 2018 12:05:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:05:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:05:37 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:05:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:05:50 GMT
CMD ["/bin/bash"]
# Sat, 28 Apr 2018 12:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:08:50 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sat, 28 Apr 2018 12:08:52 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Sat, 28 Apr 2018 12:09:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Apr 2018 12:09:34 GMT
ENV LC_ALL=C.UTF-8
# Sat, 28 Apr 2018 12:09:57 GMT
RUN rosdep init     && rosdep update
# Sat, 28 Apr 2018 12:16:42 GMT
ENV ROS_DISTRO=lunar
# Sat, 28 Apr 2018 12:18:04 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:18:11 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Sat, 28 Apr 2018 12:18:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 28 Apr 2018 12:18:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f68dc00194f474ccfe395953a935f0a65f37edc5e218b6f310f432b3866f9bac`  
		Last Modified: Sat, 28 Apr 2018 12:09:03 GMT  
		Size: 38.1 MB (38126697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281b914f46e3b5e9fac0f9436525399186a66cb5abb5403eed9940d4207e15b4`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b205ebc944011540b5d7c371fe39a5cb49890d018253fcd39db61040dfed3`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418c61fca2a7e383833d9b12bd7adf62e311bf6350037e68503fbbbdfb8cc2b`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b471dd10511e8664a33e00815086f40bdfd8c30a16f93b190084bb5bb8a993f`  
		Last Modified: Sat, 28 Apr 2018 12:08:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5050587be2fd4accc805402daed25e9344bd052ced481a6ecd1a5754102cb84`  
		Last Modified: Sat, 28 Apr 2018 12:27:40 GMT  
		Size: 4.6 MB (4614906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334ce8d248512220d545aecf150f8b8172bbd3e4c62f9cdc4c1e814053440912`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d06c2ef1c00b3cb66443790e82ae98882427dfc78b0009b2b801bdd0387146`  
		Last Modified: Sat, 28 Apr 2018 12:27:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b97dba49af961b21651a5255033ef01a2c0100029e05207d73befd0c45f6d85`  
		Last Modified: Sat, 28 Apr 2018 12:27:55 GMT  
		Size: 50.7 MB (50671071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1310601b6139b280f88b623eeaef6873b2ed293d2e09bc94346f6a444ab9973`  
		Last Modified: Sat, 28 Apr 2018 12:27:38 GMT  
		Size: 833.2 KB (833166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08118158eff956ccf6049e24b2f4fdc1f4450a505d85654be6726518a4e26b48`  
		Last Modified: Sat, 28 Apr 2018 12:32:52 GMT  
		Size: 164.9 MB (164914641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333082bc4516b0aeb21520abb86eecc31f08b6ed0c020598e2f0191242f3d8b9`  
		Last Modified: Sat, 28 Apr 2018 12:32:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:lunar-ros-core-xenial` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:c34f3c534626da603a4aedb738054f9c1b1a260d5252abdba36a7483700ee4b6
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.5 MB (271500151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00f3beabbd3352eb950cd66ccd82c08ff362a84ad32bc7d9cd302c8c2b4f9003`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:12:52 GMT
ADD file:fef3655a03a1c7f1533148016797b982955b3d5556f32c777214b8426028509b in / 
# Tue, 01 May 2018 01:12:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:13:04 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:13:10 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:13:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:13:20 GMT
CMD ["/bin/bash"]
# Tue, 01 May 2018 01:19:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:19:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 01:19:59 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 01:23:28 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:23:33 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 01:23:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 01:24:25 GMT
RUN rosdep init     && rosdep update
# Tue, 01 May 2018 02:51:26 GMT
ENV ROS_DISTRO=lunar
# Tue, 01 May 2018 02:59:44 GMT
RUN apt-get update && apt-get install -y     ros-lunar-ros-core=1.3.2-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 02:59:49 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Tue, 01 May 2018 02:59:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 01 May 2018 02:59:52 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:83c016a9a148a71d05469a3994d54eb7eb9c3d40a65e07bf68788018a71d951b`  
		Last Modified: Mon, 23 Apr 2018 14:56:07 GMT  
		Size: 39.2 MB (39223827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1976297de94ed1f5c4c0f13b0b25199c6d6ca003ddfc3e873938aa2f8e86b`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d83417bbef32ed4713f4224bcb9f9573597ee6d91174dc7403ce457f145d2`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2544c5c45beca34c948aca9c981d56b587a973354727e4c97dc99d88227fb6a`  
		Last Modified: Tue, 01 May 2018 01:17:18 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb92ef1d410a96b276ec1425b000d80d5c1d914688aae8bce3e6f20d8a5a7a5f`  
		Last Modified: Tue, 01 May 2018 01:17:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3a2ac905d0d30502b9bf9736c755da2e7a05465764ff1fb14a45f067faa71c`  
		Last Modified: Tue, 01 May 2018 04:17:49 GMT  
		Size: 4.8 MB (4819486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31df2d860f2dc7f931faa244a38a740a44c732fd7ab480a29daf8999b5fb7fcd`  
		Last Modified: Tue, 01 May 2018 04:17:40 GMT  
		Size: 13.1 KB (13082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a06299e2df93eba22547e7bbfaf291225cb3e1d85dcd160f7080d0d65647a`  
		Last Modified: Tue, 01 May 2018 04:17:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ce03745d3f424b139a80266262e70dfefbda981c88ae34eac7b56df3120657`  
		Last Modified: Tue, 01 May 2018 04:18:42 GMT  
		Size: 52.4 MB (52441627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360b2687112930e2c2a443c4f89ecbdda5be0103c5b840e39840d3aca65352a`  
		Last Modified: Tue, 01 May 2018 04:17:41 GMT  
		Size: 835.1 KB (835081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dbca386e5c6b5ffe323554a2f8bf12b018dace7d69b3b4ba8c6f9e99ac97c8`  
		Last Modified: Tue, 01 May 2018 04:34:53 GMT  
		Size: 174.2 MB (174164133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6170ad5544fce2d65ed25da27444eaad1efb07f3af011b076ca66e054d4895a`  
		Last Modified: Tue, 01 May 2018 04:32:45 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic`

```console
$ docker pull ros@sha256:65fa1c573112741d9bf457a4c01de50f383ce57281f3d196e79a02e7cba3e354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic` - linux; amd64

```console
$ docker pull ros@sha256:6cb9d04fe705668a8939f8d24b67370ec79cba45750cff9a3b4ac549dcf8c592
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **379.8 MB (379836490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8141688e843965dabe1111f59e049862a0c270b10da0cc85efa9beff999898f3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 27 Apr 2018 23:28:32 GMT
ADD file:81813d6023adb66b80fe163bc7db464004673838d17195b9d84aade4f8961b71 in / 
# Fri, 27 Apr 2018 23:28:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 27 Apr 2018 23:28:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 27 Apr 2018 23:28:35 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 27 Apr 2018 23:28:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 27 Apr 2018 23:28:36 GMT
CMD ["/bin/bash"]
# Tue, 15 May 2018 17:22:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 15 May 2018 17:22:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 15 May 2018 17:24:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:24:08 GMT
ENV LANG=C.UTF-8
# Tue, 15 May 2018 17:24:09 GMT
ENV LC_ALL=C.UTF-8
# Tue, 15 May 2018 17:24:19 GMT
RUN rosdep init     && rosdep update
# Tue, 15 May 2018 17:24:19 GMT
ENV ROS_DISTRO=melodic
# Thu, 24 May 2018 21:26:28 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:26:29 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Thu, 24 May 2018 21:26:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 24 May 2018 21:26:29 GMT
CMD ["bash"]
# Thu, 24 May 2018 21:29:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a48c500ed24e62926cb079df35f964c57d8bb08159b1d29c6a3b0a58dc365dc1`  
		Last Modified: Fri, 27 Apr 2018 22:14:33 GMT  
		Size: 31.0 MB (30957448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1de00ff7e1fea0858b6a4b5ca208eeca970607ea9a6eb5fc972494e7a0cdde`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0330ca45a200e1fcef05ae97f434366d262a1c50b3dc053e7928b58dd37211dd`  
		Last Modified: Fri, 27 Apr 2018 23:32:05 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471db38bcfbf0f5bac78012b9d458dfd37309d5cbb99d4e95310321a60a0cfdf`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4aba487617ca27519745ae722b8ea1917474c495b91b3c4887728a3f2ee7db`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8456edf85c693828820f7381dde166ac747f2cd8e10610d4c51120bc668379f`  
		Last Modified: Tue, 15 May 2018 18:06:38 GMT  
		Size: 831.1 KB (831054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2122c178c47e334cadb90a80317c074c9ab5b4ad3c03bd385e7b1cd3e348aa`  
		Last Modified: Tue, 15 May 2018 18:06:39 GMT  
		Size: 4.9 MB (4859414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d31beaa42936003685a0b05665d5767eeeddc4c318aaadc6fca1bba5debf2b`  
		Last Modified: Tue, 15 May 2018 18:06:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4b733826c103e038eda6e27b5f02bd3d2399d9c5c0a1af66b687989888289`  
		Last Modified: Tue, 15 May 2018 18:06:33 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c0ecb640b5f315f0d1dfa938e893872008c4f9a375a74e3c04c718e57bf3a5`  
		Last Modified: Tue, 15 May 2018 18:06:53 GMT  
		Size: 58.4 MB (58398228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae98d14520da6037aa61bc4046566731135de07187c4ea0f29030924bdcedb9`  
		Last Modified: Tue, 15 May 2018 18:06:35 GMT  
		Size: 848.9 KB (848891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5010f265d43daa5e2b9fbbbd090b2aa10b524945743a39cfd845a82379bd2f`  
		Last Modified: Thu, 24 May 2018 22:02:00 GMT  
		Size: 215.8 MB (215752594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0876834886b1318e9ec6eea07a901cde589827dacaef6c6179af7bb73bff5ea9`  
		Last Modified: Thu, 24 May 2018 22:01:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f4d2a0227e9474ba6418c71791baf644b56f14e7b6ab2389c7c9b071db5331`  
		Last Modified: Thu, 24 May 2018 22:02:53 GMT  
		Size: 68.2 MB (68184788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm variant v7

```console
$ docker pull ros@sha256:f46872e2c7c6a4cd2d6cf52a79b0ff955df4dc892b30856465400b371df39cd4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.9 MB (333902303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37417f98d377f368a74e8f07277aac34c9f2115dbd17839aed2f3494cdaeece`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:03:57 GMT
ADD file:5b2d516c09b4419925efe09e1b5c861cbd3a2d48ed47d6b2c7e571ec6d9ead64 in / 
# Sat, 28 Apr 2018 12:03:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:03:59 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:04:05 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:04:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:04:18 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 11:58:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 11:58:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 11:59:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:59:16 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 11:59:16 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 11:59:39 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 11:59:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 12:23:42 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 12:23:45 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 12:23:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 12:23:55 GMT
CMD ["bash"]
# Fri, 25 May 2018 12:25:08 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c68b3181adc7da3b2a5c9be4e228fe5b958ebee478e094e17cf4a61c60a75190`  
		Last Modified: Sat, 28 Apr 2018 12:06:55 GMT  
		Size: 26.5 MB (26487045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91be1119609b1847ebcb9f2621129540bc1fb01ca2c914cc9d03985f48513d24`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605e73e7288ab8c0b45ebed929576b45d7e024077e0f2ae8b1bfabc549e22b0f`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843bab014c7a7d380f7e5c7b7c205da6050bb6e3411217ebae052fae49a97708`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebf53478b460975ab3dc0b245e93b5121d21e03232fcef2d94cd838e034c3af`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ad074d342b779241149fc3fd8ca37e75b9985c3c0c75194f0baa6457643bc9`  
		Last Modified: Wed, 16 May 2018 12:07:02 GMT  
		Size: 831.2 KB (831191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2563139b45010cd554b552642217d24a54e56e1348796c0e156c8b1da6cb10`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 4.1 MB (4077205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a670c1a3040793070164343ff80a5fe224179f0542e8caa26ffdd706fc9a8f`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46573ec96640100c935e1de546d8e484aba5795ae4a439d06a5fce5ceb7bab17`  
		Last Modified: Wed, 16 May 2018 12:06:58 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c0d825eae387d208e3db5a3d2c211d2da64e3b8d2dd2eec5c4c4d33531d312`  
		Last Modified: Wed, 16 May 2018 12:07:17 GMT  
		Size: 53.3 MB (53260829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43be66fa479508bd5da868d645d6ac16277dab0c314790a1a45868b46042f4fd`  
		Last Modified: Wed, 16 May 2018 12:06:59 GMT  
		Size: 849.5 KB (849453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b73a800962eaa799f32d90e55a98ff0d75b6ec5f28b22a5e7a230c076eb77c`  
		Last Modified: Fri, 25 May 2018 12:31:35 GMT  
		Size: 188.4 MB (188390821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fff307b7b5e5b8f708310d05f17e3b91e9e87dff16e5e389a8efdf56ecbc62`  
		Last Modified: Fri, 25 May 2018 12:30:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fab2540810360b8fa43551847a14f4816b8a9d4a0e79958f8a8950a0079161`  
		Last Modified: Fri, 25 May 2018 12:32:35 GMT  
		Size: 60.0 MB (60001666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:421fe69542b69504d5185c436ab23bece33ea046c086ae3c6a28cd1b1416f87d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.0 MB (356993267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7a933463e40d905ead1f8ad4f817bbcd68225be7dd2476192fff9dc0d4ca2a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:10:30 GMT
ADD file:2738a1f35ded405c55bf8578757cc7a8a559fecd00a693b443369262b6dd3127 in / 
# Tue, 01 May 2018 01:10:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:10:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:11:00 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:11:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:11:09 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 09:17:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 09:18:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 09:20:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:20:22 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 09:20:23 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 09:21:02 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 09:21:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 14:59:45 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 14:59:50 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 14:59:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 14:59:51 GMT
CMD ["bash"]
# Fri, 25 May 2018 15:02:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5b73461db237fc125ed4bbd267b3cd588b6d3957c33cf7fc1d7f9aaf6dcd23fd`  
		Last Modified: Fri, 27 Apr 2018 22:48:27 GMT  
		Size: 27.9 MB (27906574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c642ceb6d4dae80623e35056b3672b999504c5a0cb5dfdd4017f3ff74c6613d8`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6b10168e4f59716c9bf42ae4d202df59f2177923f5e0c6a10228be5c719a2e`  
		Last Modified: Tue, 01 May 2018 01:15:00 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0393063bd61dd94962711e03eb55999a0f821b5939d53509bd5aaf041018dfd`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7da53af2791e4570af9528b9ac2c4487a67026625b4de48184810193f3aa76f`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c156a4d1ad7cd59ce110f77b00214890cbe16b288cc38dfddfe83e9a4cbf4c6`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 831.0 KB (830976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be34a6338091a5e6c7b3336a3410157dd78d861793b54433ff7d219681b4cd95`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 4.4 MB (4438186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17243111bd7f4cc4a686835d4f7d86a2a8a0f4e9cd0db83d23b3b13069bad744`  
		Last Modified: Wed, 16 May 2018 10:26:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e446f86bbda79f1e1d14edd48864be9d560d0705f48166af8f8275833fe37b2e`  
		Last Modified: Wed, 16 May 2018 10:26:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6301719156835f879808d742b36f8b71f5f44741b3081e6516c61a3165608e4`  
		Last Modified: Wed, 16 May 2018 10:26:28 GMT  
		Size: 56.3 MB (56321857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92cb898705c424115a56cd1f955c61c5731211890c95409572b1b64666e60af`  
		Last Modified: Wed, 16 May 2018 10:26:01 GMT  
		Size: 849.4 KB (849389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa2f2edfc54bc83efbb1aecee4ad233c58a7b6f678c0f27f5c95ec2d241795`  
		Last Modified: Fri, 25 May 2018 15:49:15 GMT  
		Size: 203.3 MB (203260535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a862ae50eb668fd467dd0529f7a65222c885a20ef8d430ae67c1ef80d6211e20`  
		Last Modified: Fri, 25 May 2018 15:48:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b4a39407c12801335afb2e67bf30ec79318c34459ca9c277d0fcc3b4d3aa22`  
		Last Modified: Fri, 25 May 2018 15:50:07 GMT  
		Size: 63.4 MB (63381662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception`

```console
$ docker pull ros@sha256:8b7456bc0be8f0b7b5cc4306ac203153f00b137412476f8ce33e795041c84d14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception` - linux; amd64

```console
$ docker pull ros@sha256:37aa7544c73f24b608265604e81e50064072d77e1a4eee986c5fe4fce569aa21
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **738.8 MB (738799863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8c3cf6e10bd2ee5fc43f440d13c7df98db6c7c2a4a2d95b730b22806e495ebd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 27 Apr 2018 23:28:32 GMT
ADD file:81813d6023adb66b80fe163bc7db464004673838d17195b9d84aade4f8961b71 in / 
# Fri, 27 Apr 2018 23:28:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 27 Apr 2018 23:28:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 27 Apr 2018 23:28:35 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 27 Apr 2018 23:28:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 27 Apr 2018 23:28:36 GMT
CMD ["/bin/bash"]
# Tue, 15 May 2018 17:22:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 15 May 2018 17:22:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 15 May 2018 17:24:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:24:08 GMT
ENV LANG=C.UTF-8
# Tue, 15 May 2018 17:24:09 GMT
ENV LC_ALL=C.UTF-8
# Tue, 15 May 2018 17:24:19 GMT
RUN rosdep init     && rosdep update
# Tue, 15 May 2018 17:24:19 GMT
ENV ROS_DISTRO=melodic
# Thu, 24 May 2018 21:26:28 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:26:29 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Thu, 24 May 2018 21:26:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 24 May 2018 21:26:29 GMT
CMD ["bash"]
# Thu, 24 May 2018 21:29:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:38:56 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a48c500ed24e62926cb079df35f964c57d8bb08159b1d29c6a3b0a58dc365dc1`  
		Last Modified: Fri, 27 Apr 2018 22:14:33 GMT  
		Size: 31.0 MB (30957448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1de00ff7e1fea0858b6a4b5ca208eeca970607ea9a6eb5fc972494e7a0cdde`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0330ca45a200e1fcef05ae97f434366d262a1c50b3dc053e7928b58dd37211dd`  
		Last Modified: Fri, 27 Apr 2018 23:32:05 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471db38bcfbf0f5bac78012b9d458dfd37309d5cbb99d4e95310321a60a0cfdf`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4aba487617ca27519745ae722b8ea1917474c495b91b3c4887728a3f2ee7db`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8456edf85c693828820f7381dde166ac747f2cd8e10610d4c51120bc668379f`  
		Last Modified: Tue, 15 May 2018 18:06:38 GMT  
		Size: 831.1 KB (831054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2122c178c47e334cadb90a80317c074c9ab5b4ad3c03bd385e7b1cd3e348aa`  
		Last Modified: Tue, 15 May 2018 18:06:39 GMT  
		Size: 4.9 MB (4859414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d31beaa42936003685a0b05665d5767eeeddc4c318aaadc6fca1bba5debf2b`  
		Last Modified: Tue, 15 May 2018 18:06:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4b733826c103e038eda6e27b5f02bd3d2399d9c5c0a1af66b687989888289`  
		Last Modified: Tue, 15 May 2018 18:06:33 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c0ecb640b5f315f0d1dfa938e893872008c4f9a375a74e3c04c718e57bf3a5`  
		Last Modified: Tue, 15 May 2018 18:06:53 GMT  
		Size: 58.4 MB (58398228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae98d14520da6037aa61bc4046566731135de07187c4ea0f29030924bdcedb9`  
		Last Modified: Tue, 15 May 2018 18:06:35 GMT  
		Size: 848.9 KB (848891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5010f265d43daa5e2b9fbbbd090b2aa10b524945743a39cfd845a82379bd2f`  
		Last Modified: Thu, 24 May 2018 22:02:00 GMT  
		Size: 215.8 MB (215752594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0876834886b1318e9ec6eea07a901cde589827dacaef6c6179af7bb73bff5ea9`  
		Last Modified: Thu, 24 May 2018 22:01:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f4d2a0227e9474ba6418c71791baf644b56f14e7b6ab2389c7c9b071db5331`  
		Last Modified: Thu, 24 May 2018 22:02:53 GMT  
		Size: 68.2 MB (68184788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ce61ff07b2bb82c0682f8922c4529de1256530e5bf076247ff9f1432e84eb4`  
		Last Modified: Thu, 24 May 2018 22:06:04 GMT  
		Size: 359.0 MB (358963373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:487499d6f4d05d6f354ad04ed39d9246e86931060335cd54715ef29951d673be
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **642.8 MB (642840259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5a161e4a534e4ad6e881da946240c5b80b836362e46e20c6cf1c4929b826c6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:03:57 GMT
ADD file:5b2d516c09b4419925efe09e1b5c861cbd3a2d48ed47d6b2c7e571ec6d9ead64 in / 
# Sat, 28 Apr 2018 12:03:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:03:59 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:04:05 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:04:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:04:18 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 11:58:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 11:58:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 11:59:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:59:16 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 11:59:16 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 11:59:39 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 11:59:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 12:23:42 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 12:23:45 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 12:23:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 12:23:55 GMT
CMD ["bash"]
# Fri, 25 May 2018 12:25:08 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 12:29:55 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c68b3181adc7da3b2a5c9be4e228fe5b958ebee478e094e17cf4a61c60a75190`  
		Last Modified: Sat, 28 Apr 2018 12:06:55 GMT  
		Size: 26.5 MB (26487045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91be1119609b1847ebcb9f2621129540bc1fb01ca2c914cc9d03985f48513d24`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605e73e7288ab8c0b45ebed929576b45d7e024077e0f2ae8b1bfabc549e22b0f`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843bab014c7a7d380f7e5c7b7c205da6050bb6e3411217ebae052fae49a97708`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebf53478b460975ab3dc0b245e93b5121d21e03232fcef2d94cd838e034c3af`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ad074d342b779241149fc3fd8ca37e75b9985c3c0c75194f0baa6457643bc9`  
		Last Modified: Wed, 16 May 2018 12:07:02 GMT  
		Size: 831.2 KB (831191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2563139b45010cd554b552642217d24a54e56e1348796c0e156c8b1da6cb10`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 4.1 MB (4077205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a670c1a3040793070164343ff80a5fe224179f0542e8caa26ffdd706fc9a8f`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46573ec96640100c935e1de546d8e484aba5795ae4a439d06a5fce5ceb7bab17`  
		Last Modified: Wed, 16 May 2018 12:06:58 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c0d825eae387d208e3db5a3d2c211d2da64e3b8d2dd2eec5c4c4d33531d312`  
		Last Modified: Wed, 16 May 2018 12:07:17 GMT  
		Size: 53.3 MB (53260829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43be66fa479508bd5da868d645d6ac16277dab0c314790a1a45868b46042f4fd`  
		Last Modified: Wed, 16 May 2018 12:06:59 GMT  
		Size: 849.5 KB (849453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b73a800962eaa799f32d90e55a98ff0d75b6ec5f28b22a5e7a230c076eb77c`  
		Last Modified: Fri, 25 May 2018 12:31:35 GMT  
		Size: 188.4 MB (188390821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fff307b7b5e5b8f708310d05f17e3b91e9e87dff16e5e389a8efdf56ecbc62`  
		Last Modified: Fri, 25 May 2018 12:30:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fab2540810360b8fa43551847a14f4816b8a9d4a0e79958f8a8950a0079161`  
		Last Modified: Fri, 25 May 2018 12:32:35 GMT  
		Size: 60.0 MB (60001666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec14bee7782e612cfac80b9bbb9f90624b0ea6f7db28aefb325c2d1fcf8f67fd`  
		Last Modified: Fri, 25 May 2018 12:36:34 GMT  
		Size: 308.9 MB (308937956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e88638b1f6e6e3fad795c0c39bf95f12e3a4c24fafe4475eab081c246d20f9c2
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **698.5 MB (698512055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e65df11038594e367f457d28babc17992d359caec3cd63378ed60b10c28f93`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:10:30 GMT
ADD file:2738a1f35ded405c55bf8578757cc7a8a559fecd00a693b443369262b6dd3127 in / 
# Tue, 01 May 2018 01:10:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:10:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:11:00 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:11:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:11:09 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 09:17:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 09:18:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 09:20:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:20:22 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 09:20:23 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 09:21:02 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 09:21:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 14:59:45 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 14:59:50 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 14:59:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 14:59:51 GMT
CMD ["bash"]
# Fri, 25 May 2018 15:02:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 15:18:42 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5b73461db237fc125ed4bbd267b3cd588b6d3957c33cf7fc1d7f9aaf6dcd23fd`  
		Last Modified: Fri, 27 Apr 2018 22:48:27 GMT  
		Size: 27.9 MB (27906574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c642ceb6d4dae80623e35056b3672b999504c5a0cb5dfdd4017f3ff74c6613d8`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6b10168e4f59716c9bf42ae4d202df59f2177923f5e0c6a10228be5c719a2e`  
		Last Modified: Tue, 01 May 2018 01:15:00 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0393063bd61dd94962711e03eb55999a0f821b5939d53509bd5aaf041018dfd`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7da53af2791e4570af9528b9ac2c4487a67026625b4de48184810193f3aa76f`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c156a4d1ad7cd59ce110f77b00214890cbe16b288cc38dfddfe83e9a4cbf4c6`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 831.0 KB (830976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be34a6338091a5e6c7b3336a3410157dd78d861793b54433ff7d219681b4cd95`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 4.4 MB (4438186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17243111bd7f4cc4a686835d4f7d86a2a8a0f4e9cd0db83d23b3b13069bad744`  
		Last Modified: Wed, 16 May 2018 10:26:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e446f86bbda79f1e1d14edd48864be9d560d0705f48166af8f8275833fe37b2e`  
		Last Modified: Wed, 16 May 2018 10:26:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6301719156835f879808d742b36f8b71f5f44741b3081e6516c61a3165608e4`  
		Last Modified: Wed, 16 May 2018 10:26:28 GMT  
		Size: 56.3 MB (56321857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92cb898705c424115a56cd1f955c61c5731211890c95409572b1b64666e60af`  
		Last Modified: Wed, 16 May 2018 10:26:01 GMT  
		Size: 849.4 KB (849389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa2f2edfc54bc83efbb1aecee4ad233c58a7b6f678c0f27f5c95ec2d241795`  
		Last Modified: Fri, 25 May 2018 15:49:15 GMT  
		Size: 203.3 MB (203260535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a862ae50eb668fd467dd0529f7a65222c885a20ef8d430ae67c1ef80d6211e20`  
		Last Modified: Fri, 25 May 2018 15:48:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b4a39407c12801335afb2e67bf30ec79318c34459ca9c277d0fcc3b4d3aa22`  
		Last Modified: Fri, 25 May 2018 15:50:07 GMT  
		Size: 63.4 MB (63381662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aab2bcd7690c0ad29b1476e3f7c49d2e602f4f0acc4e1237978ef162ddf43ac`  
		Last Modified: Fri, 25 May 2018 15:53:47 GMT  
		Size: 341.5 MB (341518788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:8b7456bc0be8f0b7b5cc4306ac203153f00b137412476f8ce33e795041c84d14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:37aa7544c73f24b608265604e81e50064072d77e1a4eee986c5fe4fce569aa21
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **738.8 MB (738799863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8c3cf6e10bd2ee5fc43f440d13c7df98db6c7c2a4a2d95b730b22806e495ebd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 27 Apr 2018 23:28:32 GMT
ADD file:81813d6023adb66b80fe163bc7db464004673838d17195b9d84aade4f8961b71 in / 
# Fri, 27 Apr 2018 23:28:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 27 Apr 2018 23:28:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 27 Apr 2018 23:28:35 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 27 Apr 2018 23:28:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 27 Apr 2018 23:28:36 GMT
CMD ["/bin/bash"]
# Tue, 15 May 2018 17:22:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 15 May 2018 17:22:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 15 May 2018 17:24:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:24:08 GMT
ENV LANG=C.UTF-8
# Tue, 15 May 2018 17:24:09 GMT
ENV LC_ALL=C.UTF-8
# Tue, 15 May 2018 17:24:19 GMT
RUN rosdep init     && rosdep update
# Tue, 15 May 2018 17:24:19 GMT
ENV ROS_DISTRO=melodic
# Thu, 24 May 2018 21:26:28 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:26:29 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Thu, 24 May 2018 21:26:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 24 May 2018 21:26:29 GMT
CMD ["bash"]
# Thu, 24 May 2018 21:29:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:38:56 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a48c500ed24e62926cb079df35f964c57d8bb08159b1d29c6a3b0a58dc365dc1`  
		Last Modified: Fri, 27 Apr 2018 22:14:33 GMT  
		Size: 31.0 MB (30957448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1de00ff7e1fea0858b6a4b5ca208eeca970607ea9a6eb5fc972494e7a0cdde`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0330ca45a200e1fcef05ae97f434366d262a1c50b3dc053e7928b58dd37211dd`  
		Last Modified: Fri, 27 Apr 2018 23:32:05 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471db38bcfbf0f5bac78012b9d458dfd37309d5cbb99d4e95310321a60a0cfdf`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4aba487617ca27519745ae722b8ea1917474c495b91b3c4887728a3f2ee7db`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8456edf85c693828820f7381dde166ac747f2cd8e10610d4c51120bc668379f`  
		Last Modified: Tue, 15 May 2018 18:06:38 GMT  
		Size: 831.1 KB (831054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2122c178c47e334cadb90a80317c074c9ab5b4ad3c03bd385e7b1cd3e348aa`  
		Last Modified: Tue, 15 May 2018 18:06:39 GMT  
		Size: 4.9 MB (4859414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d31beaa42936003685a0b05665d5767eeeddc4c318aaadc6fca1bba5debf2b`  
		Last Modified: Tue, 15 May 2018 18:06:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4b733826c103e038eda6e27b5f02bd3d2399d9c5c0a1af66b687989888289`  
		Last Modified: Tue, 15 May 2018 18:06:33 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c0ecb640b5f315f0d1dfa938e893872008c4f9a375a74e3c04c718e57bf3a5`  
		Last Modified: Tue, 15 May 2018 18:06:53 GMT  
		Size: 58.4 MB (58398228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae98d14520da6037aa61bc4046566731135de07187c4ea0f29030924bdcedb9`  
		Last Modified: Tue, 15 May 2018 18:06:35 GMT  
		Size: 848.9 KB (848891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5010f265d43daa5e2b9fbbbd090b2aa10b524945743a39cfd845a82379bd2f`  
		Last Modified: Thu, 24 May 2018 22:02:00 GMT  
		Size: 215.8 MB (215752594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0876834886b1318e9ec6eea07a901cde589827dacaef6c6179af7bb73bff5ea9`  
		Last Modified: Thu, 24 May 2018 22:01:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f4d2a0227e9474ba6418c71791baf644b56f14e7b6ab2389c7c9b071db5331`  
		Last Modified: Thu, 24 May 2018 22:02:53 GMT  
		Size: 68.2 MB (68184788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ce61ff07b2bb82c0682f8922c4529de1256530e5bf076247ff9f1432e84eb4`  
		Last Modified: Thu, 24 May 2018 22:06:04 GMT  
		Size: 359.0 MB (358963373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:487499d6f4d05d6f354ad04ed39d9246e86931060335cd54715ef29951d673be
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **642.8 MB (642840259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5a161e4a534e4ad6e881da946240c5b80b836362e46e20c6cf1c4929b826c6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:03:57 GMT
ADD file:5b2d516c09b4419925efe09e1b5c861cbd3a2d48ed47d6b2c7e571ec6d9ead64 in / 
# Sat, 28 Apr 2018 12:03:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:03:59 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:04:05 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:04:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:04:18 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 11:58:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 11:58:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 11:59:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:59:16 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 11:59:16 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 11:59:39 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 11:59:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 12:23:42 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 12:23:45 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 12:23:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 12:23:55 GMT
CMD ["bash"]
# Fri, 25 May 2018 12:25:08 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 12:29:55 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c68b3181adc7da3b2a5c9be4e228fe5b958ebee478e094e17cf4a61c60a75190`  
		Last Modified: Sat, 28 Apr 2018 12:06:55 GMT  
		Size: 26.5 MB (26487045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91be1119609b1847ebcb9f2621129540bc1fb01ca2c914cc9d03985f48513d24`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605e73e7288ab8c0b45ebed929576b45d7e024077e0f2ae8b1bfabc549e22b0f`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843bab014c7a7d380f7e5c7b7c205da6050bb6e3411217ebae052fae49a97708`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebf53478b460975ab3dc0b245e93b5121d21e03232fcef2d94cd838e034c3af`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ad074d342b779241149fc3fd8ca37e75b9985c3c0c75194f0baa6457643bc9`  
		Last Modified: Wed, 16 May 2018 12:07:02 GMT  
		Size: 831.2 KB (831191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2563139b45010cd554b552642217d24a54e56e1348796c0e156c8b1da6cb10`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 4.1 MB (4077205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a670c1a3040793070164343ff80a5fe224179f0542e8caa26ffdd706fc9a8f`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46573ec96640100c935e1de546d8e484aba5795ae4a439d06a5fce5ceb7bab17`  
		Last Modified: Wed, 16 May 2018 12:06:58 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c0d825eae387d208e3db5a3d2c211d2da64e3b8d2dd2eec5c4c4d33531d312`  
		Last Modified: Wed, 16 May 2018 12:07:17 GMT  
		Size: 53.3 MB (53260829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43be66fa479508bd5da868d645d6ac16277dab0c314790a1a45868b46042f4fd`  
		Last Modified: Wed, 16 May 2018 12:06:59 GMT  
		Size: 849.5 KB (849453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b73a800962eaa799f32d90e55a98ff0d75b6ec5f28b22a5e7a230c076eb77c`  
		Last Modified: Fri, 25 May 2018 12:31:35 GMT  
		Size: 188.4 MB (188390821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fff307b7b5e5b8f708310d05f17e3b91e9e87dff16e5e389a8efdf56ecbc62`  
		Last Modified: Fri, 25 May 2018 12:30:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fab2540810360b8fa43551847a14f4816b8a9d4a0e79958f8a8950a0079161`  
		Last Modified: Fri, 25 May 2018 12:32:35 GMT  
		Size: 60.0 MB (60001666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec14bee7782e612cfac80b9bbb9f90624b0ea6f7db28aefb325c2d1fcf8f67fd`  
		Last Modified: Fri, 25 May 2018 12:36:34 GMT  
		Size: 308.9 MB (308937956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e88638b1f6e6e3fad795c0c39bf95f12e3a4c24fafe4475eab081c246d20f9c2
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **698.5 MB (698512055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e65df11038594e367f457d28babc17992d359caec3cd63378ed60b10c28f93`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:10:30 GMT
ADD file:2738a1f35ded405c55bf8578757cc7a8a559fecd00a693b443369262b6dd3127 in / 
# Tue, 01 May 2018 01:10:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:10:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:11:00 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:11:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:11:09 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 09:17:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 09:18:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 09:20:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:20:22 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 09:20:23 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 09:21:02 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 09:21:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 14:59:45 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 14:59:50 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 14:59:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 14:59:51 GMT
CMD ["bash"]
# Fri, 25 May 2018 15:02:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 15:18:42 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5b73461db237fc125ed4bbd267b3cd588b6d3957c33cf7fc1d7f9aaf6dcd23fd`  
		Last Modified: Fri, 27 Apr 2018 22:48:27 GMT  
		Size: 27.9 MB (27906574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c642ceb6d4dae80623e35056b3672b999504c5a0cb5dfdd4017f3ff74c6613d8`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6b10168e4f59716c9bf42ae4d202df59f2177923f5e0c6a10228be5c719a2e`  
		Last Modified: Tue, 01 May 2018 01:15:00 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0393063bd61dd94962711e03eb55999a0f821b5939d53509bd5aaf041018dfd`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7da53af2791e4570af9528b9ac2c4487a67026625b4de48184810193f3aa76f`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c156a4d1ad7cd59ce110f77b00214890cbe16b288cc38dfddfe83e9a4cbf4c6`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 831.0 KB (830976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be34a6338091a5e6c7b3336a3410157dd78d861793b54433ff7d219681b4cd95`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 4.4 MB (4438186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17243111bd7f4cc4a686835d4f7d86a2a8a0f4e9cd0db83d23b3b13069bad744`  
		Last Modified: Wed, 16 May 2018 10:26:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e446f86bbda79f1e1d14edd48864be9d560d0705f48166af8f8275833fe37b2e`  
		Last Modified: Wed, 16 May 2018 10:26:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6301719156835f879808d742b36f8b71f5f44741b3081e6516c61a3165608e4`  
		Last Modified: Wed, 16 May 2018 10:26:28 GMT  
		Size: 56.3 MB (56321857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92cb898705c424115a56cd1f955c61c5731211890c95409572b1b64666e60af`  
		Last Modified: Wed, 16 May 2018 10:26:01 GMT  
		Size: 849.4 KB (849389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa2f2edfc54bc83efbb1aecee4ad233c58a7b6f678c0f27f5c95ec2d241795`  
		Last Modified: Fri, 25 May 2018 15:49:15 GMT  
		Size: 203.3 MB (203260535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a862ae50eb668fd467dd0529f7a65222c885a20ef8d430ae67c1ef80d6211e20`  
		Last Modified: Fri, 25 May 2018 15:48:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b4a39407c12801335afb2e67bf30ec79318c34459ca9c277d0fcc3b4d3aa22`  
		Last Modified: Fri, 25 May 2018 15:50:07 GMT  
		Size: 63.4 MB (63381662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aab2bcd7690c0ad29b1476e3f7c49d2e602f4f0acc4e1237978ef162ddf43ac`  
		Last Modified: Fri, 25 May 2018 15:53:47 GMT  
		Size: 341.5 MB (341518788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-perception-stretch`

```console
$ docker pull ros@sha256:0bf1b6db8d0c286e4581fac29e9293dd307c03a433f85cfb23398b2d43638544
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-perception-stretch` - linux; amd64

```console
$ docker pull ros@sha256:a4b3f173428206102b17281b8232f50080f3702a66b9a03a499c3a9d7b22206f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **876.8 MB (876766866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d34b1562b0b1923e88c7c0fdfc2738aab1afca32f12515845c6916e1fff96a38`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 07:08:53 GMT
ADD file:9572fdb59dfbb9b032f3331bbc2a08b31e0aef5fbde44c8f2008d22bf5290cf2 in / 
# Sat, 28 Apr 2018 07:08:53 GMT
CMD ["bash"]
# Sun, 29 Apr 2018 12:52:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:52:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sun, 29 Apr 2018 12:52:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros-latest.list
# Sun, 29 Apr 2018 12:52:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:52:42 GMT
ENV LANG=C.UTF-8
# Sun, 29 Apr 2018 12:52:42 GMT
ENV LC_ALL=C.UTF-8
# Sun, 29 Apr 2018 12:52:54 GMT
RUN rosdep init     && rosdep update
# Tue, 15 May 2018 17:47:59 GMT
ENV ROS_DISTRO=melodic
# Thu, 24 May 2018 21:46:06 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:46:07 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Thu, 24 May 2018 21:46:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 24 May 2018 21:46:07 GMT
CMD ["bash"]
# Thu, 24 May 2018 21:50:48 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:55:28 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc1a78bfd46becbfc3abb8a74d9a70a0e0dc7a5809bbd12e814f9382db003707`  
		Last Modified: Sat, 28 Apr 2018 09:27:54 GMT  
		Size: 45.3 MB (45318159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080d14fa56ef128c193fd94edf1e5eb031d02ae97b680588c7248e5e84304f13`  
		Last Modified: Sun, 29 Apr 2018 14:48:05 GMT  
		Size: 6.9 MB (6859072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604921583c4f613ebee4eb24564ca607566b8b48206868b48c018443567dd0b2`  
		Last Modified: Sun, 29 Apr 2018 14:48:03 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631afcce8e2d86cf9596b3823955679a3e770120d1da140a494003c85bf577b7`  
		Last Modified: Sun, 29 Apr 2018 14:48:00 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b0b4ce522ec73ddd931386acbe825b6203543509a3d76c51e649cb124d5ca1`  
		Last Modified: Sun, 29 Apr 2018 14:48:25 GMT  
		Size: 64.9 MB (64857453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea215428a3b38a4f7bc2be7aad6084d16a82bb84f706aebde2d34120ffc5190`  
		Last Modified: Sun, 29 Apr 2018 14:48:01 GMT  
		Size: 833.5 KB (833530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd9f60d7f6c7b6a8bb715d3a9803206d7a1eb5bfa04a9d74975b0ad026b77d1`  
		Last Modified: Thu, 24 May 2018 22:12:47 GMT  
		Size: 269.4 MB (269359856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117a3c26cbb3ca93f68e7314ae978a7e5baa750a43aa035c903facad8a260129`  
		Last Modified: Thu, 24 May 2018 22:11:40 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ffcec86733c2b1a3056d4d21fad1a14b11a3178d017035ab59c8a9bf3061ce`  
		Last Modified: Thu, 24 May 2018 22:13:28 GMT  
		Size: 108.5 MB (108461908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e320f79a3e94a10443ad3582eca653aa8942cd7ef5877374c8cffa2be45b5e4e`  
		Last Modified: Thu, 24 May 2018 22:18:58 GMT  
		Size: 381.1 MB (381075098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:5203f962c84f663f1de3734d022a207466a0d7e157c170e12ed676612f525bd1
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **794.4 MB (794366700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad2c483b56cc3cc1833b3556fce9a09ffec97cc29262837e359f0b824edcf5a8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 30 Apr 2018 23:31:58 GMT
ADD file:245a8cfe59ea071e4e215a722e0d4b4b14fa95dd6ffd03739fe048433cfaf523 in / 
# Mon, 30 Apr 2018 23:32:00 GMT
CMD ["bash"]
# Tue, 01 May 2018 03:30:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:30:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 03:30:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 03:35:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:35:21 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 03:35:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 03:36:07 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 09:54:49 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 15:27:35 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 15:27:40 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 15:27:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 15:27:41 GMT
CMD ["bash"]
# Fri, 25 May 2018 15:30:40 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 15:47:08 GMT
RUN apt-get update && apt-get install -y     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:142bf25d8d1b3ebc9dfbedd586e70a011594690acf48b2695bfce01e3a2cf0d5`  
		Last Modified: Mon, 30 Apr 2018 23:52:13 GMT  
		Size: 43.1 MB (43109349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994bacc3e1c11e50065156c511f0c11e001707e55b61e361b8dc44d236c76f24`  
		Last Modified: Tue, 01 May 2018 04:41:15 GMT  
		Size: 6.4 MB (6427112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663899231a010cf1e857473d7203c7e5f109b38379d2d822c31dba98a7f8af10`  
		Last Modified: Tue, 01 May 2018 04:41:09 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d68d9781734de3f7c1ce451752978a14ba285ad3c63d5ab58034a2008cd25ef`  
		Last Modified: Tue, 01 May 2018 04:41:06 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678cb4b8d2f95bf400236eedd95783c53081503a2ed2b39f51e57a6062cd18c7`  
		Last Modified: Tue, 01 May 2018 04:42:23 GMT  
		Size: 61.9 MB (61938600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0225d679802c170200a58607e1e5a805065659ce28bdec6f9cc91f1c5f6ac461`  
		Last Modified: Tue, 01 May 2018 04:41:08 GMT  
		Size: 835.1 KB (835084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ff3cd1cf2d3e46a7f8fe4a2e5e91ff0815a51d5c87cfd81a1b8932dea453b8`  
		Last Modified: Fri, 25 May 2018 15:55:33 GMT  
		Size: 223.5 MB (223512365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5879828040241eb3667bd05cbfcc6b14911bf87255edd35c912781995caeb5`  
		Last Modified: Fri, 25 May 2018 15:54:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c54d9a16ffc723b2aa54654d720d702140f7b6d858968eec2cd9e827e41f469`  
		Last Modified: Fri, 25 May 2018 15:56:23 GMT  
		Size: 102.9 MB (102929185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3589d7972c8745f949054779f9bc54d5142f34b56f7a7be1f0656fab81d71e37`  
		Last Modified: Fri, 25 May 2018 15:59:51 GMT  
		Size: 355.6 MB (355613209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot`

```console
$ docker pull ros@sha256:c4a631461c907473f4f493782cdd1c0203df068d2f6b4cc5f65b3b82cd497f34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:58e97f01f5fcf9c5aaf5d53c38cebb7fb730064324d028ba9fdc2b4f5e1c2291
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **417.4 MB (417423142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84338e847dc44c4b02963860e859668084c2012d05483f64e9ec3b91e8adf5b4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 27 Apr 2018 23:28:32 GMT
ADD file:81813d6023adb66b80fe163bc7db464004673838d17195b9d84aade4f8961b71 in / 
# Fri, 27 Apr 2018 23:28:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 27 Apr 2018 23:28:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 27 Apr 2018 23:28:35 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 27 Apr 2018 23:28:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 27 Apr 2018 23:28:36 GMT
CMD ["/bin/bash"]
# Tue, 15 May 2018 17:22:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 15 May 2018 17:22:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 15 May 2018 17:24:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:24:08 GMT
ENV LANG=C.UTF-8
# Tue, 15 May 2018 17:24:09 GMT
ENV LC_ALL=C.UTF-8
# Tue, 15 May 2018 17:24:19 GMT
RUN rosdep init     && rosdep update
# Tue, 15 May 2018 17:24:19 GMT
ENV ROS_DISTRO=melodic
# Thu, 24 May 2018 21:26:28 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:26:29 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Thu, 24 May 2018 21:26:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 24 May 2018 21:26:29 GMT
CMD ["bash"]
# Thu, 24 May 2018 21:29:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:30:58 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a48c500ed24e62926cb079df35f964c57d8bb08159b1d29c6a3b0a58dc365dc1`  
		Last Modified: Fri, 27 Apr 2018 22:14:33 GMT  
		Size: 31.0 MB (30957448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1de00ff7e1fea0858b6a4b5ca208eeca970607ea9a6eb5fc972494e7a0cdde`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0330ca45a200e1fcef05ae97f434366d262a1c50b3dc053e7928b58dd37211dd`  
		Last Modified: Fri, 27 Apr 2018 23:32:05 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471db38bcfbf0f5bac78012b9d458dfd37309d5cbb99d4e95310321a60a0cfdf`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4aba487617ca27519745ae722b8ea1917474c495b91b3c4887728a3f2ee7db`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8456edf85c693828820f7381dde166ac747f2cd8e10610d4c51120bc668379f`  
		Last Modified: Tue, 15 May 2018 18:06:38 GMT  
		Size: 831.1 KB (831054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2122c178c47e334cadb90a80317c074c9ab5b4ad3c03bd385e7b1cd3e348aa`  
		Last Modified: Tue, 15 May 2018 18:06:39 GMT  
		Size: 4.9 MB (4859414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d31beaa42936003685a0b05665d5767eeeddc4c318aaadc6fca1bba5debf2b`  
		Last Modified: Tue, 15 May 2018 18:06:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4b733826c103e038eda6e27b5f02bd3d2399d9c5c0a1af66b687989888289`  
		Last Modified: Tue, 15 May 2018 18:06:33 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c0ecb640b5f315f0d1dfa938e893872008c4f9a375a74e3c04c718e57bf3a5`  
		Last Modified: Tue, 15 May 2018 18:06:53 GMT  
		Size: 58.4 MB (58398228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae98d14520da6037aa61bc4046566731135de07187c4ea0f29030924bdcedb9`  
		Last Modified: Tue, 15 May 2018 18:06:35 GMT  
		Size: 848.9 KB (848891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5010f265d43daa5e2b9fbbbd090b2aa10b524945743a39cfd845a82379bd2f`  
		Last Modified: Thu, 24 May 2018 22:02:00 GMT  
		Size: 215.8 MB (215752594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0876834886b1318e9ec6eea07a901cde589827dacaef6c6179af7bb73bff5ea9`  
		Last Modified: Thu, 24 May 2018 22:01:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f4d2a0227e9474ba6418c71791baf644b56f14e7b6ab2389c7c9b071db5331`  
		Last Modified: Thu, 24 May 2018 22:02:53 GMT  
		Size: 68.2 MB (68184788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2943948cd18793ca949de95acfc3d5c683aa3e62f34e92aef3bc2885bed82832`  
		Last Modified: Thu, 24 May 2018 22:03:42 GMT  
		Size: 37.6 MB (37586652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:3f24a6538620ddd3ced5c530ae174f97cafcdd1970577c696124b9f1fe853278
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.1 MB (367116158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcc712bad262129ee6e54891ff330d9393fd4135e071455c91f9282146b67226`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:03:57 GMT
ADD file:5b2d516c09b4419925efe09e1b5c861cbd3a2d48ed47d6b2c7e571ec6d9ead64 in / 
# Sat, 28 Apr 2018 12:03:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:03:59 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:04:05 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:04:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:04:18 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 11:58:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 11:58:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 11:59:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:59:16 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 11:59:16 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 11:59:39 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 11:59:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 12:23:42 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 12:23:45 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 12:23:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 12:23:55 GMT
CMD ["bash"]
# Fri, 25 May 2018 12:25:08 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 12:26:07 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c68b3181adc7da3b2a5c9be4e228fe5b958ebee478e094e17cf4a61c60a75190`  
		Last Modified: Sat, 28 Apr 2018 12:06:55 GMT  
		Size: 26.5 MB (26487045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91be1119609b1847ebcb9f2621129540bc1fb01ca2c914cc9d03985f48513d24`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605e73e7288ab8c0b45ebed929576b45d7e024077e0f2ae8b1bfabc549e22b0f`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843bab014c7a7d380f7e5c7b7c205da6050bb6e3411217ebae052fae49a97708`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebf53478b460975ab3dc0b245e93b5121d21e03232fcef2d94cd838e034c3af`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ad074d342b779241149fc3fd8ca37e75b9985c3c0c75194f0baa6457643bc9`  
		Last Modified: Wed, 16 May 2018 12:07:02 GMT  
		Size: 831.2 KB (831191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2563139b45010cd554b552642217d24a54e56e1348796c0e156c8b1da6cb10`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 4.1 MB (4077205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a670c1a3040793070164343ff80a5fe224179f0542e8caa26ffdd706fc9a8f`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46573ec96640100c935e1de546d8e484aba5795ae4a439d06a5fce5ceb7bab17`  
		Last Modified: Wed, 16 May 2018 12:06:58 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c0d825eae387d208e3db5a3d2c211d2da64e3b8d2dd2eec5c4c4d33531d312`  
		Last Modified: Wed, 16 May 2018 12:07:17 GMT  
		Size: 53.3 MB (53260829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43be66fa479508bd5da868d645d6ac16277dab0c314790a1a45868b46042f4fd`  
		Last Modified: Wed, 16 May 2018 12:06:59 GMT  
		Size: 849.5 KB (849453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b73a800962eaa799f32d90e55a98ff0d75b6ec5f28b22a5e7a230c076eb77c`  
		Last Modified: Fri, 25 May 2018 12:31:35 GMT  
		Size: 188.4 MB (188390821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fff307b7b5e5b8f708310d05f17e3b91e9e87dff16e5e389a8efdf56ecbc62`  
		Last Modified: Fri, 25 May 2018 12:30:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fab2540810360b8fa43551847a14f4816b8a9d4a0e79958f8a8950a0079161`  
		Last Modified: Fri, 25 May 2018 12:32:35 GMT  
		Size: 60.0 MB (60001666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9e0ceb30682e2089e5daddb32daee700a048f85cb3d9d2e0927e89b2cc6ffa`  
		Last Modified: Fri, 25 May 2018 12:34:22 GMT  
		Size: 33.2 MB (33213855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6696597b6c6f9df3b19589521722980da60a7fb4d9fd90749a8f3f0ace93d3f9
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.4 MB (392365714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffd1c712e57df3ba42413e8197367ddb7ee89b341dae2d289b84b769e4d4acd2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:10:30 GMT
ADD file:2738a1f35ded405c55bf8578757cc7a8a559fecd00a693b443369262b6dd3127 in / 
# Tue, 01 May 2018 01:10:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:10:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:11:00 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:11:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:11:09 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 09:17:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 09:18:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 09:20:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:20:22 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 09:20:23 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 09:21:02 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 09:21:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 14:59:45 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 14:59:50 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 14:59:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 14:59:51 GMT
CMD ["bash"]
# Fri, 25 May 2018 15:02:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 15:05:37 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5b73461db237fc125ed4bbd267b3cd588b6d3957c33cf7fc1d7f9aaf6dcd23fd`  
		Last Modified: Fri, 27 Apr 2018 22:48:27 GMT  
		Size: 27.9 MB (27906574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c642ceb6d4dae80623e35056b3672b999504c5a0cb5dfdd4017f3ff74c6613d8`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6b10168e4f59716c9bf42ae4d202df59f2177923f5e0c6a10228be5c719a2e`  
		Last Modified: Tue, 01 May 2018 01:15:00 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0393063bd61dd94962711e03eb55999a0f821b5939d53509bd5aaf041018dfd`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7da53af2791e4570af9528b9ac2c4487a67026625b4de48184810193f3aa76f`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c156a4d1ad7cd59ce110f77b00214890cbe16b288cc38dfddfe83e9a4cbf4c6`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 831.0 KB (830976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be34a6338091a5e6c7b3336a3410157dd78d861793b54433ff7d219681b4cd95`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 4.4 MB (4438186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17243111bd7f4cc4a686835d4f7d86a2a8a0f4e9cd0db83d23b3b13069bad744`  
		Last Modified: Wed, 16 May 2018 10:26:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e446f86bbda79f1e1d14edd48864be9d560d0705f48166af8f8275833fe37b2e`  
		Last Modified: Wed, 16 May 2018 10:26:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6301719156835f879808d742b36f8b71f5f44741b3081e6516c61a3165608e4`  
		Last Modified: Wed, 16 May 2018 10:26:28 GMT  
		Size: 56.3 MB (56321857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92cb898705c424115a56cd1f955c61c5731211890c95409572b1b64666e60af`  
		Last Modified: Wed, 16 May 2018 10:26:01 GMT  
		Size: 849.4 KB (849389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa2f2edfc54bc83efbb1aecee4ad233c58a7b6f678c0f27f5c95ec2d241795`  
		Last Modified: Fri, 25 May 2018 15:49:15 GMT  
		Size: 203.3 MB (203260535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a862ae50eb668fd467dd0529f7a65222c885a20ef8d430ae67c1ef80d6211e20`  
		Last Modified: Fri, 25 May 2018 15:48:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b4a39407c12801335afb2e67bf30ec79318c34459ca9c277d0fcc3b4d3aa22`  
		Last Modified: Fri, 25 May 2018 15:50:07 GMT  
		Size: 63.4 MB (63381662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25bab31be7a7cebe9e1e4ce4193687b612805d59fa9b7be772181a70bb72ec0`  
		Last Modified: Fri, 25 May 2018 15:51:05 GMT  
		Size: 35.4 MB (35372447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:c4a631461c907473f4f493782cdd1c0203df068d2f6b4cc5f65b3b82cd497f34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:58e97f01f5fcf9c5aaf5d53c38cebb7fb730064324d028ba9fdc2b4f5e1c2291
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **417.4 MB (417423142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84338e847dc44c4b02963860e859668084c2012d05483f64e9ec3b91e8adf5b4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 27 Apr 2018 23:28:32 GMT
ADD file:81813d6023adb66b80fe163bc7db464004673838d17195b9d84aade4f8961b71 in / 
# Fri, 27 Apr 2018 23:28:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 27 Apr 2018 23:28:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 27 Apr 2018 23:28:35 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 27 Apr 2018 23:28:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 27 Apr 2018 23:28:36 GMT
CMD ["/bin/bash"]
# Tue, 15 May 2018 17:22:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 15 May 2018 17:22:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 15 May 2018 17:24:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:24:08 GMT
ENV LANG=C.UTF-8
# Tue, 15 May 2018 17:24:09 GMT
ENV LC_ALL=C.UTF-8
# Tue, 15 May 2018 17:24:19 GMT
RUN rosdep init     && rosdep update
# Tue, 15 May 2018 17:24:19 GMT
ENV ROS_DISTRO=melodic
# Thu, 24 May 2018 21:26:28 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:26:29 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Thu, 24 May 2018 21:26:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 24 May 2018 21:26:29 GMT
CMD ["bash"]
# Thu, 24 May 2018 21:29:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:30:58 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a48c500ed24e62926cb079df35f964c57d8bb08159b1d29c6a3b0a58dc365dc1`  
		Last Modified: Fri, 27 Apr 2018 22:14:33 GMT  
		Size: 31.0 MB (30957448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1de00ff7e1fea0858b6a4b5ca208eeca970607ea9a6eb5fc972494e7a0cdde`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0330ca45a200e1fcef05ae97f434366d262a1c50b3dc053e7928b58dd37211dd`  
		Last Modified: Fri, 27 Apr 2018 23:32:05 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471db38bcfbf0f5bac78012b9d458dfd37309d5cbb99d4e95310321a60a0cfdf`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4aba487617ca27519745ae722b8ea1917474c495b91b3c4887728a3f2ee7db`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8456edf85c693828820f7381dde166ac747f2cd8e10610d4c51120bc668379f`  
		Last Modified: Tue, 15 May 2018 18:06:38 GMT  
		Size: 831.1 KB (831054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2122c178c47e334cadb90a80317c074c9ab5b4ad3c03bd385e7b1cd3e348aa`  
		Last Modified: Tue, 15 May 2018 18:06:39 GMT  
		Size: 4.9 MB (4859414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d31beaa42936003685a0b05665d5767eeeddc4c318aaadc6fca1bba5debf2b`  
		Last Modified: Tue, 15 May 2018 18:06:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4b733826c103e038eda6e27b5f02bd3d2399d9c5c0a1af66b687989888289`  
		Last Modified: Tue, 15 May 2018 18:06:33 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c0ecb640b5f315f0d1dfa938e893872008c4f9a375a74e3c04c718e57bf3a5`  
		Last Modified: Tue, 15 May 2018 18:06:53 GMT  
		Size: 58.4 MB (58398228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae98d14520da6037aa61bc4046566731135de07187c4ea0f29030924bdcedb9`  
		Last Modified: Tue, 15 May 2018 18:06:35 GMT  
		Size: 848.9 KB (848891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5010f265d43daa5e2b9fbbbd090b2aa10b524945743a39cfd845a82379bd2f`  
		Last Modified: Thu, 24 May 2018 22:02:00 GMT  
		Size: 215.8 MB (215752594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0876834886b1318e9ec6eea07a901cde589827dacaef6c6179af7bb73bff5ea9`  
		Last Modified: Thu, 24 May 2018 22:01:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f4d2a0227e9474ba6418c71791baf644b56f14e7b6ab2389c7c9b071db5331`  
		Last Modified: Thu, 24 May 2018 22:02:53 GMT  
		Size: 68.2 MB (68184788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2943948cd18793ca949de95acfc3d5c683aa3e62f34e92aef3bc2885bed82832`  
		Last Modified: Thu, 24 May 2018 22:03:42 GMT  
		Size: 37.6 MB (37586652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:3f24a6538620ddd3ced5c530ae174f97cafcdd1970577c696124b9f1fe853278
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.1 MB (367116158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcc712bad262129ee6e54891ff330d9393fd4135e071455c91f9282146b67226`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:03:57 GMT
ADD file:5b2d516c09b4419925efe09e1b5c861cbd3a2d48ed47d6b2c7e571ec6d9ead64 in / 
# Sat, 28 Apr 2018 12:03:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:03:59 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:04:05 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:04:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:04:18 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 11:58:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 11:58:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 11:59:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:59:16 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 11:59:16 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 11:59:39 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 11:59:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 12:23:42 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 12:23:45 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 12:23:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 12:23:55 GMT
CMD ["bash"]
# Fri, 25 May 2018 12:25:08 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 12:26:07 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c68b3181adc7da3b2a5c9be4e228fe5b958ebee478e094e17cf4a61c60a75190`  
		Last Modified: Sat, 28 Apr 2018 12:06:55 GMT  
		Size: 26.5 MB (26487045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91be1119609b1847ebcb9f2621129540bc1fb01ca2c914cc9d03985f48513d24`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605e73e7288ab8c0b45ebed929576b45d7e024077e0f2ae8b1bfabc549e22b0f`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843bab014c7a7d380f7e5c7b7c205da6050bb6e3411217ebae052fae49a97708`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebf53478b460975ab3dc0b245e93b5121d21e03232fcef2d94cd838e034c3af`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ad074d342b779241149fc3fd8ca37e75b9985c3c0c75194f0baa6457643bc9`  
		Last Modified: Wed, 16 May 2018 12:07:02 GMT  
		Size: 831.2 KB (831191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2563139b45010cd554b552642217d24a54e56e1348796c0e156c8b1da6cb10`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 4.1 MB (4077205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a670c1a3040793070164343ff80a5fe224179f0542e8caa26ffdd706fc9a8f`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46573ec96640100c935e1de546d8e484aba5795ae4a439d06a5fce5ceb7bab17`  
		Last Modified: Wed, 16 May 2018 12:06:58 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c0d825eae387d208e3db5a3d2c211d2da64e3b8d2dd2eec5c4c4d33531d312`  
		Last Modified: Wed, 16 May 2018 12:07:17 GMT  
		Size: 53.3 MB (53260829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43be66fa479508bd5da868d645d6ac16277dab0c314790a1a45868b46042f4fd`  
		Last Modified: Wed, 16 May 2018 12:06:59 GMT  
		Size: 849.5 KB (849453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b73a800962eaa799f32d90e55a98ff0d75b6ec5f28b22a5e7a230c076eb77c`  
		Last Modified: Fri, 25 May 2018 12:31:35 GMT  
		Size: 188.4 MB (188390821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fff307b7b5e5b8f708310d05f17e3b91e9e87dff16e5e389a8efdf56ecbc62`  
		Last Modified: Fri, 25 May 2018 12:30:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fab2540810360b8fa43551847a14f4816b8a9d4a0e79958f8a8950a0079161`  
		Last Modified: Fri, 25 May 2018 12:32:35 GMT  
		Size: 60.0 MB (60001666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9e0ceb30682e2089e5daddb32daee700a048f85cb3d9d2e0927e89b2cc6ffa`  
		Last Modified: Fri, 25 May 2018 12:34:22 GMT  
		Size: 33.2 MB (33213855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6696597b6c6f9df3b19589521722980da60a7fb4d9fd90749a8f3f0ace93d3f9
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.4 MB (392365714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffd1c712e57df3ba42413e8197367ddb7ee89b341dae2d289b84b769e4d4acd2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:10:30 GMT
ADD file:2738a1f35ded405c55bf8578757cc7a8a559fecd00a693b443369262b6dd3127 in / 
# Tue, 01 May 2018 01:10:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:10:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:11:00 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:11:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:11:09 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 09:17:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 09:18:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 09:20:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:20:22 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 09:20:23 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 09:21:02 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 09:21:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 14:59:45 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 14:59:50 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 14:59:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 14:59:51 GMT
CMD ["bash"]
# Fri, 25 May 2018 15:02:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 15:05:37 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5b73461db237fc125ed4bbd267b3cd588b6d3957c33cf7fc1d7f9aaf6dcd23fd`  
		Last Modified: Fri, 27 Apr 2018 22:48:27 GMT  
		Size: 27.9 MB (27906574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c642ceb6d4dae80623e35056b3672b999504c5a0cb5dfdd4017f3ff74c6613d8`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6b10168e4f59716c9bf42ae4d202df59f2177923f5e0c6a10228be5c719a2e`  
		Last Modified: Tue, 01 May 2018 01:15:00 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0393063bd61dd94962711e03eb55999a0f821b5939d53509bd5aaf041018dfd`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7da53af2791e4570af9528b9ac2c4487a67026625b4de48184810193f3aa76f`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c156a4d1ad7cd59ce110f77b00214890cbe16b288cc38dfddfe83e9a4cbf4c6`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 831.0 KB (830976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be34a6338091a5e6c7b3336a3410157dd78d861793b54433ff7d219681b4cd95`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 4.4 MB (4438186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17243111bd7f4cc4a686835d4f7d86a2a8a0f4e9cd0db83d23b3b13069bad744`  
		Last Modified: Wed, 16 May 2018 10:26:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e446f86bbda79f1e1d14edd48864be9d560d0705f48166af8f8275833fe37b2e`  
		Last Modified: Wed, 16 May 2018 10:26:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6301719156835f879808d742b36f8b71f5f44741b3081e6516c61a3165608e4`  
		Last Modified: Wed, 16 May 2018 10:26:28 GMT  
		Size: 56.3 MB (56321857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92cb898705c424115a56cd1f955c61c5731211890c95409572b1b64666e60af`  
		Last Modified: Wed, 16 May 2018 10:26:01 GMT  
		Size: 849.4 KB (849389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa2f2edfc54bc83efbb1aecee4ad233c58a7b6f678c0f27f5c95ec2d241795`  
		Last Modified: Fri, 25 May 2018 15:49:15 GMT  
		Size: 203.3 MB (203260535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a862ae50eb668fd467dd0529f7a65222c885a20ef8d430ae67c1ef80d6211e20`  
		Last Modified: Fri, 25 May 2018 15:48:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b4a39407c12801335afb2e67bf30ec79318c34459ca9c277d0fcc3b4d3aa22`  
		Last Modified: Fri, 25 May 2018 15:50:07 GMT  
		Size: 63.4 MB (63381662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25bab31be7a7cebe9e1e4ce4193687b612805d59fa9b7be772181a70bb72ec0`  
		Last Modified: Fri, 25 May 2018 15:51:05 GMT  
		Size: 35.4 MB (35372447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-robot-stretch`

```console
$ docker pull ros@sha256:121c483b95bb17f5374142374efde5ab7e7231d6e52c6bc4ac9b63bf32ac5687
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-robot-stretch` - linux; amd64

```console
$ docker pull ros@sha256:4c6ecedaf78d657f943b819cf7b46c5a4994ac9ebffa47a5b165a6bc56b2c9fe
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **551.0 MB (551006666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe737fe1a8771a3e742386434170637c618b8651539deaf140fffde2110c0472`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 07:08:53 GMT
ADD file:9572fdb59dfbb9b032f3331bbc2a08b31e0aef5fbde44c8f2008d22bf5290cf2 in / 
# Sat, 28 Apr 2018 07:08:53 GMT
CMD ["bash"]
# Sun, 29 Apr 2018 12:52:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:52:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sun, 29 Apr 2018 12:52:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros-latest.list
# Sun, 29 Apr 2018 12:52:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:52:42 GMT
ENV LANG=C.UTF-8
# Sun, 29 Apr 2018 12:52:42 GMT
ENV LC_ALL=C.UTF-8
# Sun, 29 Apr 2018 12:52:54 GMT
RUN rosdep init     && rosdep update
# Tue, 15 May 2018 17:47:59 GMT
ENV ROS_DISTRO=melodic
# Thu, 24 May 2018 21:46:06 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:46:07 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Thu, 24 May 2018 21:46:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 24 May 2018 21:46:07 GMT
CMD ["bash"]
# Thu, 24 May 2018 21:50:48 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:51:50 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc1a78bfd46becbfc3abb8a74d9a70a0e0dc7a5809bbd12e814f9382db003707`  
		Last Modified: Sat, 28 Apr 2018 09:27:54 GMT  
		Size: 45.3 MB (45318159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080d14fa56ef128c193fd94edf1e5eb031d02ae97b680588c7248e5e84304f13`  
		Last Modified: Sun, 29 Apr 2018 14:48:05 GMT  
		Size: 6.9 MB (6859072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604921583c4f613ebee4eb24564ca607566b8b48206868b48c018443567dd0b2`  
		Last Modified: Sun, 29 Apr 2018 14:48:03 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631afcce8e2d86cf9596b3823955679a3e770120d1da140a494003c85bf577b7`  
		Last Modified: Sun, 29 Apr 2018 14:48:00 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b0b4ce522ec73ddd931386acbe825b6203543509a3d76c51e649cb124d5ca1`  
		Last Modified: Sun, 29 Apr 2018 14:48:25 GMT  
		Size: 64.9 MB (64857453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea215428a3b38a4f7bc2be7aad6084d16a82bb84f706aebde2d34120ffc5190`  
		Last Modified: Sun, 29 Apr 2018 14:48:01 GMT  
		Size: 833.5 KB (833530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd9f60d7f6c7b6a8bb715d3a9803206d7a1eb5bfa04a9d74975b0ad026b77d1`  
		Last Modified: Thu, 24 May 2018 22:12:47 GMT  
		Size: 269.4 MB (269359856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117a3c26cbb3ca93f68e7314ae978a7e5baa750a43aa035c903facad8a260129`  
		Last Modified: Thu, 24 May 2018 22:11:40 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ffcec86733c2b1a3056d4d21fad1a14b11a3178d017035ab59c8a9bf3061ce`  
		Last Modified: Thu, 24 May 2018 22:13:28 GMT  
		Size: 108.5 MB (108461908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072bc2ecc4fd8eece89f407f1a14fd7fd4c622e40d09254d897cfe209d13b851`  
		Last Modified: Thu, 24 May 2018 22:17:11 GMT  
		Size: 55.3 MB (55314898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d3a1add55f1c96f4cbdb22b2e3533ffc7bd9844da283925ec27d537ce07962bf
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **491.3 MB (491329194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c9b4c75f86ed0c1c6315458c4ed0c8417b62a8c4d9dcd953fd196576dc0a51e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 30 Apr 2018 23:31:58 GMT
ADD file:245a8cfe59ea071e4e215a722e0d4b4b14fa95dd6ffd03739fe048433cfaf523 in / 
# Mon, 30 Apr 2018 23:32:00 GMT
CMD ["bash"]
# Tue, 01 May 2018 03:30:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:30:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 03:30:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 03:35:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:35:21 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 03:35:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 03:36:07 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 09:54:49 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 15:27:35 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 15:27:40 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 15:27:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 15:27:41 GMT
CMD ["bash"]
# Fri, 25 May 2018 15:30:40 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 15:34:01 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:142bf25d8d1b3ebc9dfbedd586e70a011594690acf48b2695bfce01e3a2cf0d5`  
		Last Modified: Mon, 30 Apr 2018 23:52:13 GMT  
		Size: 43.1 MB (43109349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994bacc3e1c11e50065156c511f0c11e001707e55b61e361b8dc44d236c76f24`  
		Last Modified: Tue, 01 May 2018 04:41:15 GMT  
		Size: 6.4 MB (6427112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663899231a010cf1e857473d7203c7e5f109b38379d2d822c31dba98a7f8af10`  
		Last Modified: Tue, 01 May 2018 04:41:09 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d68d9781734de3f7c1ce451752978a14ba285ad3c63d5ab58034a2008cd25ef`  
		Last Modified: Tue, 01 May 2018 04:41:06 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678cb4b8d2f95bf400236eedd95783c53081503a2ed2b39f51e57a6062cd18c7`  
		Last Modified: Tue, 01 May 2018 04:42:23 GMT  
		Size: 61.9 MB (61938600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0225d679802c170200a58607e1e5a805065659ce28bdec6f9cc91f1c5f6ac461`  
		Last Modified: Tue, 01 May 2018 04:41:08 GMT  
		Size: 835.1 KB (835084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ff3cd1cf2d3e46a7f8fe4a2e5e91ff0815a51d5c87cfd81a1b8932dea453b8`  
		Last Modified: Fri, 25 May 2018 15:55:33 GMT  
		Size: 223.5 MB (223512365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5879828040241eb3667bd05cbfcc6b14911bf87255edd35c912781995caeb5`  
		Last Modified: Fri, 25 May 2018 15:54:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c54d9a16ffc723b2aa54654d720d702140f7b6d858968eec2cd9e827e41f469`  
		Last Modified: Fri, 25 May 2018 15:56:23 GMT  
		Size: 102.9 MB (102929185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6fa089504aa363c45e5180df89bbcfbf602523ffcbfa02177ec0ef846edf8cf`  
		Last Modified: Fri, 25 May 2018 15:57:28 GMT  
		Size: 52.6 MB (52575703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base`

```console
$ docker pull ros@sha256:65fa1c573112741d9bf457a4c01de50f383ce57281f3d196e79a02e7cba3e354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:6cb9d04fe705668a8939f8d24b67370ec79cba45750cff9a3b4ac549dcf8c592
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **379.8 MB (379836490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8141688e843965dabe1111f59e049862a0c270b10da0cc85efa9beff999898f3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 27 Apr 2018 23:28:32 GMT
ADD file:81813d6023adb66b80fe163bc7db464004673838d17195b9d84aade4f8961b71 in / 
# Fri, 27 Apr 2018 23:28:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 27 Apr 2018 23:28:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 27 Apr 2018 23:28:35 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 27 Apr 2018 23:28:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 27 Apr 2018 23:28:36 GMT
CMD ["/bin/bash"]
# Tue, 15 May 2018 17:22:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 15 May 2018 17:22:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 15 May 2018 17:24:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:24:08 GMT
ENV LANG=C.UTF-8
# Tue, 15 May 2018 17:24:09 GMT
ENV LC_ALL=C.UTF-8
# Tue, 15 May 2018 17:24:19 GMT
RUN rosdep init     && rosdep update
# Tue, 15 May 2018 17:24:19 GMT
ENV ROS_DISTRO=melodic
# Thu, 24 May 2018 21:26:28 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:26:29 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Thu, 24 May 2018 21:26:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 24 May 2018 21:26:29 GMT
CMD ["bash"]
# Thu, 24 May 2018 21:29:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a48c500ed24e62926cb079df35f964c57d8bb08159b1d29c6a3b0a58dc365dc1`  
		Last Modified: Fri, 27 Apr 2018 22:14:33 GMT  
		Size: 31.0 MB (30957448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1de00ff7e1fea0858b6a4b5ca208eeca970607ea9a6eb5fc972494e7a0cdde`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0330ca45a200e1fcef05ae97f434366d262a1c50b3dc053e7928b58dd37211dd`  
		Last Modified: Fri, 27 Apr 2018 23:32:05 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471db38bcfbf0f5bac78012b9d458dfd37309d5cbb99d4e95310321a60a0cfdf`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4aba487617ca27519745ae722b8ea1917474c495b91b3c4887728a3f2ee7db`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8456edf85c693828820f7381dde166ac747f2cd8e10610d4c51120bc668379f`  
		Last Modified: Tue, 15 May 2018 18:06:38 GMT  
		Size: 831.1 KB (831054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2122c178c47e334cadb90a80317c074c9ab5b4ad3c03bd385e7b1cd3e348aa`  
		Last Modified: Tue, 15 May 2018 18:06:39 GMT  
		Size: 4.9 MB (4859414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d31beaa42936003685a0b05665d5767eeeddc4c318aaadc6fca1bba5debf2b`  
		Last Modified: Tue, 15 May 2018 18:06:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4b733826c103e038eda6e27b5f02bd3d2399d9c5c0a1af66b687989888289`  
		Last Modified: Tue, 15 May 2018 18:06:33 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c0ecb640b5f315f0d1dfa938e893872008c4f9a375a74e3c04c718e57bf3a5`  
		Last Modified: Tue, 15 May 2018 18:06:53 GMT  
		Size: 58.4 MB (58398228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae98d14520da6037aa61bc4046566731135de07187c4ea0f29030924bdcedb9`  
		Last Modified: Tue, 15 May 2018 18:06:35 GMT  
		Size: 848.9 KB (848891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5010f265d43daa5e2b9fbbbd090b2aa10b524945743a39cfd845a82379bd2f`  
		Last Modified: Thu, 24 May 2018 22:02:00 GMT  
		Size: 215.8 MB (215752594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0876834886b1318e9ec6eea07a901cde589827dacaef6c6179af7bb73bff5ea9`  
		Last Modified: Thu, 24 May 2018 22:01:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f4d2a0227e9474ba6418c71791baf644b56f14e7b6ab2389c7c9b071db5331`  
		Last Modified: Thu, 24 May 2018 22:02:53 GMT  
		Size: 68.2 MB (68184788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm variant v7

```console
$ docker pull ros@sha256:f46872e2c7c6a4cd2d6cf52a79b0ff955df4dc892b30856465400b371df39cd4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.9 MB (333902303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37417f98d377f368a74e8f07277aac34c9f2115dbd17839aed2f3494cdaeece`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:03:57 GMT
ADD file:5b2d516c09b4419925efe09e1b5c861cbd3a2d48ed47d6b2c7e571ec6d9ead64 in / 
# Sat, 28 Apr 2018 12:03:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:03:59 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:04:05 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:04:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:04:18 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 11:58:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 11:58:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 11:59:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:59:16 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 11:59:16 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 11:59:39 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 11:59:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 12:23:42 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 12:23:45 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 12:23:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 12:23:55 GMT
CMD ["bash"]
# Fri, 25 May 2018 12:25:08 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c68b3181adc7da3b2a5c9be4e228fe5b958ebee478e094e17cf4a61c60a75190`  
		Last Modified: Sat, 28 Apr 2018 12:06:55 GMT  
		Size: 26.5 MB (26487045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91be1119609b1847ebcb9f2621129540bc1fb01ca2c914cc9d03985f48513d24`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605e73e7288ab8c0b45ebed929576b45d7e024077e0f2ae8b1bfabc549e22b0f`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843bab014c7a7d380f7e5c7b7c205da6050bb6e3411217ebae052fae49a97708`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebf53478b460975ab3dc0b245e93b5121d21e03232fcef2d94cd838e034c3af`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ad074d342b779241149fc3fd8ca37e75b9985c3c0c75194f0baa6457643bc9`  
		Last Modified: Wed, 16 May 2018 12:07:02 GMT  
		Size: 831.2 KB (831191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2563139b45010cd554b552642217d24a54e56e1348796c0e156c8b1da6cb10`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 4.1 MB (4077205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a670c1a3040793070164343ff80a5fe224179f0542e8caa26ffdd706fc9a8f`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46573ec96640100c935e1de546d8e484aba5795ae4a439d06a5fce5ceb7bab17`  
		Last Modified: Wed, 16 May 2018 12:06:58 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c0d825eae387d208e3db5a3d2c211d2da64e3b8d2dd2eec5c4c4d33531d312`  
		Last Modified: Wed, 16 May 2018 12:07:17 GMT  
		Size: 53.3 MB (53260829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43be66fa479508bd5da868d645d6ac16277dab0c314790a1a45868b46042f4fd`  
		Last Modified: Wed, 16 May 2018 12:06:59 GMT  
		Size: 849.5 KB (849453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b73a800962eaa799f32d90e55a98ff0d75b6ec5f28b22a5e7a230c076eb77c`  
		Last Modified: Fri, 25 May 2018 12:31:35 GMT  
		Size: 188.4 MB (188390821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fff307b7b5e5b8f708310d05f17e3b91e9e87dff16e5e389a8efdf56ecbc62`  
		Last Modified: Fri, 25 May 2018 12:30:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fab2540810360b8fa43551847a14f4816b8a9d4a0e79958f8a8950a0079161`  
		Last Modified: Fri, 25 May 2018 12:32:35 GMT  
		Size: 60.0 MB (60001666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:421fe69542b69504d5185c436ab23bece33ea046c086ae3c6a28cd1b1416f87d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.0 MB (356993267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7a933463e40d905ead1f8ad4f817bbcd68225be7dd2476192fff9dc0d4ca2a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:10:30 GMT
ADD file:2738a1f35ded405c55bf8578757cc7a8a559fecd00a693b443369262b6dd3127 in / 
# Tue, 01 May 2018 01:10:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:10:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:11:00 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:11:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:11:09 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 09:17:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 09:18:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 09:20:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:20:22 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 09:20:23 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 09:21:02 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 09:21:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 14:59:45 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 14:59:50 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 14:59:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 14:59:51 GMT
CMD ["bash"]
# Fri, 25 May 2018 15:02:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5b73461db237fc125ed4bbd267b3cd588b6d3957c33cf7fc1d7f9aaf6dcd23fd`  
		Last Modified: Fri, 27 Apr 2018 22:48:27 GMT  
		Size: 27.9 MB (27906574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c642ceb6d4dae80623e35056b3672b999504c5a0cb5dfdd4017f3ff74c6613d8`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6b10168e4f59716c9bf42ae4d202df59f2177923f5e0c6a10228be5c719a2e`  
		Last Modified: Tue, 01 May 2018 01:15:00 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0393063bd61dd94962711e03eb55999a0f821b5939d53509bd5aaf041018dfd`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7da53af2791e4570af9528b9ac2c4487a67026625b4de48184810193f3aa76f`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c156a4d1ad7cd59ce110f77b00214890cbe16b288cc38dfddfe83e9a4cbf4c6`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 831.0 KB (830976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be34a6338091a5e6c7b3336a3410157dd78d861793b54433ff7d219681b4cd95`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 4.4 MB (4438186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17243111bd7f4cc4a686835d4f7d86a2a8a0f4e9cd0db83d23b3b13069bad744`  
		Last Modified: Wed, 16 May 2018 10:26:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e446f86bbda79f1e1d14edd48864be9d560d0705f48166af8f8275833fe37b2e`  
		Last Modified: Wed, 16 May 2018 10:26:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6301719156835f879808d742b36f8b71f5f44741b3081e6516c61a3165608e4`  
		Last Modified: Wed, 16 May 2018 10:26:28 GMT  
		Size: 56.3 MB (56321857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92cb898705c424115a56cd1f955c61c5731211890c95409572b1b64666e60af`  
		Last Modified: Wed, 16 May 2018 10:26:01 GMT  
		Size: 849.4 KB (849389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa2f2edfc54bc83efbb1aecee4ad233c58a7b6f678c0f27f5c95ec2d241795`  
		Last Modified: Fri, 25 May 2018 15:49:15 GMT  
		Size: 203.3 MB (203260535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a862ae50eb668fd467dd0529f7a65222c885a20ef8d430ae67c1ef80d6211e20`  
		Last Modified: Fri, 25 May 2018 15:48:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b4a39407c12801335afb2e67bf30ec79318c34459ca9c277d0fcc3b4d3aa22`  
		Last Modified: Fri, 25 May 2018 15:50:07 GMT  
		Size: 63.4 MB (63381662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:65fa1c573112741d9bf457a4c01de50f383ce57281f3d196e79a02e7cba3e354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:6cb9d04fe705668a8939f8d24b67370ec79cba45750cff9a3b4ac549dcf8c592
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **379.8 MB (379836490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8141688e843965dabe1111f59e049862a0c270b10da0cc85efa9beff999898f3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 27 Apr 2018 23:28:32 GMT
ADD file:81813d6023adb66b80fe163bc7db464004673838d17195b9d84aade4f8961b71 in / 
# Fri, 27 Apr 2018 23:28:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 27 Apr 2018 23:28:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 27 Apr 2018 23:28:35 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 27 Apr 2018 23:28:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 27 Apr 2018 23:28:36 GMT
CMD ["/bin/bash"]
# Tue, 15 May 2018 17:22:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 15 May 2018 17:22:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 15 May 2018 17:24:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:24:08 GMT
ENV LANG=C.UTF-8
# Tue, 15 May 2018 17:24:09 GMT
ENV LC_ALL=C.UTF-8
# Tue, 15 May 2018 17:24:19 GMT
RUN rosdep init     && rosdep update
# Tue, 15 May 2018 17:24:19 GMT
ENV ROS_DISTRO=melodic
# Thu, 24 May 2018 21:26:28 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:26:29 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Thu, 24 May 2018 21:26:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 24 May 2018 21:26:29 GMT
CMD ["bash"]
# Thu, 24 May 2018 21:29:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a48c500ed24e62926cb079df35f964c57d8bb08159b1d29c6a3b0a58dc365dc1`  
		Last Modified: Fri, 27 Apr 2018 22:14:33 GMT  
		Size: 31.0 MB (30957448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1de00ff7e1fea0858b6a4b5ca208eeca970607ea9a6eb5fc972494e7a0cdde`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0330ca45a200e1fcef05ae97f434366d262a1c50b3dc053e7928b58dd37211dd`  
		Last Modified: Fri, 27 Apr 2018 23:32:05 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471db38bcfbf0f5bac78012b9d458dfd37309d5cbb99d4e95310321a60a0cfdf`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4aba487617ca27519745ae722b8ea1917474c495b91b3c4887728a3f2ee7db`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8456edf85c693828820f7381dde166ac747f2cd8e10610d4c51120bc668379f`  
		Last Modified: Tue, 15 May 2018 18:06:38 GMT  
		Size: 831.1 KB (831054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2122c178c47e334cadb90a80317c074c9ab5b4ad3c03bd385e7b1cd3e348aa`  
		Last Modified: Tue, 15 May 2018 18:06:39 GMT  
		Size: 4.9 MB (4859414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d31beaa42936003685a0b05665d5767eeeddc4c318aaadc6fca1bba5debf2b`  
		Last Modified: Tue, 15 May 2018 18:06:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4b733826c103e038eda6e27b5f02bd3d2399d9c5c0a1af66b687989888289`  
		Last Modified: Tue, 15 May 2018 18:06:33 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c0ecb640b5f315f0d1dfa938e893872008c4f9a375a74e3c04c718e57bf3a5`  
		Last Modified: Tue, 15 May 2018 18:06:53 GMT  
		Size: 58.4 MB (58398228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae98d14520da6037aa61bc4046566731135de07187c4ea0f29030924bdcedb9`  
		Last Modified: Tue, 15 May 2018 18:06:35 GMT  
		Size: 848.9 KB (848891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5010f265d43daa5e2b9fbbbd090b2aa10b524945743a39cfd845a82379bd2f`  
		Last Modified: Thu, 24 May 2018 22:02:00 GMT  
		Size: 215.8 MB (215752594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0876834886b1318e9ec6eea07a901cde589827dacaef6c6179af7bb73bff5ea9`  
		Last Modified: Thu, 24 May 2018 22:01:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f4d2a0227e9474ba6418c71791baf644b56f14e7b6ab2389c7c9b071db5331`  
		Last Modified: Thu, 24 May 2018 22:02:53 GMT  
		Size: 68.2 MB (68184788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:f46872e2c7c6a4cd2d6cf52a79b0ff955df4dc892b30856465400b371df39cd4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.9 MB (333902303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37417f98d377f368a74e8f07277aac34c9f2115dbd17839aed2f3494cdaeece`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:03:57 GMT
ADD file:5b2d516c09b4419925efe09e1b5c861cbd3a2d48ed47d6b2c7e571ec6d9ead64 in / 
# Sat, 28 Apr 2018 12:03:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:03:59 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:04:05 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:04:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:04:18 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 11:58:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 11:58:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 11:59:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:59:16 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 11:59:16 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 11:59:39 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 11:59:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 12:23:42 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 12:23:45 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 12:23:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 12:23:55 GMT
CMD ["bash"]
# Fri, 25 May 2018 12:25:08 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c68b3181adc7da3b2a5c9be4e228fe5b958ebee478e094e17cf4a61c60a75190`  
		Last Modified: Sat, 28 Apr 2018 12:06:55 GMT  
		Size: 26.5 MB (26487045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91be1119609b1847ebcb9f2621129540bc1fb01ca2c914cc9d03985f48513d24`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605e73e7288ab8c0b45ebed929576b45d7e024077e0f2ae8b1bfabc549e22b0f`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843bab014c7a7d380f7e5c7b7c205da6050bb6e3411217ebae052fae49a97708`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebf53478b460975ab3dc0b245e93b5121d21e03232fcef2d94cd838e034c3af`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ad074d342b779241149fc3fd8ca37e75b9985c3c0c75194f0baa6457643bc9`  
		Last Modified: Wed, 16 May 2018 12:07:02 GMT  
		Size: 831.2 KB (831191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2563139b45010cd554b552642217d24a54e56e1348796c0e156c8b1da6cb10`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 4.1 MB (4077205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a670c1a3040793070164343ff80a5fe224179f0542e8caa26ffdd706fc9a8f`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46573ec96640100c935e1de546d8e484aba5795ae4a439d06a5fce5ceb7bab17`  
		Last Modified: Wed, 16 May 2018 12:06:58 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c0d825eae387d208e3db5a3d2c211d2da64e3b8d2dd2eec5c4c4d33531d312`  
		Last Modified: Wed, 16 May 2018 12:07:17 GMT  
		Size: 53.3 MB (53260829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43be66fa479508bd5da868d645d6ac16277dab0c314790a1a45868b46042f4fd`  
		Last Modified: Wed, 16 May 2018 12:06:59 GMT  
		Size: 849.5 KB (849453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b73a800962eaa799f32d90e55a98ff0d75b6ec5f28b22a5e7a230c076eb77c`  
		Last Modified: Fri, 25 May 2018 12:31:35 GMT  
		Size: 188.4 MB (188390821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fff307b7b5e5b8f708310d05f17e3b91e9e87dff16e5e389a8efdf56ecbc62`  
		Last Modified: Fri, 25 May 2018 12:30:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fab2540810360b8fa43551847a14f4816b8a9d4a0e79958f8a8950a0079161`  
		Last Modified: Fri, 25 May 2018 12:32:35 GMT  
		Size: 60.0 MB (60001666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:421fe69542b69504d5185c436ab23bece33ea046c086ae3c6a28cd1b1416f87d
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.0 MB (356993267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7a933463e40d905ead1f8ad4f817bbcd68225be7dd2476192fff9dc0d4ca2a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:10:30 GMT
ADD file:2738a1f35ded405c55bf8578757cc7a8a559fecd00a693b443369262b6dd3127 in / 
# Tue, 01 May 2018 01:10:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:10:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:11:00 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:11:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:11:09 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 09:17:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 09:18:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 09:20:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:20:22 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 09:20:23 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 09:21:02 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 09:21:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 14:59:45 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 14:59:50 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 14:59:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 14:59:51 GMT
CMD ["bash"]
# Fri, 25 May 2018 15:02:41 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5b73461db237fc125ed4bbd267b3cd588b6d3957c33cf7fc1d7f9aaf6dcd23fd`  
		Last Modified: Fri, 27 Apr 2018 22:48:27 GMT  
		Size: 27.9 MB (27906574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c642ceb6d4dae80623e35056b3672b999504c5a0cb5dfdd4017f3ff74c6613d8`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6b10168e4f59716c9bf42ae4d202df59f2177923f5e0c6a10228be5c719a2e`  
		Last Modified: Tue, 01 May 2018 01:15:00 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0393063bd61dd94962711e03eb55999a0f821b5939d53509bd5aaf041018dfd`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7da53af2791e4570af9528b9ac2c4487a67026625b4de48184810193f3aa76f`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c156a4d1ad7cd59ce110f77b00214890cbe16b288cc38dfddfe83e9a4cbf4c6`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 831.0 KB (830976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be34a6338091a5e6c7b3336a3410157dd78d861793b54433ff7d219681b4cd95`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 4.4 MB (4438186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17243111bd7f4cc4a686835d4f7d86a2a8a0f4e9cd0db83d23b3b13069bad744`  
		Last Modified: Wed, 16 May 2018 10:26:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e446f86bbda79f1e1d14edd48864be9d560d0705f48166af8f8275833fe37b2e`  
		Last Modified: Wed, 16 May 2018 10:26:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6301719156835f879808d742b36f8b71f5f44741b3081e6516c61a3165608e4`  
		Last Modified: Wed, 16 May 2018 10:26:28 GMT  
		Size: 56.3 MB (56321857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92cb898705c424115a56cd1f955c61c5731211890c95409572b1b64666e60af`  
		Last Modified: Wed, 16 May 2018 10:26:01 GMT  
		Size: 849.4 KB (849389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa2f2edfc54bc83efbb1aecee4ad233c58a7b6f678c0f27f5c95ec2d241795`  
		Last Modified: Fri, 25 May 2018 15:49:15 GMT  
		Size: 203.3 MB (203260535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a862ae50eb668fd467dd0529f7a65222c885a20ef8d430ae67c1ef80d6211e20`  
		Last Modified: Fri, 25 May 2018 15:48:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b4a39407c12801335afb2e67bf30ec79318c34459ca9c277d0fcc3b4d3aa22`  
		Last Modified: Fri, 25 May 2018 15:50:07 GMT  
		Size: 63.4 MB (63381662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-base-stretch`

```console
$ docker pull ros@sha256:15a38c6fb350769645f28b91d2a5399617d89716fe70ef8932d5aa84da858287
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-stretch` - linux; amd64

```console
$ docker pull ros@sha256:421bc58643fb25a48aad6951d7c3d61c4675ce54c939fa52212631c5b0539138
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **495.7 MB (495691768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6daa7089b4fe82d5741a0c27095e07a2f46c41f0203c7cab0ce241d527ed3b8c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 07:08:53 GMT
ADD file:9572fdb59dfbb9b032f3331bbc2a08b31e0aef5fbde44c8f2008d22bf5290cf2 in / 
# Sat, 28 Apr 2018 07:08:53 GMT
CMD ["bash"]
# Sun, 29 Apr 2018 12:52:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:52:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sun, 29 Apr 2018 12:52:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros-latest.list
# Sun, 29 Apr 2018 12:52:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:52:42 GMT
ENV LANG=C.UTF-8
# Sun, 29 Apr 2018 12:52:42 GMT
ENV LC_ALL=C.UTF-8
# Sun, 29 Apr 2018 12:52:54 GMT
RUN rosdep init     && rosdep update
# Tue, 15 May 2018 17:47:59 GMT
ENV ROS_DISTRO=melodic
# Thu, 24 May 2018 21:46:06 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:46:07 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Thu, 24 May 2018 21:46:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 24 May 2018 21:46:07 GMT
CMD ["bash"]
# Thu, 24 May 2018 21:50:48 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc1a78bfd46becbfc3abb8a74d9a70a0e0dc7a5809bbd12e814f9382db003707`  
		Last Modified: Sat, 28 Apr 2018 09:27:54 GMT  
		Size: 45.3 MB (45318159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080d14fa56ef128c193fd94edf1e5eb031d02ae97b680588c7248e5e84304f13`  
		Last Modified: Sun, 29 Apr 2018 14:48:05 GMT  
		Size: 6.9 MB (6859072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604921583c4f613ebee4eb24564ca607566b8b48206868b48c018443567dd0b2`  
		Last Modified: Sun, 29 Apr 2018 14:48:03 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631afcce8e2d86cf9596b3823955679a3e770120d1da140a494003c85bf577b7`  
		Last Modified: Sun, 29 Apr 2018 14:48:00 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b0b4ce522ec73ddd931386acbe825b6203543509a3d76c51e649cb124d5ca1`  
		Last Modified: Sun, 29 Apr 2018 14:48:25 GMT  
		Size: 64.9 MB (64857453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea215428a3b38a4f7bc2be7aad6084d16a82bb84f706aebde2d34120ffc5190`  
		Last Modified: Sun, 29 Apr 2018 14:48:01 GMT  
		Size: 833.5 KB (833530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd9f60d7f6c7b6a8bb715d3a9803206d7a1eb5bfa04a9d74975b0ad026b77d1`  
		Last Modified: Thu, 24 May 2018 22:12:47 GMT  
		Size: 269.4 MB (269359856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117a3c26cbb3ca93f68e7314ae978a7e5baa750a43aa035c903facad8a260129`  
		Last Modified: Thu, 24 May 2018 22:11:40 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ffcec86733c2b1a3056d4d21fad1a14b11a3178d017035ab59c8a9bf3061ce`  
		Last Modified: Thu, 24 May 2018 22:13:28 GMT  
		Size: 108.5 MB (108461908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:fba806c5caa28c4f95cd1ad39858f4802dc466a0b96c966d80b43828564ea427
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **438.8 MB (438753491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5a056136cca0a7897fcf7dca1cab14e4bc48f5f8562d5df346f112a4250a47`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 30 Apr 2018 23:31:58 GMT
ADD file:245a8cfe59ea071e4e215a722e0d4b4b14fa95dd6ffd03739fe048433cfaf523 in / 
# Mon, 30 Apr 2018 23:32:00 GMT
CMD ["bash"]
# Tue, 01 May 2018 03:30:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:30:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 03:30:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 03:35:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:35:21 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 03:35:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 03:36:07 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 09:54:49 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 15:27:35 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 15:27:40 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 15:27:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 15:27:41 GMT
CMD ["bash"]
# Fri, 25 May 2018 15:30:40 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:142bf25d8d1b3ebc9dfbedd586e70a011594690acf48b2695bfce01e3a2cf0d5`  
		Last Modified: Mon, 30 Apr 2018 23:52:13 GMT  
		Size: 43.1 MB (43109349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994bacc3e1c11e50065156c511f0c11e001707e55b61e361b8dc44d236c76f24`  
		Last Modified: Tue, 01 May 2018 04:41:15 GMT  
		Size: 6.4 MB (6427112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663899231a010cf1e857473d7203c7e5f109b38379d2d822c31dba98a7f8af10`  
		Last Modified: Tue, 01 May 2018 04:41:09 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d68d9781734de3f7c1ce451752978a14ba285ad3c63d5ab58034a2008cd25ef`  
		Last Modified: Tue, 01 May 2018 04:41:06 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678cb4b8d2f95bf400236eedd95783c53081503a2ed2b39f51e57a6062cd18c7`  
		Last Modified: Tue, 01 May 2018 04:42:23 GMT  
		Size: 61.9 MB (61938600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0225d679802c170200a58607e1e5a805065659ce28bdec6f9cc91f1c5f6ac461`  
		Last Modified: Tue, 01 May 2018 04:41:08 GMT  
		Size: 835.1 KB (835084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ff3cd1cf2d3e46a7f8fe4a2e5e91ff0815a51d5c87cfd81a1b8932dea453b8`  
		Last Modified: Fri, 25 May 2018 15:55:33 GMT  
		Size: 223.5 MB (223512365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5879828040241eb3667bd05cbfcc6b14911bf87255edd35c912781995caeb5`  
		Last Modified: Fri, 25 May 2018 15:54:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c54d9a16ffc723b2aa54654d720d702140f7b6d858968eec2cd9e827e41f469`  
		Last Modified: Fri, 25 May 2018 15:56:23 GMT  
		Size: 102.9 MB (102929185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core`

```console
$ docker pull ros@sha256:8d8d5a8ce317bf5d50f788560636af578e14173bffc3d8f3d5897e0181ced508
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:cb755415255f6977ada8f32cdfbb9bba9bc6925d716da950b99b115c28213800
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.7 MB (311651702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:220d358a2874eb7aaad8c85bf4536e2d82eb7dc97ae3701b29278af591cdf5ba`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 27 Apr 2018 23:28:32 GMT
ADD file:81813d6023adb66b80fe163bc7db464004673838d17195b9d84aade4f8961b71 in / 
# Fri, 27 Apr 2018 23:28:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 27 Apr 2018 23:28:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 27 Apr 2018 23:28:35 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 27 Apr 2018 23:28:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 27 Apr 2018 23:28:36 GMT
CMD ["/bin/bash"]
# Tue, 15 May 2018 17:22:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 15 May 2018 17:22:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 15 May 2018 17:24:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:24:08 GMT
ENV LANG=C.UTF-8
# Tue, 15 May 2018 17:24:09 GMT
ENV LC_ALL=C.UTF-8
# Tue, 15 May 2018 17:24:19 GMT
RUN rosdep init     && rosdep update
# Tue, 15 May 2018 17:24:19 GMT
ENV ROS_DISTRO=melodic
# Thu, 24 May 2018 21:26:28 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:26:29 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Thu, 24 May 2018 21:26:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 24 May 2018 21:26:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a48c500ed24e62926cb079df35f964c57d8bb08159b1d29c6a3b0a58dc365dc1`  
		Last Modified: Fri, 27 Apr 2018 22:14:33 GMT  
		Size: 31.0 MB (30957448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1de00ff7e1fea0858b6a4b5ca208eeca970607ea9a6eb5fc972494e7a0cdde`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0330ca45a200e1fcef05ae97f434366d262a1c50b3dc053e7928b58dd37211dd`  
		Last Modified: Fri, 27 Apr 2018 23:32:05 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471db38bcfbf0f5bac78012b9d458dfd37309d5cbb99d4e95310321a60a0cfdf`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4aba487617ca27519745ae722b8ea1917474c495b91b3c4887728a3f2ee7db`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8456edf85c693828820f7381dde166ac747f2cd8e10610d4c51120bc668379f`  
		Last Modified: Tue, 15 May 2018 18:06:38 GMT  
		Size: 831.1 KB (831054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2122c178c47e334cadb90a80317c074c9ab5b4ad3c03bd385e7b1cd3e348aa`  
		Last Modified: Tue, 15 May 2018 18:06:39 GMT  
		Size: 4.9 MB (4859414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d31beaa42936003685a0b05665d5767eeeddc4c318aaadc6fca1bba5debf2b`  
		Last Modified: Tue, 15 May 2018 18:06:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4b733826c103e038eda6e27b5f02bd3d2399d9c5c0a1af66b687989888289`  
		Last Modified: Tue, 15 May 2018 18:06:33 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c0ecb640b5f315f0d1dfa938e893872008c4f9a375a74e3c04c718e57bf3a5`  
		Last Modified: Tue, 15 May 2018 18:06:53 GMT  
		Size: 58.4 MB (58398228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae98d14520da6037aa61bc4046566731135de07187c4ea0f29030924bdcedb9`  
		Last Modified: Tue, 15 May 2018 18:06:35 GMT  
		Size: 848.9 KB (848891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5010f265d43daa5e2b9fbbbd090b2aa10b524945743a39cfd845a82379bd2f`  
		Last Modified: Thu, 24 May 2018 22:02:00 GMT  
		Size: 215.8 MB (215752594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0876834886b1318e9ec6eea07a901cde589827dacaef6c6179af7bb73bff5ea9`  
		Last Modified: Thu, 24 May 2018 22:01:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm variant v7

```console
$ docker pull ros@sha256:361ba5324994f0d1cbd9b4ef33e30821f0f7ce3ed24b6d6803b0838881c7ec01
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.9 MB (273900637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a94496354f4d78bfaa494010448e0f2968b0b1b42341a0a2b4892bd8d3797bb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:03:57 GMT
ADD file:5b2d516c09b4419925efe09e1b5c861cbd3a2d48ed47d6b2c7e571ec6d9ead64 in / 
# Sat, 28 Apr 2018 12:03:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:03:59 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:04:05 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:04:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:04:18 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 11:58:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 11:58:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 11:59:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:59:16 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 11:59:16 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 11:59:39 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 11:59:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 12:23:42 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 12:23:45 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 12:23:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 12:23:55 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c68b3181adc7da3b2a5c9be4e228fe5b958ebee478e094e17cf4a61c60a75190`  
		Last Modified: Sat, 28 Apr 2018 12:06:55 GMT  
		Size: 26.5 MB (26487045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91be1119609b1847ebcb9f2621129540bc1fb01ca2c914cc9d03985f48513d24`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605e73e7288ab8c0b45ebed929576b45d7e024077e0f2ae8b1bfabc549e22b0f`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843bab014c7a7d380f7e5c7b7c205da6050bb6e3411217ebae052fae49a97708`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebf53478b460975ab3dc0b245e93b5121d21e03232fcef2d94cd838e034c3af`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ad074d342b779241149fc3fd8ca37e75b9985c3c0c75194f0baa6457643bc9`  
		Last Modified: Wed, 16 May 2018 12:07:02 GMT  
		Size: 831.2 KB (831191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2563139b45010cd554b552642217d24a54e56e1348796c0e156c8b1da6cb10`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 4.1 MB (4077205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a670c1a3040793070164343ff80a5fe224179f0542e8caa26ffdd706fc9a8f`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46573ec96640100c935e1de546d8e484aba5795ae4a439d06a5fce5ceb7bab17`  
		Last Modified: Wed, 16 May 2018 12:06:58 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c0d825eae387d208e3db5a3d2c211d2da64e3b8d2dd2eec5c4c4d33531d312`  
		Last Modified: Wed, 16 May 2018 12:07:17 GMT  
		Size: 53.3 MB (53260829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43be66fa479508bd5da868d645d6ac16277dab0c314790a1a45868b46042f4fd`  
		Last Modified: Wed, 16 May 2018 12:06:59 GMT  
		Size: 849.5 KB (849453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b73a800962eaa799f32d90e55a98ff0d75b6ec5f28b22a5e7a230c076eb77c`  
		Last Modified: Fri, 25 May 2018 12:31:35 GMT  
		Size: 188.4 MB (188390821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fff307b7b5e5b8f708310d05f17e3b91e9e87dff16e5e389a8efdf56ecbc62`  
		Last Modified: Fri, 25 May 2018 12:30:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:60740870deeed16614ce12efc92ee17f1c030111f81dc247831e0c8d1cced8c1
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.6 MB (293611605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:774de31b14d5b5b138fa39bf4531312c39995c6a100d0fbf5036e6204211b927`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:10:30 GMT
ADD file:2738a1f35ded405c55bf8578757cc7a8a559fecd00a693b443369262b6dd3127 in / 
# Tue, 01 May 2018 01:10:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:10:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:11:00 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:11:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:11:09 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 09:17:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 09:18:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 09:20:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:20:22 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 09:20:23 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 09:21:02 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 09:21:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 14:59:45 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 14:59:50 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 14:59:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 14:59:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5b73461db237fc125ed4bbd267b3cd588b6d3957c33cf7fc1d7f9aaf6dcd23fd`  
		Last Modified: Fri, 27 Apr 2018 22:48:27 GMT  
		Size: 27.9 MB (27906574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c642ceb6d4dae80623e35056b3672b999504c5a0cb5dfdd4017f3ff74c6613d8`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6b10168e4f59716c9bf42ae4d202df59f2177923f5e0c6a10228be5c719a2e`  
		Last Modified: Tue, 01 May 2018 01:15:00 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0393063bd61dd94962711e03eb55999a0f821b5939d53509bd5aaf041018dfd`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7da53af2791e4570af9528b9ac2c4487a67026625b4de48184810193f3aa76f`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c156a4d1ad7cd59ce110f77b00214890cbe16b288cc38dfddfe83e9a4cbf4c6`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 831.0 KB (830976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be34a6338091a5e6c7b3336a3410157dd78d861793b54433ff7d219681b4cd95`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 4.4 MB (4438186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17243111bd7f4cc4a686835d4f7d86a2a8a0f4e9cd0db83d23b3b13069bad744`  
		Last Modified: Wed, 16 May 2018 10:26:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e446f86bbda79f1e1d14edd48864be9d560d0705f48166af8f8275833fe37b2e`  
		Last Modified: Wed, 16 May 2018 10:26:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6301719156835f879808d742b36f8b71f5f44741b3081e6516c61a3165608e4`  
		Last Modified: Wed, 16 May 2018 10:26:28 GMT  
		Size: 56.3 MB (56321857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92cb898705c424115a56cd1f955c61c5731211890c95409572b1b64666e60af`  
		Last Modified: Wed, 16 May 2018 10:26:01 GMT  
		Size: 849.4 KB (849389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa2f2edfc54bc83efbb1aecee4ad233c58a7b6f678c0f27f5c95ec2d241795`  
		Last Modified: Fri, 25 May 2018 15:49:15 GMT  
		Size: 203.3 MB (203260535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a862ae50eb668fd467dd0529f7a65222c885a20ef8d430ae67c1ef80d6211e20`  
		Last Modified: Fri, 25 May 2018 15:48:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:8d8d5a8ce317bf5d50f788560636af578e14173bffc3d8f3d5897e0181ced508
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:cb755415255f6977ada8f32cdfbb9bba9bc6925d716da950b99b115c28213800
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.7 MB (311651702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:220d358a2874eb7aaad8c85bf4536e2d82eb7dc97ae3701b29278af591cdf5ba`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 27 Apr 2018 23:28:32 GMT
ADD file:81813d6023adb66b80fe163bc7db464004673838d17195b9d84aade4f8961b71 in / 
# Fri, 27 Apr 2018 23:28:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 27 Apr 2018 23:28:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 27 Apr 2018 23:28:35 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 27 Apr 2018 23:28:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 27 Apr 2018 23:28:36 GMT
CMD ["/bin/bash"]
# Tue, 15 May 2018 17:22:24 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:22:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 15 May 2018 17:22:55 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 15 May 2018 17:24:08 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 15 May 2018 17:24:08 GMT
ENV LANG=C.UTF-8
# Tue, 15 May 2018 17:24:09 GMT
ENV LC_ALL=C.UTF-8
# Tue, 15 May 2018 17:24:19 GMT
RUN rosdep init     && rosdep update
# Tue, 15 May 2018 17:24:19 GMT
ENV ROS_DISTRO=melodic
# Thu, 24 May 2018 21:26:28 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:26:29 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Thu, 24 May 2018 21:26:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 24 May 2018 21:26:29 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a48c500ed24e62926cb079df35f964c57d8bb08159b1d29c6a3b0a58dc365dc1`  
		Last Modified: Fri, 27 Apr 2018 22:14:33 GMT  
		Size: 31.0 MB (30957448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1de00ff7e1fea0858b6a4b5ca208eeca970607ea9a6eb5fc972494e7a0cdde`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0330ca45a200e1fcef05ae97f434366d262a1c50b3dc053e7928b58dd37211dd`  
		Last Modified: Fri, 27 Apr 2018 23:32:05 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471db38bcfbf0f5bac78012b9d458dfd37309d5cbb99d4e95310321a60a0cfdf`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4aba487617ca27519745ae722b8ea1917474c495b91b3c4887728a3f2ee7db`  
		Last Modified: Fri, 27 Apr 2018 23:32:06 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8456edf85c693828820f7381dde166ac747f2cd8e10610d4c51120bc668379f`  
		Last Modified: Tue, 15 May 2018 18:06:38 GMT  
		Size: 831.1 KB (831054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2122c178c47e334cadb90a80317c074c9ab5b4ad3c03bd385e7b1cd3e348aa`  
		Last Modified: Tue, 15 May 2018 18:06:39 GMT  
		Size: 4.9 MB (4859414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d31beaa42936003685a0b05665d5767eeeddc4c318aaadc6fca1bba5debf2b`  
		Last Modified: Tue, 15 May 2018 18:06:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4b733826c103e038eda6e27b5f02bd3d2399d9c5c0a1af66b687989888289`  
		Last Modified: Tue, 15 May 2018 18:06:33 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c0ecb640b5f315f0d1dfa938e893872008c4f9a375a74e3c04c718e57bf3a5`  
		Last Modified: Tue, 15 May 2018 18:06:53 GMT  
		Size: 58.4 MB (58398228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae98d14520da6037aa61bc4046566731135de07187c4ea0f29030924bdcedb9`  
		Last Modified: Tue, 15 May 2018 18:06:35 GMT  
		Size: 848.9 KB (848891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5010f265d43daa5e2b9fbbbd090b2aa10b524945743a39cfd845a82379bd2f`  
		Last Modified: Thu, 24 May 2018 22:02:00 GMT  
		Size: 215.8 MB (215752594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0876834886b1318e9ec6eea07a901cde589827dacaef6c6179af7bb73bff5ea9`  
		Last Modified: Thu, 24 May 2018 22:01:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:361ba5324994f0d1cbd9b4ef33e30821f0f7ce3ed24b6d6803b0838881c7ec01
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.9 MB (273900637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a94496354f4d78bfaa494010448e0f2968b0b1b42341a0a2b4892bd8d3797bb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 12:03:57 GMT
ADD file:5b2d516c09b4419925efe09e1b5c861cbd3a2d48ed47d6b2c7e571ec6d9ead64 in / 
# Sat, 28 Apr 2018 12:03:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 28 Apr 2018 12:03:59 GMT
RUN rm -rf /var/lib/apt/lists/*
# Sat, 28 Apr 2018 12:04:05 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Sat, 28 Apr 2018 12:04:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 28 Apr 2018 12:04:18 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 11:58:18 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:58:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 11:58:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 11:59:14 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 11:59:16 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 11:59:16 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 11:59:39 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 11:59:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 12:23:42 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 12:23:45 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 12:23:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 12:23:55 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c68b3181adc7da3b2a5c9be4e228fe5b958ebee478e094e17cf4a61c60a75190`  
		Last Modified: Sat, 28 Apr 2018 12:06:55 GMT  
		Size: 26.5 MB (26487045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91be1119609b1847ebcb9f2621129540bc1fb01ca2c914cc9d03985f48513d24`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605e73e7288ab8c0b45ebed929576b45d7e024077e0f2ae8b1bfabc549e22b0f`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843bab014c7a7d380f7e5c7b7c205da6050bb6e3411217ebae052fae49a97708`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebf53478b460975ab3dc0b245e93b5121d21e03232fcef2d94cd838e034c3af`  
		Last Modified: Sat, 28 Apr 2018 12:06:48 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ad074d342b779241149fc3fd8ca37e75b9985c3c0c75194f0baa6457643bc9`  
		Last Modified: Wed, 16 May 2018 12:07:02 GMT  
		Size: 831.2 KB (831191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2563139b45010cd554b552642217d24a54e56e1348796c0e156c8b1da6cb10`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 4.1 MB (4077205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a670c1a3040793070164343ff80a5fe224179f0542e8caa26ffdd706fc9a8f`  
		Last Modified: Wed, 16 May 2018 12:07:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46573ec96640100c935e1de546d8e484aba5795ae4a439d06a5fce5ceb7bab17`  
		Last Modified: Wed, 16 May 2018 12:06:58 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c0d825eae387d208e3db5a3d2c211d2da64e3b8d2dd2eec5c4c4d33531d312`  
		Last Modified: Wed, 16 May 2018 12:07:17 GMT  
		Size: 53.3 MB (53260829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43be66fa479508bd5da868d645d6ac16277dab0c314790a1a45868b46042f4fd`  
		Last Modified: Wed, 16 May 2018 12:06:59 GMT  
		Size: 849.5 KB (849453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b73a800962eaa799f32d90e55a98ff0d75b6ec5f28b22a5e7a230c076eb77c`  
		Last Modified: Fri, 25 May 2018 12:31:35 GMT  
		Size: 188.4 MB (188390821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fff307b7b5e5b8f708310d05f17e3b91e9e87dff16e5e389a8efdf56ecbc62`  
		Last Modified: Fri, 25 May 2018 12:30:34 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:60740870deeed16614ce12efc92ee17f1c030111f81dc247831e0c8d1cced8c1
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.6 MB (293611605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:774de31b14d5b5b138fa39bf4531312c39995c6a100d0fbf5036e6204211b927`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 May 2018 01:10:30 GMT
ADD file:2738a1f35ded405c55bf8578757cc7a8a559fecd00a693b443369262b6dd3127 in / 
# Tue, 01 May 2018 01:10:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 01 May 2018 01:10:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 01:11:00 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Tue, 01 May 2018 01:11:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 01 May 2018 01:11:09 GMT
CMD ["/bin/bash"]
# Wed, 16 May 2018 09:17:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update && apt-get install -q -y tzdata && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:18:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Wed, 16 May 2018 09:18:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros-latest.list
# Wed, 16 May 2018 09:20:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 16 May 2018 09:20:22 GMT
ENV LANG=C.UTF-8
# Wed, 16 May 2018 09:20:23 GMT
ENV LC_ALL=C.UTF-8
# Wed, 16 May 2018 09:21:02 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 09:21:02 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 14:59:45 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 14:59:50 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 14:59:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 14:59:51 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:5b73461db237fc125ed4bbd267b3cd588b6d3957c33cf7fc1d7f9aaf6dcd23fd`  
		Last Modified: Fri, 27 Apr 2018 22:48:27 GMT  
		Size: 27.9 MB (27906574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c642ceb6d4dae80623e35056b3672b999504c5a0cb5dfdd4017f3ff74c6613d8`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6b10168e4f59716c9bf42ae4d202df59f2177923f5e0c6a10228be5c719a2e`  
		Last Modified: Tue, 01 May 2018 01:15:00 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0393063bd61dd94962711e03eb55999a0f821b5939d53509bd5aaf041018dfd`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7da53af2791e4570af9528b9ac2c4487a67026625b4de48184810193f3aa76f`  
		Last Modified: Tue, 01 May 2018 01:14:58 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c156a4d1ad7cd59ce110f77b00214890cbe16b288cc38dfddfe83e9a4cbf4c6`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 831.0 KB (830976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be34a6338091a5e6c7b3336a3410157dd78d861793b54433ff7d219681b4cd95`  
		Last Modified: Wed, 16 May 2018 10:26:04 GMT  
		Size: 4.4 MB (4438186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17243111bd7f4cc4a686835d4f7d86a2a8a0f4e9cd0db83d23b3b13069bad744`  
		Last Modified: Wed, 16 May 2018 10:26:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e446f86bbda79f1e1d14edd48864be9d560d0705f48166af8f8275833fe37b2e`  
		Last Modified: Wed, 16 May 2018 10:26:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6301719156835f879808d742b36f8b71f5f44741b3081e6516c61a3165608e4`  
		Last Modified: Wed, 16 May 2018 10:26:28 GMT  
		Size: 56.3 MB (56321857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92cb898705c424115a56cd1f955c61c5731211890c95409572b1b64666e60af`  
		Last Modified: Wed, 16 May 2018 10:26:01 GMT  
		Size: 849.4 KB (849389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fa2f2edfc54bc83efbb1aecee4ad233c58a7b6f678c0f27f5c95ec2d241795`  
		Last Modified: Fri, 25 May 2018 15:49:15 GMT  
		Size: 203.3 MB (203260535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a862ae50eb668fd467dd0529f7a65222c885a20ef8d430ae67c1ef80d6211e20`  
		Last Modified: Fri, 25 May 2018 15:48:00 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:melodic-ros-core-stretch`

```console
$ docker pull ros@sha256:cc703ab9d3fe2545d0bb8f2dd6a5679eb2c722a8e4c65e88072ed4a6f4206603
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-stretch` - linux; amd64

```console
$ docker pull ros@sha256:8f50e20366dae88c80cd0d88d2d7c94923fb35799cddda6def4a9b4e02417efd
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.2 MB (387229860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8599c8496128620f5a387471feeede6dd304f392b2241761e239c3ba8e04ec9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Apr 2018 07:08:53 GMT
ADD file:9572fdb59dfbb9b032f3331bbc2a08b31e0aef5fbde44c8f2008d22bf5290cf2 in / 
# Sat, 28 Apr 2018 07:08:53 GMT
CMD ["bash"]
# Sun, 29 Apr 2018 12:52:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:52:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Sun, 29 Apr 2018 12:52:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros-latest.list
# Sun, 29 Apr 2018 12:52:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sun, 29 Apr 2018 12:52:42 GMT
ENV LANG=C.UTF-8
# Sun, 29 Apr 2018 12:52:42 GMT
ENV LC_ALL=C.UTF-8
# Sun, 29 Apr 2018 12:52:54 GMT
RUN rosdep init     && rosdep update
# Tue, 15 May 2018 17:47:59 GMT
ENV ROS_DISTRO=melodic
# Thu, 24 May 2018 21:46:06 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 May 2018 21:46:07 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Thu, 24 May 2018 21:46:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 24 May 2018 21:46:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cc1a78bfd46becbfc3abb8a74d9a70a0e0dc7a5809bbd12e814f9382db003707`  
		Last Modified: Sat, 28 Apr 2018 09:27:54 GMT  
		Size: 45.3 MB (45318159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080d14fa56ef128c193fd94edf1e5eb031d02ae97b680588c7248e5e84304f13`  
		Last Modified: Sun, 29 Apr 2018 14:48:05 GMT  
		Size: 6.9 MB (6859072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604921583c4f613ebee4eb24564ca607566b8b48206868b48c018443567dd0b2`  
		Last Modified: Sun, 29 Apr 2018 14:48:03 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631afcce8e2d86cf9596b3823955679a3e770120d1da140a494003c85bf577b7`  
		Last Modified: Sun, 29 Apr 2018 14:48:00 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b0b4ce522ec73ddd931386acbe825b6203543509a3d76c51e649cb124d5ca1`  
		Last Modified: Sun, 29 Apr 2018 14:48:25 GMT  
		Size: 64.9 MB (64857453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea215428a3b38a4f7bc2be7aad6084d16a82bb84f706aebde2d34120ffc5190`  
		Last Modified: Sun, 29 Apr 2018 14:48:01 GMT  
		Size: 833.5 KB (833530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd9f60d7f6c7b6a8bb715d3a9803206d7a1eb5bfa04a9d74975b0ad026b77d1`  
		Last Modified: Thu, 24 May 2018 22:12:47 GMT  
		Size: 269.4 MB (269359856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117a3c26cbb3ca93f68e7314ae978a7e5baa750a43aa035c903facad8a260129`  
		Last Modified: Thu, 24 May 2018 22:11:40 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e7234b454c9a07e6d684ba7460a428f574598530f4776a0e1e1cf24f715f89db
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.8 MB (335824306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb2cd0f74f1c5bf0e72d21fe1d0c67040a6e1a1b88953cf08f2c0082d213eecf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 30 Apr 2018 23:31:58 GMT
ADD file:245a8cfe59ea071e4e215a722e0d4b4b14fa95dd6ffd03739fe048433cfaf523 in / 
# Mon, 30 Apr 2018 23:32:00 GMT
CMD ["bash"]
# Tue, 01 May 2018 03:30:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:30:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Tue, 01 May 2018 03:30:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros-latest.list
# Tue, 01 May 2018 03:35:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 01 May 2018 03:35:21 GMT
ENV LANG=C.UTF-8
# Tue, 01 May 2018 03:35:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 01 May 2018 03:36:07 GMT
RUN rosdep init     && rosdep update
# Wed, 16 May 2018 09:54:49 GMT
ENV ROS_DISTRO=melodic
# Fri, 25 May 2018 15:27:35 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 25 May 2018 15:27:40 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in / 
# Fri, 25 May 2018 15:27:41 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 25 May 2018 15:27:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:142bf25d8d1b3ebc9dfbedd586e70a011594690acf48b2695bfce01e3a2cf0d5`  
		Last Modified: Mon, 30 Apr 2018 23:52:13 GMT  
		Size: 43.1 MB (43109349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994bacc3e1c11e50065156c511f0c11e001707e55b61e361b8dc44d236c76f24`  
		Last Modified: Tue, 01 May 2018 04:41:15 GMT  
		Size: 6.4 MB (6427112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663899231a010cf1e857473d7203c7e5f109b38379d2d822c31dba98a7f8af10`  
		Last Modified: Tue, 01 May 2018 04:41:09 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d68d9781734de3f7c1ce451752978a14ba285ad3c63d5ab58034a2008cd25ef`  
		Last Modified: Tue, 01 May 2018 04:41:06 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678cb4b8d2f95bf400236eedd95783c53081503a2ed2b39f51e57a6062cd18c7`  
		Last Modified: Tue, 01 May 2018 04:42:23 GMT  
		Size: 61.9 MB (61938600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0225d679802c170200a58607e1e5a805065659ce28bdec6f9cc91f1c5f6ac461`  
		Last Modified: Tue, 01 May 2018 04:41:08 GMT  
		Size: 835.1 KB (835084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ff3cd1cf2d3e46a7f8fe4a2e5e91ff0815a51d5c87cfd81a1b8932dea453b8`  
		Last Modified: Fri, 25 May 2018 15:55:33 GMT  
		Size: 223.5 MB (223512365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5879828040241eb3667bd05cbfcc6b14911bf87255edd35c912781995caeb5`  
		Last Modified: Fri, 25 May 2018 15:54:14 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
