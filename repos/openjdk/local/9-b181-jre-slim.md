# `openjdk:9-b181-jre-slim`

## Docker Metadata

- Image ID: `sha256:6e1d5aaeae0297ef78e3f95ab49ce1d28f0e6294ad7b1c9c7c5687a01ca45430`
- Created: `2017-10-10T01:02:32.216261551Z`
- Virtual Size: ~ 371.21 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `LANG=C.UTF-8`
  - `JAVA_HOME=/docker-java-home`
  - `JAVA_VERSION=9-b181`
  - `JAVA_DEBIAN_VERSION=9~b181-4`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.2.52-3`

Binary Packages:

- `libacl1:amd64=2.2.52-3+b1`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.2.52-3
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.52-3.dsc' acl_2.2.52-3.dsc 2025 SHA256:82e344b9ab176559a85630b74ee5a68d678d7f24b6fe8139f2fd9fcf38a48095
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.52.orig.tar.bz2' acl_2.2.52.orig.tar.bz2 312128 SHA256:59d05b38af76baf2eddccbf08c7968a17451cc785ffecc657fcb46ce32b2631d
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.52-3.debian.tar.xz' acl_2.2.52-3.debian.tar.xz 8740 SHA256:fc3f1178d18288993fc4ce4853b7f9dcdf0bd1fd26e4f69349a4e4e5916d1fa8
```

Other potentially useful URLs:

- https://sources.debian.net/src/acl/2.2.52-3/ (for browsing the source)
- https://sources.debian.net/src/acl/2.2.52-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/acl/2.2.52-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `adduser=3.116`

Binary Packages:

- `adduser=3.116`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.116
'http://deb.debian.org/debian/pool/main/a/adduser/adduser_3.116.dsc' adduser_3.116.dsc 1740 SHA256:50e4154d3101101a890864185a09478c182155dc13f73dbb465c4279213bfafa
'http://deb.debian.org/debian/pool/main/a/adduser/adduser_3.116.tar.xz' adduser_3.116.tar.xz 212012 SHA256:72d811ad3ba17d2794b14d19acd1d6b57f9dd31d9250d51e786895dee2daeac0
```

Other potentially useful URLs:

- https://sources.debian.net/src/adduser/3.116/ (for browsing the source)
- https://sources.debian.net/src/adduser/3.116/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/adduser/3.116/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apparmor=2.11.0-11`

Binary Packages:

- `libapparmor1:amd64=2.11.0-11`

Licenses: (parsed from: `/usr/share/doc/libapparmor1/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris apparmor=2.11.0-11
'http://deb.debian.org/debian/pool/main/a/apparmor/apparmor_2.11.0-11.dsc' apparmor_2.11.0-11.dsc 3125 SHA256:418e6c1a67c8e970d3b0b0417f6124dbe1e5371908e8af60a88d1487de1ff2f8
'http://deb.debian.org/debian/pool/main/a/apparmor/apparmor_2.11.0.orig.tar.gz' apparmor_2.11.0.orig.tar.gz 5013297 SHA256:b1c489ea11e7771b8e6b181532cafbf9ebe6603e3cb00e2558f21b7a5bdd739a
'http://deb.debian.org/debian/pool/main/a/apparmor/apparmor_2.11.0-11.debian.tar.xz' apparmor_2.11.0-11.debian.tar.xz 88956 SHA256:07dc32b369c62a05fd4a0a7c0007ba5bb6f2f36ace6db38989c8b99b8fa0c050
```

Other potentially useful URLs:

- https://sources.debian.net/src/apparmor/2.11.0-11/ (for browsing the source)
- https://sources.debian.net/src/apparmor/2.11.0-11/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apparmor/2.11.0-11/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apt=1.5`

Binary Packages:

- `apt=1.5`
- `libapt-pkg5.0:amd64=1.5`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg5.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=1.5
'http://deb.debian.org/debian/pool/main/a/apt/apt_1.5.dsc' apt_1.5.dsc 2599 SHA256:6e4600cf5e30c4aeba4203f0c869a60be6296ef35504b39a217a18f8b0f963cf
'http://deb.debian.org/debian/pool/main/a/apt/apt_1.5.tar.xz' apt_1.5.tar.xz 2095240 SHA256:7d9a4daf7a4ae87de7ff4b1423e951ce66fe0535944f0774c8890d8f2a23e920
```

Other potentially useful URLs:

- https://sources.debian.net/src/apt/1.5/ (for browsing the source)
- https://sources.debian.net/src/apt/1.5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apt/1.5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `attr=1:2.4.47-2`

Binary Packages:

- `libattr1:amd64=1:2.4.47-2+b2`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.4.47-2
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.47-2.dsc' attr_2.4.47-2.dsc 2027 SHA256:ee842d6d62d473acf02b494c432cf33128fa46455a09d3172c77c252449fa1a6
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.47.orig.tar.bz2' attr_2.4.47.orig.tar.bz2 281877 SHA256:6c1208035757f5ce9b516402dd45b8299a53ae4d69ad2c352116f9cb8d7bc274
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.47-2.debian.tar.xz' attr_2.4.47-2.debian.tar.xz 8096 SHA256:f65909562def601b1556393f5656032c058dc574ba622414ad3eb80c7b05a42a
```

Other potentially useful URLs:

- https://sources.debian.net/src/attr/1:2.4.47-2/ (for browsing the source)
- https://sources.debian.net/src/attr/1:2.4.47-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/attr/1:2.4.47-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `audit=1:2.7.8-1`

Binary Packages:

- `libaudit-common=1:2.7.8-1`
- `libaudit1:amd64=1:2.7.8-1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/audit/1:2.7.8-1/


### `dpkg` source package: `avahi=0.7-3`

Binary Packages:

- `libavahi-client3:amd64=0.7-3`
- `libavahi-common-data:amd64=0.7-3`
- `libavahi-common3:amd64=0.7-3`

Licenses: (parsed from: `/usr/share/doc/libavahi-client3/copyright`, `/usr/share/doc/libavahi-common-data/copyright`, `/usr/share/doc/libavahi-common3/copyright`)

- `GPL`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris avahi=0.7-3
'http://deb.debian.org/debian/pool/main/a/avahi/avahi_0.7-3.dsc' avahi_0.7-3.dsc 3911 SHA256:b6fd44fc4044283e5a0db3558db08329548e86741da879f4da42ec817706e72d
'http://deb.debian.org/debian/pool/main/a/avahi/avahi_0.7.orig.tar.gz' avahi_0.7.orig.tar.gz 1333400 SHA256:57a99b5dfe7fdae794e3d1ee7a62973a368e91e414bd0dfa5d84434de5b14804
'http://deb.debian.org/debian/pool/main/a/avahi/avahi_0.7-3.debian.tar.xz' avahi_0.7-3.debian.tar.xz 30472 SHA256:b711982b1a1d301b6c40b29318c25617cb5eaedb212ce6acb4e6fbfac221f55c
```

Other potentially useful URLs:

- https://sources.debian.net/src/avahi/0.7-3/ (for browsing the source)
- https://sources.debian.net/src/avahi/0.7-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/avahi/0.7-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-files=10`

Binary Packages:

- `base-files=10`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=10
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_10.dsc' base-files_10.dsc 1063 SHA256:9e0e1f9fa67c55c552e053c340327f2d6c366b882fab74197170b03caefac488
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_10.tar.xz' base-files_10.tar.xz 62872 SHA256:11a1f87511c26be242ad549b6d1262aed9c6a7eb2dd3a005d2e49bf41c445b83
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-files/10/ (for browsing the source)
- https://sources.debian.net/src/base-files/10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-files/10/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-passwd=3.5.44`

Binary Packages:

- `base-passwd=3.5.44`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.44
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.44.dsc' base-passwd_3.5.44.dsc 1685 SHA256:22a5db1e9bb71fa8a4d682b3f9c01470a61b8041eb6212471181c6808b268c13
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.44.tar.xz' base-passwd_3.5.44.tar.xz 52644 SHA256:f17a0746024572e86e60e4614cf226a81ffe682ceaf1a1fce9dc1a8002683e90
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-passwd/3.5.44/ (for browsing the source)
- https://sources.debian.net/src/base-passwd/3.5.44/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-passwd/3.5.44/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bash=4.4-5`

Binary Packages:

- `bash=4.4-5`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=4.4-5
'http://deb.debian.org/debian/pool/main/b/bash/bash_4.4-5.dsc' bash_4.4-5.dsc 2251 SHA256:1605c608c48f3d866e23a3d6989d23c1d910d58b2a64eee13ad0efd2d98d4b06
'http://deb.debian.org/debian/pool/main/b/bash/bash_4.4.orig.tar.xz' bash_4.4.orig.tar.xz 4878580 SHA256:819ebb6a23799e9e4ca56ac579778c46902005bd5ade4f131ed293d9f77108e7
'http://deb.debian.org/debian/pool/main/b/bash/bash_4.4-5.debian.tar.xz' bash_4.4-5.debian.tar.xz 65640 SHA256:e01cc0f49941d81bee4e81f3eeefede280a91ad9365947234f29f1cb783f9dd8
```

Other potentially useful URLs:

- https://sources.debian.net/src/bash/4.4-5/ (for browsing the source)
- https://sources.debian.net/src/bash/4.4-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bash/4.4-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bzip2=1.0.6-8.1`

Binary Packages:

- `bzip2=1.0.6-8.1`
- `libbz2-1.0:amd64=1.0.6-8.1`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.6-8.1
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.6-8.1.dsc' bzip2_1.0.6-8.1.dsc 2082 SHA256:d80deed11a1419ad090cb486dd2335850fd8719b809c32002dea04b485f55dbd
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.6.orig.tar.bz2' bzip2_1.0.6.orig.tar.bz2 708737 SHA256:d70a9ccd8bdf47e302d96c69fecd54925f45d9c7b966bb4ef5f56b770960afa7
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.6-8.1.debian.tar.bz2' bzip2_1.0.6-8.1.debian.tar.bz2 59875 SHA256:bdbe7bf29e014e44d79bb7c733fe63cae990ab50882a4a07867cf69c61ad72b7
```

Other potentially useful URLs:

- https://sources.debian.net/src/bzip2/1.0.6-8.1/ (for browsing the source)
- https://sources.debian.net/src/bzip2/1.0.6-8.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bzip2/1.0.6-8.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ca-certificates-java=20170930`

Binary Packages:

- `ca-certificates-java=20170930`

Licenses: (parsed from: `/usr/share/doc/ca-certificates-java/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates-java=20170930
'http://deb.debian.org/debian/pool/main/c/ca-certificates-java/ca-certificates-java_20170930.dsc' ca-certificates-java_20170930.dsc 1813 SHA256:737af3f4b8aee01a8c21414441f0bac0a77ecbb71c4cb1ef0722c9166e45402d
'http://deb.debian.org/debian/pool/main/c/ca-certificates-java/ca-certificates-java_20170930.tar.xz' ca-certificates-java_20170930.tar.xz 16324 SHA256:369855f552500446e9dfcf5e5ae7e1225315cdf5a9880944ca03865f2d880e91
```

Other potentially useful URLs:

- https://sources.debian.net/src/ca-certificates-java/20170930/ (for browsing the source)
- https://sources.debian.net/src/ca-certificates-java/20170930/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ca-certificates-java/20170930/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ca-certificates=20170717`

Binary Packages:

- `ca-certificates=20170717`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20170717
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20170717.dsc' ca-certificates_20170717.dsc 1506 SHA256:da6268ff88e05c85c23c62add13d3d127087467d0c7e83974ca28db5543a252a
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20170717.tar.xz' ca-certificates_20170717.tar.xz 293028 SHA256:e487639b641fa75445174734dd6e9d600373e3248b3d86a7e3c6d0f6977decd2
```

Other potentially useful URLs:

- https://sources.debian.net/src/ca-certificates/20170717/ (for browsing the source)
- https://sources.debian.net/src/ca-certificates/20170717/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ca-certificates/20170717/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cdebconf=0.230`

Binary Packages:

- `libdebconfclient0:amd64=0.230`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/cdebconf/0.230/


### `dpkg` source package: `coreutils=8.28-1`

Binary Packages:

- `coreutils=8.28-1`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coreutils=8.28-1
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.28-1.dsc' coreutils_8.28-1.dsc 2111 SHA256:e9221d4c6f9d93474239beac1f8033d7215e3023d7d68d2effad8ed2fb71bd2c
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.28.orig.tar.xz' coreutils_8.28.orig.tar.xz 5252336 SHA256:1117b1a16039ddd84d51a9923948307cfa28c2cea03d1a2438742253df0a0c65
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.28.orig.tar.xz.asc' coreutils_8.28.orig.tar.xz.asc 1196 SHA256:505b1a530a55732a9ed659d419ff4973d1b15059078d2060675927058db9607d
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.28-1.debian.tar.xz' coreutils_8.28-1.debian.tar.xz 31332 SHA256:103ed661baf57ea9015418ff9e2d4afd35c17c35f10224c340cfe317c1d81215
```

Other potentially useful URLs:

- https://sources.debian.net/src/coreutils/8.28-1/ (for browsing the source)
- https://sources.debian.net/src/coreutils/8.28-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coreutils/8.28-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cups=2.2.4-7`

Binary Packages:

- `libcups2:amd64=2.2.4-7`

Licenses: (parsed from: `/usr/share/doc/libcups2/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2.0 with AOSDL exception`
- `LGPL-2`
- `LGPL-2.0 with AOSDL exception`
- `Zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/cups/2.2.4-7/


### `dpkg` source package: `dash=0.5.8-2.5`

Binary Packages:

- `dash=0.5.8-2.5`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.8-2.5
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.8-2.5.dsc' dash_0.5.8-2.5.dsc 1807 SHA256:42e77c37a5a4db1cc8274c3183d83e7173883cc611339815d92358562b74d066
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.8.orig.tar.gz' dash_0.5.8.orig.tar.gz 223028 SHA256:c6db3a237747b02d20382a761397563d813b306c020ae28ce25a1c3915fac60f
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.8-2.5.diff.gz' dash_0.5.8-2.5.diff.gz 44513 SHA256:53f55bbcb327b0e2dd687c44bf0610f5e304dd00733c81c101be46e0adf8ec89
```

Other potentially useful URLs:

- https://sources.debian.net/src/dash/0.5.8-2.5/ (for browsing the source)
- https://sources.debian.net/src/dash/0.5.8-2.5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dash/0.5.8-2.5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `db5.3=5.3.28-13.1`

Binary Packages:

- `libdb5.3:amd64=5.3.28-13.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28-13.1
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28-13.1.dsc' db5.3_5.3.28-13.1.dsc 3124 SHA256:8941edcad8e16fe6bc76ffcbe86dbdaadc654b5ed994654689cf5408602a84f3
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28.orig.tar.xz' db5.3_5.3.28.orig.tar.xz 24154920 SHA256:e1f85c8b6ebd0ed3ca72fa0ae97b65006f6d0bd0cd6f4ac24bed103cb5497bf5
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28-13.1.debian.tar.xz' db5.3_5.3.28-13.1.debian.tar.xz 28180 SHA256:9e04b9269be51de4e73536584addc61e19b29e34f769e263c180228064c72ec9
```

Other potentially useful URLs:

- https://sources.debian.net/src/db5.3/5.3.28-13.1/ (for browsing the source)
- https://sources.debian.net/src/db5.3/5.3.28-13.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/db5.3/5.3.28-13.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dbus=1.11.20-1`

Binary Packages:

- `dbus=1.11.20-1`
- `libdbus-1-3:amd64=1.11.20-1`

Licenses: (parsed from: `/usr/share/doc/dbus/copyright`, `/usr/share/doc/libdbus-1-3/copyright`)

- `AFL-2.1`
- `AFL-2.1,`
- `BSD-3-clause`
- `BSD-3-clause-generic`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `Tcl-BSDish`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris dbus=1.11.20-1
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.11.20-1.dsc' dbus_1.11.20-1.dsc 3676 SHA256:69b9485a05455e46f93733544d8b9cc45d629f6296d82d2ce125facdd044c196
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.11.20.orig.tar.gz' dbus_1.11.20.orig.tar.gz 2061444 SHA256:7fd9d0536f7ec2f2afc94b84d5b5487f88c464e8d47c661d8e0b54aa83974bfa
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.11.20.orig.tar.gz.asc' dbus_1.11.20.orig.tar.gz.asc 833 SHA256:d523edc62262f50c1584934c6b461cadc619ba63af132c08235a9cfc4b26556d
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.11.20-1.debian.tar.xz' dbus_1.11.20-1.debian.tar.xz 59424 SHA256:c857c548eccf13cbb7eb0e210b448a60c5f5096dc49ecd9acb55871d1c2388b2
```

Other potentially useful URLs:

- https://sources.debian.net/src/dbus/1.11.20-1/ (for browsing the source)
- https://sources.debian.net/src/dbus/1.11.20-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dbus/1.11.20-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debconf=1.5.63`

Binary Packages:

- `debconf=1.5.63`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/debconf/1.5.63/


### `dpkg` source package: `debian-archive-keyring=2017.6`

Binary Packages:

- `debian-archive-keyring=2017.6`

Licenses: (parsed from: `/usr/share/doc/debian-archive-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debian-archive-keyring=2017.6
'http://deb.debian.org/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2017.6.dsc' debian-archive-keyring_2017.6.dsc 1788 SHA256:366f7e854cc3686755e1988977fb276790beb581dd4bb2a0faac87a59ebef5b0
'http://deb.debian.org/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2017.6.tar.xz' debian-archive-keyring_2017.6.tar.xz 79560 SHA256:d5b3a7ad4030324489fa783235d3c5cd98e47ecb24e23533cb419cc696d6f7be
```

Other potentially useful URLs:

- https://sources.debian.net/src/debian-archive-keyring/2017.6/ (for browsing the source)
- https://sources.debian.net/src/debian-archive-keyring/2017.6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debian-archive-keyring/2017.6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debianutils=4.8.2`

Binary Packages:

- `debianutils=4.8.2`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debianutils=4.8.2
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_4.8.2.dsc' debianutils_4.8.2.dsc 1731 SHA256:175edfd4a94f20d34784b36c644cf8c23ee23686ebee6ad0c10c32b76e41c34f
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_4.8.2.tar.xz' debianutils_4.8.2.tar.xz 155944 SHA256:4deb5f293fd3e43c5d4a625a30b18d0fb07662ff77f769e3272841cdb61e7c68
```

Other potentially useful URLs:

- https://sources.debian.net/src/debianutils/4.8.2/ (for browsing the source)
- https://sources.debian.net/src/debianutils/4.8.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debianutils/4.8.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `diffutils=1:3.6-1`

Binary Packages:

- `diffutils=1:3.6-1`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.6-1
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.6-1.dsc' diffutils_3.6-1.dsc 1453 SHA256:26fe7690b45748dc92cee6af224192e78db2ac574e16ae0aeb8ed6a472c883cd
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.6.orig.tar.xz' diffutils_3.6.orig.tar.xz 1398296 SHA256:d621e8bdd4b573918c8145f7ae61817d1be9deb4c8d2328a65cea8e11d783bd6
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.6-1.debian.tar.xz' diffutils_3.6-1.debian.tar.xz 10808 SHA256:f6ab546a134bde18a87ca8e3c98919680e79d81a65a24801ae06ef69b33f24d8
```

Other potentially useful URLs:

- https://sources.debian.net/src/diffutils/1:3.6-1/ (for browsing the source)
- https://sources.debian.net/src/diffutils/1:3.6-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/diffutils/1:3.6-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dpkg=1.18.24`

Binary Packages:

- `dpkg=1.18.24`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.18.24
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.18.24.dsc' dpkg_1.18.24.dsc 2032 SHA256:9f1560a0d237ec570f98f8aacfd1cbdd372371cce40e4c7ee4a31315b0c40823
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.18.24.tar.xz' dpkg_1.18.24.tar.xz 4530444 SHA256:d853081d3e06bfd46a227056e591f094e42e78fa8a5793b0093bad30b710d7b4
```

Other potentially useful URLs:

- https://sources.debian.net/src/dpkg/1.18.24/ (for browsing the source)
- https://sources.debian.net/src/dpkg/1.18.24/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dpkg/1.18.24/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `e2fsprogs=1.43.6-1`

Binary Packages:

- `e2fslibs:amd64=1.43.6-1`
- `e2fsprogs=1.43.6-1`
- `libcomerr2:amd64=1.43.6-1`
- `libss2:amd64=1.43.6-1`

Licenses: (parsed from: `/usr/share/doc/e2fslibs/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcomerr2/copyright`, `/usr/share/doc/libss2/copyright`)

- `GPL-2`
- `LGPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/e2fsprogs/1.43.6-1/


### `dpkg` source package: `elfutils=0.170-0.1`

Binary Packages:

- `libelf1:amd64=0.170-0.1`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-`

Source:

```console
$ apt-get source -qq --print-uris elfutils=0.170-0.1
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.170-0.1.dsc' elfutils_0.170-0.1.dsc 2293 SHA256:a4f4a38b6bbb939080323243584362129b54a1cedc873b3c449067c3055e7523
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.170.orig.tar.bz2' elfutils_0.170.orig.tar.bz2 8358001 SHA256:1f844775576b79bdc9f9c717a50058d08620323c1e935458223a12f249c9e066
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.170-0.1.debian.tar.xz' elfutils_0.170-0.1.debian.tar.xz 37504 SHA256:71accbdfb81c3abe45e746b96bd62cc08d2b3c4c4073acece2e6a354f1595fa2
```

Other potentially useful URLs:

- https://sources.debian.net/src/elfutils/0.170-0.1/ (for browsing the source)
- https://sources.debian.net/src/elfutils/0.170-0.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/elfutils/0.170-0.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `expat=2.2.3-1`

Binary Packages:

- `libexpat1:amd64=2.2.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris expat=2.2.3-1
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.3-1.dsc' expat_2.2.3-1.dsc 2284 SHA256:c5f2c77f5b69361a38fbf9b2b3044cf823b6243d1029ca9e5754da2bd08f936d
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.3.orig.tar.bz2' expat_2.2.3.orig.tar.bz2 435593 SHA256:b31890fb02f85c002a67491923f89bda5028a880fd6c374f707193ad81aace5f
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.3-1.debian.tar.xz' expat_2.2.3-1.debian.tar.xz 10640 SHA256:885dda6baf300f15ef2c75f225d10736236056c7a9bf9405d1d3d138fbb7c63e
```

Other potentially useful URLs:

- https://sources.debian.net/src/expat/2.2.3-1/ (for browsing the source)
- https://sources.debian.net/src/expat/2.2.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/expat/2.2.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `findutils=4.6.0+git+20170729-2`

Binary Packages:

- `findutils=4.6.0+git+20170729-2`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.6.0+git+20170729-2
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.6.0+git+20170729-2.dsc' findutils_4.6.0+git+20170729-2.dsc 2220 SHA256:c59d5c89d6d5e794fd27cd2399d52d033629ae22a7551c1029aa8a779acaab56
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.6.0+git+20170729.orig.tar.xz' findutils_4.6.0+git+20170729.orig.tar.xz 1865076 SHA256:a8be399ed28bca5042313dcaa8e6b90550b8da0d6497311fcdb3823259b5d7ac
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.6.0+git+20170729-2.debian.tar.xz' findutils_4.6.0+git+20170729-2.debian.tar.xz 25572 SHA256:aa6d4a9f31870313a807d455bbc98030659ae69985d2e6893619e3997d01f022
```

Other potentially useful URLs:

- https://sources.debian.net/src/findutils/4.6.0+git+20170729-2/ (for browsing the source)
- https://sources.debian.net/src/findutils/4.6.0+git+20170729-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/findutils/4.6.0+git+20170729-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `freetype=2.8-0.2`

Binary Packages:

- `libfreetype6:amd64=2.8-0.2`

Licenses: (parsed from: `/usr/share/doc/libfreetype6/copyright`)

- `BSD-2-Clause`
- `BSD-3-Clause`
- `Catharon-OSL`
- `FTL`
- `GPL-2`
- `GPL-2+`
- `GZip`
- `OpenGroup-BSD-like`

Source:

```console
$ apt-get source -qq --print-uris freetype=2.8-0.2
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.8-0.2.dsc' freetype_2.8-0.2.dsc 1802 SHA256:d43fec201f695524148e691e73c4dfc243ff57b3a238feb7b50148385e00441d
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.8.orig.tar.gz' freetype_2.8.orig.tar.gz 4225710 SHA256:7ba438204ec4532cfa770faff63a90f0555369bb594c15014cc0fb5f0d52e3b4
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.8-0.2.diff.gz' freetype_2.8-0.2.diff.gz 37779 SHA256:5060fb3ad83ddbec18334a80bcf6697468131d9ec2a03d3ab992e5b695b84352
```

Other potentially useful URLs:

- https://sources.debian.net/src/freetype/2.8-0.2/ (for browsing the source)
- https://sources.debian.net/src/freetype/2.8-0.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/freetype/2.8-0.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-5=5.4.1-14`

Binary Packages:

- `gcc-5-base:amd64=5.4.1-14`

Licenses: (parsed from: `/usr/share/doc/gcc-5-base/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/gcc-5/5.4.1-14/


### `dpkg` source package: `gcc-6=6.4.0-7`

Binary Packages:

- `gcc-6-base:amd64=6.4.0-7`

Licenses: (parsed from: `/usr/share/doc/gcc-6-base/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris gcc-6=6.4.0-7
'http://deb.debian.org/debian/pool/main/g/gcc-6/gcc-6_6.4.0-7.dsc' gcc-6_6.4.0-7.dsc 19495 SHA256:83ec86854680b4793dcf737c4f2167a1c8629bb5b2c3f3e15ba650fecd4cff5c
'http://deb.debian.org/debian/pool/main/g/gcc-6/gcc-6_6.4.0.orig.tar.gz' gcc-6_6.4.0.orig.tar.gz 81632257 SHA256:13220c723ddb7a69ff5690070b245886ac99afe5a31ee106ac36d6f013234a67
'http://deb.debian.org/debian/pool/main/g/gcc-6/gcc-6_6.4.0-7.diff.gz' gcc-6_6.4.0-7.diff.gz 1706240 SHA256:86d8530e94e00a21608b7092acd48e704fb35eb8477a43bfe004ebffc444737f
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-6/6.4.0-7/ (for browsing the source)
- https://sources.debian.net/src/gcc-6/6.4.0-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-6/6.4.0-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-7=7.2.0-8`

Binary Packages:

- `gcc-7-base:amd64=7.2.0-8`
- `libgcc1:amd64=1:7.2.0-8`
- `libstdc++6:amd64=7.2.0-8`

Licenses: (parsed from: `/usr/share/doc/gcc-7-base/copyright`, `/usr/share/doc/libgcc1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-7=7.2.0-8
'http://deb.debian.org/debian/pool/main/g/gcc-7/gcc-7_7.2.0-8.dsc' gcc-7_7.2.0-8.dsc 26328 SHA256:8cfedde7bca4730357bfc04b396913946a86f288287fc39cd49d18e46e6d3ebf
'http://deb.debian.org/debian/pool/main/g/gcc-7/gcc-7_7.2.0.orig.tar.gz' gcc-7_7.2.0.orig.tar.gz 70028185 SHA256:a1050ca96c2b931ad82da3caf2868cd68b95a62151ac9af53fbe9b69b6e9b651
'http://deb.debian.org/debian/pool/main/g/gcc-7/gcc-7_7.2.0-8.diff.gz' gcc-7_7.2.0-8.diff.gz 3094749 SHA256:3a6a3bf78a4282ff51f729aaf0b81985afe85a35063be23ec31ac7c620c02daa
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-7/7.2.0-8/ (for browsing the source)
- https://sources.debian.net/src/gcc-7/7.2.0-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-7/7.2.0-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glibc=2.24-17`

Binary Packages:

- `libc-bin=2.24-17`
- `libc6:amd64=2.24-17`
- `multiarch-support=2.24-17`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/multiarch-support/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.24-17
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.24-17.dsc' glibc_2.24-17.dsc 8226 SHA256:8f8db58051f431525439dae692242124befba9cfab64b406ec8964818ba46a43
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.24.orig.tar.xz' glibc_2.24.orig.tar.xz 13921912 SHA256:ed71e8afd2b270f7947a2cea2457a31e1ca4fac08e2731d80edd7ec1730ec84f
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.24-17.debian.tar.xz' glibc_2.24-17.debian.tar.xz 1036004 SHA256:a66991c3d29bb30e57ef8eaeb1732b3694689cb8d4eb999ccb018076a02c5940
```

Other potentially useful URLs:

- https://sources.debian.net/src/glibc/2.24-17/ (for browsing the source)
- https://sources.debian.net/src/glibc/2.24-17/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glibc/2.24-17/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gmp=2:6.1.2+dfsg-1.1`

Binary Packages:

- `libgmp10:amd64=2:6.1.2+dfsg-1.1`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.1.2+dfsg-1.1
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.1.2+dfsg-1.1.dsc' gmp_6.1.2+dfsg-1.1.dsc 2216 SHA256:64148f371d169bd803ffcc29f407de7bdf0742b7503ba7d9c0f973045e200c98
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.1.2+dfsg.orig.tar.xz' gmp_6.1.2+dfsg.orig.tar.xz 1804424 SHA256:18016f718f621e7641ddd4e57f8e140391c5183252e5998263ffff59198a65b7
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.1.2+dfsg-1.1.debian.tar.xz' gmp_6.1.2+dfsg-1.1.debian.tar.xz 20756 SHA256:d1ef813f1874720069bda6fe9417672f21123a59d82a4c13ffc4b4e951905ac5
```

Other potentially useful URLs:

- https://sources.debian.net/src/gmp/2:6.1.2+dfsg-1.1/ (for browsing the source)
- https://sources.debian.net/src/gmp/2:6.1.2+dfsg-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gmp/2:6.1.2+dfsg-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnupg2=2.2.1-1`

Binary Packages:

- `gpgv=2.2.1-1`

Licenses: (parsed from: `/usr/share/doc/gpgv/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`
- `RFC-Reference`
- `TinySCHEME`
- `permissive`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/gnupg2/2.2.1-1/


### `dpkg` source package: `gnutls28=3.5.15-2`

Binary Packages:

- `libgnutls30:amd64=3.5.15-2`

Licenses: (parsed from: `/usr/share/doc/libgnutls30/copyright`)

- `CC0 license`
- `GFDL-1.3`
- `GPL`
- `GPL-3`
- `LGPL`
- `LGPL-3`
- `LGPL2.1`
- `The MIT License (MIT)`
- `The main library is licensed under GNU Lesser`

Source:

```console
$ apt-get source -qq --print-uris gnutls28=3.5.15-2
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.5.15-2.dsc' gnutls28_3.5.15-2.dsc 3322 SHA256:16712db8bb067d802958d462274fcc87dcaece8ea4ab5a3d6fd182520fbc4272
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.5.15.orig.tar.xz' gnutls28_3.5.15.orig.tar.xz 7238928 SHA256:046081108b8b1fe455a13a4c5a4eaa0368e185b678f1670fe09a11a2d7ecfad5
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.5.15.orig.tar.xz.asc' gnutls28_3.5.15.orig.tar.xz.asc 310 SHA256:8e19becd65224aefc70a0ea15df7369ed9588f9d692cc5cd790a72b541a48de2
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.5.15-2.debian.tar.xz' gnutls28_3.5.15-2.debian.tar.xz 100840 SHA256:b470739833727c0f4f58c14b598c4e3ad56384e4fbb271a10106418c9a44143e
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnutls28/3.5.15-2/ (for browsing the source)
- https://sources.debian.net/src/gnutls28/3.5.15-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnutls28/3.5.15-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `grep=3.1-2`

Binary Packages:

- `grep=3.1-2`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.1-2
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.1-2.dsc' grep_3.1-2.dsc 2046 SHA256:b75ef8eb1399a49274bafe972679680b7add1500a4ee82eedaa0372f8ed744a0
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.1.orig.tar.xz' grep_3.1.orig.tar.xz 1370880 SHA256:db625c7ab3bb3ee757b3926a5cfa8d9e1c3991ad24707a83dde8a5ef2bf7a07e
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.1-2.debian.tar.bz2' grep_3.1-2.debian.tar.bz2 110067 SHA256:f09ce7a3c860a5de8939ebceb5fcd85d00d1537ad9f998dae5f623d9bcfe4e40
```

Other potentially useful URLs:

- https://sources.debian.net/src/grep/3.1-2/ (for browsing the source)
- https://sources.debian.net/src/grep/3.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/grep/3.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gzip=1.6-5`

Binary Packages:

- `gzip=1.6-5+b1`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.6-5
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.6-5.dsc' gzip_1.6-5.dsc 1867 SHA256:922751ee5fc426d623e824c55f7822fa60f26f35b5389b37c8b15feff639608c
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.6.orig.tar.gz' gzip_1.6.orig.tar.gz 1074924 SHA256:97eb83b763d9e5ad35f351fe5517e6b71521d7aac7acf3e3cacdb6b1496d8f7e
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.6-5.debian.tar.xz' gzip_1.6-5.debian.tar.xz 14684 SHA256:ac5282c32083ff58fc01317ee402b687b3806555aa1d4e80a62bb0f2ad93167e
```

Other potentially useful URLs:

- https://sources.debian.net/src/gzip/1.6-5/ (for browsing the source)
- https://sources.debian.net/src/gzip/1.6-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gzip/1.6-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `hostname=3.18`

Binary Packages:

- `hostname=3.18+b1`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.18
'http://deb.debian.org/debian/pool/main/h/hostname/hostname_3.18.dsc' hostname_3.18.dsc 1446 SHA256:4d3d5c8ded08ffc2ebfb39817ba1994b5fc1966652b132ff3e16389b70af28d7
'http://deb.debian.org/debian/pool/main/h/hostname/hostname_3.18.tar.gz' hostname_3.18.tar.gz 13732 SHA256:5cc3ec120967b8f911e86b9561b53977bcc77191c84fe9c607177ccd09f8d207
```

Other potentially useful URLs:

- https://sources.debian.net/src/hostname/3.18/ (for browsing the source)
- https://sources.debian.net/src/hostname/3.18/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/hostname/3.18/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `init-system-helpers=1.49`

Binary Packages:

- `init-system-helpers=1.49`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/init-system-helpers/1.49/


### `dpkg` source package: `java-common=0.59`

Binary Packages:

- `java-common=0.59`

Licenses: (parsed from: `/usr/share/doc/java-common/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris java-common=0.59
'http://deb.debian.org/debian/pool/main/j/java-common/java-common_0.59.dsc' java-common_0.59.dsc 2134 SHA256:44f77a693749779f3bd78bf2b2ac1a5a2a9a7278eb0a9e00190e206d3cb31537
'http://deb.debian.org/debian/pool/main/j/java-common/java-common_0.59.tar.xz' java-common_0.59.tar.xz 13064 SHA256:d5737f7bacf02c81cace29176d8bddc3552b0857841aeb3435bcf52265d695ca
```

Other potentially useful URLs:

- https://sources.debian.net/src/java-common/0.59/ (for browsing the source)
- https://sources.debian.net/src/java-common/0.59/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/java-common/0.59/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `keyutils=1.5.9-9`

Binary Packages:

- `libkeyutils1:amd64=1.5.9-9`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.5.9-9
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.5.9-9.1.dsc' keyutils_1.5.9-9.1.dsc 2118 SHA256:a16d70de62b984b7064d6517884438846f4270948ff4680761112301beb0a20e
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.5.9.orig.tar.bz2' keyutils_1.5.9.orig.tar.bz2 74683 SHA256:4da2c5552c688b65ab14d4fd40fbdf720c8b396d8ece643e040cf6e707e083ae
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.5.9-9.1.debian.tar.xz' keyutils_1.5.9-9.1.debian.tar.xz 17644 SHA256:899184c857c9acdc62bd704666def7e7e733fc17b9da4f23d891ea31ce543127
```

Other potentially useful URLs:

- https://sources.debian.net/src/keyutils/1.5.9-9/ (for browsing the source)
- https://sources.debian.net/src/keyutils/1.5.9-9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/keyutils/1.5.9-9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `krb5=1.15.1-2`

Binary Packages:

- `krb5-locales=1.15.1-2`
- `libgssapi-krb5-2:amd64=1.15.1-2`
- `libk5crypto3:amd64=1.15.1-2`
- `libkrb5-3:amd64=1.15.1-2`
- `libkrb5support0:amd64=1.15.1-2`

Licenses: (parsed from: `/usr/share/doc/krb5-locales/copyright`, `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.15.1-2
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.15.1-2.dsc' krb5_1.15.1-2.dsc 3294 SHA256:717416ea51edbfd2555568631e700c15cce1244f730a97d317288ab0be20d43a
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.15.1.orig.tar.gz' krb5_1.15.1.orig.tar.gz 9375538 SHA256:437c8831ddd5fde2a993fef425dedb48468109bb3d3261ef838295045a89eb45
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.15.1-2.debian.tar.xz' krb5_1.15.1-2.debian.tar.xz 143404 SHA256:e44c17efbf26e5d2a3de7577a039085683efe21afb0da3eacc12c17dc01e9d1a
```

Other potentially useful URLs:

- https://sources.debian.net/src/krb5/1.15.1-2/ (for browsing the source)
- https://sources.debian.net/src/krb5/1.15.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/krb5/1.15.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lcms2=2.8-4`

Binary Packages:

- `liblcms2-2:amd64=2.8-4`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`)

- `GPL-2`
- `GPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris lcms2=2.8-4
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.8-4.dsc' lcms2_2.8-4.dsc 1997 SHA256:3b92900948848eef62fa91b78f6b6661bd84eae6c49c224248c7c48a09b5f028
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.8.orig.tar.gz' lcms2_2.8.orig.tar.gz 6687005 SHA256:66d02b229d2ea9474e62c2b6cd6720fde946155cd1d0d2bffdab829790a0fb22
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.8-4.debian.tar.xz' lcms2_2.8-4.debian.tar.xz 11036 SHA256:50c0040fc92e1f2ca27740f608ae248acdd5b21a633f34cf2fe4d66f1d05c4b4
```

Other potentially useful URLs:

- https://sources.debian.net/src/lcms2/2.8-4/ (for browsing the source)
- https://sources.debian.net/src/lcms2/2.8-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lcms2/2.8-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libbsd=0.8.6-2`

Binary Packages:

- `libbsd0:amd64=0.8.6-2`

Licenses: (parsed from: `/usr/share/doc/libbsd0/copyright`)

- `BSD-2-clause`
- `BSD-2-clause-NetBSD`
- `BSD-2-clause-author`
- `BSD-2-clause-verbatim`
- `BSD-3-clause`
- `BSD-3-clause-John-Birrell`
- `BSD-3-clause-Peter-Wemm`
- `BSD-3-clause-Regents`
- `BSD-4-clause-Christopher-G-Demetriou`
- `BSD-4-clause-Niels-Provos`
- `BSD-5-clause-Peter-Wemm`
- `Beerware`
- `Expat`
- `ISC`
- `ISC-Original`
- `public-domain`
- `public-domain-Colin-Plumb`

Source:

```console
$ apt-get source -qq --print-uris libbsd=0.8.6-2
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.8.6-2.dsc' libbsd_0.8.6-2.dsc 2181 SHA256:8adbd1e8bd9e36248be2530eb2ceb4ed0ebd6d16ad108f9620483a1f9b6ed055
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.8.6.orig.tar.xz' libbsd_0.8.6.orig.tar.xz 371112 SHA256:467fbf9df1f49af11f7f686691057c8c0a7613ae5a870577bef9155de39f9687
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.8.6.orig.tar.xz.asc' libbsd_0.8.6.orig.tar.xz.asc 833 SHA256:8b579470e8249b2ad24134989cc77404e3620e8ccda3d57650cfbcc7c50c26ce
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.8.6-2.debian.tar.xz' libbsd_0.8.6-2.debian.tar.xz 15684 SHA256:3ba08d93c36002737c4707b2dfdc13118d302487a53f1789d8ee22ed7107c491
```

Other potentially useful URLs:

- https://sources.debian.net/src/libbsd/0.8.6-2/ (for browsing the source)
- https://sources.debian.net/src/libbsd/0.8.6-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libbsd/0.8.6-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcap-ng=0.7.7-3`

Binary Packages:

- `libcap-ng0:amd64=0.7.7-3+b1`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libcap-ng/0.7.7-3/


### `dpkg` source package: `libffi=3.2.1-6`

Binary Packages:

- `libffi6:amd64=3.2.1-6`

Licenses: (parsed from: `/usr/share/doc/libffi6/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.2.1-6
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.2.1-6.dsc' libffi_3.2.1-6.dsc 1923 SHA256:f901298b078c7d7f3f75459b5ff74cc804f6f2cfd65ed619d2082d5f77089954
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.2.1.orig.tar.gz' libffi_3.2.1.orig.tar.gz 940837 SHA256:d06ebb8e1d9a22d19e38d63fdb83954253f39bedc5d46232a05645685722ca37
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.2.1-6.debian.tar.xz' libffi_3.2.1-6.debian.tar.xz 11252 SHA256:477709fa90f8c7631fa226a48cdf38737c9f195f3686f62aa76714bcffaee512
```

Other potentially useful URLs:

- https://sources.debian.net/src/libffi/3.2.1-6/ (for browsing the source)
- https://sources.debian.net/src/libffi/3.2.1-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libffi/3.2.1-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgcrypt20=1.7.9-1`

Binary Packages:

- `libgcrypt20:amd64=1.7.9-1`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.7.9-1
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.7.9-1.dsc' libgcrypt20_1.7.9-1.dsc 2914 SHA256:d922d12b25a64cd25601b34380bed9c9ca3c8fd4c9625951641fcc8766c7796d
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.7.9.orig.tar.bz2' libgcrypt20_1.7.9.orig.tar.bz2 2897137 SHA256:bfe9bb703c1126c3647da2810fd23039c2f09d46969f71612c2065dc3fa9373b
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.7.9.orig.tar.bz2.asc' libgcrypt20_1.7.9.orig.tar.bz2.asc 310 SHA256:96108d1701cd3c8a6826d7d2a27056de79421fe20bf9ef447e8c12e982f64414
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.7.9-1.debian.tar.xz' libgcrypt20_1.7.9-1.debian.tar.xz 26020 SHA256:1a0775f8e8921aa537db92c06cca82780cb24adf04775e2f944a23d867414d55
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgcrypt20/1.7.9-1/ (for browsing the source)
- https://sources.debian.net/src/libgcrypt20/1.7.9-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgcrypt20/1.7.9-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgpg-error=1.27-3`

Binary Packages:

- `libgpg-error0:amd64=1.27-3`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.27-3
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.27-3.dsc' libgpg-error_1.27-3.dsc 2377 SHA256:427eba727e5ff13b1f29493edc281cfa811aabe4c0d0f07f747ab11bc8e9574f
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.27.orig.tar.bz2' libgpg-error_1.27.orig.tar.bz2 813060 SHA256:4f93aac6fecb7da2b92871bb9ee33032be6a87b174f54abf8ddf0911a22d29d2
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.27-3.debian.tar.xz' libgpg-error_1.27-3.debian.tar.xz 15856 SHA256:c1a17ea7066c955be7f7117efdd0961cd43f3fd81152854e53a60cb08fba0a10
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgpg-error/1.27-3/ (for browsing the source)
- https://sources.debian.net/src/libgpg-error/1.27-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgpg-error/1.27-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libidn2-0=2.0.2-5`

Binary Packages:

- `libidn2-0:amd64=2.0.2-5`

Licenses: (parsed from: `/usr/share/doc/libidn2-0/copyright`)

- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-3+`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris libidn2-0=2.0.2-5
'http://deb.debian.org/debian/pool/main/libi/libidn2-0/libidn2-0_2.0.2-5.dsc' libidn2-0_2.0.2-5.dsc 2325 SHA256:59ae6b2cfb8a49f09710e3b42c1c3a5a48136051ed49445bd6925473dcfe1af5
'http://deb.debian.org/debian/pool/main/libi/libidn2-0/libidn2-0_2.0.2.orig.tar.gz' libidn2-0_2.0.2.orig.tar.gz 1925342 SHA256:8cd62828b2ab0171e0f35a302f3ad60c3a3fffb45733318b3a8205f9d187eeab
'http://deb.debian.org/debian/pool/main/libi/libidn2-0/libidn2-0_2.0.2-5.debian.tar.xz' libidn2-0_2.0.2-5.debian.tar.xz 60940 SHA256:5cf1e578a3bb2d302bd6276401e1d6bbea78b82c9acb0828e3d995d4ad4357eb
```

Other potentially useful URLs:

- https://sources.debian.net/src/libidn2-0/2.0.2-5/ (for browsing the source)
- https://sources.debian.net/src/libidn2-0/2.0.2-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libidn2-0/2.0.2-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libjpeg-turbo=1:1.5.2-2`

Binary Packages:

- `libjpeg62-turbo:amd64=1:1.5.2-2`

Licenses: (parsed from: `/usr/share/doc/libjpeg62-turbo/copyright`)

- `BSD-3`
- `BSD-BY-LC-NE`
- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=1:1.5.2-2
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.5.2-2.dsc' libjpeg-turbo_1.5.2-2.dsc 2434 SHA256:f975bd4b2192e3f1aeacef7f0de33035f386225035aea6157b413b1c500d46a1
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.5.2.orig.tar.gz' libjpeg-turbo_1.5.2.orig.tar.gz 1657235 SHA256:9098943b270388727ae61de82adec73cf9f0dbb240b3bc8b172595ebf405b528
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.5.2-2.debian.tar.xz' libjpeg-turbo_1.5.2-2.debian.tar.xz 78360 SHA256:964a2d747f8e74cbd558f343afd11b7dfe37212a611eeca863f1908eba66f728
```

Other potentially useful URLs:

- https://sources.debian.net/src/libjpeg-turbo/1:1.5.2-2/ (for browsing the source)
- https://sources.debian.net/src/libjpeg-turbo/1:1.5.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libjpeg-turbo/1:1.5.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpng1.6=1.6.34-1`

Binary Packages:

- `libpng16-16:amd64=1.6.34-1`

Licenses: (parsed from: `/usr/share/doc/libpng16-16/copyright`)

- `Apache-2.0`
- `BSD-3-clause`
- `BSD-like-with-advertising-clause`
- `GPL-2`
- `GPL-2+`
- `expat`
- `libpng`
- `libpng OR Apache-2.0 OR BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris libpng1.6=1.6.34-1
'http://deb.debian.org/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.34-1.dsc' libpng1.6_1.6.34-1.dsc 2191 SHA256:e491569d9015036d43c7a9dfcf2d835abde8c9817b057d55d929cb78501d5a30
'http://deb.debian.org/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.34.orig.tar.xz' libpng1.6_1.6.34.orig.tar.xz 997968 SHA256:2f1e960d92ce3b3abd03d06dfec9637dfbd22febf107a536b44f7a47c60659f6
'http://deb.debian.org/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.34-1.debian.tar.xz' libpng1.6_1.6.34-1.debian.tar.xz 23568 SHA256:8ca33d2930b340412f04d76cac3159f6b3b823cff33b35b72426a75f3f02a8a0
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpng1.6/1.6.34-1/ (for browsing the source)
- https://sources.debian.net/src/libpng1.6/1.6.34-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpng1.6/1.6.34-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libselinux=2.7-2`

Binary Packages:

- `libselinux1:amd64=2.7-2`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=2.7-2
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_2.7-2.dsc' libselinux_2.7-2.dsc 2369 SHA256:09e23dce37d309751db1b5a411a330c6fac9f392a67e56ce943bad88757af1df
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_2.7.orig.tar.gz' libselinux_2.7.orig.tar.gz 187574 SHA256:d0fec0769b3ad60aa7baf9b9a4b7a056827769dc2dadda0dc0eb59b3d1c18c57
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_2.7-2.debian.tar.xz' libselinux_2.7-2.debian.tar.xz 23044 SHA256:acd5c8f6607a5b10aeaa705214ea4924939cbe2de7cce174eccf5973c6f92771
```

Other potentially useful URLs:

- https://sources.debian.net/src/libselinux/2.7-2/ (for browsing the source)
- https://sources.debian.net/src/libselinux/2.7-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libselinux/2.7-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsemanage=2.7-2`

Binary Packages:

- `libsemanage-common=2.7-2`
- `libsemanage1:amd64=2.7-2`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=2.7-2
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_2.7-2.dsc' libsemanage_2.7-2.dsc 2456 SHA256:7054ef9c206cac2e698627040df04dd159ff7aa982348e25c315dd817fb8926b
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_2.7.orig.tar.gz' libsemanage_2.7.orig.tar.gz 153465 SHA256:07e9477714ce6a4557a1fe924ea4cb06501b62d0fa0e3c0dc32a2cf47cb8d476
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_2.7-2.debian.tar.xz' libsemanage_2.7-2.debian.tar.xz 16968 SHA256:6679667dc2ceafbe214eddfe84c3f6a18d457a4c78d6ae63165bc65e71b174e7
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsemanage/2.7-2/ (for browsing the source)
- https://sources.debian.net/src/libsemanage/2.7-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsemanage/2.7-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsepol=2.7-1`

Binary Packages:

- `libsepol1:amd64=2.7-1`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=2.7-1
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_2.7-1.dsc' libsepol_2.7-1.dsc 1814 SHA256:7de809477acd60d256eca160d5fc6986e5e65227706b1cdb23f8139bb49d2782
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_2.7.orig.tar.gz' libsepol_2.7.orig.tar.gz 471147 SHA256:d69d3bd8ec901a3bd5adf2be2fb47fb1a685ed73066ab482e7e505371a48f9e7
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_2.7-1.debian.tar.xz' libsepol_2.7-1.debian.tar.xz 13944 SHA256:56b1c2b0e492b2089f23a0d7a95a260377a0e3adefc60e90c0ff6eff6be08450
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsepol/2.7-1/ (for browsing the source)
- https://sources.debian.net/src/libsepol/2.7-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsepol/2.7-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtasn1-6=4.12-2.1`

Binary Packages:

- `libtasn1-6:amd64=4.12-2.1`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.12-2.1
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.12-2.1.dsc' libtasn1-6_4.12-2.1.dsc 2586 SHA256:0f762f07bbb39e9a49687e8bd7a18a5d3cc435d6c226eaecfcda7a8d325c2cef
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.12.orig.tar.gz' libtasn1-6_4.12.orig.tar.gz 1888450 SHA256:6753da2e621257f33f5b051cc114d417e5206a0818fe0b1ecfd6153f70934753
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.12-2.1.debian.tar.xz' libtasn1-6_4.12-2.1.debian.tar.xz 58728 SHA256:df32c448a8472eff20fa6989f939cbc0e2caf0d4bb712e54b31b39bbd6d8b781
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtasn1-6/4.12-2.1/ (for browsing the source)
- https://sources.debian.net/src/libtasn1-6/4.12-2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtasn1-6/4.12-2.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libunistring=0.9.7-2`

Binary Packages:

- `libunistring2:amd64=0.9.7-2`

Licenses: (parsed from: `/usr/share/doc/libunistring2/copyright`)

- `FreeSoftware`
- `GFDL-1.2`
- `GFDL-1.2+`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with distribution exception`
- `GPL-3`
- `GPL-3+`
- `LGPL-3`
- `LGPL-3+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libunistring=0.9.7-2
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.7-2.dsc' libunistring_0.9.7-2.dsc 1985 SHA256:2ac1f77b0fc421eadcbfbe1e2e022137f31404f4874f6ff326ed8644f8ca18c8
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.7.orig.tar.xz' libunistring_0.9.7.orig.tar.xz 1967300 SHA256:2e3764512aaf2ce598af5a38818c0ea23dedf1ff5460070d1b6cee5c3336e797
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.7-2.debian.tar.xz' libunistring_0.9.7-2.debian.tar.xz 39776 SHA256:6eaa5343ae3c40627a35fc8ac85a07c0da8236c8aa49205be7e51139f278c95c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libunistring/0.9.7-2/ (for browsing the source)
- https://sources.debian.net/src/libunistring/0.9.7-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libunistring/0.9.7-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libx11=2:1.6.4-3`

Binary Packages:

- `libx11-6:amd64=2:1.6.4-3`
- `libx11-data=2:1.6.4-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.6.4-3
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.4-3.dsc' libx11_1.6.4-3.dsc 2397 SHA256:4c5d6add2ba969067ca111c827ae94264e4c22776e22f318d264545dc1c6a300
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.4.orig.tar.gz' libx11_1.6.4.orig.tar.gz 3095115 SHA256:5d7fbb9e15c27900ea8963218a59750b674a8d7c94161b66e96fcfbdaa1c6263
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.4-3.diff.gz' libx11_1.6.4-3.diff.gz 41366 SHA256:2c936827bca63eaf5b66683bdcd0ecf013d152c35439f792475db85c5c2338fd
```

Other potentially useful URLs:

- https://sources.debian.net/src/libx11/2:1.6.4-3/ (for browsing the source)
- https://sources.debian.net/src/libx11/2:1.6.4-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libx11/2:1.6.4-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxau=1:1.0.8-1`

Binary Packages:

- `libxau6:amd64=1:1.0.8-1+b2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxau=1:1.0.8-1
'http://deb.debian.org/debian/pool/main/libx/libxau/libxau_1.0.8-1.dsc' libxau_1.0.8-1.dsc 2040 SHA256:3ddb5f2c7a49ef7507b8d1e63e891238db877b4d1bb1c5486a3e3242c8523602
'http://deb.debian.org/debian/pool/main/libx/libxau/libxau_1.0.8.orig.tar.gz' libxau_1.0.8.orig.tar.gz 362044 SHA256:c343b4ef66d66a6b3e0e27aa46b37ad5cab0f11a5c565eafb4a1c7590bc71d7b
'http://deb.debian.org/debian/pool/main/libx/libxau/libxau_1.0.8-1.diff.gz' libxau_1.0.8-1.diff.gz 15287 SHA256:b493479d6a52a0e753dd357ad8a4bc5c4296015f3f7b96cf546f7c5c5843cbb0
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxau/1:1.0.8-1/ (for browsing the source)
- https://sources.debian.net/src/libxau/1:1.0.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxau/1:1.0.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxcb=1.12-1`

Binary Packages:

- `libxcb1:amd64=1.12-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.12-1
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.12-1.dsc' libxcb_1.12-1.dsc 6558 SHA256:d6ed3f5ef255a692c9654d954da4421c535e02f21e56a657383ea9d52389080d
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.12.orig.tar.gz' libxcb_1.12.orig.tar.gz 745984 SHA256:092f147149d8a6410647a848378aaae749304d5b73e028ccb8306aa8a9e26f06
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.12-1.diff.gz' libxcb_1.12-1.diff.gz 25044 SHA256:e2af982573638874bca1f4159139e2bffa0ee51148544b4c3b09bad84622648c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcb/1.12-1/ (for browsing the source)
- https://sources.debian.net/src/libxcb/1.12-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcb/1.12-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxdmcp=1:1.1.2-3`

Binary Packages:

- `libxdmcp6:amd64=1:1.1.2-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdmcp=1:1.1.2-3
'http://deb.debian.org/debian/pool/main/libx/libxdmcp/libxdmcp_1.1.2-3.dsc' libxdmcp_1.1.2-3.dsc 2145 SHA256:f9697dca6a275aeee9a3eee9fb2d55e0f77485481e8b84efc6950fc9b1988460
'http://deb.debian.org/debian/pool/main/libx/libxdmcp/libxdmcp_1.1.2.orig.tar.gz' libxdmcp_1.1.2.orig.tar.gz 404115 SHA256:6f7c7e491a23035a26284d247779174dedc67e34e93cc3548b648ffdb6fc57c0
'http://deb.debian.org/debian/pool/main/libx/libxdmcp/libxdmcp_1.1.2-3.diff.gz' libxdmcp_1.1.2-3.diff.gz 18017 SHA256:5844df115c17e5ba40ac116f80373304d821c607e763ef6f40562421f5cc0cf3
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxdmcp/1:1.1.2-3/ (for browsing the source)
- https://sources.debian.net/src/libxdmcp/1:1.1.2-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxdmcp/1:1.1.2-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxext=2:1.3.3-1`

Binary Packages:

- `libxext6:amd64=2:1.3.3-1+b2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxext=2:1.3.3-1
'http://deb.debian.org/debian/pool/main/libx/libxext/libxext_1.3.3-1.dsc' libxext_1.3.3-1.dsc 2221 SHA256:47106df75b8f3db1e43803e8e94a2e966cd23f7daa8cfc393af739a9e33ef955
'http://deb.debian.org/debian/pool/main/libx/libxext/libxext_1.3.3.orig.tar.gz' libxext_1.3.3.orig.tar.gz 468441 SHA256:eb0b88050491fef4716da4b06a4d92b4fc9e76f880d6310b2157df604342cfe5
'http://deb.debian.org/debian/pool/main/libx/libxext/libxext_1.3.3-1.diff.gz' libxext_1.3.3-1.diff.gz 20763 SHA256:e294a4884eb68acbd151312cb0c973aad63268b637b15ccf1911864b7197557e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxext/2:1.3.3-1/ (for browsing the source)
- https://sources.debian.net/src/libxext/2:1.3.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxext/2:1.3.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxi=2:1.7.9-1`

Binary Packages:

- `libxi6:amd64=2:1.7.9-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxi=2:1.7.9-1
'http://deb.debian.org/debian/pool/main/libx/libxi/libxi_1.7.9-1.dsc' libxi_1.7.9-1.dsc 2202 SHA256:fb19b7e8b9ad6306c3e8a6728f29576f956f07a7980e7b4d727259714d6ca686
'http://deb.debian.org/debian/pool/main/libx/libxi/libxi_1.7.9.orig.tar.gz' libxi_1.7.9.orig.tar.gz 604214 SHA256:463cc5370191404bc0f8a450fdbf6d9159efbbf274e5e0f427a60191fed9cf4b
'http://deb.debian.org/debian/pool/main/libx/libxi/libxi_1.7.9-1.diff.gz' libxi_1.7.9-1.diff.gz 15892 SHA256:8c9c221faecc97a7ba7ff1a1a14fad580c49b72e270dc3aae40b72b2d7f4dc5e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxi/2:1.7.9-1/ (for browsing the source)
- https://sources.debian.net/src/libxi/2:1.7.9-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxi/2:1.7.9-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxrender=1:0.9.10-1`

Binary Packages:

- `libxrender1:amd64=1:0.9.10-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxrender=1:0.9.10-1
'http://deb.debian.org/debian/pool/main/libx/libxrender/libxrender_0.9.10-1.dsc' libxrender_0.9.10-1.dsc 2064 SHA256:95d6471218b44f4e60c48cea60cfb4865bbe861530add23f6c859515bee92dbd
'http://deb.debian.org/debian/pool/main/libx/libxrender/libxrender_0.9.10.orig.tar.gz' libxrender_0.9.10.orig.tar.gz 373717 SHA256:770527cce42500790433df84ec3521e8bf095dfe5079454a92236494ab296adf
'http://deb.debian.org/debian/pool/main/libx/libxrender/libxrender_0.9.10-1.diff.gz' libxrender_0.9.10-1.diff.gz 15399 SHA256:ff56a0a00119383adc5f1731e86155ae5c2de069e1d059a9da1d777917430588
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxrender/1:0.9.10-1/ (for browsing the source)
- https://sources.debian.net/src/libxrender/1:0.9.10-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxrender/1:0.9.10-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxtst=2:1.2.3-1`

Binary Packages:

- `libxtst6:amd64=2:1.2.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxtst=2:1.2.3-1
'http://deb.debian.org/debian/pool/main/libx/libxtst/libxtst_1.2.3-1.dsc' libxtst_1.2.3-1.dsc 2243 SHA256:979f05e505ea319c3f75955e10345338f77a512f5a6a0a887d6f4633d6bd4633
'http://deb.debian.org/debian/pool/main/libx/libxtst/libxtst_1.2.3.orig.tar.gz' libxtst_1.2.3.orig.tar.gz 400197 SHA256:a0c83acce02d4923018c744662cb28eb0dbbc33b4adc027726879ccf68fbc2c2
'http://deb.debian.org/debian/pool/main/libx/libxtst/libxtst_1.2.3-1.diff.gz' libxtst_1.2.3-1.diff.gz 10177 SHA256:c4739fc7ccda7caaffcf36f934b7c33463390e71d567c7d62f635db1946b74ed
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxtst/2:1.2.3-1/ (for browsing the source)
- https://sources.debian.net/src/libxtst/2:1.2.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxtst/2:1.2.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lsb=9.20170808`

Binary Packages:

- `lsb-base=9.20170808`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=9.20170808
'http://deb.debian.org/debian/pool/main/l/lsb/lsb_9.20170808.dsc' lsb_9.20170808.dsc 1597 SHA256:d767e622530f73df4f041f7bace54412a6da3d66ddcc73df7913cdebdbf258a9
'http://deb.debian.org/debian/pool/main/l/lsb/lsb_9.20170808.tar.xz' lsb_9.20170808.tar.xz 42120 SHA256:ec9cb022cedcdf34c5b8dc2dca530777ce3f491ad364222557691e87807729b1
```

Other potentially useful URLs:

- https://sources.debian.net/src/lsb/9.20170808/ (for browsing the source)
- https://sources.debian.net/src/lsb/9.20170808/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lsb/9.20170808/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lz4=0.0~r131-2`

Binary Packages:

- `liblz4-1:amd64=0.0~r131-2+b1`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=0.0~r131-2
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_0.0~r131-2.dsc' lz4_0.0~r131-2.dsc 1973 SHA256:304cf9dddee387377929adf3f2cef0ae19fb2e56b6cc9eab05798845b58bd9b6
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_0.0~r131.orig.tar.gz' lz4_0.0~r131.orig.tar.gz 133784 SHA256:9d4d00614d6b9dec3114b33d1224b6262b99ace24434c53487a0c8fd0b18cfed
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_0.0~r131-2.debian.tar.xz' lz4_0.0~r131-2.debian.tar.xz 4936 SHA256:966df055dd8fa7f292c283452b43a5d2d2047d542fe49e97025006e69525e224
```

Other potentially useful URLs:

- https://sources.debian.net/src/lz4/0.0~r131-2/ (for browsing the source)
- https://sources.debian.net/src/lz4/0.0~r131-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lz4/0.0~r131-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mawk=1.3.3-17`

Binary Packages:

- `mawk=1.3.3-17+b3`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.3-17
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.3-17.dsc' mawk_1.3.3-17.dsc 1801 SHA256:f98ce6e153e8ac1faf8165bbf77447a4279313f1c18f6bfeec0c5ce35e4b9c03
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.3.orig.tar.gz' mawk_1.3.3.orig.tar.gz 209942 SHA256:32649c46063d4ef0777a12ae6e9a26bcc920833d54e1abca7edb8d37481e7485
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.3-17.diff.gz' mawk_1.3.3-17.diff.gz 63506 SHA256:13cb66b6eb5ee654d5626621d5ef476ede6b0bebac18ce765516de810e58490c
```

Other potentially useful URLs:

- https://sources.debian.net/src/mawk/1.3.3-17/ (for browsing the source)
- https://sources.debian.net/src/mawk/1.3.3-17/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mawk/1.3.3-17/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ncurses=6.0+20170902-1`

Binary Packages:

- `libncursesw5:amd64=6.0+20170902-1`
- `libtinfo5:amd64=6.0+20170902-1`
- `ncurses-base=6.0+20170902-1`
- `ncurses-bin=6.0+20170902-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris ncurses=6.0+20170902-1
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.0+20170902-1.dsc' ncurses_6.0+20170902-1.dsc 4021 SHA256:6d57899b77e12869ef69d953c7b0af978a46091899401196cd2437c5825d27f4
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.0+20170902.orig.tar.gz' ncurses_6.0+20170902.orig.tar.gz 3322744 SHA256:2437043fe3bb6a0deebe758a9744ee8e9d2e0b272ae2cb0d978804f2f5237ab2
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.0+20170902.orig.tar.gz.asc' ncurses_6.0+20170902.orig.tar.gz.asc 267 SHA256:10a8ea1bca1f94f7c0a95b2789352a4d279802065400d7a680591100ab75469c
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.0+20170902-1.debian.tar.xz' ncurses_6.0+20170902-1.debian.tar.xz 53496 SHA256:b8bd83ec458ab21bb038addc846297206ad9f636e3a8eb7cbab5c5879071dcb2
```

Other potentially useful URLs:

- https://sources.debian.net/src/ncurses/6.0+20170902-1/ (for browsing the source)
- https://sources.debian.net/src/ncurses/6.0+20170902-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ncurses/6.0+20170902-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nettle=3.3-2`

Binary Packages:

- `libhogweed4:amd64=3.3-2`
- `libnettle6:amd64=3.3-2`

Licenses: (parsed from: `/usr/share/doc/libhogweed4/copyright`, `/usr/share/doc/libnettle6/copyright`)

- `GAP`
- `GPL`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `LGPL`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1+`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris nettle=3.3-2
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.3-2.dsc' nettle_3.3-2.dsc 2022 SHA256:502530701faa5bcebc73c55aafd53096d650f55c77dec996fab96796a60ac78d
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.3.orig.tar.gz' nettle_3.3.orig.tar.gz 1887927 SHA256:46942627d5d0ca11720fec18d81fc38f7ef837ea4197c1f630e71ce0d470b11e
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.3-2.debian.tar.xz' nettle_3.3-2.debian.tar.xz 19812 SHA256:91b1e04d3d0cc188f3490fe8bc7f2ad9ec60b1c6f6b29f53b6a72dbedb40dc0e
```

Other potentially useful URLs:

- https://sources.debian.net/src/nettle/3.3-2/ (for browsing the source)
- https://sources.debian.net/src/nettle/3.3-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nettle/3.3-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nspr=2:4.16-1`

Binary Packages:

- `libnspr4:amd64=2:4.16-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris nspr=2:4.16-1
'http://deb.debian.org/debian/pool/main/n/nspr/nspr_4.16-1.dsc' nspr_4.16-1.dsc 2061 SHA256:77eeb81db61d32b89762e566a36249d251fcc9ac475bf4445cd99bf558f9f1f9
'http://deb.debian.org/debian/pool/main/n/nspr/nspr_4.16.orig.tar.gz' nspr_4.16.orig.tar.gz 1140681 SHA256:9b3102d97665504aeee73363c11a21c062ad67a2522242368b7f019f96a53cd1
'http://deb.debian.org/debian/pool/main/n/nspr/nspr_4.16-1.debian.tar.xz' nspr_4.16-1.debian.tar.xz 15244 SHA256:776198b99b6ae188a3c3b09f12373be97fb3d381eabb3e6c42b591ca37dadd3c
```

Other potentially useful URLs:

- https://sources.debian.net/src/nspr/2:4.16-1/ (for browsing the source)
- https://sources.debian.net/src/nspr/2:4.16-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nspr/2:4.16-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nss=2:3.33-1`

Binary Packages:

- `libnss3:amd64=2:3.33-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris nss=2:3.33-1
'http://deb.debian.org/debian/pool/main/n/nss/nss_3.33-1.dsc' nss_3.33-1.dsc 2223 SHA256:cb0e58eb938451b838bca24b3a53d1cd29e69fd807a704d7c1f01502eb354939
'http://deb.debian.org/debian/pool/main/n/nss/nss_3.33.orig.tar.gz' nss_3.33.orig.tar.gz 9578033 SHA256:98f0dabd36408e83dd3a11727336cc3cdfee4cbdd9aede2b2831eb2389c284e4
'http://deb.debian.org/debian/pool/main/n/nss/nss_3.33-1.debian.tar.xz' nss_3.33-1.debian.tar.xz 24964 SHA256:bd6b970cf0e46a986cf87daa81974ae4cd09492ec89bac0d392f38abdae5bf3c
```

Other potentially useful URLs:

- https://sources.debian.net/src/nss/2:3.33-1/ (for browsing the source)
- https://sources.debian.net/src/nss/2:3.33-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nss/2:3.33-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openjdk-9=9~b181-4`

Binary Packages:

- `openjdk-9-jre-headless:amd64=9~b181-4`

Licenses: (parsed from: `/usr/share/doc/openjdk-9-jre-headless/copyright`)

- `Apache-2.0`
- `GPL-2`
- `LGPL-2`
- `LGPL-2-1`

Source:

```console
$ apt-get source -qq --print-uris openjdk-9=9~b181-4
'http://deb.debian.org/debian/pool/main/o/openjdk-9/openjdk-9_9~b181-4.dsc' openjdk-9_9~b181-4.dsc 4500 SHA256:37dc3e62c9aeecb896e91f281f3a5b64c33b93b9a5a6a3b7cbb31ae86ed29bdb
'http://deb.debian.org/debian/pool/main/o/openjdk-9/openjdk-9_9~b181.orig.tar.gz' openjdk-9_9~b181.orig.tar.gz 74709643 SHA256:fae669a3a6ef266bb8bda75bed0d26b861051181ced63609cdef5e30bde93df1
'http://deb.debian.org/debian/pool/main/o/openjdk-9/openjdk-9_9~b181-4.debian.tar.xz' openjdk-9_9~b181-4.debian.tar.xz 175152 SHA256:220f579685c4491f1d1be53ec7135eba7f9f646fd19a000c9108379b49b9f160
```

Other potentially useful URLs:

- https://sources.debian.net/src/openjdk-9/9~b181-4/ (for browsing the source)
- https://sources.debian.net/src/openjdk-9/9~b181-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openjdk-9/9~b181-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssl=1.1.0f-5`

Binary Packages:

- `libssl1.1:amd64=1.1.0f-5`
- `openssl=1.1.0f-5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.0f-5
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.0f-5.dsc' openssl_1.1.0f-5.dsc 2583 SHA256:44c38165dc9c99d069bb19c510d58778bb79e0530d5967cb74c556999f0b4b7e
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.0f.orig.tar.gz' openssl_1.1.0f.orig.tar.gz 5278176 SHA256:12f746f3f2493b2f39da7ecf63d7ee19c6ac9ec6a4fcd8c229da8a522cb12765
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.0f.orig.tar.gz.asc' openssl_1.1.0f.orig.tar.gz.asc 455 SHA256:9f2feb0494ebcc1cf152d95a11bc966cb94bc1957d88650285db3966866801b0
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.0f-5.debian.tar.xz' openssl_1.1.0f-5.debian.tar.xz 59536 SHA256:7ae7fc632d259f1e4ed5e2475847d31db18d9bc6b96a6a3405a77cff7020b97e
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssl/1.1.0f-5/ (for browsing the source)
- https://sources.debian.net/src/openssl/1.1.0f-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssl/1.1.0f-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `p11-kit=0.23.7-3`

Binary Packages:

- `libp11-kit0:amd64=0.23.7-3`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/p11-kit/0.23.7-3/


### `dpkg` source package: `pam=1.1.8-3.6`

Binary Packages:

- `libpam-modules:amd64=1.1.8-3.6`
- `libpam-modules-bin=1.1.8-3.6`
- `libpam-runtime=1.1.8-3.6`
- `libpam0g:amd64=1.1.8-3.6`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.1.8-3.6
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.1.8-3.6.dsc' pam_1.1.8-3.6.dsc 2572 SHA256:7bd7a3059c6ea5b97f5ce0460cbe20788f21bc59bd31ef5a28d7968f53373f5f
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.1.8.orig.tar.gz' pam_1.1.8.orig.tar.gz 1892765 SHA256:4183409a450708a976eca5af561dbf4f0490141a08e86e4a1e649c7c1b094876
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.1.8-3.6.diff.gz' pam_1.1.8-3.6.diff.gz 139492 SHA256:beba99299941c5648ff412d75ebd3407e4d769f5e5ab1fce6a5f2e58c40341ae
```

Other potentially useful URLs:

- https://sources.debian.net/src/pam/1.1.8-3.6/ (for browsing the source)
- https://sources.debian.net/src/pam/1.1.8-3.6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pam/1.1.8-3.6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pcre3=2:8.39-5`

Binary Packages:

- `libpcre3:amd64=2:8.39-5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.39-5
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.39-5.dsc' pcre3_8.39-5.dsc 2224 SHA256:228e6495d610bb001c66509786f65023bb672db31575157b92c741158019d039
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.39.orig.tar.bz2' pcre3_8.39.orig.tar.bz2 1560758 SHA256:b858099f82483031ee02092711689e7245586ada49e534a06e678b8ea9549e8b
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.39-5.debian.tar.gz' pcre3_8.39-5.debian.tar.gz 25511 SHA256:33f51d04b363f20a808f6069955a661be28d29a480adce65458add27b8d11314
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcre3/2:8.39-5/ (for browsing the source)
- https://sources.debian.net/src/pcre3/2:8.39-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcre3/2:8.39-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pcsc-lite=1.8.22-1`

Binary Packages:

- `libpcsclite1:amd64=1.8.22-1`

Licenses: (parsed from: `/usr/share/doc/libpcsclite1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-3`
- `GPL-3+`
- `ISC`

Source:

```console
$ apt-get source -qq --print-uris pcsc-lite=1.8.22-1
'http://deb.debian.org/debian/pool/main/p/pcsc-lite/pcsc-lite_1.8.22-1.dsc' pcsc-lite_1.8.22-1.dsc 2225 SHA256:8a4f990542143ae0d951de9d9a4906dd6cdee716fc27d7f82bd90976999efe5f
'http://deb.debian.org/debian/pool/main/p/pcsc-lite/pcsc-lite_1.8.22.orig.tar.bz2' pcsc-lite_1.8.22.orig.tar.bz2 751724 SHA256:6a358f61ed3b66a7f6e1f4e794a94c7be4c81b7a58ec360c33791e8d7d9bd405
'http://deb.debian.org/debian/pool/main/p/pcsc-lite/pcsc-lite_1.8.22-1.debian.tar.xz' pcsc-lite_1.8.22-1.debian.tar.xz 14644 SHA256:07d413dcb710a95581c18c0162983a87084329620da4e6906ee3ba3b4d596d90
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcsc-lite/1.8.22-1/ (for browsing the source)
- https://sources.debian.net/src/pcsc-lite/1.8.22-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcsc-lite/1.8.22-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `perl=5.26.0-8`

Binary Packages:

- `perl-base=5.26.0-8`

Licenses: (parsed from: `/usr/share/doc/perl-base/copyright`)

- `Artistic`
- `Artistic,`
- `Artistic-2`
- `BSD-3-clause`
- `BSD-3-clause-GENERIC`
- `BSD-3-clause-with-weird-numbering`
- `BSD-4-clause-POWERDOG`
- `BZIP`
- `CC0-1.0`
- `DONT-CHANGE-THE-GPL`
- `Expat`
- `GPL-1`
- `GPL-1+`
- `GPL-2`
- `GPL-2+`
- `GPL-3+-WITH-BISON-EXCEPTION`
- `HSIEH-BSD`
- `HSIEH-DERIVATIVE`
- `LGPL-2.1`
- `REGCOMP`
- `REGCOMP,`
- `RRA-KEEP-THIS-NOTICE`
- `S2P`
- `SDBM-PUBLIC-DOMAIN`
- `TEXT-TABS`
- `Unicode`
- `ZLIB`

Source:

```console
$ apt-get source -qq --print-uris perl=5.26.0-8
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.26.0-8.dsc' perl_5.26.0-8.dsc 2369 SHA256:14287efb9981734a2e15c3508b91e1fd3ca1342e9fc6f49c37ed00acd757aece
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.26.0.orig.tar.xz' perl_5.26.0.orig.tar.xz 11961692 SHA256:9bf2e3d0d72aad77865c3bdbc20d3b576d769c5c255c4ceb30fdb9335266bf55
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.26.0-8.debian.tar.xz' perl_5.26.0-8.debian.tar.xz 159896 SHA256:e6c7f4b6a5790f5909c007d3efe4dcb1f6c6b41da95e4f7ea74748bfb7e198d1
```

Other potentially useful URLs:

- https://sources.debian.net/src/perl/5.26.0-8/ (for browsing the source)
- https://sources.debian.net/src/perl/5.26.0-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/perl/5.26.0-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sed=4.4-1`

Binary Packages:

- `sed=4.4-1`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris sed=4.4-1
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.4-1.dsc' sed_4.4-1.dsc 2048 SHA256:bb2a11d04f3aeba73cc994e097219fde8c5e0fd1bcf42e0ecc8a4f2282c00fc9
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.4.orig.tar.xz' sed_4.4.orig.tar.xz 1181664 SHA256:cbd6ebc5aaf080ed60d0162d7f6aeae58211a1ee9ba9bb25623daa6cd942683b
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.4-1.debian.tar.xz' sed_4.4-1.debian.tar.xz 59552 SHA256:56dd1f91c5e33b419f38cde93afc90d6fad9064ef4594a877424a0ab2ac9a4bf
```

Other potentially useful URLs:

- https://sources.debian.net/src/sed/4.4-1/ (for browsing the source)
- https://sources.debian.net/src/sed/4.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sed/4.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sensible-utils=0.0.10`

Binary Packages:

- `sensible-utils=0.0.10`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `All-permissive`
- `GPL-2`
- `GPL-2+`
- `configure`
- `installsh`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.10
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.10.dsc' sensible-utils_0.0.10.dsc 1671 SHA256:9f19f464d6edc9c086a92c7ac03cc72b285dccd56f9d640b9979a3e5aac3457e
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.10.tar.xz' sensible-utils_0.0.10.tar.xz 57140 SHA256:137f67f34cbe2066407889d6ee15f4e51440e0f1378e9763da5922388a6510f3
```

Other potentially useful URLs:

- https://sources.debian.net/src/sensible-utils/0.0.10/ (for browsing the source)
- https://sources.debian.net/src/sensible-utils/0.0.10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sensible-utils/0.0.10/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `shadow=1:4.5-1`

Binary Packages:

- `login=1:4.5-1`
- `passwd=1:4.5-1`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.5-1
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.5-1.dsc' shadow_4.5-1.dsc 2282 SHA256:1e93b2e4cb3f0f14a52dd9603bf8153f31a3117c580c0b46fd94822437516ff6
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.5.orig.tar.xz' shadow_4.5.orig.tar.xz 1344524 SHA256:22b0952dc944b163e2370bb911b11ca275fc80ad024267cf21e496b28c23d500
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.5-1.debian.tar.xz' shadow_4.5-1.debian.tar.xz 462752 SHA256:0aa8980eddef9159ee6532d40bda92237ad2163dcc2bb6601aecc415ab9662ee
```

Other potentially useful URLs:

- https://sources.debian.net/src/shadow/1:4.5-1/ (for browsing the source)
- https://sources.debian.net/src/shadow/1:4.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/shadow/1:4.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sqlite3=3.20.1-1`

Binary Packages:

- `libsqlite3-0:amd64=3.20.1-1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/sqlite3/3.20.1-1/


### `dpkg` source package: `systemd=234-3`

Binary Packages:

- `libsystemd0:amd64=234-3`
- `libudev1:amd64=234-3`

Licenses: (parsed from: `/usr/share/doc/libsystemd0/copyright`, `/usr/share/doc/libudev1/copyright`)

- `CC0`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/systemd/234-3/


### `dpkg` source package: `sysvinit=2.88dsf-59.10`

Binary Packages:

- `sysvinit-utils=2.88dsf-59.10`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.88dsf-59.10
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.88dsf-59.10.dsc' sysvinit_2.88dsf-59.10.dsc 2353 SHA256:b25f6800b2c0f1cfd978979f25371a79493c81c6ad0815b541d12deaae75e319
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.88dsf.orig.tar.gz' sysvinit_2.88dsf.orig.tar.gz 125330 SHA256:b016f937958d2809a020d407e1287bdc09abf1d44efaa96530e2ea57f544f4e8
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.88dsf-59.10.debian.tar.xz' sysvinit_2.88dsf-59.10.debian.tar.xz 132504 SHA256:3dd24f403de4565abe55181fbde15ac013e520bf65f159b875637f6c41972519
```

Other potentially useful URLs:

- https://sources.debian.net/src/sysvinit/2.88dsf-59.10/ (for browsing the source)
- https://sources.debian.net/src/sysvinit/2.88dsf-59.10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sysvinit/2.88dsf-59.10/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tar=1.29b-2`

Binary Packages:

- `tar=1.29b-2`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.29b-2
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.29b-2.dsc' tar_1.29b-2.dsc 1965 SHA256:cae92504d2622b0a3d353df387c44beb1e9040ed2d527272a226f0ba247a17f1
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.29b.orig.tar.xz' tar_1.29b.orig.tar.xz 1822008 SHA256:6a59706ebee384a6cd2fb3ee1dbfbfc20c5c66c7efd7cedb28edc054fca8ba00
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.29b-2.debian.tar.xz' tar_1.29b-2.debian.tar.xz 28552 SHA256:caa4e76e821b87e842d0bfc8285abd47103d47d56e93dae0a8df4b787f7c8d72
```

Other potentially useful URLs:

- https://sources.debian.net/src/tar/1.29b-2/ (for browsing the source)
- https://sources.debian.net/src/tar/1.29b-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tar/1.29b-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tzdata=2017b-2`

Binary Packages:

- `tzdata=2017b-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tzdata=2017b-2
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2017b-2.dsc' tzdata_2017b-2.dsc 2005 SHA256:479f7a077690c3d84f15dc8be1da0a732a54cc07f7b30ca7fad6a5bd00921748
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2017b.orig.tar.gz' tzdata_2017b.orig.tar.gz 324317 SHA256:f8242a522ea3496b0ce4ff4f2e75a049178da21001a08b8e666d8cbe07d18086
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2017b-2.debian.tar.xz' tzdata_2017b-2.debian.tar.xz 101096 SHA256:2607bdfaa4535e59223d194c1cc1891a3c26a731d20a4a1d9311d22d1a9175d8
```

Other potentially useful URLs:

- https://sources.debian.net/src/tzdata/2017b-2/ (for browsing the source)
- https://sources.debian.net/src/tzdata/2017b-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tzdata/2017b-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `unzip=6.0-21`

Binary Packages:

- `unzip=6.0-21`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-21
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0-21.dsc' unzip_6.0-21.dsc 1344 SHA256:c51fca0f9d8af19ead119addf4b56ea25443b64951b85eceb873f0ca76b378d4
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA256:036d96991646d0449ed0aa952e4fbe21b476ce994abc276e49d30e686708bd37
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0-21.debian.tar.xz' unzip_6.0-21.debian.tar.xz 17740 SHA256:8accd9d214630a366476437a3ec1842f2e057fdce16042a7b19ee569c33490a3
```

Other potentially useful URLs:

- https://sources.debian.net/src/unzip/6.0-21/ (for browsing the source)
- https://sources.debian.net/src/unzip/6.0-21/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/unzip/6.0-21/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `util-linux=2.29.2-5`

Binary Packages:

- `bsdutils=1:2.29.2-5+b1`
- `fdisk=2.29.2-5+b1`
- `libblkid1:amd64=2.29.2-5+b1`
- `libfdisk1:amd64=2.29.2-5+b1`
- `libmount1:amd64=2.29.2-5+b1`
- `libsmartcols1:amd64=2.29.2-5+b1`
- `libuuid1:amd64=2.29.2-5+b1`
- `mount=2.29.2-5+b1`
- `util-linux=2.29.2-5+b1`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/fdisk/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libfdisk1/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-4-clause`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`
- `MIT`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/util-linux/2.29.2-5/


### `dpkg` source package: `xorg=1:7.7+19`

Binary Packages:

- `x11-common=1:7.7+19`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+19
'http://deb.debian.org/debian/pool/main/x/xorg/xorg_7.7+19.dsc' xorg_7.7+19.dsc 2016 SHA256:fc4a577eee67f3604c56701e21b28dccd3858da0f110b708ca3359e2718e3d46
'http://deb.debian.org/debian/pool/main/x/xorg/xorg_7.7+19.tar.gz' xorg_7.7+19.tar.gz 288723 SHA256:5de6df9e19009450b94f4f5307049bc2c7dc1114222f6f2f6fc60d737a33a537
```

Other potentially useful URLs:

- https://sources.debian.net/src/xorg/1:7.7+19/ (for browsing the source)
- https://sources.debian.net/src/xorg/1:7.7+19/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xorg/1:7.7+19/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xz-utils=5.2.2-1.3`

Binary Packages:

- `liblzma5:amd64=5.2.2-1.3`
- `xz-utils=5.2.2-1.3`

Licenses: (parsed from: `/usr/share/doc/liblzma5/copyright`, `/usr/share/doc/xz-utils/copyright`)

- `Autoconf`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `LGPL-2`
- `LGPL-2.1`
- `LGPL-2.1+`
- `PD`
- `PD-debian`
- `config-h`
- `noderivs`
- `none`
- `permissive-fsf`
- `permissive-nowarranty`
- `probably-PD`

Source:

```console
$ apt-get source -qq --print-uris xz-utils=5.2.2-1.3
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.2-1.3.dsc' xz-utils_5.2.2-1.3.dsc 2575 SHA256:3ea4e6a32f6265b152f89ceafe78c8839e5f4bb1cad137b159fe2013817f9342
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.2.orig.tar.xz' xz-utils_5.2.2.orig.tar.xz 1016404 SHA256:f341b1906ebcdde291dd619399ae944600edc9193619dd0c0110a5f05bfcc89e
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.2.orig.tar.xz.asc' xz-utils_5.2.2.orig.tar.xz.asc 543 SHA256:2cc0575556e1331b3f468e6e7dca5969ce86efcc315d62672279b4e68b2e449f
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.2-1.3.debian.tar.xz' xz-utils_5.2.2-1.3.debian.tar.xz 108680 SHA256:d76c3acf39d0999c14384695394970e8f98853fd6736ba91972d3e67106bc6f6
```

Other potentially useful URLs:

- https://sources.debian.net/src/xz-utils/5.2.2-1.3/ (for browsing the source)
- https://sources.debian.net/src/xz-utils/5.2.2-1.3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xz-utils/5.2.2-1.3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `zlib=1:1.2.8.dfsg-5`

Binary Packages:

- `zlib1g:amd64=1:1.2.8.dfsg-5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.8.dfsg-5
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.8.dfsg-5.dsc' zlib_1.2.8.dfsg-5.dsc 2259 SHA256:35ebfdbb74b3563d344b2bb946909f5d3221cdf971876549ea7ccec01fabcbec
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.8.dfsg.orig.tar.gz' zlib_1.2.8.dfsg.orig.tar.gz 361943 SHA256:2caecc2c3f1ef8b87b8f72b128a03e61c307e8c14f5ec9b422ef7914ba75cf9f
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.8.dfsg-5.debian.tar.xz' zlib_1.2.8.dfsg-5.debian.tar.xz 18500 SHA256:7b88f58d1bfe8e873b8362ede3d0bc569793decc60094189fad1a110599cdd95
```

Other potentially useful URLs:

- https://sources.debian.net/src/zlib/1:1.2.8.dfsg-5/ (for browsing the source)
- https://sources.debian.net/src/zlib/1:1.2.8.dfsg-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/zlib/1:1.2.8.dfsg-5/ (for access to the source package after it no longer exists in the archive)
