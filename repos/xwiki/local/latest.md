# `xwiki:8`

## Docker Metadata

- Image ID: `sha256:385ce5a59052f8271db7ae4aca2f53c4d97a6e21c3271973874482bee56ac290`
- Created: `2017-04-11T23:35:54.659736024Z`
- Virtual Size: ~ 1.16 Gb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["docker-entrypoint.sh"]`
- Command: `["xwiki"]`
- Environment:
  - `PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `LANG=C.UTF-8`
  - `JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64/jre`
  - `JAVA_VERSION=8u121`
  - `JAVA_DEBIAN_VERSION=8u121-b13-1~bpo8+1`
  - `CA_CERTIFICATES_JAVA_VERSION=20161107~bpo8+1`
  - `CATALINA_HOME=/usr/local/tomcat`
  - `TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib`
  - `LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib`
  - `OPENSSL_VERSION=1.1.0e-1`
  - `GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23`
  - `TOMCAT_MAJOR=8`
  - `TOMCAT_VERSION=8.5.13`
  - `TOMCAT_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=tomcat/tomcat-8/v8.5.13/bin/apache-tomcat-8.5.13.tar.gz`
  - `TOMCAT_ASC_URL=https://www.apache.org/dist/tomcat/tomcat-8/v8.5.13/bin/apache-tomcat-8.5.13.tar.gz.asc`
  - `XWIKI_VERSION=8.4.4`
  - `XWIKI_URL_PREFIX=http://maven.xwiki.org/releases/org/xwiki/enterprise/xwiki-enterprise-web/8.4.4`
  - `XWIKI_DOWNLOAD_SHA256=b414edb4527e3d8b27c40a8c3f2f09423980de7963207b7dc89da71d14e7fb23`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.2.52-2`

Binary Packages:

- `acl=2.2.52-2`
- `libacl1:amd64=2.2.52-2`

Licenses: (parsed from: `/usr/share/doc/acl/copyright`, `/usr/share/doc/libacl1/copyright`)

- `GPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.2.52-2
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.52-2.dsc' acl_2.2.52-2.dsc 2025 SHA256:015097e04740e84fefbe6c890d02c603f79edece45c51cbb5c18431647cd7aad
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.52.orig.tar.bz2' acl_2.2.52.orig.tar.bz2 312128 SHA256:59d05b38af76baf2eddccbf08c7968a17451cc785ffecc657fcb46ce32b2631d
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.52-2.debian.tar.xz' acl_2.2.52-2.debian.tar.xz 8524 SHA256:de81ec13cab6d33538db24a53c17838c5bdb32dd0e00e0b0b5d3325114e64e10
```

Likely also available for browsing at:

- https://sources.debian.net/src/acl/2.2.52-2/
- https://sources.debian.net/src/acl/2.2.52-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `adduser=3.113+nmu3`

Binary Packages:

- `adduser=3.113+nmu3`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.113+nmu3
'http://deb.debian.org/debian/pool/main/a/adduser/adduser_3.113+nmu3.dsc' adduser_3.113+nmu3.dsc 1733 SHA256:7f9fa8841080591834389fd56352e2d05ca3d86eb4df15d2f13bea9faf4a6f2d
'http://deb.debian.org/debian/pool/main/a/adduser/adduser_3.113+nmu3.tar.gz' adduser_3.113+nmu3.tar.gz 342554 SHA256:02682be3f51f3e732121f20a3e4922bb8bef15cfacb8767fc250a01d09502122
```

Likely also available for browsing at:

- https://sources.debian.net/src/adduser/3.113+nmu3/
- https://sources.debian.net/src/adduser/3.113+nmu3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `apr=1.5.1-3`

Binary Packages:

- `libapr1:amd64=1.5.1-3`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.5.1-3
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.5.1-3.dsc' apr_1.5.1-3.dsc 2090 SHA256:f3f78ab76365a17a233220357eb2b7f3102d7e9d21c59b3f82d9f0300c554433
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.5.1.orig.tar.bz2' apr_1.5.1.orig.tar.bz2 817569 SHA256:e94abe431d4da48425fcccdb27b469bd0f8151488f82e5630a56f26590e198ac
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.5.1-3.debian.tar.xz' apr_1.5.1-3.debian.tar.xz 17844 SHA256:c7f270ab445e2646bd7dfdfaf9ea44b2642a43c48012689c6f3bf52fe8c9e9c5
```

Likely also available for browsing at:

- https://sources.debian.net/src/apr/1.5.1-3/
- https://sources.debian.net/src/apr/1.5.1-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `apt=1.0.9.8.4`

Binary Packages:

- `apt=1.0.9.8.4`
- `libapt-pkg4.12:amd64=1.0.9.8.4`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg4.12/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=1.0.9.8.4
'http://deb.debian.org/debian/pool/main/a/apt/apt_1.0.9.8.4.dsc' apt_1.0.9.8.4.dsc 2530 SHA256:51fe8ce9490de264e55220e4c5f61a8bbb6d2f824c49c90914b2248db3e28bd3
'http://deb.debian.org/debian/pool/main/a/apt/apt_1.0.9.8.4.tar.xz' apt_1.0.9.8.4.tar.xz 1793116 SHA256:ac2a267b9f98685977d421e41b4518eceb66e9b85cd0d4a9f9a03db729190f7a
```

Likely also available for browsing at:

- https://sources.debian.net/src/apt/1.0.9.8.4/
- https://sources.debian.net/src/apt/1.0.9.8.4/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `atk1.0=2.14.0-1`

Binary Packages:

- `libatk1.0-0:amd64=2.14.0-1`
- `libatk1.0-data=2.14.0-1`

Licenses: (parsed from: `/usr/share/doc/libatk1.0-0/copyright`, `/usr/share/doc/libatk1.0-data/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris atk1.0=2.14.0-1
'http://deb.debian.org/debian/pool/main/a/atk1.0/atk1.0_2.14.0-1.dsc' atk1.0_2.14.0-1.dsc 2037 SHA256:4535882fa01ef66455fca326aa7576c34181045a0814ecf16bdf99f5fbdc9ba5
'http://deb.debian.org/debian/pool/main/a/atk1.0/atk1.0_2.14.0.orig.tar.xz' atk1.0_2.14.0.orig.tar.xz 696064 SHA256:2875cc0b32bfb173c066c22a337f79793e0c99d2cc5e81c4dac0d5a523b8fbad
'http://deb.debian.org/debian/pool/main/a/atk1.0/atk1.0_2.14.0-1.debian.tar.xz' atk1.0_2.14.0-1.debian.tar.xz 10372 SHA256:d17bd76ea933603f5426497039219bd9aa9693d91a4ae585c490b5500dc9aa92
```

Likely also available for browsing at:

- https://sources.debian.net/src/atk1.0/2.14.0-1/
- https://sources.debian.net/src/atk1.0/2.14.0-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `attr=1:2.4.47-2`

Binary Packages:

- `libattr1:amd64=1:2.4.47-2`

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

Likely also available for browsing at:

- https://sources.debian.net/src/attr/1:2.4.47-2/
- https://sources.debian.net/src/attr/1:2.4.47-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `audit=1:2.4-1`

Binary Packages:

- `libaudit-common=1:2.4-1`
- `libaudit1:amd64=1:2.4-1+b1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:2.4-1
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.4-1.dsc' audit_2.4-1.dsc 2068 SHA256:01d240bd783697b8ab4cd941f944612eebc81e1f535a8afb36b25ab3021cd15f
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.4.orig.tar.gz' audit_2.4.orig.tar.gz 937809 SHA256:6e5d39e7af9d00477ef60f824be8c93bd23a227869d6993ff36b7e7fa28fe99b
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.4-1.debian.tar.xz' audit_2.4-1.debian.tar.xz 15808 SHA256:c18c1b88c41f3b8be9e59d3041563599f822994cb10574ffc17f00f0a157c12c
```

Likely also available for browsing at:

- https://sources.debian.net/src/audit/1:2.4-1/
- https://sources.debian.net/src/audit/1:2.4-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `avahi=0.6.31-5`

Binary Packages:

- `libavahi-client3:amd64=0.6.31-5`
- `libavahi-common-data:amd64=0.6.31-5`
- `libavahi-common3:amd64=0.6.31-5`

Licenses: (parsed from: `/usr/share/doc/libavahi-client3/copyright`, `/usr/share/doc/libavahi-common-data/copyright`, `/usr/share/doc/libavahi-common3/copyright`)

- `GPL`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris avahi=0.6.31-5
'http://deb.debian.org/debian/pool/main/a/avahi/avahi_0.6.31-5.dsc' avahi_0.6.31-5.dsc 4069 SHA256:0fd83a73ecc0378fa9db09b59c0679ed52230601e23d43dabb62ba7dcf8e9383
'http://deb.debian.org/debian/pool/main/a/avahi/avahi_0.6.31.orig.tar.gz' avahi_0.6.31.orig.tar.gz 1268686 SHA256:8372719b24e2dd75de6f59bb1315e600db4fd092805bd1201ed0cb651a2dab48
'http://deb.debian.org/debian/pool/main/a/avahi/avahi_0.6.31-5.debian.tar.xz' avahi_0.6.31-5.debian.tar.xz 31300 SHA256:3fd413d85ab8650d448adbdf82fddbff688d159d19a3f2c8ba26c1a49ee7605d
```

Likely also available for browsing at:

- https://sources.debian.net/src/avahi/0.6.31-5/
- https://sources.debian.net/src/avahi/0.6.31-5/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `base-files=8+deb8u7`

Binary Packages:

- `base-files=8+deb8u7`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=8+deb8u7
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_8+deb8u7.dsc' base-files_8+deb8u7.dsc 1026 SHA256:c7bf8d93dc4fd63986e3f6b94d04a74e945486007a207b2a92cb4154f1e7fad8
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_8+deb8u7.tar.xz' base-files_8+deb8u7.tar.xz 53192 SHA256:0db2deea05f4a4338a99e159b0dbe4c63d5ac090e9dda72e1381d1bb75f8b5f0
```

Likely also available for browsing at:

- https://sources.debian.net/src/base-files/8+deb8u7/
- https://sources.debian.net/src/base-files/8+deb8u7/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `base-passwd=3.5.37`

Binary Packages:

- `base-passwd=3.5.37`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.37
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.37.dsc' base-passwd_3.5.37.dsc 1733 SHA256:211a49b6a3bbfdb61a91e9b5d9994c59d8a511a047c2cfc489c03c4c379d6cfe
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.37.tar.xz' base-passwd_3.5.37.tar.xz 51392 SHA256:7cb1cdd8e4aee39b5f59a3dc42d63619590fc4a2136db482fdb6be6e74bb3d04
```

Likely also available for browsing at:

- https://sources.debian.net/src/base-passwd/3.5.37/
- https://sources.debian.net/src/base-passwd/3.5.37/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `bash=4.3-11+deb8u1`

Binary Packages:

- `bash=4.3-11+deb8u1`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=4.3-11+deb8u1
'http://deb.debian.org/debian/pool/main/b/bash/bash_4.3-11+deb8u1.dsc' bash_4.3-11+deb8u1.dsc 2348 SHA256:8433fa4a2bc18f2ca9cbcf7f16ae088a5135b37c9928e64ee80fa6804cb5b592
'http://deb.debian.org/debian/pool/main/b/bash/bash_4.3.orig.tar.gz' bash_4.3.orig.tar.gz 7516231 SHA256:b2fe79ddf9e7abdb4695e3070afa866d2a94a58d1cc9d731585330c753815491
'http://deb.debian.org/debian/pool/main/b/bash/bash_4.3-11+deb8u1.debian.tar.xz' bash_4.3-11+deb8u1.debian.tar.xz 80096 SHA256:6d0ae7d128c742d9f7490993fe5708ed90b2ff40ebab2eb45140805cfa98269f
```

Likely also available for browsing at:

- https://sources.debian.net/src/bash/4.3-11+deb8u1/
- https://sources.debian.net/src/bash/4.3-11+deb8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `blas=1.2.20110419-10`

Binary Packages:

- `libblas-common=1.2.20110419-10`
- `libblas3=1.2.20110419-10`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris blas=1.2.20110419-10
'http://deb.debian.org/debian/pool/main/b/blas/blas_1.2.20110419-10.dsc' blas_1.2.20110419-10.dsc 2314 SHA256:a2af619c0c032f186d621a50006f16b6b6d5f4b6d351feea6bacbd645a51ae58
'http://deb.debian.org/debian/pool/main/b/blas/blas_1.2.20110419.orig.tar.gz' blas_1.2.20110419.orig.tar.gz 485409 SHA256:73a52b2034da239909f57c75ba25cab917d587d6b877683773d6646b732bff58
'http://deb.debian.org/debian/pool/main/b/blas/blas_1.2.20110419-10.debian.tar.xz' blas_1.2.20110419-10.debian.tar.xz 46436 SHA256:44b721e4cbf75c812dbb0959a50571894363d0954848747741ff780297e9d95e
```

Likely also available for browsing at:

- https://sources.debian.net/src/blas/1.2.20110419-10/
- https://sources.debian.net/src/blas/1.2.20110419-10/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `boost1.55=1.55.0+dfsg-3`

Binary Packages:

- `libboost-date-time1.55.0:amd64=1.55.0+dfsg-3`
- `libboost-iostreams1.55.0:amd64=1.55.0+dfsg-3`
- `libboost-system1.55.0:amd64=1.55.0+dfsg-3`

Licenses: (parsed from: `/usr/share/doc/libboost-date-time1.55.0/copyright`, `/usr/share/doc/libboost-iostreams1.55.0/copyright`, `/usr/share/doc/libboost-system1.55.0/copyright`)

- `Boost`

Source:

```console
$ apt-get source -qq --print-uris boost1.55=1.55.0+dfsg-3
'http://deb.debian.org/debian/pool/main/b/boost1.55/boost1.55_1.55.0+dfsg-3.dsc' boost1.55_1.55.0+dfsg-3.dsc 5816 SHA256:37beaf286af0e8fb59b8d8927477d2840d408ca3be8c22a685d256432f2a2080
'http://deb.debian.org/debian/pool/main/b/boost1.55/boost1.55_1.55.0+dfsg.orig.tar.gz' boost1.55_1.55.0+dfsg.orig.tar.gz 71173322 SHA256:a9aff4c5d85790401ee48ba7170c0edd5ce17009215e1d36e026052146b55bc6
'http://deb.debian.org/debian/pool/main/b/boost1.55/boost1.55_1.55.0+dfsg-3.debian.tar.xz' boost1.55_1.55.0+dfsg-3.debian.tar.xz 102280 SHA256:04c95a4583214a6ca3d2df9ae7bcc0f705c8cf3992a0da73af395a2db0ae400a
```

Likely also available for browsing at:

- https://sources.debian.net/src/boost1.55/1.55.0+dfsg-3/
- https://sources.debian.net/src/boost1.55/1.55.0+dfsg-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `bzip2=1.0.6-7`

Binary Packages:

- `bzip2=1.0.6-7+b3`
- `libbz2-1.0:amd64=1.0.6-7+b3`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.6-7
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.6-7.dsc' bzip2_1.0.6-7.dsc 2261 SHA256:098b7e38d1d634fc361847602bf85753dadeca121b9531f6dba2614b16e0637c
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.6.orig.tar.bz2' bzip2_1.0.6.orig.tar.bz2 708737 SHA256:d70a9ccd8bdf47e302d96c69fecd54925f45d9c7b966bb4ef5f56b770960afa7
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.6-7.debian.tar.bz2' bzip2_1.0.6-7.debian.tar.bz2 59542 SHA256:17e030ccb2908d15553c1510869e09d8ef41b5f8e72c7c65d1d5503396a5bd3a
```

Likely also available for browsing at:

- https://sources.debian.net/src/bzip2/1.0.6-7/
- https://sources.debian.net/src/bzip2/1.0.6-7/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `ca-certificates-java=20161107~bpo8+1`

Binary Packages:

- `ca-certificates-java=20161107~bpo8+1`

Licenses: (parsed from: `/usr/share/doc/ca-certificates-java/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates-java=20161107~bpo8+1
'http://deb.debian.org/debian/pool/main/c/ca-certificates-java/ca-certificates-java_20161107~bpo8+1.dsc' ca-certificates-java_20161107~bpo8+1.dsc 1887 SHA256:a73671a95ce5480353d9f5082c3cb2a372d316f45f5274d89623d6bf33eb4222
'http://deb.debian.org/debian/pool/main/c/ca-certificates-java/ca-certificates-java_20161107~bpo8+1.tar.xz' ca-certificates-java_20161107~bpo8+1.tar.xz 15972 SHA256:908902ec1623019d7e77c28006acc806d9bb3310909e74ddeae27b5266857895
```

Likely also available for browsing at:

- https://sources.debian.net/src/ca-certificates-java/20161107~bpo8+1/
- https://sources.debian.net/src/ca-certificates-java/20161107~bpo8+1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `ca-certificates=20141019+deb8u2`

Binary Packages:

- `ca-certificates=20141019+deb8u2`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20141019+deb8u2
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20141019+deb8u2.dsc' ca-certificates_20141019+deb8u2.dsc 1433 SHA256:6d3790d1a3a62311c274b19b8de9b4ab197133f83a8716d95148ae39dce47e46
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20141019+deb8u2.tar.xz' ca-certificates_20141019+deb8u2.tar.xz 299020 SHA256:24257d25cedabfa303c02b8aba7b52300b66ff8dcd13424c2fc70489541ae26f
```

Likely also available for browsing at:

- https://sources.debian.net/src/ca-certificates/20141019+deb8u2/
- https://sources.debian.net/src/ca-certificates/20141019+deb8u2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `cairo=1.14.0-2.1+deb8u2`

Binary Packages:

- `libcairo2:amd64=1.14.0-2.1+deb8u2`

Licenses: (parsed from: `/usr/share/doc/libcairo2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.14.0-2.1+deb8u2
'http://deb.debian.org/debian/pool/main/c/cairo/cairo_1.14.0-2.1+deb8u2.dsc' cairo_1.14.0-2.1+deb8u2.dsc 3069 SHA256:c5440748278b608bf060193a7515222cc9e1967f3fec7585219f1b5278a229d5
'http://deb.debian.org/debian/pool/main/c/cairo/cairo_1.14.0.orig.tar.xz' cairo_1.14.0.orig.tar.xz 36584076 SHA256:2cf5f81432e77ea4359af9dcd0f4faf37d015934501391c311bfd2d19a0134b7
'http://deb.debian.org/debian/pool/main/c/cairo/cairo_1.14.0-2.1+deb8u2.debian.tar.xz' cairo_1.14.0-2.1+deb8u2.debian.tar.xz 31872 SHA256:66f6a5f01b351b0ba53fbbb146d6fb5ac46146bf0a974016d0f318a387f17abf
```

Likely also available for browsing at:

- https://sources.debian.net/src/cairo/1.14.0-2.1+deb8u2/
- https://sources.debian.net/src/cairo/1.14.0-2.1+deb8u2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `cdebconf=0.192`

Binary Packages:

- `libdebconfclient0:amd64=0.192`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.192
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.192.dsc' cdebconf_0.192.dsc 2574 SHA256:85d39068de77c67036b6e2ca5ebdf3990e19a6c5b0f01422608ff7656c166dbd
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.192.tar.xz' cdebconf_0.192.tar.xz 266320 SHA256:bb09e6c04b514dd12684dbc6eacde57fb03e282f67f0199e67078c13ffffd667
```

Likely also available for browsing at:

- https://sources.debian.net/src/cdebconf/0.192/
- https://sources.debian.net/src/cdebconf/0.192/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `clp=1.15.10-1`

Binary Packages:

- `coinor-libclp1=1.15.10-1`

Licenses: (parsed from: `/usr/share/doc/coinor-libclp1/copyright`)

- `EPL-1`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris clp=1.15.10-1
'http://deb.debian.org/debian/pool/main/c/clp/clp_1.15.10-1.dsc' clp_1.15.10-1.dsc 2318 SHA256:d3c48e06d150842305882184a7c32a018123ccef1fd38cce61da2eab67ca9ce1
'http://deb.debian.org/debian/pool/main/c/clp/clp_1.15.10.orig.tar.gz' clp_1.15.10.orig.tar.gz 1856909 SHA256:44b6f7e05ac64a9eed63eb67b8175a3a7d054ae1928156a5cc1dce5ee044706c
'http://deb.debian.org/debian/pool/main/c/clp/clp_1.15.10-1.debian.tar.xz' clp_1.15.10-1.debian.tar.xz 9220 SHA256:5bc3a658d7f566e30131761dab44cf4e1acd091148825661b00c9f9d7402db00
```

Likely also available for browsing at:

- https://sources.debian.net/src/clp/1.15.10-1/
- https://sources.debian.net/src/clp/1.15.10-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `clucene-core=2.3.3.4-4`

Binary Packages:

- `libclucene-contribs1:amd64=2.3.3.4-4`
- `libclucene-core1:amd64=2.3.3.4-4`

Licenses: (parsed from: `/usr/share/doc/libclucene-contribs1/copyright`, `/usr/share/doc/libclucene-core1/copyright`)

- `Apache-2.0`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris clucene-core=2.3.3.4-4
'http://deb.debian.org/debian/pool/main/c/clucene-core/clucene-core_2.3.3.4-4.dsc' clucene-core_2.3.3.4-4.dsc 1442 SHA256:7c76cca36898f0e691aac13bfbe50c647712062b12f2e9072b9baef611b8d8a7
'http://deb.debian.org/debian/pool/main/c/clucene-core/clucene-core_2.3.3.4.orig.tar.gz' clucene-core_2.3.3.4.orig.tar.gz 2241498 SHA256:ddfdc433dd8ad31b5c5819cc4404a8d2127472a3b720d3e744e8c51d79732eab
'http://deb.debian.org/debian/pool/main/c/clucene-core/clucene-core_2.3.3.4-4.debian.tar.gz' clucene-core_2.3.3.4-4.debian.tar.gz 8742 SHA256:f24a1a20ac766ec43019beef5aab1e3d9e18d1be5060331f28759eb7f40077c6
```

Likely also available for browsing at:

- https://sources.debian.net/src/clucene-core/2.3.3.4-4/
- https://sources.debian.net/src/clucene-core/2.3.3.4-4/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `coinmp=1.7.6+dfsg1-1`

Binary Packages:

- `coinor-libcoinmp1:amd64=1.7.6+dfsg1-1`

Licenses: (parsed from: `/usr/share/doc/coinor-libcoinmp1/copyright`)

- `CPL-1`
- `EPL-1`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris coinmp=1.7.6+dfsg1-1
'http://deb.debian.org/debian/pool/main/c/coinmp/coinmp_1.7.6+dfsg1-1.dsc' coinmp_1.7.6+dfsg1-1.dsc 2021 SHA256:e1c7633a16654dad6e0b75d92e7e6d18603d7dee4fd6cfbf766ee27d6324083e
'http://deb.debian.org/debian/pool/main/c/coinmp/coinmp_1.7.6+dfsg1.orig.tar.gz' coinmp_1.7.6+dfsg1.orig.tar.gz 659163 SHA256:859ed08310ec47da0b57dceb9ca60e9db8f53ea0e0e76b7cffa41cbaf569caa2
'http://deb.debian.org/debian/pool/main/c/coinmp/coinmp_1.7.6+dfsg1-1.debian.tar.xz' coinmp_1.7.6+dfsg1-1.debian.tar.xz 7652 SHA256:bcc10d7dfc5b560eedbb3a353a6bef171ed3f063856935050bbb227e6934494c
```

Likely also available for browsing at:

- https://sources.debian.net/src/coinmp/1.7.6+dfsg1-1/
- https://sources.debian.net/src/coinmp/1.7.6+dfsg1-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `coinor-cbc=2.8.12-1`

Binary Packages:

- `coinor-libcbc3=2.8.12-1`

Licenses: (parsed from: `/usr/share/doc/coinor-libcbc3/copyright`)

- `EPL-1`
- `GPL-3`
- `LUCENT`

Source:

```console
$ apt-get source -qq --print-uris coinor-cbc=2.8.12-1
'http://deb.debian.org/debian/pool/main/c/coinor-cbc/coinor-cbc_2.8.12-1.dsc' coinor-cbc_2.8.12-1.dsc 2438 SHA256:226034354ccd2faa4d74a8d32bf54fa7ebb806b328e2e04f991ec042f092c4ff
'http://deb.debian.org/debian/pool/main/c/coinor-cbc/coinor-cbc_2.8.12.orig.tar.gz' coinor-cbc_2.8.12.orig.tar.gz 1344877 SHA256:50618a41d23022cdf5be4306b4a3cb75157c33876fdcaca26955ef7349bdbc7f
'http://deb.debian.org/debian/pool/main/c/coinor-cbc/coinor-cbc_2.8.12-1.debian.tar.xz' coinor-cbc_2.8.12-1.debian.tar.xz 10616 SHA256:5c805bf73e9029750b1fa077013a0db5ee646cd2d83d3f364491973c50e98a30
```

Likely also available for browsing at:

- https://sources.debian.net/src/coinor-cbc/2.8.12-1/
- https://sources.debian.net/src/coinor-cbc/2.8.12-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `coinor-cgl=0.58.9-1`

Binary Packages:

- `coinor-libcgl1=0.58.9-1`

Licenses: (parsed from: `/usr/share/doc/coinor-libcgl1/copyright`)

- `EPL-1`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coinor-cgl=0.58.9-1
'http://deb.debian.org/debian/pool/main/c/coinor-cgl/coinor-cgl_0.58.9-1.dsc' coinor-cgl_0.58.9-1.dsc 2289 SHA256:cfb321193be4a6450c811c088f770bb8437d907e470ccc6eaa91777370ee7c38
'http://deb.debian.org/debian/pool/main/c/coinor-cgl/coinor-cgl_0.58.9.orig.tar.gz' coinor-cgl_0.58.9.orig.tar.gz 982607 SHA256:d23d621f9f80bb3753536f1fa34008ed56202bc01ef99e72e4c4241b18c269fc
'http://deb.debian.org/debian/pool/main/c/coinor-cgl/coinor-cgl_0.58.9-1.debian.tar.xz' coinor-cgl_0.58.9-1.debian.tar.xz 7504 SHA256:b24e2d67aec8a23e23dc3c0648a8cdd06625a3f8f1d9bb330b39651036f20dda
```

Likely also available for browsing at:

- https://sources.debian.net/src/coinor-cgl/0.58.9-1/
- https://sources.debian.net/src/coinor-cgl/0.58.9-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `coinor-osi=0.106.9-1`

Binary Packages:

- `coinor-libosi1=0.106.9-1`

Licenses: (parsed from: `/usr/share/doc/coinor-libosi1/copyright`)

- `EPL-1`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coinor-osi=0.106.9-1
'http://deb.debian.org/debian/pool/main/c/coinor-osi/coinor-osi_0.106.9-1.dsc' coinor-osi_0.106.9-1.dsc 2280 SHA256:b8f63e0788f2a7ff422d25d8fb62ef445715767ebbaa8e9b7745a2249d5f8fef
'http://deb.debian.org/debian/pool/main/c/coinor-osi/coinor-osi_0.106.9.orig.tar.gz' coinor-osi_0.106.9.orig.tar.gz 751902 SHA256:3e7db33360a63d1315d3b0f64fe0031ff96c8bbc7af9fc5faf036a4fcf7fe68e
'http://deb.debian.org/debian/pool/main/c/coinor-osi/coinor-osi_0.106.9-1.debian.tar.xz' coinor-osi_0.106.9-1.debian.tar.xz 7600 SHA256:2e0f444924cae32a6b3b00904a82aad7b6068cace0cc5912ead684dee0b1e6ed
```

Likely also available for browsing at:

- https://sources.debian.net/src/coinor-osi/0.106.9-1/
- https://sources.debian.net/src/coinor-osi/0.106.9-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `coinutils=2.9.15-3`

Binary Packages:

- `coinor-libcoinutils3=2.9.15-3`

Licenses: (parsed from: `/usr/share/doc/coinor-libcoinutils3/copyright`)

- `EPL-1`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coinutils=2.9.15-3
'http://deb.debian.org/debian/pool/main/c/coinutils/coinutils_2.9.15-3.dsc' coinutils_2.9.15-3.dsc 1951 SHA256:44918ee4c809b9041c578fd07ae54c1ea1421731324393ac37f033ee64b149d0
'http://deb.debian.org/debian/pool/main/c/coinutils/coinutils_2.9.15.orig.tar.gz' coinutils_2.9.15.orig.tar.gz 1742562 SHA256:db1a0504f3334929462b7ee72a6c6f6c2ad23331716f829c5be8899193bf414d
'http://deb.debian.org/debian/pool/main/c/coinutils/coinutils_2.9.15-3.debian.tar.xz' coinutils_2.9.15-3.debian.tar.xz 8368 SHA256:c1ad448fc76ed100f24794692645206363ed0c372c3556bf7b51fa081db6b43d
```

Likely also available for browsing at:

- https://sources.debian.net/src/coinutils/2.9.15-3/
- https://sources.debian.net/src/coinutils/2.9.15-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `coreutils=8.23-4`

Binary Packages:

- `coreutils=8.23-4`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coreutils=8.23-4
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.23-4.dsc' coreutils_8.23-4.dsc 1942 SHA256:280ace2d2f1740c2319338e96da6b5000b9e65ddb9549c772917123633afe772
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.23.orig.tar.gz' coreutils_8.23.orig.tar.gz 12582141 SHA256:d606551dccd8c4ed079d7aa8d74af152b1d16215cae763d86b40b26fdbde9c73
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.23-4.diff.gz' coreutils_8.23-4.diff.gz 48759 SHA256:19ab6ff1b82f29e8a8f8107f925eec91b1eaad53b690f2d7154ab07101bf8c01
```

Likely also available for browsing at:

- https://sources.debian.net/src/coreutils/8.23-4/
- https://sources.debian.net/src/coreutils/8.23-4/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `cryptsetup=2:1.6.6-5`

Binary Packages:

- `libcryptsetup4:amd64=2:1.6.6-5`

Licenses: (parsed from: `/usr/share/doc/libcryptsetup4/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris cryptsetup=2:1.6.6-5
'http://deb.debian.org/debian/pool/main/c/cryptsetup/cryptsetup_1.6.6-5.dsc' cryptsetup_1.6.6-5.dsc 2624 SHA256:f7582c8becb38fecaed22aa531bd748dee2ebdbdac64e00c7e39e45afe7eaae1
'http://deb.debian.org/debian/pool/main/c/cryptsetup/cryptsetup_1.6.6.orig.tar.xz' cryptsetup_1.6.6.orig.tar.xz 1145940 SHA256:2d2ce28e4e1137dd599d87884b62ef6dbf14fd7848b2a2bf7d61cf125fbd8e6f
'http://deb.debian.org/debian/pool/main/c/cryptsetup/cryptsetup_1.6.6-5.debian.tar.xz' cryptsetup_1.6.6-5.debian.tar.xz 82944 SHA256:fa12da2f5448e0b02e1e5c89357de3749f854b2b96441f9c56737766c11cded0
```

Likely also available for browsing at:

- https://sources.debian.net/src/cryptsetup/2:1.6.6-5/
- https://sources.debian.net/src/cryptsetup/2:1.6.6-5/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `cups=1.7.5-11+deb8u1`

Binary Packages:

- `libcups2:amd64=1.7.5-11+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libcups2/copyright`)

- `GPL-2`
- `GPL-2 with exceptions`
- `LGPL-2`
- `LGPL-2 with exceptions`

Source:

```console
$ apt-get source -qq --print-uris cups=1.7.5-11+deb8u1
'http://deb.debian.org/debian/pool/main/c/cups/cups_1.7.5-11+deb8u1.dsc' cups_1.7.5-11+deb8u1.dsc 3450 SHA256:4c00719c6e888784e771de6cef1c16590052c16a89e5d470dba55bba97714c79
'http://deb.debian.org/debian/pool/main/c/cups/cups_1.7.5.orig.tar.bz2' cups_1.7.5.orig.tar.bz2 8793338 SHA256:18cb4c6847dbaaaa05c8b35af787f19dd5c7686970b46548e72c711c6f26bd02
'http://deb.debian.org/debian/pool/main/c/cups/cups_1.7.5-11+deb8u1.debian.tar.xz' cups_1.7.5-11+deb8u1.debian.tar.xz 300548 SHA256:b11190dfbc8fd97cf6e8d9c2ae286f70495ac9fda47290bc6f0277bb07692adf
```

Likely also available for browsing at:

- https://sources.debian.net/src/cups/1.7.5-11+deb8u1/
- https://sources.debian.net/src/cups/1.7.5-11+deb8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `curl=7.38.0-4+deb8u5`

Binary Packages:

- `curl=7.38.0-4+deb8u5`
- `libcurl3:amd64=7.38.0-4+deb8u5`
- `libcurl3-gnutls:amd64=7.38.0-4+deb8u5`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`

Source:

```console
$ apt-get source -qq --print-uris curl=7.38.0-4+deb8u5
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.38.0-4+deb8u5.dsc' curl_7.38.0-4+deb8u5.dsc 2637 SHA256:2b5e0bf7ea27efaa23d3274a487227436a8b6777dc571c957ae1c9fb4e455d8d
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.38.0.orig.tar.gz' curl_7.38.0.orig.tar.gz 4094034 SHA256:5661028aa6532882fa228cd23c99ddbb8b87643dbb1a7ea55c068d34a943dff1
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.38.0-4+deb8u5.debian.tar.xz' curl_7.38.0-4+deb8u5.debian.tar.xz 40224 SHA256:3f917091d1694a77852fe05293dafff079382e70d93f62f7de5c61f1812cf69d
```

Likely also available for browsing at:

- https://sources.debian.net/src/curl/7.38.0-4+deb8u5/
- https://sources.debian.net/src/curl/7.38.0-4+deb8u5/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `cyrus-sasl2=2.1.26.dfsg1-13+deb8u1`

Binary Packages:

- `libsasl2-2:amd64=2.1.26.dfsg1-13+deb8u1`
- `libsasl2-modules-db:amd64=2.1.26.dfsg1-13+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-2-clause`
- `BSD-4-clause`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.26.dfsg1-13+deb8u1
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.26.dfsg1-13+deb8u1.dsc' cyrus-sasl2_2.1.26.dfsg1-13+deb8u1.dsc 3461 SHA256:ed1cba2b699aaf1ad08b99ea82d40c583c02817f6fbd765b9bbcd940d72fc3f3
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.26.dfsg1.orig.tar.gz' cyrus-sasl2_2.1.26.dfsg1.orig.tar.gz 1494337 SHA256:172c39555012f479543ce7305949db75df708771fe8f8b34248027f09e53bb85
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.26.dfsg1-13+deb8u1.debian.tar.xz' cyrus-sasl2_2.1.26.dfsg1-13+deb8u1.debian.tar.xz 94284 SHA256:14e00798c41b6fae965211f1af8b47a67d22001146d0019f81af0fc7be9f162f
```

Likely also available for browsing at:

- https://sources.debian.net/src/cyrus-sasl2/2.1.26.dfsg1-13+deb8u1/
- https://sources.debian.net/src/cyrus-sasl2/2.1.26.dfsg1-13+deb8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `dash=0.5.7-4`

Binary Packages:

- `dash=0.5.7-4+b1`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.7-4
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.7-4.dsc' dash_0.5.7-4.dsc 1105 SHA256:c77f4baef8cbdc105a783bf6e4d3253ae10671ad98c27bf8537c8c731f073310
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.7.orig.tar.gz' dash_0.5.7.orig.tar.gz 223794 SHA256:ae89fa9f1145b7748cf0740e1df04cd52fdf8a285da4911dd0f04983efba4e39
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.7-4.diff.gz' dash_0.5.7-4.diff.gz 42834 SHA256:649d97aa0c48dc0db73c08d7e89a004b9d413279a823388161940342016284f0
```

Likely also available for browsing at:

- https://sources.debian.net/src/dash/0.5.7-4/
- https://sources.debian.net/src/dash/0.5.7-4/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `db5.3=5.3.28-9`

Binary Packages:

- `libdb5.3:amd64=5.3.28-9`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28-9
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28-9.dsc' db5.3_5.3.28-9.dsc 3166 SHA256:0020cd1491a10a2bfc7a125eb5f3a4db3745387e2d5f8f8f079be27ddfbdcf05
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28.orig.tar.xz' db5.3_5.3.28.orig.tar.xz 24154920 SHA256:e1f85c8b6ebd0ed3ca72fa0ae97b65006f6d0bd0cd6f4ac24bed103cb5497bf5
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28-9.debian.tar.xz' db5.3_5.3.28-9.debian.tar.xz 27664 SHA256:62adde71eda43c1300cdff51118721cef03dbc4bbe219f2669db5dcd90278ac3
```

Likely also available for browsing at:

- https://sources.debian.net/src/db5.3/5.3.28-9/
- https://sources.debian.net/src/db5.3/5.3.28-9/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `dbus-glib=0.102-1`

Binary Packages:

- `libdbus-glib-1-2:amd64=0.102-1`

Licenses: (parsed from: `/usr/share/doc/libdbus-glib-1-2/copyright`)

- `AFL-2.1`
- `Expat`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris dbus-glib=0.102-1
'http://deb.debian.org/debian/pool/main/d/dbus-glib/dbus-glib_0.102-1.dsc' dbus-glib_0.102-1.dsc 2336 SHA256:78f952039adb19be593147ca151842f06a38f4c09201ac4c9e22ce4947dc0444
'http://deb.debian.org/debian/pool/main/d/dbus-glib/dbus-glib_0.102.orig.tar.gz' dbus-glib_0.102.orig.tar.gz 783792 SHA256:6964ed585bb8149a14ab744b5ded5e77cf71ec5446e6dcc5fcf5eebcc52df29c
'http://deb.debian.org/debian/pool/main/d/dbus-glib/dbus-glib_0.102-1.debian.tar.xz' dbus-glib_0.102-1.debian.tar.xz 18780 SHA256:b330c124c786940d607d5ede3f0b36c5dcb0b6f84cf0cab7a0ac8eab3b7ecd92
```

Likely also available for browsing at:

- https://sources.debian.net/src/dbus-glib/0.102-1/
- https://sources.debian.net/src/dbus-glib/0.102-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `dbus=1.8.22-0+deb8u1`

Binary Packages:

- `dbus=1.8.22-0+deb8u1`
- `libdbus-1-3:amd64=1.8.22-0+deb8u1`

Licenses: (parsed from: `/usr/share/doc/dbus/copyright`, `/usr/share/doc/libdbus-1-3/copyright`)

- `AFL-2.1`
- `AFL-2.1,`
- `BSD-3-clause`
- `BSD-3-clause-generic`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `Tcl-BSDish`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris dbus=1.8.22-0+deb8u1
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.8.22-0+deb8u1.dsc' dbus_1.8.22-0+deb8u1.dsc 2889 SHA256:13cf18c13043baccf6fb26d18ea4e0fcb4b6859942175b3b735a1f63608c75c1
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.8.22.orig.tar.gz' dbus_1.8.22.orig.tar.gz 1894768 SHA256:19a52e5a42b2a2faf15a54745a098bb8cf55a76598fa4a0b8b6d886adcbe1d53
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.8.22-0+deb8u1.debian.tar.xz' dbus_1.8.22-0+deb8u1.debian.tar.xz 38168 SHA256:9c702fd70d8b451351bf8566dae78ef57e129d7cad9fcde000923575131fda5c
```

Likely also available for browsing at:

- https://sources.debian.net/src/dbus/1.8.22-0+deb8u1/
- https://sources.debian.net/src/dbus/1.8.22-0+deb8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `debconf=1.5.56`

Binary Packages:

- `debconf=1.5.56`
- `debconf-i18n=1.5.56`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`, `/usr/share/doc/debconf-i18n/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.56
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.56.dsc' debconf_1.5.56.dsc 1977 SHA256:584e73f5a84791f4b25ac0bcb65dd5a63de10e5398d986cb005597566fd23ca4
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.56.tar.gz' debconf_1.5.56.tar.gz 1004238 SHA256:e8371becb1ad91b69b0f2b2e580d30a0a4c63b4c2803dea2fb8e3136b662bfa5
```

Likely also available for browsing at:

- https://sources.debian.net/src/debconf/1.5.56/
- https://sources.debian.net/src/debconf/1.5.56/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `debian-archive-keyring=2014.3`

Binary Packages:

- `debian-archive-keyring=2014.3`

Licenses: (parsed from: `/usr/share/doc/debian-archive-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debian-archive-keyring=2014.3
'http://deb.debian.org/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2014.3.dsc' debian-archive-keyring_2014.3.dsc 1597 SHA256:2a3e604f936b8fbaf1beeea0a7611a1a88cacffd26571df4cc58c16ecefa362a
'http://deb.debian.org/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2014.3.tar.xz' debian-archive-keyring_2014.3.tar.xz 61380 SHA256:46be978ec2f72b0277d9e71bda30ea1b2b9aa00b1952cb35e8b22a2c016f5e22
```

Likely also available for browsing at:

- https://sources.debian.net/src/debian-archive-keyring/2014.3/
- https://sources.debian.net/src/debian-archive-keyring/2014.3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `debianutils=4.4`

Binary Packages:

- `debianutils=4.4+b1`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debianutils=4.4
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_4.4.dsc' debianutils_4.4.dsc 1560 SHA256:e365ad42af528f46eb117ef244216aaf265372f2b92635b28452a8f0d981bb17
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_4.4.tar.gz' debianutils_4.4.tar.gz 272098 SHA256:190850cdd6b5302e0a1ba1aaed1bc7074d67d3bd8d04c613f242f7145afa53a6
```

Likely also available for browsing at:

- https://sources.debian.net/src/debianutils/4.4/
- https://sources.debian.net/src/debianutils/4.4/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `dh-python=1.20141111-2`

Binary Packages:

- `dh-python=1.20141111-2`

Licenses: (parsed from: `/usr/share/doc/dh-python/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris dh-python=1.20141111-2
'http://deb.debian.org/debian/pool/main/d/dh-python/dh-python_1.20141111-2.dsc' dh-python_1.20141111-2.dsc 1975 SHA256:05f53d964951fb2422f273beb0667333e6327c78537332b19b33fd3c14dd5ae9
'http://deb.debian.org/debian/pool/main/d/dh-python/dh-python_1.20141111.orig.tar.xz' dh-python_1.20141111.orig.tar.xz 67988 SHA256:726bd70f10d26adb3d2b2b24627ea592ce6508b516dee97319dc303b950a5c1e
'http://deb.debian.org/debian/pool/main/d/dh-python/dh-python_1.20141111-2.debian.tar.xz' dh-python_1.20141111-2.debian.tar.xz 5728 SHA256:683e90cabb3831ca707f6a7a99f3c5c86e981232d09b7d45d531d044977947e6
```

Likely also available for browsing at:

- https://sources.debian.net/src/dh-python/1.20141111-2/
- https://sources.debian.net/src/dh-python/1.20141111-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `diffutils=1:3.3-1`

Binary Packages:

- `diffutils=1:3.3-1+b1`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.3-1
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.3-1.dsc' diffutils_3.3-1.dsc 1427 SHA256:72df1fed003b47509a063dfa8aa89108c884cd3bf52a06ce40e1ffb61f5a256c
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.3.orig.tar.xz' diffutils_3.3.orig.tar.xz 1197832 SHA256:a25e89a8ab65fded1731e4186be1bb25cda967834b6df973599cdcd5abdfc19c
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.3-1.debian.tar.gz' diffutils_3.3-1.debian.tar.gz 10584 SHA256:23765ea43cd1b4e5e504ce0984a16e27d5c01e9272cba489ebbebd217f227fc7
```

Likely also available for browsing at:

- https://sources.debian.net/src/diffutils/1:3.3-1/
- https://sources.debian.net/src/diffutils/1:3.3-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `dpkg=1.17.27`

Binary Packages:

- `dpkg=1.17.27`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.17.27
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.17.27.dsc' dpkg_1.17.27.dsc 2018 SHA256:730ad9445990322551acf79a752515d27ffca5c8b6d978b3276d28e88d60e34f
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.17.27.tar.xz' dpkg_1.17.27.tar.xz 4413092 SHA256:90749c31b9f1fceb46dd9fab5b50de34272efef333cc16d9e144f514fd944bb6
```

Likely also available for browsing at:

- https://sources.debian.net/src/dpkg/1.17.27/
- https://sources.debian.net/src/dpkg/1.17.27/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `e2fsprogs=1.42.12-2`

Binary Packages:

- `e2fslibs:amd64=1.42.12-2+b1`
- `e2fsprogs=1.42.12-2+b1`
- `libcomerr2:amd64=1.42.12-2+b1`
- `libss2:amd64=1.42.12-2+b1`

Licenses: (parsed from: `/usr/share/doc/e2fslibs/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcomerr2/copyright`, `/usr/share/doc/libss2/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.42.12-2
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.42.12-2.dsc' e2fsprogs_1.42.12-2.dsc 2200 SHA256:c0edf462e2d55c64bc0e8278602066f458efd1b744627238a1d2b38e4ac2af94
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.42.12.orig.tar.gz' e2fsprogs_1.42.12.orig.tar.gz 6381695 SHA256:e17846d91a0edd89fa59b064bde8f8e5cec5851e35f587bcccb4014dbd63186c
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.42.12-2.debian.tar.xz' e2fsprogs_1.42.12-2.debian.tar.xz 68700 SHA256:23b927df5556f4854ea26bb8e7c55cdc9a31b920d1dd0be7a2965378dde30bd4
```

Likely also available for browsing at:

- https://sources.debian.net/src/e2fsprogs/1.42.12-2/
- https://sources.debian.net/src/e2fsprogs/1.42.12-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `expat=2.1.0-6+deb8u3`

Binary Packages:

- `libexpat1:amd64=2.1.0-6+deb8u3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris expat=2.1.0-6+deb8u3
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.1.0-6+deb8u3.dsc' expat_2.1.0-6+deb8u3.dsc 2278 SHA256:3485be5c4ffc922aea14718c48c4107b04559ec013cc0e98a61597da50320e25
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.1.0.orig.tar.gz' expat_2.1.0.orig.tar.gz 562616 SHA256:823705472f816df21c8f6aa026dd162b280806838bb55b3432b0fb1fcca7eb86
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.1.0-6+deb8u3.debian.tar.xz' expat_2.1.0-6+deb8u3.debian.tar.xz 21716 SHA256:5e756a68a7634b7b7109024bd33df4df3c5964ea0d0f5e8db0ca98f623bcd841
```

Likely also available for browsing at:

- https://sources.debian.net/src/expat/2.1.0-6+deb8u3/
- https://sources.debian.net/src/expat/2.1.0-6+deb8u3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `findutils=4.4.2-9`

Binary Packages:

- `findutils=4.4.2-9+b1`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.2`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.4.2-9
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.4.2-9.dsc' findutils_4.4.2-9.dsc 1996 SHA256:0dd9d96af8260d2e81c5819d2e5536f95cb894e771c9adcab44ba70726adb13e
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.4.2.orig.tar.gz' findutils_4.4.2.orig.tar.gz 2149838 SHA256:434f32d171cbc0a5e72cfc5372c6fc4cb0e681f8dce566a0de5b6fccd702b62a
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.4.2-9.debian.tar.xz' findutils_4.4.2-9.debian.tar.xz 27384 SHA256:8a9f5fb20c255b833994d7dfff1999b3f4f95dea6008495f2b0ef6c549d62c34
```

Likely also available for browsing at:

- https://sources.debian.net/src/findutils/4.4.2-9/
- https://sources.debian.net/src/findutils/4.4.2-9/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `fontconfig=2.11.0-6.3+deb8u1`

Binary Packages:

- `fontconfig=2.11.0-6.3+deb8u1`
- `fontconfig-config=2.11.0-6.3+deb8u1`
- `libfontconfig1:amd64=2.11.0-6.3+deb8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fontconfig=2.11.0-6.3+deb8u1
'http://deb.debian.org/debian/pool/main/f/fontconfig/fontconfig_2.11.0-6.3+deb8u1.dsc' fontconfig_2.11.0-6.3+deb8u1.dsc 2235 SHA256:c496170e75ece48a19c5b60745eef5522b62ae1a817c23125ebd9745bc255fcd
'http://deb.debian.org/debian/pool/main/f/fontconfig/fontconfig_2.11.0.orig.tar.xz' fontconfig_2.11.0.orig.tar.xz 319652 SHA256:f19c7366d59dc4e79eaf3eedabd44b6375b238f29316db5020a183c7d9a78db9
'http://deb.debian.org/debian/pool/main/f/fontconfig/fontconfig_2.11.0-6.3+deb8u1.debian.tar.xz' fontconfig_2.11.0-6.3+deb8u1.debian.tar.xz 1073796 SHA256:a8140c4576a2c43614930e8a307966018551ae71ad448af5f75faf4f47f70173
```

Likely also available for browsing at:

- https://sources.debian.net/src/fontconfig/2.11.0-6.3+deb8u1/
- https://sources.debian.net/src/fontconfig/2.11.0-6.3+deb8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `fonts-dejavu=2.34-1`

Binary Packages:

- `fonts-dejavu=2.34-1`
- `fonts-dejavu-core=2.34-1`
- `fonts-dejavu-extra=2.34-1`

Licenses: (parsed from: `/usr/share/doc/fonts-dejavu/copyright`, `/usr/share/doc/fonts-dejavu-core/copyright`, `/usr/share/doc/fonts-dejavu-extra/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris fonts-dejavu=2.34-1
'http://deb.debian.org/debian/pool/main/f/fonts-dejavu/fonts-dejavu_2.34-1.dsc' fonts-dejavu_2.34-1.dsc 2484 SHA256:843b22fff349667b83f66cf3ab2e93a187ff016f4bd90fbfbe9001bf82a9d66d
'http://deb.debian.org/debian/pool/main/f/fonts-dejavu/fonts-dejavu_2.34.orig.tar.bz2' fonts-dejavu_2.34.orig.tar.bz2 11329547 SHA256:b5ca9e671635a9fe04c791cdc82c707ba57380c2cc8de3f92451a039134b9027
'http://deb.debian.org/debian/pool/main/f/fonts-dejavu/fonts-dejavu_2.34-1.debian.tar.gz' fonts-dejavu_2.34-1.debian.tar.gz 11231 SHA256:46044164bdc385037a1694a07e8c5a1c183511cb68743914219ebb93750dac19
```

Likely also available for browsing at:

- https://sources.debian.net/src/fonts-dejavu/2.34-1/
- https://sources.debian.net/src/fonts-dejavu/2.34-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `fonts-sil-gentium-basic=1.1-7`

Binary Packages:

- `fonts-sil-gentium-basic=1.1-7`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fonts-sil-gentium-basic=1.1-7
'http://deb.debian.org/debian/pool/main/f/fonts-sil-gentium-basic/fonts-sil-gentium-basic_1.1-7.dsc' fonts-sil-gentium-basic_1.1-7.dsc 2156 SHA256:1d4e22b38de39420dacec6f47c68f12ee65256a425127b799520a18263b6525f
'http://deb.debian.org/debian/pool/main/f/fonts-sil-gentium-basic/fonts-sil-gentium-basic_1.1.orig.tar.bz2' fonts-sil-gentium-basic_1.1.orig.tar.bz2 1144657 SHA256:3c094fe3cdc2ba3ed9cab6c8e566a34ddea0e9a167a71547ad4a9c3d6290a84f
'http://deb.debian.org/debian/pool/main/f/fonts-sil-gentium-basic/fonts-sil-gentium-basic_1.1-7.debian.tar.gz' fonts-sil-gentium-basic_1.1-7.debian.tar.gz 5489 SHA256:1047618b2705d1d32c1677aeece8cf440841402e33e43b4d92aa7d178551d2f3
```

Likely also available for browsing at:

- https://sources.debian.net/src/fonts-sil-gentium-basic/1.1-7/
- https://sources.debian.net/src/fonts-sil-gentium-basic/1.1-7/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `freetype=2.5.2-3+deb8u1`

Binary Packages:

- `libfreetype6:amd64=2.5.2-3+deb8u1`

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
$ apt-get source -qq --print-uris freetype=2.5.2-3+deb8u1
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.5.2-3+deb8u1.dsc' freetype_2.5.2-3+deb8u1.dsc 2096 SHA256:a56cdf04463a7d9b13c1a2fd1c257b9626f28516efc7243fd2ee34eae2f14a13
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.5.2.orig.tar.gz' freetype_2.5.2.orig.tar.gz 1971155 SHA256:5fda4996e43cfdf9b602a0eb5abde014f1a3c3b2d82bbb9b86942011c63f5c3a
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.5.2-3+deb8u1.diff.gz' freetype_2.5.2-3+deb8u1.diff.gz 68796 SHA256:196918fc99a74441d7f7e6e85133b0ba7d6b85b2d5b5cd764fc32edd7dd97923
```

Likely also available for browsing at:

- https://sources.debian.net/src/freetype/2.5.2-3+deb8u1/
- https://sources.debian.net/src/freetype/2.5.2-3+deb8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `gcc-4.8=4.8.4-1`

Binary Packages:

- `gcc-4.8-base:amd64=4.8.4-1`

Licenses: (parsed from: `/usr/share/doc/gcc-4.8-base/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris gcc-4.8=4.8.4-1
'http://deb.debian.org/debian/pool/main/g/gcc-4.8/gcc-4.8_4.8.4-1.dsc' gcc-4.8_4.8.4-1.dsc 10638 SHA256:9ba284727055aba04bb3122ef7f857587a403a5c9a2f924948829da49ca2ef02
'http://deb.debian.org/debian/pool/main/g/gcc-4.8/gcc-4.8_4.8.4-1.tar.gz' gcc-4.8_4.8.4-1.tar.gz 187653934 SHA256:c38d9687b6fef3010f250adaf89a3f1bd0f12c9cd82ed531a52e7d394b8226cf
```

Likely also available for browsing at:

- https://sources.debian.net/src/gcc-4.8/4.8.4-1/
- https://sources.debian.net/src/gcc-4.8/4.8.4-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `gcc-4.9=4.9.2-10`

Binary Packages:

- `gcc-4.9-base:amd64=4.9.2-10`
- `libgcc1:amd64=1:4.9.2-10`
- `libgfortran3:amd64=4.9.2-10`
- `libquadmath0:amd64=4.9.2-10`
- `libstdc++6:amd64=4.9.2-10`

Licenses: (parsed from: `/usr/share/doc/gcc-4.9-base/copyright`, `/usr/share/doc/libgcc1/copyright`, `/usr/share/doc/libgfortran3/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris gcc-4.9=4.9.2-10
'http://deb.debian.org/debian/pool/main/g/gcc-4.9/gcc-4.9_4.9.2-10.dsc' gcc-4.9_4.9.2-10.dsc 19222 SHA256:591b7db6bd972dd1a7b99953e367a89f859deb3a13efa8531034c2ab568314b1
'http://deb.debian.org/debian/pool/main/g/gcc-4.9/gcc-4.9_4.9.2.orig.tar.gz' gcc-4.9_4.9.2.orig.tar.gz 73565212 SHA256:861aa811d5f9e9ecf32d8195d2346fc434eba7e17330878ed3d876c49a32ec4e
'http://deb.debian.org/debian/pool/main/g/gcc-4.9/gcc-4.9_4.9.2-10.diff.gz' gcc-4.9_4.9.2-10.diff.gz 848893 SHA256:7e566640487ea9456186656848bfc1e43242ed448766ed3553b79fee16d25edb
```

Likely also available for browsing at:

- https://sources.debian.net/src/gcc-4.9/4.9.2-10/
- https://sources.debian.net/src/gcc-4.9/4.9.2-10/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `gdbm=1.8.3-13.1`

Binary Packages:

- `libgdbm3:amd64=1.8.3-13.1`

Licenses: (parsed from: `/usr/share/doc/libgdbm3/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.8.3-13.1
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.8.3-13.1.dsc' gdbm_1.8.3-13.1.dsc 1830 SHA256:b1d8bef30edc491315c337930cbe2b61f44f55035adfc26ae945bab5ca57d5c9
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.8.3.orig.tar.bz2' gdbm_1.8.3.orig.tar.bz2 172796 SHA256:1d5995b6e9e6be4ff62c8126d019f184a083dd8e6f75f6c74b9fe023b5b9440e
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.8.3-13.1.debian.tar.xz' gdbm_1.8.3-13.1.debian.tar.xz 14748 SHA256:251401e1f5210226f384e936b1b7ea1df40119a918d9f3dbf48b2e51d4df8983
```

Likely also available for browsing at:

- https://sources.debian.net/src/gdbm/1.8.3-13.1/
- https://sources.debian.net/src/gdbm/1.8.3-13.1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `gdk-pixbuf=2.31.1-2+deb8u5`

Binary Packages:

- `libgdk-pixbuf2.0-0:amd64=2.31.1-2+deb8u5`
- `libgdk-pixbuf2.0-common=2.31.1-2+deb8u5`

Licenses: (parsed from: `/usr/share/doc/libgdk-pixbuf2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf=2.31.1-2+deb8u5
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.31.1-2+deb8u5.dsc' gdk-pixbuf_2.31.1-2+deb8u5.dsc 2902 SHA256:d2fd75ff6c0ae20bc3b67621b09e980a1c78fad20a1b21df054275eeaab4a9c0
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.31.1.orig.tar.xz' gdk-pixbuf_2.31.1.orig.tar.xz 1340056 SHA256:25a75e3c61dac11e6ff6416ad846951ccafac6486b1c6a1bfb0b213b99db52cd
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.31.1-2+deb8u5.debian.tar.xz' gdk-pixbuf_2.31.1-2+deb8u5.debian.tar.xz 18300 SHA256:3a8ffeac00c1020e2429454adbea06b15389aa5bfb308550c8c6d176c7c1fe63
```

Likely also available for browsing at:

- https://sources.debian.net/src/gdk-pixbuf/2.31.1-2+deb8u5/
- https://sources.debian.net/src/gdk-pixbuf/2.31.1-2+deb8u5/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `glew=1.10.0-3`

Binary Packages:

- `libglew1.10:amd64=1.10.0-3`

Licenses: (parsed from: `/usr/share/doc/libglew1.10/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `Mesa`

Source:

```console
$ apt-get source -qq --print-uris glew=1.10.0-3
'http://deb.debian.org/debian/pool/main/g/glew/glew_1.10.0-3.dsc' glew_1.10.0-3.dsc 2276 SHA256:63bb683a5a0fd90b51505ee5c59184f3375cccfd0e0c6c6fac05e8337ba6e3eb
'http://deb.debian.org/debian/pool/main/g/glew/glew_1.10.0.orig.tar.gz' glew_1.10.0.orig.tar.gz 567605 SHA256:99c41320b63f6860869b5fb9af9a1854b15582796c64ee3dfd7096dc0c89f307
'http://deb.debian.org/debian/pool/main/g/glew/glew_1.10.0-3.debian.tar.gz' glew_1.10.0-3.debian.tar.gz 39265 SHA256:f03049d2d0ca15199136909ff7209af3ffe3b88aeea8e52ab55abd226b3261d8
```

Likely also available for browsing at:

- https://sources.debian.net/src/glew/1.10.0-3/
- https://sources.debian.net/src/glew/1.10.0-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `glib2.0=2.42.1-1`

Binary Packages:

- `libglib2.0-0:amd64=2.42.1-1+b1`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.42.1-1
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.42.1-1.dsc' glib2.0_2.42.1-1.dsc 3119 SHA256:61b01cb94e8bb8b9fdd1799b2e1bed907371dc45d364beec4b79a129745f588f
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.42.1.orig.tar.xz' glib2.0_2.42.1.orig.tar.xz 6985120 SHA256:8f3f0865280e45b8ce840e176ef83bcfd511148918cc8d39df2ee89b67dcf89a
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.42.1-1.debian.tar.xz' glib2.0_2.42.1-1.debian.tar.xz 68072 SHA256:1cd368c2bce6100c07b8a07ff7f3f38572679d88563356b8784560606fcfac56
```

Likely also available for browsing at:

- https://sources.debian.net/src/glib2.0/2.42.1-1/
- https://sources.debian.net/src/glib2.0/2.42.1-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `glibc=2.19-18+deb8u7`

Binary Packages:

- `libc-bin=2.19-18+deb8u7`
- `libc6:amd64=2.19-18+deb8u7`
- `multiarch-support=2.19-18+deb8u7`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/multiarch-support/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.19-18+deb8u7
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.19-18+deb8u7.dsc' glibc_2.19-18+deb8u7.dsc 8252 SHA256:79d177b7b0ddbed7d92d667a5a574f501c3ed7a465900691d9238b9d1066f510
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.19.orig.tar.xz' glibc_2.19.orig.tar.xz 12387008 SHA256:746e52bb4fc9b2f30bcd33d415172a40ab56c5fff6c494052d31b0795593cc60
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.19-18+deb8u7.debian.tar.xz' glibc_2.19-18+deb8u7.debian.tar.xz 1055688 SHA256:d2c6d89b297fe55d58315f96ac510b3b6969ffc82318276545d0264903ab82ec
```

Likely also available for browsing at:

- https://sources.debian.net/src/glibc/2.19-18+deb8u7/
- https://sources.debian.net/src/glibc/2.19-18+deb8u7/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `gmp=2:6.0.0+dfsg-6`

Binary Packages:

- `libgmp10:amd64=2:6.0.0+dfsg-6`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.0.0+dfsg-6
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.0.0+dfsg-6.dsc' gmp_6.0.0+dfsg-6.dsc 1840 SHA256:40f44bfae4ed9df69a8c64fe9bf9deded10cc4a75844c95bbfbfc3307976f53a
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.0.0+dfsg.orig.tar.xz' gmp_6.0.0+dfsg.orig.tar.xz 1756792 SHA256:7539e094815fc321f4dc64b0a6968db9e1bee85a459bc64d4cc2b9dd0f6729a5
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.0.0+dfsg-6.debian.tar.xz' gmp_6.0.0+dfsg-6.debian.tar.xz 21024 SHA256:83219073eab9fb886dd1123b6b571b45fbe2f7c290c4201b07696784ffcf7fd1
```

Likely also available for browsing at:

- https://sources.debian.net/src/gmp/2:6.0.0+dfsg-6/
- https://sources.debian.net/src/gmp/2:6.0.0+dfsg-6/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `gnupg=1.4.18-7+deb8u3`

Binary Packages:

- `gnupg=1.4.18-7+deb8u3`
- `gpgv=1.4.18-7+deb8u3`

Licenses: (parsed from: `/usr/share/doc/gnupg/copyright`, `/usr/share/doc/gpgv/copyright`)

- `GPL-3`
- `GPL-3+ with OpenSSL exception`
- `RFC-Reference`

Source:

```console
$ apt-get source -qq --print-uris gnupg=1.4.18-7+deb8u3
'http://deb.debian.org/debian/pool/main/g/gnupg/gnupg_1.4.18-7+deb8u3.dsc' gnupg_1.4.18-7+deb8u3.dsc 2432 SHA256:936c6e278b978f3edd24264940fca2f16d3c22c58437400578cdc7a9e6cb4148
'http://deb.debian.org/debian/pool/main/g/gnupg/gnupg_1.4.18.orig.tar.gz' gnupg_1.4.18.orig.tar.gz 5047888 SHA256:10a8936b76ccadb98521535b5f41cc5b41b3c159a6c2915f062bd4dc8ac12d12
'http://deb.debian.org/debian/pool/main/g/gnupg/gnupg_1.4.18-7+deb8u3.debian.tar.xz' gnupg_1.4.18-7+deb8u3.debian.tar.xz 301204 SHA256:2117df33f763efb2afbd9c154b6bfbf6a91c0ef1c1bee73357c03fd15f18605f
```

Likely also available for browsing at:

- https://sources.debian.net/src/gnupg/1.4.18-7+deb8u3/
- https://sources.debian.net/src/gnupg/1.4.18-7+deb8u3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `gnutls28=3.3.8-6+deb8u4`

Binary Packages:

- `libgnutls-deb0-28:amd64=3.3.8-6+deb8u4`

Licenses: (parsed from: `/usr/share/doc/libgnutls-deb0-28/copyright`)

- `GFDL-1.3`
- `GPL`
- `GPL-3`
- `GPLv3+`
- `LGPL`
- `LGPL-3`
- `LGPL2.1`
- `The main library is licensed under GNU Lesser`
- `nonstandard, see below`

Source:

```console
$ apt-get source -qq --print-uris gnutls28=3.3.8-6+deb8u4
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.3.8-6+deb8u4.dsc' gnutls28_3.3.8-6+deb8u4.dsc 2923 SHA256:90fb209fc1579d99b95be81df2a5fc7add9e5aa989f00f93805177d4e440620f
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.3.8.orig.tar.xz' gnutls28_3.3.8.orig.tar.xz 6153180 SHA256:bd4642f180e19632f4ed3a1e62d60c824c7b695f5cddf41a8fba1b272eaef046
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.3.8-6+deb8u4.debian.tar.xz' gnutls28_3.3.8-6+deb8u4.debian.tar.xz 96652 SHA256:a7e794a7ccf9133f00db2eeebe1d89a2e76f85bf31e2ab9ebe9108989c1ffeae
```

Likely also available for browsing at:

- https://sources.debian.net/src/gnutls28/3.3.8-6+deb8u4/
- https://sources.debian.net/src/gnutls28/3.3.8-6+deb8u4/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `graphite2=1.3.6-1~deb8u1`

Binary Packages:

- `libgraphite2-3:amd64=1.3.6-1~deb8u1`

Licenses: (parsed from: `/usr/share/doc/libgraphite2-3/copyright`)

- `Artistic`
- `GPL`
- `GPL-1+`
- `GPL1+ | Artistic`
- `LGPL | other`
- `LGPL-2`
- `LGPL-2+`
- `MPL-1.1 | GPL-2 | LGPL-2.1`
- `other`

Source:

```console
$ apt-get source -qq --print-uris graphite2=1.3.6-1~deb8u1
'http://deb.debian.org/debian/pool/main/g/graphite2/graphite2_1.3.6-1~deb8u1.dsc' graphite2_1.3.6-1~deb8u1.dsc 2173 SHA256:efb076e920bf14c190af776076711d1e3ea35ea55046cec43e48afbdbc647efc
'http://deb.debian.org/debian/pool/main/g/graphite2/graphite2_1.3.6.orig.tar.gz' graphite2_1.3.6.orig.tar.gz 3881106 SHA256:475e7657ac606ed8805518031729c1273cf7d9d422169ac6f7882e01d832af75
'http://deb.debian.org/debian/pool/main/g/graphite2/graphite2_1.3.6-1~deb8u1.debian.tar.xz' graphite2_1.3.6-1~deb8u1.debian.tar.xz 9664 SHA256:200c6dc8b54801dbc0080a857c00ef8856ab5bd36624c8d3918d00efd779ff4d
```

Likely also available for browsing at:

- https://sources.debian.net/src/graphite2/1.3.6-1~deb8u1/
- https://sources.debian.net/src/graphite2/1.3.6-1~deb8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `grep=2.20-4.1`

Binary Packages:

- `grep=2.20-4.1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=2.20-4.1
'http://deb.debian.org/debian/pool/main/g/grep/grep_2.20-4.1.dsc' grep_2.20-4.1.dsc 2627 SHA256:62ae6c19839e940462d27b2a234e925210cdb9209e2a4080b695fcec439c1d04
'http://deb.debian.org/debian/pool/main/g/grep/grep_2.20.orig.tar.xz' grep_2.20.orig.tar.xz 1237196 SHA256:f0af452bc0d09464b6d089b6d56a0a3c16672e9ed9118fbe37b0b6aeaf069a65
'http://deb.debian.org/debian/pool/main/g/grep/grep_2.20-4.1.debian.tar.bz2' grep_2.20-4.1.debian.tar.bz2 113054 SHA256:4aa8c4487d05dc82498668deeb485a9d4891a74df29466adf74e2faf738d2917
```

Likely also available for browsing at:

- https://sources.debian.net/src/grep/2.20-4.1/
- https://sources.debian.net/src/grep/2.20-4.1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `gst-plugins-base1.0=1.4.4-2+deb8u1`

Binary Packages:

- `libgstreamer-plugins-base1.0-0:amd64=1.4.4-2+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libgstreamer-plugins-base1.0-0/copyright`)

- `BSD (2 clause)`
- `BSD (3 clause)`
- `GPL-2+`
- `LGPL`
- `LGPL-2+`
- `MIT/X11 (BSD like) LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris gst-plugins-base1.0=1.4.4-2+deb8u1
'http://security.debian.org/pool/updates/main/g/gst-plugins-base1.0/gst-plugins-base1.0_1.4.4-2+deb8u1.dsc' gst-plugins-base1.0_1.4.4-2+deb8u1.dsc 3922 SHA256:9027629b9e790cef343b5effd757aa051f00293082e979b899ed9cefb6c24263
'http://security.debian.org/pool/updates/main/g/gst-plugins-base1.0/gst-plugins-base1.0_1.4.4.orig.tar.xz' gst-plugins-base1.0_1.4.4.orig.tar.xz 2632996 SHA256:49cd9e8f23c416b1607b43837a09833fa03e0106929d81ead2ddfde6c0ade44b
'http://security.debian.org/pool/updates/main/g/gst-plugins-base1.0/gst-plugins-base1.0_1.4.4-2+deb8u1.debian.tar.xz' gst-plugins-base1.0_1.4.4-2+deb8u1.debian.tar.xz 41864 SHA256:84f294f7ec18997ff2eef38b338ee33576584d016ebb9979fbce418a146f2ece
```

Likely also available for browsing at:

- https://sources.debian.net/src/gst-plugins-base1.0/1.4.4-2+deb8u1/
- https://sources.debian.net/src/gst-plugins-base1.0/1.4.4-2+deb8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `gstreamer1.0=1.4.4-2+deb8u1`

Binary Packages:

- `libgstreamer1.0-0:amd64=1.4.4-2+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libgstreamer1.0-0/copyright`)

- `GPL-2+`
- `GPL-3+`
- `LGPL`
- `LGPL-2+`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris gstreamer1.0=1.4.4-2+deb8u1
'http://security.debian.org/pool/updates/main/g/gstreamer1.0/gstreamer1.0_1.4.4-2+deb8u1.dsc' gstreamer1.0_1.4.4-2+deb8u1.dsc 3160 SHA256:bdcfa67dc38f142f94e7708dc469088f5efad2eb32a85289ab08635c2a3187a3
'http://security.debian.org/pool/updates/main/g/gstreamer1.0/gstreamer1.0_1.4.4.orig.tar.xz' gstreamer1.0_1.4.4.orig.tar.xz 3323860 SHA256:f0e305d91a93d05bf9e332cd4256ca07d77f5186a4d73847b7ae6db218f2c237
'http://security.debian.org/pool/updates/main/g/gstreamer1.0/gstreamer1.0_1.4.4-2+deb8u1.debian.tar.xz' gstreamer1.0_1.4.4-2+deb8u1.debian.tar.xz 40548 SHA256:7272d846b7b1cc6de83de2eafe878b51df79d4e88f8a2d3d4b38936e847b9131
```

Likely also available for browsing at:

- https://sources.debian.net/src/gstreamer1.0/1.4.4-2+deb8u1/
- https://sources.debian.net/src/gstreamer1.0/1.4.4-2+deb8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `gtk+2.0=2.24.25-3+deb8u1`

Binary Packages:

- `libgtk2.0-0:amd64=2.24.25-3+deb8u1`
- `libgtk2.0-common=2.24.25-3+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libgtk2.0-0/copyright`, `/usr/share/doc/libgtk2.0-common/copyright`)

- `LGPL-2`
- `other`

Source:

```console
$ apt-get source -qq --print-uris gtk+2.0=2.24.25-3+deb8u1
'http://deb.debian.org/debian/pool/main/g/gtk+2.0/gtk+2.0_2.24.25-3+deb8u1.dsc' gtk+2.0_2.24.25-3+deb8u1.dsc 3699 SHA256:d641410a476fb70739d56d0a2be9aa8afdf8a798592badb37ea51ce621b25eee
'http://deb.debian.org/debian/pool/main/g/gtk+2.0/gtk+2.0_2.24.25.orig.tar.xz' gtk+2.0_2.24.25.orig.tar.xz 13327832 SHA256:38af1020cb8ff3d10dda2c8807f11e92af9d2fa4045de61c62eedb7fbc7ea5b3
'http://deb.debian.org/debian/pool/main/g/gtk+2.0/gtk+2.0_2.24.25-3+deb8u1.debian.tar.xz' gtk+2.0_2.24.25-3+deb8u1.debian.tar.xz 91480 SHA256:3c205a052efd9b18fc92c596208141f77e76e9356edc85406db1e1c57d666531
```

Likely also available for browsing at:

- https://sources.debian.net/src/gtk+2.0/2.24.25-3+deb8u1/
- https://sources.debian.net/src/gtk+2.0/2.24.25-3+deb8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `gzip=1.6-4`

Binary Packages:

- `gzip=1.6-4`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.6-4
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.6-4.dsc' gzip_1.6-4.dsc 1853 SHA256:9605bb67aa336e3f1dd68429fa713a80dff3439d67f944160895b14c98503147
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.6.orig.tar.gz' gzip_1.6.orig.tar.gz 1074924 SHA256:97eb83b763d9e5ad35f351fe5517e6b71521d7aac7acf3e3cacdb6b1496d8f7e
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.6-4.debian.tar.xz' gzip_1.6-4.debian.tar.xz 14476 SHA256:20a474283cc0063de7db623ccc3b17da7df6bc15f681de4e9e1da12b990a2743
```

Likely also available for browsing at:

- https://sources.debian.net/src/gzip/1.6-4/
- https://sources.debian.net/src/gzip/1.6-4/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `harfbuzz=0.9.35-2`

Binary Packages:

- `libharfbuzz-icu0:amd64=0.9.35-2`
- `libharfbuzz0b:amd64=0.9.35-2`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz-icu0/copyright`, `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=0.9.35-2
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_0.9.35-2.dsc' harfbuzz_0.9.35-2.dsc 2303 SHA256:6e9428c29ecbb4beeb186a00121fda23362eebb4d389eb6f24f398cef1e1b9ec
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_0.9.35.orig.tar.bz2' harfbuzz_0.9.35.orig.tar.bz2 1165359 SHA256:0aa1a8aba6f502321cf6fef3c9d2c73dde48389c5ed1d3615a7691944c2a06ed
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_0.9.35-2.debian.tar.xz' harfbuzz_0.9.35-2.debian.tar.xz 7440 SHA256:a51eef8e3a9565865fc10d19fcd0d8d5be421a715f3f1445a9015274a8778532
```

Likely also available for browsing at:

- https://sources.debian.net/src/harfbuzz/0.9.35-2/
- https://sources.debian.net/src/harfbuzz/0.9.35-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `hostname=3.15`

Binary Packages:

- `hostname=3.15`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.15
'http://deb.debian.org/debian/pool/main/h/hostname/hostname_3.15.dsc' hostname_3.15.dsc 804 SHA256:e787dec3ac9ee20ff564d6d7afde242103e71830907ee8fa63367162b04e9844
'http://deb.debian.org/debian/pool/main/h/hostname/hostname_3.15.tar.gz' hostname_3.15.tar.gz 13039 SHA256:b6d10114ed14306b21745d2cac1b9adf7a2546f16b9fd719bec14bd7cec61d20
```

Likely also available for browsing at:

- https://sources.debian.net/src/hostname/3.15/
- https://sources.debian.net/src/hostname/3.15/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `hunspell=1.3.3-3`

Binary Packages:

- `libhunspell-1.3-0:amd64=1.3.3-3`

Licenses: (parsed from: `/usr/share/doc/libhunspell-1.3-0/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris hunspell=1.3.3-3
'http://deb.debian.org/debian/pool/main/h/hunspell/hunspell_1.3.3-3.dsc' hunspell_1.3.3-3.dsc 2167 SHA256:52f27ad32b641e0a24f537c727278124883d4d0fbe447713e628def4c4bbd116
'http://deb.debian.org/debian/pool/main/h/hunspell/hunspell_1.3.3.orig.tar.gz' hunspell_1.3.3.orig.tar.gz 986081 SHA256:a7b2c0de0e2ce17426821dc1ac8eb115029959b3ada9d80a81739fa19373246c
'http://deb.debian.org/debian/pool/main/h/hunspell/hunspell_1.3.3-3.debian.tar.xz' hunspell_1.3.3-3.debian.tar.xz 20928 SHA256:bc914a17cf0f7f967a3c5747fa7b680f611361521d509e72ace1916017b5e683
```

Likely also available for browsing at:

- https://sources.debian.net/src/hunspell/1.3.3-3/
- https://sources.debian.net/src/hunspell/1.3.3-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `hyphen=2.8.8-1`

Binary Packages:

- `libhyphen0=2.8.8-1`

Licenses: (parsed from: `/usr/share/doc/libhyphen0/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris hyphen=2.8.8-1
'http://deb.debian.org/debian/pool/main/h/hyphen/hyphen_2.8.8-1.dsc' hyphen_2.8.8-1.dsc 1944 SHA256:0846a3497adb4c5022d5bf331a32597341b230c9788a9246352591a9648511a5
'http://deb.debian.org/debian/pool/main/h/hyphen/hyphen_2.8.8.orig.tar.gz' hyphen_2.8.8.orig.tar.gz 638369 SHA256:304636d4eccd81a14b6914d07b84c79ebb815288c76fe027b9ebff6ff24d5705
'http://deb.debian.org/debian/pool/main/h/hyphen/hyphen_2.8.8-1.debian.tar.xz' hyphen_2.8.8-1.debian.tar.xz 12488 SHA256:602838e1850b77e2289a76239618761a03cbd43ebf9e0693d569f2f5cac8fe4d
```

Likely also available for browsing at:

- https://sources.debian.net/src/hyphen/2.8.8-1/
- https://sources.debian.net/src/hyphen/2.8.8-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `icu=52.1-8+deb8u4`

Binary Packages:

- `libicu52:amd64=52.1-8+deb8u4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris icu=52.1-8+deb8u4
'http://deb.debian.org/debian/pool/main/i/icu/icu_52.1-8+deb8u4.dsc' icu_52.1-8+deb8u4.dsc 2015 SHA256:cabdf27f9976550a61f1b5c84d7353f19f3338b55b2b9002f0db593fccda86c7
'http://deb.debian.org/debian/pool/main/i/icu/icu_52.1.orig.tar.gz' icu_52.1.orig.tar.gz 23875368 SHA256:2f4d5e68d4698e87759dbdc1a586d053d96935787f79961d192c477b029d8092
'http://deb.debian.org/debian/pool/main/i/icu/icu_52.1-8+deb8u4.debian.tar.xz' icu_52.1-8+deb8u4.debian.tar.xz 35588 SHA256:cf298a04a576aaa8016d25ebe1387f6c923de1acea4411a27f9858bf1af72f5a
```

Likely also available for browsing at:

- https://sources.debian.net/src/icu/52.1-8+deb8u4/
- https://sources.debian.net/src/icu/52.1-8+deb8u4/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `inetutils=2:1.9.2.39.3a460-3`

Binary Packages:

- `inetutils-ping=2:1.9.2.39.3a460-3`

Licenses: (parsed from: `/usr/share/doc/inetutils-ping/copyright`)

- `BSD-3-clause`
- `GFDL-1.3`
- `GFDL-1.3+`
- `GPL-3`
- `GPL-3+`
- `MIT`
- `Wietse`

Source:

```console
$ apt-get source -qq --print-uris inetutils=2:1.9.2.39.3a460-3
'http://deb.debian.org/debian/pool/main/i/inetutils/inetutils_1.9.2.39.3a460-3.dsc' inetutils_1.9.2.39.3a460-3.dsc 2700 SHA256:021a37cd7a0f71452f02390ee449974892b88b07605ec73b1393138950c2783a
'http://deb.debian.org/debian/pool/main/i/inetutils/inetutils_1.9.2.39.3a460.orig.tar.xz' inetutils_1.9.2.39.3a460.orig.tar.xz 1337612 SHA256:b24c6ebe9c4a3ae10d421c4b59cc173fc72ea9cddf03386553c3740d247d0865
'http://deb.debian.org/debian/pool/main/i/inetutils/inetutils_1.9.2.39.3a460-3.debian.tar.xz' inetutils_1.9.2.39.3a460-3.debian.tar.xz 75536 SHA256:496fbacdb8b0aad5669a55ac04cbd0f7eefe03227e2fc9e140f4f676116e7ef6
```

Likely also available for browsing at:

- https://sources.debian.net/src/inetutils/2:1.9.2.39.3a460-3/
- https://sources.debian.net/src/inetutils/2:1.9.2.39.3a460-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `init-system-helpers=1.22`

Binary Packages:

- `init=1.22`

Licenses: (parsed from: `/usr/share/doc/init/copyright`)

- `BSD`
- `GPL`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.22
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.22.dsc' init-system-helpers_1.22.dsc 1880 SHA256:f2ba7e0e1804b56d9c2967ed60be92274619068d7d3894c2dc750f31dbb0ff25
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.22.tar.xz' init-system-helpers_1.22.tar.xz 30728 SHA256:4f64b9fd86f2c68a3996903e03d6024d73f637ff8a06f1bd4f73bedcf8154124
```

Likely also available for browsing at:

- https://sources.debian.net/src/init-system-helpers/1.22/
- https://sources.debian.net/src/init-system-helpers/1.22/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `insserv=1.14.0-5`

Binary Packages:

- `insserv=1.14.0-5`

Licenses: (parsed from: `/usr/share/doc/insserv/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris insserv=1.14.0-5
'http://deb.debian.org/debian/pool/main/i/insserv/insserv_1.14.0-5.dsc' insserv_1.14.0-5.dsc 1947 SHA256:183dbcd57db6061d61e781197231275fe49c321f6600ec147546d5c24a8ba021
'http://deb.debian.org/debian/pool/main/i/insserv/insserv_1.14.0.orig.tar.gz' insserv_1.14.0.orig.tar.gz 53851 SHA256:da74dcf5225a00aa8aef4d5afc6a20e009b2ed9af328dabd55fef1cb3a32140e
'http://deb.debian.org/debian/pool/main/i/insserv/insserv_1.14.0-5.debian.tar.gz' insserv_1.14.0-5.debian.tar.gz 53943 SHA256:496a3ece3cf4b53ff19f45eeffab6b5a7714785d1db524087c9cbe9cbdd88b2a
```

Likely also available for browsing at:

- https://sources.debian.net/src/insserv/1.14.0-5/
- https://sources.debian.net/src/insserv/1.14.0-5/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `iproute2=3.16.0-2`

Binary Packages:

- `iproute2=3.16.0-2`

Licenses: (parsed from: `/usr/share/doc/iproute2/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris iproute2=3.16.0-2
'http://deb.debian.org/debian/pool/main/i/iproute2/iproute2_3.16.0-2.dsc' iproute2_3.16.0-2.dsc 1693 SHA256:dd657e1707a85c7a15a3a2ba17e3e02fbf133aac4513ed86e4d8b1d6e4cd6a45
'http://deb.debian.org/debian/pool/main/i/iproute2/iproute2_3.16.0.orig.tar.xz' iproute2_3.16.0.orig.tar.xz 438820 SHA256:1f0a8a6c0e872166f75433f5cbf9766f3002b5c2f13501b3bb8c51846a127b79
'http://deb.debian.org/debian/pool/main/i/iproute2/iproute2_3.16.0-2.debian.tar.xz' iproute2_3.16.0-2.debian.tar.xz 27032 SHA256:9e5c631b4465ee258a2d61150f6a591f37d116b1b465b363f9e50d496e0359ab
```

Likely also available for browsing at:

- https://sources.debian.net/src/iproute2/3.16.0-2/
- https://sources.debian.net/src/iproute2/3.16.0-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `iso-codes=3.57-1`

Binary Packages:

- `iso-codes=3.57-1`

Licenses: (parsed from: `/usr/share/doc/iso-codes/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris iso-codes=3.57-1
'http://deb.debian.org/debian/pool/main/i/iso-codes/iso-codes_3.57-1.dsc' iso-codes_3.57-1.dsc 1957 SHA256:23c1dbba83de579c1b99f318eeac30e38ee0453106c751f7863a30c819ce0666
'http://deb.debian.org/debian/pool/main/i/iso-codes/iso-codes_3.57.orig.tar.xz' iso-codes_3.57.orig.tar.xz 3773756 SHA256:dd6acd92843b69530fce535d3d6fd947ddb3802f0d5fc1bd214d1cb7d2bf5c47
'http://deb.debian.org/debian/pool/main/i/iso-codes/iso-codes_3.57-1.debian.tar.xz' iso-codes_3.57-1.debian.tar.xz 23696 SHA256:d1a6f214b41bc05bde765aa17e0e2cc9d4166b717599a5771af9cf2119a10a59
```

Likely also available for browsing at:

- https://sources.debian.net/src/iso-codes/3.57-1/
- https://sources.debian.net/src/iso-codes/3.57-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `jasper=1.900.1-debian1-2.4+deb8u3`

Binary Packages:

- `libjasper1:amd64=1.900.1-debian1-2.4+deb8u3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris jasper=1.900.1-debian1-2.4+deb8u3
'http://security.debian.org/pool/updates/main/j/jasper/jasper_1.900.1-debian1-2.4+deb8u3.dsc' jasper_1.900.1-debian1-2.4+deb8u3.dsc 1969 SHA256:9c5228e9f5107ef3ce7565b93bdb00718412b8d15e6dad0328774df223a3c3b5
'http://security.debian.org/pool/updates/main/j/jasper/jasper_1.900.1-debian1.orig.tar.gz' jasper_1.900.1-debian1.orig.tar.gz 1140771 SHA256:7276e8407080d8263b39aeac8305032b0534c7df25bf02718b3944711e3c81d7
'http://security.debian.org/pool/updates/main/j/jasper/jasper_1.900.1-debian1-2.4+deb8u3.debian.tar.xz' jasper_1.900.1-debian1-2.4+deb8u3.debian.tar.xz 34032 SHA256:57b9d7b949a4a0696d6bdc93d56a7ee59d85f3c7cfa34e33a493b3fbf3d99bbf
```

Likely also available for browsing at:

- https://sources.debian.net/src/jasper/1.900.1-debian1-2.4+deb8u3/
- https://sources.debian.net/src/jasper/1.900.1-debian1-2.4+deb8u3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `java-common=0.52`

Binary Packages:

- `java-common=0.52`

Licenses: (parsed from: `/usr/share/doc/java-common/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris java-common=0.52
'http://deb.debian.org/debian/pool/main/j/java-common/java-common_0.52.dsc' java-common_0.52.dsc 2085 SHA256:348d6709b0d7ed5f4a944dc59f3cbf896f622b328d0c0bc4c2578980753b376d
'http://deb.debian.org/debian/pool/main/j/java-common/java-common_0.52.tar.xz' java-common_0.52.tar.xz 47380 SHA256:1118793faa2f41b9424c7014558713cdea0a401b3e2d904925fc20cf68464143
```

Likely also available for browsing at:

- https://sources.debian.net/src/java-common/0.52/
- https://sources.debian.net/src/java-common/0.52/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `jbigkit=2.1-3.1`

Binary Packages:

- `libjbig0:amd64=2.1-3.1`

Licenses: (parsed from: `/usr/share/doc/libjbig0/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris jbigkit=2.1-3.1
'http://deb.debian.org/debian/pool/main/j/jbigkit/jbigkit_2.1-3.1.dsc' jbigkit_2.1-3.1.dsc 1299 SHA256:62c8812d508958c5d35f2b1579dc3052fb5bd8d2e77d023fad064c4b48c8c3f8
'http://deb.debian.org/debian/pool/main/j/jbigkit/jbigkit_2.1.orig.tar.gz' jbigkit_2.1.orig.tar.gz 438710 SHA256:de7106b6bfaf495d6865c7dd7ac6ca1381bd12e0d81405ea81e7f2167263d932
'http://deb.debian.org/debian/pool/main/j/jbigkit/jbigkit_2.1-3.1.debian.tar.xz' jbigkit_2.1-3.1.debian.tar.xz 7600 SHA256:ebc3c52deaf37d52baea54d648a713640dc262926abda7bf05cd08e7db5dd1ee
```

Likely also available for browsing at:

- https://sources.debian.net/src/jbigkit/2.1-3.1/
- https://sources.debian.net/src/jbigkit/2.1-3.1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `keyutils=1.5.9-5`

Binary Packages:

- `libkeyutils1:amd64=1.5.9-5+b1`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.5.9-5
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.5.9-5.dsc' keyutils_1.5.9-5.dsc 2080 SHA256:8c8ca9ef9274046901b107f143260bd1255387939ee517ae842829bd167fd49d
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.5.9.orig.tar.bz2' keyutils_1.5.9.orig.tar.bz2 74683 SHA256:4da2c5552c688b65ab14d4fd40fbdf720c8b396d8ece643e040cf6e707e083ae
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.5.9-5.debian.tar.xz' keyutils_1.5.9-5.debian.tar.xz 14596 SHA256:8cef47fc1fd688cc54e36cbb7cee26f38b38d10a1c59af8d8dc0869a0e4359fc
```

Likely also available for browsing at:

- https://sources.debian.net/src/keyutils/1.5.9-5/
- https://sources.debian.net/src/keyutils/1.5.9-5/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `kmod=18-3`

Binary Packages:

- `libkmod2:amd64=18-3`

Licenses: (parsed from: `/usr/share/doc/libkmod2/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris kmod=18-3
'http://deb.debian.org/debian/pool/main/k/kmod/kmod_18-3.dsc' kmod_18-3.dsc 1865 SHA256:f16ef133e00db0fa360dcfb0d4723afc31e3803141b5f864e4df6a8b810eaeea
'http://deb.debian.org/debian/pool/main/k/kmod/kmod_18.orig.tar.gz' kmod_18.orig.tar.gz 3692996 SHA256:cdd7c8627e9bbfe5e39232886d08db2c87b4cc2ea7e9f8d3034577324809f2c0
'http://deb.debian.org/debian/pool/main/k/kmod/kmod_18-3.debian.tar.xz' kmod_18-3.debian.tar.xz 10468 SHA256:7a55a9d2c97913cdfde6e29d2784b5b82c7fdad6581d466b4aa571eef3270ea2
```

Likely also available for browsing at:

- https://sources.debian.net/src/kmod/18-3/
- https://sources.debian.net/src/kmod/18-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `krb5=1.12.1+dfsg-19+deb8u2`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.12.1+dfsg-19+deb8u2`
- `libk5crypto3:amd64=1.12.1+dfsg-19+deb8u2`
- `libkrb5-3:amd64=1.12.1+dfsg-19+deb8u2`
- `libkrb5support0:amd64=1.12.1+dfsg-19+deb8u2`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.12.1+dfsg-19+deb8u2
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.12.1+dfsg-19+deb8u2.dsc' krb5_1.12.1+dfsg-19+deb8u2.dsc 3368 SHA256:2b10ecb8b8c3015a12a764e4e6eb99fcca45cc1946d211a18db64b46dfa2cb81
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.12.1+dfsg.orig.tar.gz' krb5_1.12.1+dfsg.orig.tar.gz 11792370 SHA256:eb29959f1e9f8d71e7401f5809daefae067296eb5b0da1176366280a16bdd784
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.12.1+dfsg-19+deb8u2.debian.tar.xz' krb5_1.12.1+dfsg-19+deb8u2.debian.tar.xz 123456 SHA256:242155b4ac6add762c1bac60e6eaa73b25abd985fb41bcdd13d4eae022f592ec
```

Likely also available for browsing at:

- https://sources.debian.net/src/krb5/1.12.1+dfsg-19+deb8u2/
- https://sources.debian.net/src/krb5/1.12.1+dfsg-19+deb8u2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `lapack=3.5.0-4`

Binary Packages:

- `liblapack3=3.5.0-4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris lapack=3.5.0-4
'http://deb.debian.org/debian/pool/main/l/lapack/lapack_3.5.0-4.dsc' lapack_3.5.0-4.dsc 2540 SHA256:2b5946f4476e901c6fb0429b3d8d057c8ddb90fbe860cff6f1a273c1373af5c9
'http://deb.debian.org/debian/pool/main/l/lapack/lapack_3.5.0.orig.tar.xz' lapack_3.5.0.orig.tar.xz 2112856 SHA256:c4dddb0f924c16c7a366462848ccee3ecc4c3e422645772bbce2e3df25ae1ffb
'http://deb.debian.org/debian/pool/main/l/lapack/lapack_3.5.0-4.debian.tar.xz' lapack_3.5.0-4.debian.tar.xz 18144 SHA256:d09b4f31467ae356ccb84df2119368fe484eda149406f163e60ae3b282eadd0e
```

Likely also available for browsing at:

- https://sources.debian.net/src/lapack/3.5.0-4/
- https://sources.debian.net/src/lapack/3.5.0-4/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `lcms2=2.6-3+deb8u1`

Binary Packages:

- `liblcms2-2:amd64=2.6-3+deb8u1`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`)

- `GPL-2`
- `GPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris lcms2=2.6-3+deb8u1
'http://security.debian.org/pool/updates/main/l/lcms2/lcms2_2.6-3+deb8u1.dsc' lcms2_2.6-3+deb8u1.dsc 2287 SHA256:c81475db156883e857dd6c456e8a22e6554c6fb0f8e47622915a76d716d1ee5e
'http://security.debian.org/pool/updates/main/l/lcms2/lcms2_2.6.orig.tar.gz' lcms2_2.6.orig.tar.gz 4583389 SHA256:5172528839647c54c3da211837225e221be93e4733f5b5e9f57668f7107e14b1
'http://security.debian.org/pool/updates/main/l/lcms2/lcms2_2.6-3+deb8u1.debian.tar.xz' lcms2_2.6-3+deb8u1.debian.tar.xz 2416964 SHA256:81fcf1658e51d55408143e91b1c3469a63f3b4607e92604bd8a18dd8d6435d05
```

Likely also available for browsing at:

- https://sources.debian.net/src/lcms2/2.6-3+deb8u1/
- https://sources.debian.net/src/lcms2/2.6-3+deb8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libabw=0.1.0-2`

Binary Packages:

- `libabw-0.1-1=0.1.0-2`

Licenses: (parsed from: `/usr/share/doc/libabw-0.1-1/copyright`)

- `GPL-3`
- `LGPL-3`
- `MPL-1.1 | GPL-3 | LGPL-3`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libabw=0.1.0-2
'http://deb.debian.org/debian/pool/main/liba/libabw/libabw_0.1.0-2.dsc' libabw_0.1.0-2.dsc 1874 SHA256:c3e26ac473028a00c497129e49d2db29411ffb3b335c12adfc4cfc1482d341f4
'http://deb.debian.org/debian/pool/main/liba/libabw/libabw_0.1.0.orig.tar.bz2' libabw_0.1.0.orig.tar.bz2 362087 SHA256:49380c24e04e8d2a4824adc9b1b8f5026ad759bc335497e05f0983412821f8d9
'http://deb.debian.org/debian/pool/main/liba/libabw/libabw_0.1.0-2.debian.tar.xz' libabw_0.1.0-2.debian.tar.xz 12704 SHA256:0cdf2a2ef4dfa904983e785c1b83dacc8d24303b9fc8fe7e071404982d4cd907
```

Likely also available for browsing at:

- https://sources.debian.net/src/libabw/0.1.0-2/
- https://sources.debian.net/src/libabw/0.1.0-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libcap-ng=0.7.4-2`

Binary Packages:

- `libcap-ng0:amd64=0.7.4-2`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.7.4-2
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.7.4-2.dsc' libcap-ng_0.7.4-2.dsc 1622 SHA256:96c4637dbbbe9c51fad1b3c2234ab07fdb7dbebd3e01cb5044acf43c7ba82867
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.7.4.orig.tar.gz' libcap-ng_0.7.4.orig.tar.gz 407007 SHA256:48a2083276f9820cb92dcb05d001b30733bcbf48c14c230303cac3cd08b45b6b
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.7.4-2.debian.tar.xz' libcap-ng_0.7.4-2.debian.tar.xz 5000 SHA256:ae7dfe1d7828eef82879ebfc81f636de73e1130c8675f9c5059a40808a0825cd
```

Likely also available for browsing at:

- https://sources.debian.net/src/libcap-ng/0.7.4-2/
- https://sources.debian.net/src/libcap-ng/0.7.4-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libcap2=1:2.24-8`

Binary Packages:

- `libcap2:amd64=1:2.24-8`
- `libcap2-bin=1:2.24-8`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`, `/usr/share/doc/libcap2-bin/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.24-8
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.24-8.dsc' libcap2_2.24-8.dsc 2134 SHA256:b042a6c89079d02113bd15ec52948f265edb6c725830d1b79434af06c4e6006a
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.24.orig.tar.xz' libcap2_2.24.orig.tar.xz 63264 SHA256:51cd1c568a2baf1e687573bd6117a94b07f33b46a05acaa50ee208792a830b79
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.24-8.debian.tar.xz' libcap2_2.24-8.debian.tar.xz 17528 SHA256:d1dd71eb19ce4cb7ea37f827c155382773e7724d5356619539874dca647aa94e
```

Likely also available for browsing at:

- https://sources.debian.net/src/libcap2/1:2.24-8/
- https://sources.debian.net/src/libcap2/1:2.24-8/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libcdr=0.1.0-3`

Binary Packages:

- `libcdr-0.1-1=0.1.0-3`

Licenses: (parsed from: `/usr/share/doc/libcdr-0.1-1/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libcdr=0.1.0-3
'http://deb.debian.org/debian/pool/main/libc/libcdr/libcdr_0.1.0-3.dsc' libcdr_0.1.0-3.dsc 1996 SHA256:47748846ab0ce7bc6e2bb558022534b6ce111dc932561e93191f8381422b87b2
'http://deb.debian.org/debian/pool/main/libc/libcdr/libcdr_0.1.0.orig.tar.bz2' libcdr_0.1.0.orig.tar.bz2 659119 SHA256:ef6c180db88e7024f91a949dd41aeafde0e074008c259ba4c1f8c3eefda48fd0
'http://deb.debian.org/debian/pool/main/libc/libcdr/libcdr_0.1.0-3.debian.tar.xz' libcdr_0.1.0-3.debian.tar.xz 7272 SHA256:1dfba6dc72709a983a23bf127f3cb6e1bf40eff5b95b0c8bb9f29f6e5dadec3b
```

Likely also available for browsing at:

- https://sources.debian.net/src/libcdr/0.1.0-3/
- https://sources.debian.net/src/libcdr/0.1.0-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libcmis=0.4.1-7`

Binary Packages:

- `libcmis-0.4-4=0.4.1-7`

Licenses: (parsed from: `/usr/share/doc/libcmis-0.4-4/copyright`)

- `GPL`
- `LGPL`
- `MPL | GPL2+ | LGPL2+`

Source:

```console
$ apt-get source -qq --print-uris libcmis=0.4.1-7
'http://deb.debian.org/debian/pool/main/libc/libcmis/libcmis_0.4.1-7.dsc' libcmis_0.4.1-7.dsc 2023 SHA256:11046e849dc4f8e03ec8c84e6edb361338c4b677d7b32b32c581bf92bdac574c
'http://deb.debian.org/debian/pool/main/libc/libcmis/libcmis_0.4.1.orig.tar.gz' libcmis_0.4.1.orig.tar.gz 637615 SHA256:7d52dcf2b5832d3663b18fbf40f0bdefb1e1a40cfb3cf01903301b0bf629395f
'http://deb.debian.org/debian/pool/main/libc/libcmis/libcmis_0.4.1-7.debian.tar.xz' libcmis_0.4.1-7.debian.tar.xz 3584 SHA256:5a85e0d13f7942180c7c2dfdb0dc43e70a1af96c3bc6cf57174bb46888c514f7
```

Likely also available for browsing at:

- https://sources.debian.net/src/libcmis/0.4.1-7/
- https://sources.debian.net/src/libcmis/0.4.1-7/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libdatrie=0.2.8-1`

Binary Packages:

- `libdatrie1:amd64=0.2.8-1`

Licenses: (parsed from: `/usr/share/doc/libdatrie1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libdatrie=0.2.8-1
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.8-1.dsc' libdatrie_0.2.8-1.dsc 2082 SHA256:4cea8f61d67778ae16fa24eb28c413b5c3cc3203f84a50ba0944956a9bba05a2
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.8.orig.tar.xz' libdatrie_0.2.8.orig.tar.xz 286428 SHA256:6a14d55c5687fc325216fffb5db0cf55d31b108cce65314a6d5c8042417ab7c2
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.8-1.debian.tar.gz' libdatrie_0.2.8-1.debian.tar.gz 7651 SHA256:7563b262c917cb507d17b35437a484c54c2964cff9994ffbbac1f78fb5f3c59b
```

Likely also available for browsing at:

- https://sources.debian.net/src/libdatrie/0.2.8-1/
- https://sources.debian.net/src/libdatrie/0.2.8-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libdrm=2.4.58-2`

Binary Packages:

- `libdrm2:amd64=2.4.58-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libdrm=2.4.58-2
'http://deb.debian.org/debian/pool/main/libd/libdrm/libdrm_2.4.58-2.dsc' libdrm_2.4.58-2.dsc 3002 SHA256:1286092e26403ea459a77df792fabfcad35ae68c05313d60362947d8eaa04c72
'http://deb.debian.org/debian/pool/main/libd/libdrm/libdrm_2.4.58.orig.tar.gz' libdrm_2.4.58.orig.tar.gz 732395 SHA256:e6f6901b0dd431d4e21f6e81ae5a5aef65885ed5f066e8d9751ca69ba9a71186
'http://deb.debian.org/debian/pool/main/libd/libdrm/libdrm_2.4.58-2.diff.gz' libdrm_2.4.58-2.diff.gz 18700 SHA256:51f9a553461a26cd3757c05e792187c3fdec4744cefda6ce1e103f201ef7c0f0
```

Likely also available for browsing at:

- https://sources.debian.net/src/libdrm/2.4.58-2/
- https://sources.debian.net/src/libdrm/2.4.58-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libe-book=0.1.1-2`

Binary Packages:

- `libe-book-0.1-1=0.1.1-2`

Licenses: (parsed from: `/usr/share/doc/libe-book-0.1-1/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libe-book=0.1.1-2
'http://deb.debian.org/debian/pool/main/libe/libe-book/libe-book_0.1.1-2.dsc' libe-book_0.1.1-2.dsc 1949 SHA256:0eb91ddc36df5b60f99bc40516ec721dfed62bd6b3c145a46d8ad854288c3198
'http://deb.debian.org/debian/pool/main/libe/libe-book/libe-book_0.1.1.orig.tar.bz2' libe-book_0.1.1.orig.tar.bz2 466712 SHA256:90353fc60827a33b391d0b63ecfe5239229d489af99ff6ea014ede3b39fa32b5
'http://deb.debian.org/debian/pool/main/libe/libe-book/libe-book_0.1.1-2.debian.tar.xz' libe-book_0.1.1-2.debian.tar.xz 6784 SHA256:1f289e180826e408ddc27d6629287d384b17763c169de9b0f0ad5ac5b50b63c9
```

Likely also available for browsing at:

- https://sources.debian.net/src/libe-book/0.1.1-2/
- https://sources.debian.net/src/libe-book/0.1.1-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libeot=0.01-3`

Binary Packages:

- `libeot0=0.01-3`

Licenses: (parsed from: `/usr/share/doc/libeot0/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libeot=0.01-3
'http://deb.debian.org/debian/pool/main/libe/libeot/libeot_0.01-3.dsc' libeot_0.01-3.dsc 1761 SHA256:b8be662796b39954c34d306b5c075b74bd4deafee319ec83448784390fd8c323
'http://deb.debian.org/debian/pool/main/libe/libeot/libeot_0.01.orig.tar.bz2' libeot_0.01.orig.tar.bz2 260288 SHA256:cf5091fa8e7dcdbe667335eb90a2cfdd0a3fe8f8c7c8d1ece44d9d055736a06a
'http://deb.debian.org/debian/pool/main/libe/libeot/libeot_0.01-3.debian.tar.xz' libeot_0.01-3.debian.tar.xz 7312 SHA256:fe70b71d9e4b1cb33533bdcdfd5dce42d6039d7d90f2b202a5738fc2de05c78a
```

Likely also available for browsing at:

- https://sources.debian.net/src/libeot/0.01-3/
- https://sources.debian.net/src/libeot/0.01-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libetonyek=0.1.1-2`

Binary Packages:

- `libetonyek-0.1-1=0.1.1-2`

Licenses: (parsed from: `/usr/share/doc/libetonyek-0.1-1/copyright`)

- `MPL 2.0`

Source:

```console
$ apt-get source -qq --print-uris libetonyek=0.1.1-2
'http://deb.debian.org/debian/pool/main/libe/libetonyek/libetonyek_0.1.1-2.dsc' libetonyek_0.1.1-2.dsc 1949 SHA256:593092208d7b829d58ca25f485f0e4d125df8f28c8ff89e0802d65af5500c621
'http://deb.debian.org/debian/pool/main/libe/libetonyek/libetonyek_0.1.1.orig.tar.bz2' libetonyek_0.1.1.orig.tar.bz2 423556 SHA256:716edf726ba3896fe85eea9a75786948d5ddeda63a54c00f3308658cc3bbd9e4
'http://deb.debian.org/debian/pool/main/libe/libetonyek/libetonyek_0.1.1-2.debian.tar.xz' libetonyek_0.1.1-2.debian.tar.xz 6700 SHA256:839c6551b3c571c03befbb02adf84453f20fe18be164ec818c7b1586bdbec8f8
```

Likely also available for browsing at:

- https://sources.debian.net/src/libetonyek/0.1.1-2/
- https://sources.debian.net/src/libetonyek/0.1.1-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libexttextcat=3.4.4-1`

Binary Packages:

- `libexttextcat-2.0-0=3.4.4-1`
- `libexttextcat-data=3.4.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libexttextcat=3.4.4-1
'http://deb.debian.org/debian/pool/main/libe/libexttextcat/libexttextcat_3.4.4-1.dsc' libexttextcat_3.4.4-1.dsc 1988 SHA256:533c370a2402a775bfa1c0bcbacc868f3f27c63c7292addb319f3754baac912b
'http://deb.debian.org/debian/pool/main/libe/libexttextcat/libexttextcat_3.4.4.orig.tar.bz2' libexttextcat_3.4.4.orig.tar.bz2 1129140 SHA256:9595601c41051356d03d0a7d5dcad334fe1b420d221f6885d143c14bb8d62163
'http://deb.debian.org/debian/pool/main/libe/libexttextcat/libexttextcat_3.4.4-1.debian.tar.xz' libexttextcat_3.4.4-1.debian.tar.xz 6952 SHA256:3b0a213d9fc62258daa213063890e9313fd3732d3e18b161fbc4e5d362b9d1e7
```

Likely also available for browsing at:

- https://sources.debian.net/src/libexttextcat/3.4.4-1/
- https://sources.debian.net/src/libexttextcat/3.4.4-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libffi=3.1-2`

Binary Packages:

- `libffi6:amd64=3.1-2+b2`

Licenses: (parsed from: `/usr/share/doc/libffi6/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.1-2
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.1-2.dsc' libffi_3.1-2.dsc 1358 SHA256:6249efd7d44527de06e9e1fba9c7695c069d93b0fa5149f604435792c5a30f6c
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.1.orig.tar.gz' libffi_3.1.orig.tar.gz 937214 SHA256:97feeeadca5e21870fa4433bc953d1b3af3f698d5df8a428f68b73cd60aef6eb
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.1-2.debian.tar.xz' libffi_3.1-2.debian.tar.xz 8408 SHA256:7e7826c1ee6152d31a3e341efc34df923ec903b6caecc2701694dc95f2efd3ab
```

Likely also available for browsing at:

- https://sources.debian.net/src/libffi/3.1-2/
- https://sources.debian.net/src/libffi/3.1-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libfreehand=0.1.0-2`

Binary Packages:

- `libfreehand-0.1-1=0.1.0-2`

Licenses: (parsed from: `/usr/share/doc/libfreehand-0.1-1/copyright`)

- `GPL-3`
- `LGPL-3`
- `MPL-1.1 | GPL-3+ | LGPL-3+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libfreehand=0.1.0-2
'http://deb.debian.org/debian/pool/main/libf/libfreehand/libfreehand_0.1.0-2.dsc' libfreehand_0.1.0-2.dsc 1921 SHA256:425f7ce424f3026f8b3bb69deacbdbc2ba976f550341bdaed399c1cbeb0afb16
'http://deb.debian.org/debian/pool/main/libf/libfreehand/libfreehand_0.1.0.orig.tar.bz2' libfreehand_0.1.0.orig.tar.bz2 340549 SHA256:c69962d5947561afeefeee71bc78ba7419e9d9b0fea8bcef2f625be867afe307
'http://deb.debian.org/debian/pool/main/libf/libfreehand/libfreehand_0.1.0-2.debian.tar.xz' libfreehand_0.1.0-2.debian.tar.xz 12800 SHA256:94ae41475dc40d7d4e1a54fcc2de7ded6f8d71a07bee7f2e5fea0f45a80850ad
```

Likely also available for browsing at:

- https://sources.debian.net/src/libfreehand/0.1.0-2/
- https://sources.debian.net/src/libfreehand/0.1.0-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libgcrypt20=1.6.3-2+deb8u2`

Binary Packages:

- `libgcrypt20:amd64=1.6.3-2+deb8u2`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.6.3-2+deb8u2
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.6.3-2+deb8u2.dsc' libgcrypt20_1.6.3-2+deb8u2.dsc 2583 SHA256:982179928629a477dad47b667ac64708eb791f77241807cafbee2b730c94654d
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.6.3.orig.tar.bz2' libgcrypt20_1.6.3.orig.tar.bz2 2494052 SHA256:41b4917b93ae34c6a0e2127378d7a4d66d805a2a86a09911d4f9bd871db7025f
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.6.3-2+deb8u2.debian.tar.xz' libgcrypt20_1.6.3-2+deb8u2.debian.tar.xz 30964 SHA256:49cea0b68a4eb67461909088ffa190bcb13296dfe2da4821f7968dd992ed97a6
```

Likely also available for browsing at:

- https://sources.debian.net/src/libgcrypt20/1.6.3-2+deb8u2/
- https://sources.debian.net/src/libgcrypt20/1.6.3-2+deb8u2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libgltf=0.0.2-2`

Binary Packages:

- `libgltf-0.0-0=0.0.2-2`

Licenses: (parsed from: `/usr/share/doc/libgltf-0.0-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libgltf=0.0.2-2
'http://deb.debian.org/debian/pool/main/libg/libgltf/libgltf_0.0.2-2.dsc' libgltf_0.0.2-2.dsc 1773 SHA256:65eeec25a72fed3a470e50ee07ccb71f6ea54e09f229d88ec964bb9b411c6afe
'http://deb.debian.org/debian/pool/main/libg/libgltf/libgltf_0.0.2.orig.tar.bz2' libgltf_0.0.2.orig.tar.bz2 538040 SHA256:d1cc7297ed1921aa969e26413b4c4e18afc882ce4d2f5a2aa2a2905706f7206b
'http://deb.debian.org/debian/pool/main/libg/libgltf/libgltf_0.0.2-2.debian.tar.xz' libgltf_0.0.2-2.debian.tar.xz 8516 SHA256:e186e8f3360a41cfe0eb1035616b72453c05bd5ba82d4d0d1c6299db191d1ee6
```

Likely also available for browsing at:

- https://sources.debian.net/src/libgltf/0.0.2-2/
- https://sources.debian.net/src/libgltf/0.0.2-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libglu=9.0.0-2`

Binary Packages:

- `libglu1-mesa:amd64=9.0.0-2`

Licenses: (parsed from: `/usr/share/doc/libglu1-mesa/copyright`)

- `GPL-2`
- `LGPL-2`
- `SGI-1.1`
- `SGI-2`

Source:

```console
$ apt-get source -qq --print-uris libglu=9.0.0-2
'http://deb.debian.org/debian/pool/main/libg/libglu/libglu_9.0.0-2.dsc' libglu_9.0.0-2.dsc 1269 SHA256:8e48765b33a1769794017a77307c08bcca4712007307c3df08a660dea4de7a09
'http://deb.debian.org/debian/pool/main/libg/libglu/libglu_9.0.0.orig.tar.gz' libglu_9.0.0.orig.tar.gz 626786 SHA256:4387476a1933f36fec1531178ea204057bbeb04cc2d8396c9ea32720a1f7e264
'http://deb.debian.org/debian/pool/main/libg/libglu/libglu_9.0.0-2.diff.gz' libglu_9.0.0-2.diff.gz 14472 SHA256:85fce52d91b7429e8604eda58be13ff9f27706f0fdecd7fc584295f3a2f4e2a8
```

Likely also available for browsing at:

- https://sources.debian.net/src/libglu/9.0.0-2/
- https://sources.debian.net/src/libglu/9.0.0-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libgpg-error=1.17-3`

Binary Packages:

- `libgpg-error0:amd64=1.17-3`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `GPL-2.1+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.17-3
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.17-3.dsc' libgpg-error_1.17-3.dsc 2344 SHA256:42d9ff8517b1149b453d947b515cef088b83ac6a6b4fdcbd143570c42e2216c9
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.17.orig.tar.bz2' libgpg-error_1.17.orig.tar.bz2 669914 SHA256:3ff4e5a71116eb862cd14185fcd282850927b8608e3b4186834fd940fbef57b5
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.17-3.debian.tar.xz' libgpg-error_1.17-3.debian.tar.xz 38460 SHA256:3e0af89c65e61ed2b53555eaecd5dc7fa19519490ef447313f441728ae490f29
```

Likely also available for browsing at:

- https://sources.debian.net/src/libgpg-error/1.17-3/
- https://sources.debian.net/src/libgpg-error/1.17-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libice=2:1.0.9-1`

Binary Packages:

- `libice6:amd64=2:1.0.9-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libice=2:1.0.9-1
'http://deb.debian.org/debian/pool/main/libi/libice/libice_1.0.9-1.dsc' libice_1.0.9-1.dsc 2140 SHA256:f90a79944f147b5db208677d92381fd0886c201616172bac0b28ef0e85912ebd
'http://deb.debian.org/debian/pool/main/libi/libice/libice_1.0.9.orig.tar.gz' libice_1.0.9.orig.tar.gz 455871 SHA256:7812a824a66dd654c830d21982749b3b563d9c2dfe0b88b203cefc14a891edc0
'http://deb.debian.org/debian/pool/main/libi/libice/libice_1.0.9-1.diff.gz' libice_1.0.9-1.diff.gz 6260 SHA256:85d68a69d5e6b25b352eb98c6c33fa7a324da8dd913d7e84a049852fb87287e7
```

Likely also available for browsing at:

- https://sources.debian.net/src/libice/2:1.0.9-1/
- https://sources.debian.net/src/libice/2:1.0.9-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libidn=1.29-1+deb8u2`

Binary Packages:

- `libidn11:amd64=1.29-1+deb8u2`

Licenses: (parsed from: `/usr/share/doc/libidn11/copyright`)

- `GAP`
- `GFDL-1.3`
- `GFDL-1.3+`
- `GPL-2`
- `GPL-3`
- `GPL-3+`
- `LGPL-2`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+ | GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libidn=1.29-1+deb8u2
'http://deb.debian.org/debian/pool/main/libi/libidn/libidn_1.29-1+deb8u2.dsc' libidn_1.29-1+deb8u2.dsc 2177 SHA256:8346d3ad4ea48159c1008a7482685c7abfb0e3bcdc4bbda937b6a1774df1798f
'http://deb.debian.org/debian/pool/main/libi/libidn/libidn_1.29.orig.tar.gz' libidn_1.29.orig.tar.gz 3474087 SHA256:fb82747dbbf9b36f703ed27293317d818d7e851d4f5773dedf3efa4db32a7c7c
'http://deb.debian.org/debian/pool/main/libi/libidn/libidn_1.29-1+deb8u2.debian.tar.xz' libidn_1.29-1+deb8u2.debian.tar.xz 70728 SHA256:5f3be629b7185609bb2aed149f568a014524f69dec1368a4455a4eb0972a61d9
```

Likely also available for browsing at:

- https://sources.debian.net/src/libidn/1.29-1+deb8u2/
- https://sources.debian.net/src/libidn/1.29-1+deb8u2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libjpeg-turbo=1:1.3.1-12`

Binary Packages:

- `libjpeg62-turbo:amd64=1:1.3.1-12`

Licenses: (parsed from: `/usr/share/doc/libjpeg62-turbo/copyright`)

- `BSD-3`
- `BSD-BY-LC-NE`
- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=1:1.3.1-12
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.3.1-12.dsc' libjpeg-turbo_1.3.1-12.dsc 2650 SHA256:1606a068d653c40da819e0ac4f9c560cf891d665ad5299c0eb994168830ce95d
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.3.1.orig.tar.gz' libjpeg-turbo_1.3.1.orig.tar.gz 1390282 SHA256:c132907417ddc40ed552fe53d6b91d5fecbb14a356a60ddc7ea50d6be9666fb9
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.3.1-12.debian.tar.xz' libjpeg-turbo_1.3.1-12.debian.tar.xz 78596 SHA256:046f88108246665a433cc60b0e9cec6c243b0163899c039542dbfb183fef6e71
```

Likely also available for browsing at:

- https://sources.debian.net/src/libjpeg-turbo/1:1.3.1-12/
- https://sources.debian.net/src/libjpeg-turbo/1:1.3.1-12/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `liblangtag=0.5.1-3`

Binary Packages:

- `liblangtag-common=0.5.1-3`
- `liblangtag1=0.5.1-3`

Licenses: (parsed from: `/usr/share/doc/liblangtag-common/copyright`, `/usr/share/doc/liblangtag1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL | MPL`

Source:

```console
$ apt-get source -qq --print-uris liblangtag=0.5.1-3
'http://deb.debian.org/debian/pool/main/libl/liblangtag/liblangtag_0.5.1-3.dsc' liblangtag_0.5.1-3.dsc 2292 SHA256:09e74884d3ec2f42fa270ab2529369968ec865d8475476dd9905ea2cfa4bc330
'http://deb.debian.org/debian/pool/main/libl/liblangtag/liblangtag_0.5.1.orig.tar.bz2' liblangtag_0.5.1.orig.tar.bz2 651785 SHA256:c3dd456762cd0b5fd1687f066c4bdf253d70b14729851b9cd05936a1cb46923b
'http://deb.debian.org/debian/pool/main/libl/liblangtag/liblangtag_0.5.1-3.debian.tar.xz' liblangtag_0.5.1-3.debian.tar.xz 5648 SHA256:eaaa138aa8d4de328bed2f3b96bcfecd14abbff784f75a561089a458812905b0
```

Likely also available for browsing at:

- https://sources.debian.net/src/liblangtag/0.5.1-3/
- https://sources.debian.net/src/liblangtag/0.5.1-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `liblocale-gettext-perl=1.05-8`

Binary Packages:

- `liblocale-gettext-perl=1.05-8+b1`

Licenses: (parsed from: `/usr/share/doc/liblocale-gettext-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris liblocale-gettext-perl=1.05-8
'http://deb.debian.org/debian/pool/main/libl/liblocale-gettext-perl/liblocale-gettext-perl_1.05-8.dsc' liblocale-gettext-perl_1.05-8.dsc 2114 SHA256:0549ab2b517c1aed9fb12e2fee3ee2eded5efa80758491089f531b3ca10cc4ab
'http://deb.debian.org/debian/pool/main/libl/liblocale-gettext-perl/liblocale-gettext-perl_1.05.orig.tar.gz' liblocale-gettext-perl_1.05.orig.tar.gz 7693 SHA256:27367f3dc1be79c9ed178732756e37e4cfce45f9e2a27ebf26e1f40d80124694
'http://deb.debian.org/debian/pool/main/libl/liblocale-gettext-perl/liblocale-gettext-perl_1.05-8.debian.tar.xz' liblocale-gettext-perl_1.05-8.debian.tar.xz 5472 SHA256:2bd28828012a6289052e1905779f0505d2e09f279d77a79611990ad8d2f27ba1
```

Likely also available for browsing at:

- https://sources.debian.net/src/liblocale-gettext-perl/1.05-8/
- https://sources.debian.net/src/liblocale-gettext-perl/1.05-8/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libmspub=0.1.1-2`

Binary Packages:

- `libmspub-0.1-1=0.1.1-2`

Licenses: (parsed from: `/usr/share/doc/libmspub-0.1-1/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libmspub=0.1.1-2
'http://deb.debian.org/debian/pool/main/libm/libmspub/libmspub_0.1.1-2.dsc' libmspub_0.1.1-2.dsc 2029 SHA256:6e1be6f4725cab1effaae522819f793a8ff572a38e51f2ab46989bbe0ffa112f
'http://deb.debian.org/debian/pool/main/libm/libmspub/libmspub_0.1.1.orig.tar.bz2' libmspub_0.1.1.orig.tar.bz2 419812 SHA256:c3b69a4cf50ad80af5c9c00cb8ebca0586fc9ba9d6bdeeb40112d6f43ecdbbbb
'http://deb.debian.org/debian/pool/main/libm/libmspub/libmspub_0.1.1-2.debian.tar.xz' libmspub_0.1.1-2.debian.tar.xz 6912 SHA256:f48247510ed3a7d83bf49a31115e42fe292693ef311bd01f1ccae0f089e0949c
```

Likely also available for browsing at:

- https://sources.debian.net/src/libmspub/0.1.1-2/
- https://sources.debian.net/src/libmspub/0.1.1-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libmwaw=0.3.1-2`

Binary Packages:

- `libmwaw-0.3-3=0.3.1-2`

Licenses: (parsed from: `/usr/share/doc/libmwaw-0.3-3/copyright`)

- `BSD`
- `LGPL`
- `MPL2.0 | LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libmwaw=0.3.1-2
'http://deb.debian.org/debian/pool/main/libm/libmwaw/libmwaw_0.3.1-2.dsc' libmwaw_0.3.1-2.dsc 1969 SHA256:95b9ffb005438ae11cee5f610bf2c5816d2db0fb8e7a9d9c3866b13fa5d99789
'http://deb.debian.org/debian/pool/main/libm/libmwaw/libmwaw_0.3.1.orig.tar.bz2' libmwaw_0.3.1.orig.tar.bz2 1147351 SHA256:66d3dbc4421daa628326204b5d14bb99f2b9d4423184027aabe207d677c89845
'http://deb.debian.org/debian/pool/main/libm/libmwaw/libmwaw_0.3.1-2.debian.tar.xz' libmwaw_0.3.1-2.debian.tar.xz 7576 SHA256:dbab76cdff54c36b9ed6ba3d0fe3e81dea0518c3e477da736817404fe1b924ac
```

Likely also available for browsing at:

- https://sources.debian.net/src/libmwaw/0.3.1-2/
- https://sources.debian.net/src/libmwaw/0.3.1-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libodfgen=0.1.1-2`

Binary Packages:

- `libodfgen-0.1-1=0.1.1-2`

Licenses: (parsed from: `/usr/share/doc/libodfgen-0.1-1/copyright`)

- `LGPL`
- `MPL-2.0 | LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libodfgen=0.1.1-2
'http://deb.debian.org/debian/pool/main/libo/libodfgen/libodfgen_0.1.1-2.dsc' libodfgen_0.1.1-2.dsc 1860 SHA256:db3d34a237b3bca4e6a95257edae8af8a0c2e1d88351dc29facd6f9ce1339573
'http://deb.debian.org/debian/pool/main/libo/libodfgen/libodfgen_0.1.1.orig.tar.bz2' libodfgen_0.1.1.orig.tar.bz2 388955 SHA256:b8d5974de49b523c7a5b800d9817ff7ced9615ef456ba39128e2eb5a470483be
'http://deb.debian.org/debian/pool/main/libo/libodfgen/libodfgen_0.1.1-2.debian.tar.xz' libodfgen_0.1.1-2.debian.tar.xz 6728 SHA256:16a3d7656e84e31d9213bb4780cdd1ef6cfc37df7e01ca319e3e2e0f501a699a
```

Likely also available for browsing at:

- https://sources.debian.net/src/libodfgen/0.1.1-2/
- https://sources.debian.net/src/libodfgen/0.1.1-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `liborcus=0.7.0+dfsg-9`

Binary Packages:

- `liborcus-0.8-0=0.7.0+dfsg-9`

Licenses: (parsed from: `/usr/share/doc/liborcus-0.8-0/copyright`)

- `BSD`
- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris liborcus=0.7.0+dfsg-9
'http://deb.debian.org/debian/pool/main/libo/liborcus/liborcus_0.7.0+dfsg-9.dsc' liborcus_0.7.0+dfsg-9.dsc 2098 SHA256:faccb566d7d2390d3d8f3c74f294b5537916d0132fffd00000533e5c1c3eb30c
'http://deb.debian.org/debian/pool/main/libo/liborcus/liborcus_0.7.0+dfsg.orig.tar.bz2' liborcus_0.7.0+dfsg.orig.tar.bz2 1379076 SHA256:a8a1da8d5f5d19bc03acec6139f316575ef371129b4f8aa5de257a7cea28b00a
'http://deb.debian.org/debian/pool/main/libo/liborcus/liborcus_0.7.0+dfsg-9.debian.tar.xz' liborcus_0.7.0+dfsg-9.debian.tar.xz 9296 SHA256:be50205ad1a463602d779d552f472313040b613adea4ee048011878591cea8d2
```

Likely also available for browsing at:

- https://sources.debian.net/src/liborcus/0.7.0+dfsg-9/
- https://sources.debian.net/src/liborcus/0.7.0+dfsg-9/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libpng=1.2.50-2+deb8u3`

Binary Packages:

- `libpng12-0:amd64=1.2.50-2+deb8u3`

Licenses: (parsed from: `/usr/share/doc/libpng12-0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libpng=1.2.50-2+deb8u3
'http://deb.debian.org/debian/pool/main/libp/libpng/libpng_1.2.50-2+deb8u3.dsc' libpng_1.2.50-2+deb8u3.dsc 2036 SHA256:0db1eafb75ca276bc5b3e69810149ab53cc7344effa67e94269cde0c162fc720
'http://deb.debian.org/debian/pool/main/libp/libpng/libpng_1.2.50.orig.tar.xz' libpng_1.2.50.orig.tar.xz 539152 SHA256:4724f81f8c92ac7f360ad1fbf173396ea7c535923424db9fbaff07bfd9d8e8e7
'http://deb.debian.org/debian/pool/main/libp/libpng/libpng_1.2.50-2+deb8u3.debian.tar.xz' libpng_1.2.50-2+deb8u3.debian.tar.xz 21788 SHA256:b47238628a87fac02640b05bb4af5ada003c5180958a143ef670780ad4208cd7
```

Likely also available for browsing at:

- https://sources.debian.net/src/libpng/1.2.50-2+deb8u3/
- https://sources.debian.net/src/libpng/1.2.50-2+deb8u3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libpsl=0.5.1-1`

Binary Packages:

- `libpsl0:amd64=0.5.1-1`

Licenses: (parsed from: `/usr/share/doc/libpsl0/copyright`)

- `CC0`
- `MIT`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.5.1-1
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.5.1-1.dsc' libpsl_0.5.1-1.dsc 2201 SHA256:bf97e1fca2374470955b08c654877d38d4cc31b82fe51bbe89d8338ea79211d5
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.5.1.orig.tar.gz' libpsl_0.5.1.orig.tar.gz 81875 SHA256:c4e33bc2c2a04e6a989a0dac529d8ca6604a77e59b638ce263a71153d3a48ceb
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.5.1-1.debian.tar.xz' libpsl_0.5.1-1.debian.tar.xz 9972 SHA256:b6a49905a56c3da3d3292b6b50f471cdbdca25d426ca937be3f0f961ba94c0bc
```

Likely also available for browsing at:

- https://sources.debian.net/src/libpsl/0.5.1-1/
- https://sources.debian.net/src/libpsl/0.5.1-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libreoffice=1:4.3.3-2+deb8u6`

Binary Packages:

- `fonts-opensymbol=2:102.6+LibO4.3.3-2+deb8u6`
- `libreoffice=1:4.3.3-2+deb8u6`
- `libreoffice-avmedia-backend-gstreamer=1:4.3.3-2+deb8u6`
- `libreoffice-base=1:4.3.3-2+deb8u6`
- `libreoffice-base-core=1:4.3.3-2+deb8u6`
- `libreoffice-base-drivers=1:4.3.3-2+deb8u6`
- `libreoffice-calc=1:4.3.3-2+deb8u6`
- `libreoffice-common=1:4.3.3-2+deb8u6`
- `libreoffice-core=1:4.3.3-2+deb8u6`
- `libreoffice-draw=1:4.3.3-2+deb8u6`
- `libreoffice-impress=1:4.3.3-2+deb8u6`
- `libreoffice-java-common=1:4.3.3-2+deb8u6`
- `libreoffice-math=1:4.3.3-2+deb8u6`
- `libreoffice-report-builder-bin=1:4.3.3-2+deb8u6`
- `libreoffice-style-galaxy=1:4.3.3-2+deb8u6`
- `libreoffice-writer=1:4.3.3-2+deb8u6`
- `python3-uno=1:4.3.3-2+deb8u6`
- `uno-libs3=4.3.3-2+deb8u6`
- `ure=4.3.3-2+deb8u6`

Licenses: (parsed from: `/usr/share/doc/fonts-opensymbol/copyright`, `/usr/share/doc/libreoffice/copyright`, `/usr/share/doc/libreoffice-avmedia-backend-gstreamer/copyright`, `/usr/share/doc/libreoffice-base/copyright`, `/usr/share/doc/libreoffice-base-core/copyright`, `/usr/share/doc/libreoffice-base-drivers/copyright`, `/usr/share/doc/libreoffice-calc/copyright`, `/usr/share/doc/libreoffice-common/copyright`, `/usr/share/doc/libreoffice-core/copyright`, `/usr/share/doc/libreoffice-draw/copyright`, `/usr/share/doc/libreoffice-impress/copyright`, `/usr/share/doc/libreoffice-java-common/copyright`, `/usr/share/doc/libreoffice-math/copyright`, `/usr/share/doc/libreoffice-report-builder-bin/copyright`, `/usr/share/doc/libreoffice-style-galaxy/copyright`, `/usr/share/doc/libreoffice-writer/copyright`, `/usr/share/doc/python3-uno/copyright`, `/usr/share/doc/uno-libs3/copyright`, `/usr/share/doc/ure/copyright`)

- `Apache-2.0`
- `BSD-3-clause`
- `BSD-4-clause`
- `CDDL-1.0`
- `CDDL-1.0 | GPPL-2`
- `GPL`
- `GPL-1`
- `GPL-2`
- `GPL-2 | LGPL-2.1 | MPL-1.1`
- `GPL-2+`
- `LGPL`
- `LGPL | Apache-2.0`
- `LGPL-2`
- `LGPL-2 | Apache-2.0`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-3`
- `LGPL2+`
- `MIT`
- `MIT/X`
- `MPL 1.1 | LGPL-2+ | GPL-2+`
- `MPL-1.1`
- `MPL-1.1 | GPL-2 | LGPL-2`
- `MPL-1.1 | GPL-3+ | LGPL-3+`
- `MPL-1.1 | LGPL-2.1`
- `MPL-2.0`
- `PSF-2`
- `W3C`
- `Zlib`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libreoffice=1:4.3.3-2+deb8u6
'http://security.debian.org/pool/updates/main/libr/libreoffice/libreoffice_4.3.3-2+deb8u6.dsc' libreoffice_4.3.3-2+deb8u6.dsc 25856 SHA256:d3ab26135640eb7627b93fa0ffe75ddacfd93cd1d3bc7cfd5ef44c9ffb30aba8
'http://security.debian.org/pool/updates/main/libr/libreoffice/libreoffice_4.3.3.orig-external.tar.xz' libreoffice_4.3.3.orig-external.tar.xz 322296536 SHA256:744787778b944c94a67bf80947e5f096d10dc408a6bf4be73c2953d0588670a0
'http://security.debian.org/pool/updates/main/libr/libreoffice/libreoffice_4.3.3.orig-helpcontent2.tar.xz' libreoffice_4.3.3.orig-helpcontent2.tar.xz 1400052 SHA256:5c1668f8770fa657cc762b34e75cc8555d0dd504b200742e03a9113ce556bd80
'http://security.debian.org/pool/updates/main/libr/libreoffice/libreoffice_4.3.3.orig-translations.tar.xz' libreoffice_4.3.3.orig-translations.tar.xz 127000868 SHA256:67fbd8ef11dab0a4fa02893f050c7ff566efb83a75a7a4173286687091191fda
'http://security.debian.org/pool/updates/main/libr/libreoffice/libreoffice_4.3.3.orig.tar.xz' libreoffice_4.3.3.orig.tar.xz 149850184 SHA256:69afdc225be44a1d13cefc6fa5783cfb5535e72932cd08a427d62a6f44e27619
'http://security.debian.org/pool/updates/main/libr/libreoffice/libreoffice_4.3.3-2+deb8u6.debian.tar.xz' libreoffice_4.3.3-2+deb8u6.debian.tar.xz 2126640 SHA256:0894c0ca1b872e00b4d1c7d9368992459cbb248b05d7c3ed653577b9629525dc
```

Likely also available for browsing at:

- https://sources.debian.net/src/libreoffice/1:4.3.3-2+deb8u6/
- https://sources.debian.net/src/libreoffice/1:4.3.3-2+deb8u6/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `librevenge=0.0.1-3`

Binary Packages:

- `librevenge-0.0-0=0.0.1-3`

Licenses: (parsed from: `/usr/share/doc/librevenge-0.0-0/copyright`)

- `LGPL-2.1`
- `MPL-1.1 | GPL-3+ | LGPL-3+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris librevenge=0.0.1-3
'http://deb.debian.org/debian/pool/main/libr/librevenge/librevenge_0.0.1-3.dsc' librevenge_0.0.1-3.dsc 1928 SHA256:4479e990232323117213bdadbeda3f606c2b9d5462d3682d82e77ca7f6fb7fc8
'http://deb.debian.org/debian/pool/main/libr/librevenge/librevenge_0.0.1.orig.tar.bz2' librevenge_0.0.1.orig.tar.bz2 481475 SHA256:428c918c7775a860f4fb642643099932abcf6fe5cb72c8b0d25ee6b84ad55490
'http://deb.debian.org/debian/pool/main/libr/librevenge/librevenge_0.0.1-3.debian.tar.xz' librevenge_0.0.1-3.debian.tar.xz 12944 SHA256:abeec6e69f886eed16edf858b789a31c39a3b12bef72b6018d073d41a14e8e44
```

Likely also available for browsing at:

- https://sources.debian.net/src/librevenge/0.0.1-3/
- https://sources.debian.net/src/librevenge/0.0.1-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libselinux=2.3-2`

Binary Packages:

- `libselinux1:amd64=2.3-2`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=2.3-2
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_2.3-2.dsc' libselinux_2.3-2.dsc 2024 SHA256:aea0e0502dd1d4df17be644efb0bfe2d38e32ba2e0769eaaf8a2b64a0eb99786
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_2.3.orig.tar.gz' libselinux_2.3.orig.tar.gz 171254 SHA256:0b1e0b43ecd84a812713d09564019b08e7c205d89072b5cbcd07b052cd8e77b2
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_2.3-2.debian.tar.xz' libselinux_2.3-2.debian.tar.xz 24384 SHA256:8ec4bdb5acc066d1b369877e9a94ec1a723e4d31691753e0e1861d0884b3fd1a
```

Likely also available for browsing at:

- https://sources.debian.net/src/libselinux/2.3-2/
- https://sources.debian.net/src/libselinux/2.3-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libsemanage=2.3-1`

Binary Packages:

- `libsemanage-common=2.3-1`
- `libsemanage1:amd64=2.3-1+b1`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=2.3-1
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_2.3-1.dsc' libsemanage_2.3-1.dsc 2131 SHA256:21b321c61399deeb3d1b04b76a0c9f43e968371f3afc8a8eb859e3cc79f295aa
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_2.3.orig.tar.gz' libsemanage_2.3.orig.tar.gz 138231 SHA256:03e09e35e611c286e446bef92b6023ef2623815996f5a53394bb02e49a312e4b
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_2.3-1.debian.tar.xz' libsemanage_2.3-1.debian.tar.xz 14848 SHA256:e6e8002ae5084daf6628ac836e4724005dd7591f9a015203bb55e445508e55e6
```

Likely also available for browsing at:

- https://sources.debian.net/src/libsemanage/2.3-1/
- https://sources.debian.net/src/libsemanage/2.3-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libsepol=2.3-2`

Binary Packages:

- `libsepol1:amd64=2.3-2`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=2.3-2
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_2.3-2.dsc' libsepol_2.3-2.dsc 1762 SHA256:115ab27d7662fc03e64d9e70ed20b5dcb2adb6206155ba2577072352a5b79b6a
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_2.3.orig.tar.gz' libsepol_2.3.orig.tar.gz 209570 SHA256:cc8d8642c3b7b95d6928d65dcbca2ab0627abc1c05166637851e63c1a6eae68f
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_2.3-2.debian.tar.xz' libsepol_2.3-2.debian.tar.xz 12904 SHA256:4fea6f6de03cf6a8ba80579988ad56202d3652fe3153b0d2f8c65c89bba097a5
```

Likely also available for browsing at:

- https://sources.debian.net/src/libsepol/2.3-2/
- https://sources.debian.net/src/libsepol/2.3-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libsm=2:1.2.2-1`

Binary Packages:

- `libsm6:amd64=2:1.2.2-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libsm=2:1.2.2-1
'http://deb.debian.org/debian/pool/main/libs/libsm/libsm_1.2.2-1.dsc' libsm_1.2.2-1.dsc 2107 SHA256:1347efa550751179c0a3f1042a9f8ae43ee0c22cf0c2283921fa83e52a68433f
'http://deb.debian.org/debian/pool/main/libs/libsm/libsm_1.2.2.orig.tar.gz' libsm_1.2.2.orig.tar.gz 415990 SHA256:14bb7c669ce2b8ff712fbdbf48120e3742a77edcd5e025d6b3325ed30cf120f4
'http://deb.debian.org/debian/pool/main/libs/libsm/libsm_1.2.2-1.diff.gz' libsm_1.2.2-1.diff.gz 6183 SHA256:9848714292ead15fcc48ab2d337f2cc5fc08910abbdfaf69d3ef1b89d3fdb2d5
```

Likely also available for browsing at:

- https://sources.debian.net/src/libsm/2:1.2.2-1/
- https://sources.debian.net/src/libsm/2:1.2.2-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libssh2=1.4.3-4.1+deb8u1`

Binary Packages:

- `libssh2-1:amd64=1.4.3-4.1+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libssh2-1/copyright`)

- `BSD`

Source:

```console
$ apt-get source -qq --print-uris libssh2=1.4.3-4.1+deb8u1
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.4.3-4.1+deb8u1.dsc' libssh2_1.4.3-4.1+deb8u1.dsc 1882 SHA256:38e3ec8ae8014a721d2f08f83494c927fe42aae11f8cf1592104205da2857ca8
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.4.3.orig.tar.gz' libssh2_1.4.3.orig.tar.gz 685712 SHA256:eac6f85f9df9db2e6386906a6227eb2cd7b3245739561cad7d6dc1d5d021b96d
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.4.3-4.1+deb8u1.debian.tar.xz' libssh2_1.4.3-4.1+deb8u1.debian.tar.xz 8276 SHA256:5da712fcae528ca559be8865dc9521ef11f006bda68c39e0bde8c0495e5a2cb7
```

Likely also available for browsing at:

- https://sources.debian.net/src/libssh2/1.4.3-4.1+deb8u1/
- https://sources.debian.net/src/libssh2/1.4.3-4.1+deb8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libtasn1-6=4.2-3+deb8u2`

Binary Packages:

- `libtasn1-6:amd64=4.2-3+deb8u2`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.2-3+deb8u2
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.2-3+deb8u2.dsc' libtasn1-6_4.2-3+deb8u2.dsc 2434 SHA256:b22337782c8f2edf9adf6e42c37808f116ad4cfab2b81c1e30a6fddb8aa0acf2
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.2.orig.tar.gz' libtasn1-6_4.2.orig.tar.gz 1866192 SHA256:693b41cb36c2ac02d5990180b0712a79a591168e93d85f7fcbb75a0a0be4cdbb
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.2-3+deb8u2.debian.tar.xz' libtasn1-6_4.2-3+deb8u2.debian.tar.xz 58556 SHA256:0f7587e82f702eb757c2ad842f4511ff1619b286bd2ccc3d61fa8bb490b839d1
```

Likely also available for browsing at:

- https://sources.debian.net/src/libtasn1-6/4.2-3+deb8u2/
- https://sources.debian.net/src/libtasn1-6/4.2-3+deb8u2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libtext-charwidth-perl=0.04-7`

Binary Packages:

- `libtext-charwidth-perl=0.04-7+b3`

Licenses: (parsed from: `/usr/share/doc/libtext-charwidth-perl/copyright`)

- `Artistic`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libtext-charwidth-perl=0.04-7
'http://deb.debian.org/debian/pool/main/libt/libtext-charwidth-perl/libtext-charwidth-perl_0.04-7.dsc' libtext-charwidth-perl_0.04-7.dsc 1810 SHA256:482493991d54786bc12b38f26b90d2bbc9234ac87c3e54e0474ac00cd979dd68
'http://deb.debian.org/debian/pool/main/libt/libtext-charwidth-perl/libtext-charwidth-perl_0.04.orig.tar.bz2' libtext-charwidth-perl_0.04.orig.tar.bz2 8327 SHA256:2990c13c3f4a5479d7dbc5a94b86c23798cf0dc7df54ffe54e065f072558b6ed
'http://deb.debian.org/debian/pool/main/libt/libtext-charwidth-perl/libtext-charwidth-perl_0.04-7.debian.tar.bz2' libtext-charwidth-perl_0.04-7.debian.tar.bz2 3220 SHA256:4aa60af66136cad15d3c9ed73696b822c9f944a3b8484b03c388393302fa6038
```

Likely also available for browsing at:

- https://sources.debian.net/src/libtext-charwidth-perl/0.04-7/
- https://sources.debian.net/src/libtext-charwidth-perl/0.04-7/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libtext-iconv-perl=1.7-5`

Binary Packages:

- `libtext-iconv-perl=1.7-5+b2`

Licenses: (parsed from: `/usr/share/doc/libtext-iconv-perl/copyright`)

- `Artistic`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libtext-iconv-perl=1.7-5
'http://deb.debian.org/debian/pool/main/libt/libtext-iconv-perl/libtext-iconv-perl_1.7-5.dsc' libtext-iconv-perl_1.7-5.dsc 1828 SHA256:6f049f3ed556a9c429f00c88a28ce595446f26996f2f5173e02f51f51277749d
'http://deb.debian.org/debian/pool/main/libt/libtext-iconv-perl/libtext-iconv-perl_1.7.orig.tar.bz2' libtext-iconv-perl_1.7.orig.tar.bz2 9977 SHA256:815c5169b7afc40bc6f681b4c615ff8fb0e073d87422280c8c759a4666567490
'http://deb.debian.org/debian/pool/main/libt/libtext-iconv-perl/libtext-iconv-perl_1.7-5.debian.tar.bz2' libtext-iconv-perl_1.7-5.debian.tar.bz2 3157 SHA256:e0ee2ae3908bbde6d43098a6491284fdc7a0a117229053d1e9c539eb66127092
```

Likely also available for browsing at:

- https://sources.debian.net/src/libtext-iconv-perl/1.7-5/
- https://sources.debian.net/src/libtext-iconv-perl/1.7-5/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libtext-wrapi18n-perl=0.06-7`

Binary Packages:

- `libtext-wrapi18n-perl=0.06-7`

Licenses: (parsed from: `/usr/share/doc/libtext-wrapi18n-perl/copyright`)

- `Artistic`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtext-wrapi18n-perl=0.06-7
'http://deb.debian.org/debian/pool/main/libt/libtext-wrapi18n-perl/libtext-wrapi18n-perl_0.06-7.dsc' libtext-wrapi18n-perl_0.06-7.dsc 1156 SHA256:777dd5309172c3fa6ccea73b3c821cf6533ddb72b4adbe4def9d45fd8902b544
'http://deb.debian.org/debian/pool/main/libt/libtext-wrapi18n-perl/libtext-wrapi18n-perl_0.06.orig.tar.gz' libtext-wrapi18n-perl_0.06.orig.tar.gz 3797 SHA256:432c2a801efe9f12d631124c1163439eac4c99449ba13d80133c45ecacc627f5
'http://deb.debian.org/debian/pool/main/libt/libtext-wrapi18n-perl/libtext-wrapi18n-perl_0.06-7.diff.gz' libtext-wrapi18n-perl_0.06-7.diff.gz 3031 SHA256:fae1a435e8b2604bf78666e58e4603728990495db302a9799d63cb099e3b4001
```

Likely also available for browsing at:

- https://sources.debian.net/src/libtext-wrapi18n-perl/0.06-7/
- https://sources.debian.net/src/libtext-wrapi18n-perl/0.06-7/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libthai=0.1.21-1`

Binary Packages:

- `libthai-data=0.1.21-1`
- `libthai0:amd64=0.1.21-1`

Licenses: (parsed from: `/usr/share/doc/libthai-data/copyright`, `/usr/share/doc/libthai0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libthai=0.1.21-1
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.21-1.dsc' libthai_0.1.21-1.dsc 2161 SHA256:ad9171fb789a184ed1061ced80c453e6229d0b4b299d7e91fcb39655f5f29e83
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.21.orig.tar.xz' libthai_0.1.21.orig.tar.xz 385384 SHA256:ff0e41143a8be7e01a785778c2addae48945c8bad4a275d2135afec35959fae3
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.21-1.debian.tar.xz' libthai_0.1.21-1.debian.tar.xz 10024 SHA256:5ad02dcfe536379884f43b1a540c641567a29a17ef6d3fcceb814c67bd2959b3
```

Likely also available for browsing at:

- https://sources.debian.net/src/libthai/0.1.21-1/
- https://sources.debian.net/src/libthai/0.1.21-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libtool=2.4.2-1.11`

Binary Packages:

- `libltdl7:amd64=2.4.2-1.11+b1`

Licenses: (parsed from: `/usr/share/doc/libltdl7/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.2-1.11
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.2-1.11.dsc' libtool_2.4.2-1.11.dsc 1467 SHA256:155ccf84638725c278b641fbd1c5c76a98d612cacf00f5f00a10f8e6826e643f
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.2.orig.tar.gz' libtool_2.4.2.orig.tar.gz 2632347 SHA256:b38de44862a987293cd3d8dfae1c409d514b6c4e794ebc93648febf9afc38918
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.2-1.11.debian.tar.xz' libtool_2.4.2-1.11.debian.tar.xz 17408 SHA256:524c916ae9bdf39311aa9e713024ca7b48b0367481c8e6217f407e194e908a7b
```

Likely also available for browsing at:

- https://sources.debian.net/src/libtool/2.4.2-1.11/
- https://sources.debian.net/src/libtool/2.4.2-1.11/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libusb=2:0.1.12-25`

Binary Packages:

- `libusb-0.1-4:amd64=2:0.1.12-25`

Licenses: (parsed from: `/usr/share/doc/libusb-0.1-4/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libusb=2:0.1.12-25
'http://deb.debian.org/debian/pool/main/libu/libusb/libusb_0.1.12-25.dsc' libusb_0.1.12-25.dsc 1958 SHA256:905e7cc36c9ba24f6d58e416f8882bc2522673cfb9f63687b48c62c9e3b6c80c
'http://deb.debian.org/debian/pool/main/libu/libusb/libusb_0.1.12.orig.tar.gz' libusb_0.1.12.orig.tar.gz 389343 SHA256:37f6f7d9de74196eb5fc0bbe0aea9b5c939de7f500acba3af6fd643f3b538b44
'http://deb.debian.org/debian/pool/main/libu/libusb/libusb_0.1.12-25.debian.tar.xz' libusb_0.1.12-25.debian.tar.xz 22008 SHA256:9e42ea2a8e0ec85b13cb8c9df7dc3aff58ee82e3692a7656558ae91ceeabf7d1
```

Likely also available for browsing at:

- https://sources.debian.net/src/libusb/2:0.1.12-25/
- https://sources.debian.net/src/libusb/2:0.1.12-25/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libvisio=0.1.0-2`

Binary Packages:

- `libvisio-0.1-1=0.1.0-2`

Licenses: (parsed from: `/usr/share/doc/libvisio-0.1-1/copyright`)

- `MIT | GPL-2`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libvisio=0.1.0-2
'http://deb.debian.org/debian/pool/main/libv/libvisio/libvisio_0.1.0-2.dsc' libvisio_0.1.0-2.dsc 2034 SHA256:06ba5e7a58f0b522925207cdea1bb0f9993ffcd00475943598f1e8bdad0b6d5a
'http://deb.debian.org/debian/pool/main/libv/libvisio/libvisio_0.1.0.orig.tar.bz2' libvisio_0.1.0.orig.tar.bz2 446641 SHA256:12383fcf39098ed0685a595d43e466dbc6222ee289e6f4e5e006e232973debee
'http://deb.debian.org/debian/pool/main/libv/libvisio/libvisio_0.1.0-2.debian.tar.xz' libvisio_0.1.0-2.debian.tar.xz 7336 SHA256:686686eb6d58cf4ceae554039d444ece692cbc2886a3ced5b097dfa1abd26e91
```

Likely also available for browsing at:

- https://sources.debian.net/src/libvisio/0.1.0-2/
- https://sources.debian.net/src/libvisio/0.1.0-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libwpd=0.10.0-2`

Binary Packages:

- `libwpd-0.10-10=0.10.0-2+b1`

Licenses: (parsed from: `/usr/share/doc/libwpd-0.10-10/copyright`)

- `LGPL`
- `MPL-2.0 | LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libwpd=0.10.0-2
'http://deb.debian.org/debian/pool/main/libw/libwpd/libwpd_0.10.0-2.dsc' libwpd_0.10.0-2.dsc 1994 SHA256:830adcedd4998c75b8a35f0276cf71e2bad6e4c65edecc3d75c4f3a6ebbaca65
'http://deb.debian.org/debian/pool/main/libw/libwpd/libwpd_0.10.0.orig.tar.bz2' libwpd_0.10.0.orig.tar.bz2 632272 SHA256:f2bf5d65156a351ce404550dd822c8db8ab8740b393f61dba828d1b2cb33fe91
'http://deb.debian.org/debian/pool/main/libw/libwpd/libwpd_0.10.0-2.debian.tar.xz' libwpd_0.10.0-2.debian.tar.xz 11088 SHA256:1ea79082110d42ec9bd1e34f350968369c9ea1c136cb9a1455a89779691966ca
```

Likely also available for browsing at:

- https://sources.debian.net/src/libwpd/0.10.0-2/
- https://sources.debian.net/src/libwpd/0.10.0-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libwpg=0.3.0-3`

Binary Packages:

- `libwpg-0.3-3=0.3.0-3`

Licenses: (parsed from: `/usr/share/doc/libwpg-0.3-3/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libwpg=0.3.0-3
'http://deb.debian.org/debian/pool/main/libw/libwpg/libwpg_0.3.0-3.dsc' libwpg_0.3.0-3.dsc 1925 SHA256:76bbe5cb885f60f23617e929d3c41d950782154556eda26cd4df5532960350cf
'http://deb.debian.org/debian/pool/main/libw/libwpg/libwpg_0.3.0.orig.tar.bz2' libwpg_0.3.0.orig.tar.bz2 381878 SHA256:28fc3580228a82948dfc01d07abd5076c8b0df76a68702c1a81eb88fdf377348
'http://deb.debian.org/debian/pool/main/libw/libwpg/libwpg_0.3.0-3.debian.tar.xz' libwpg_0.3.0-3.debian.tar.xz 8884 SHA256:1da18f6e81dcde4577258523b00fda6016f7da438185ea748e4bf107f1a9fa58
```

Likely also available for browsing at:

- https://sources.debian.net/src/libwpg/0.3.0-3/
- https://sources.debian.net/src/libwpg/0.3.0-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libwps=0.3.0-2`

Binary Packages:

- `libwps-0.3-3=0.3.0-2`

Licenses: (parsed from: `/usr/share/doc/libwps-0.3-3/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libwps=0.3.0-2
'http://deb.debian.org/debian/pool/main/libw/libwps/libwps_0.3.0-2.dsc' libwps_0.3.0-2.dsc 1895 SHA256:d2d46f2e74156bd7f1113d230584652df034d0c054ec212370fa053ab4a4a8a4
'http://deb.debian.org/debian/pool/main/libw/libwps/libwps_0.3.0.orig.tar.bz2' libwps_0.3.0.orig.tar.bz2 502782 SHA256:243d1dfc9bb53ac9d05405379a119e9b7d999714de3a3d56f4d3c505cedad43a
'http://deb.debian.org/debian/pool/main/libw/libwps/libwps_0.3.0-2.debian.tar.xz' libwps_0.3.0-2.debian.tar.xz 9252 SHA256:d06f52983149fa30da317393c2e0cea8c3b8bde595522ab5e94098d45bd3d87a
```

Likely also available for browsing at:

- https://sources.debian.net/src/libwps/0.3.0-2/
- https://sources.debian.net/src/libwps/0.3.0-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libx11=2:1.6.2-3`

Binary Packages:

- `libx11-6:amd64=2:1.6.2-3`
- `libx11-data=2:1.6.2-3`
- `libx11-xcb1:amd64=2:1.6.2-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.6.2-3
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.2-3.dsc' libx11_1.6.2-3.dsc 2510 SHA256:fa8e2912122ccd6bbf06060aa14afc84c5a7e76c603d63f29071081513907737
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.2.orig.tar.gz' libx11_1.6.2.orig.tar.gz 3119924 SHA256:b93739bcd517723121f508bcaf0c213c1bae9c5eacffdca571ff0d86c30ead3e
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.2-3.diff.gz' libx11_1.6.2-3.diff.gz 72788 SHA256:5d516aa06837bfe29e8b5f9015f1028835e61e5fb52f1b7d28feb22668547cdc
```

Likely also available for browsing at:

- https://sources.debian.net/src/libx11/2:1.6.2-3/
- https://sources.debian.net/src/libx11/2:1.6.2-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libxau=1:1.0.8-1`

Binary Packages:

- `libxau6:amd64=1:1.0.8-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxau=1:1.0.8-1
'http://deb.debian.org/debian/pool/main/libx/libxau/libxau_1.0.8-1.dsc' libxau_1.0.8-1.dsc 2040 SHA256:3ddb5f2c7a49ef7507b8d1e63e891238db877b4d1bb1c5486a3e3242c8523602
'http://deb.debian.org/debian/pool/main/libx/libxau/libxau_1.0.8.orig.tar.gz' libxau_1.0.8.orig.tar.gz 362044 SHA256:c343b4ef66d66a6b3e0e27aa46b37ad5cab0f11a5c565eafb4a1c7590bc71d7b
'http://deb.debian.org/debian/pool/main/libx/libxau/libxau_1.0.8-1.diff.gz' libxau_1.0.8-1.diff.gz 15287 SHA256:b493479d6a52a0e753dd357ad8a4bc5c4296015f3f7b96cf546f7c5c5843cbb0
```

Likely also available for browsing at:

- https://sources.debian.net/src/libxau/1:1.0.8-1/
- https://sources.debian.net/src/libxau/1:1.0.8-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libxcb=1.10-3`

Binary Packages:

- `libxcb-dri2-0:amd64=1.10-3+b1`
- `libxcb-dri3-0:amd64=1.10-3+b1`
- `libxcb-glx0:amd64=1.10-3+b1`
- `libxcb-present0:amd64=1.10-3+b1`
- `libxcb-render0:amd64=1.10-3+b1`
- `libxcb-shm0:amd64=1.10-3+b1`
- `libxcb-sync1:amd64=1.10-3+b1`
- `libxcb1:amd64=1.10-3+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.10-3
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.10-3.dsc' libxcb_1.10-3.dsc 6940 SHA256:d9915049a5efb76badb8c05d1cf2cdc695910cae5c1c4719a37be1256abdbeab
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.10.orig.tar.gz' libxcb_1.10.orig.tar.gz 601241 SHA256:c4cd324ac7bf810e95b1c1b56f413b13850eaa1d7eca60ddc46c61ac9d5f4441
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.10-3.diff.gz' libxcb_1.10-3.diff.gz 24425 SHA256:c9c6dc0fedfe20e4a00dc96cb37dfe96ee2980063e941a07f0758b3e6bec57cd
```

Likely also available for browsing at:

- https://sources.debian.net/src/libxcb/1.10-3/
- https://sources.debian.net/src/libxcb/1.10-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libxcomposite=1:0.4.4-1`

Binary Packages:

- `libxcomposite1:amd64=1:0.4.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcomposite=1:0.4.4-1
'http://deb.debian.org/debian/pool/main/libx/libxcomposite/libxcomposite_0.4.4-1.dsc' libxcomposite_0.4.4-1.dsc 2170 SHA256:b304040285ca2d6e2667bfec45097814bdd017380c629a5972993407c656469a
'http://deb.debian.org/debian/pool/main/libx/libxcomposite/libxcomposite_0.4.4.orig.tar.gz' libxcomposite_0.4.4.orig.tar.gz 354584 SHA256:83c04649819c6f52cda1b0ce8bcdcc48ad8618428ad803fb07f20b802f1bdad1
'http://deb.debian.org/debian/pool/main/libx/libxcomposite/libxcomposite_0.4.4-1.diff.gz' libxcomposite_0.4.4-1.diff.gz 15633 SHA256:09fe6dd7d98d935e7307d57f926912d477b929f06c159962840d3a398f376988
```

Likely also available for browsing at:

- https://sources.debian.net/src/libxcomposite/1:0.4.4-1/
- https://sources.debian.net/src/libxcomposite/1:0.4.4-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libxcursor=1:1.1.14-1`

Binary Packages:

- `libxcursor1:amd64=1:1.1.14-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcursor=1:1.1.14-1
'http://deb.debian.org/debian/pool/main/libx/libxcursor/libxcursor_1.1.14-1.dsc' libxcursor_1.1.14-1.dsc 2275 SHA256:cef5e720065219d46f150dde03d7fdffe113a961036d8fd3e836ff3f0c53686a
'http://deb.debian.org/debian/pool/main/libx/libxcursor/libxcursor_1.1.14.orig.tar.gz' libxcursor_1.1.14.orig.tar.gz 374910 SHA256:be0954faf274969ffa6d95b9606b9c0cfee28c13b6fc014f15606a0c8b05c17b
'http://deb.debian.org/debian/pool/main/libx/libxcursor/libxcursor_1.1.14-1.diff.gz' libxcursor_1.1.14-1.diff.gz 18173 SHA256:45fec45ab41dd3e5ca2147c3c7751063a732699ab1c93524d8af24ef19b3d776
```

Likely also available for browsing at:

- https://sources.debian.net/src/libxcursor/1:1.1.14-1/
- https://sources.debian.net/src/libxcursor/1:1.1.14-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libxdamage=1:1.1.4-2`

Binary Packages:

- `libxdamage1:amd64=1:1.1.4-2+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdamage=1:1.1.4-2
'http://deb.debian.org/debian/pool/main/libx/libxdamage/libxdamage_1.1.4-2.dsc' libxdamage_1.1.4-2.dsc 2127 SHA256:43cbefb5c69f51d89a11cf84718fe0c42058fc9b6ec7c0076e7c37b9e829feb5
'http://deb.debian.org/debian/pool/main/libx/libxdamage/libxdamage_1.1.4.orig.tar.gz' libxdamage_1.1.4.orig.tar.gz 339060 SHA256:4bb3e9d917f5f593df2277d452926ee6ad96de7b7cd1017cbcf4579fe5d3442b
'http://deb.debian.org/debian/pool/main/libx/libxdamage/libxdamage_1.1.4-2.diff.gz' libxdamage_1.1.4-2.diff.gz 14930 SHA256:d238c1a266c30cd124ede7e6c86635bfaa108fa552c4a82919101cebf22670e9
```

Likely also available for browsing at:

- https://sources.debian.net/src/libxdamage/1:1.1.4-2/
- https://sources.debian.net/src/libxdamage/1:1.1.4-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libxdmcp=1:1.1.1-1`

Binary Packages:

- `libxdmcp6:amd64=1:1.1.1-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdmcp=1:1.1.1-1
'http://deb.debian.org/debian/pool/main/libx/libxdmcp/libxdmcp_1.1.1-1.dsc' libxdmcp_1.1.1-1.dsc 2102 SHA256:1713ac047ad1d235fe51476f2224d0dc0f170e9623c0735d1941c474942b24d3
'http://deb.debian.org/debian/pool/main/libx/libxdmcp/libxdmcp_1.1.1.orig.tar.gz' libxdmcp_1.1.1.orig.tar.gz 376525 SHA256:ae6e677911e2696a2976b2f565f116ba9ce99e89cc7e140c4a791270c3aff96f
'http://deb.debian.org/debian/pool/main/libx/libxdmcp/libxdmcp_1.1.1-1.diff.gz' libxdmcp_1.1.1-1.diff.gz 14891 SHA256:bb79bc8439d63d5bed6bf7544f1ed14b4606c246f724523da2fa921cc9929f19
```

Likely also available for browsing at:

- https://sources.debian.net/src/libxdmcp/1:1.1.1-1/
- https://sources.debian.net/src/libxdmcp/1:1.1.1-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libxext=2:1.3.3-1`

Binary Packages:

- `libxext6:amd64=2:1.3.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxext=2:1.3.3-1
'http://deb.debian.org/debian/pool/main/libx/libxext/libxext_1.3.3-1.dsc' libxext_1.3.3-1.dsc 2221 SHA256:47106df75b8f3db1e43803e8e94a2e966cd23f7daa8cfc393af739a9e33ef955
'http://deb.debian.org/debian/pool/main/libx/libxext/libxext_1.3.3.orig.tar.gz' libxext_1.3.3.orig.tar.gz 468441 SHA256:eb0b88050491fef4716da4b06a4d92b4fc9e76f880d6310b2157df604342cfe5
'http://deb.debian.org/debian/pool/main/libx/libxext/libxext_1.3.3-1.diff.gz' libxext_1.3.3-1.diff.gz 20763 SHA256:e294a4884eb68acbd151312cb0c973aad63268b637b15ccf1911864b7197557e
```

Likely also available for browsing at:

- https://sources.debian.net/src/libxext/2:1.3.3-1/
- https://sources.debian.net/src/libxext/2:1.3.3-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libxfixes=1:5.0.1-2`

Binary Packages:

- `libxfixes3:amd64=1:5.0.1-2+b2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxfixes=1:5.0.1-2
'http://deb.debian.org/debian/pool/main/libx/libxfixes/libxfixes_5.0.1-2.dsc' libxfixes_5.0.1-2.dsc 2160 SHA256:1569c87546b8d59ee7f60b395b10ea1a6f9d52418aed9d7cf2d633b14a1f1f25
'http://deb.debian.org/debian/pool/main/libx/libxfixes/libxfixes_5.0.1.orig.tar.gz' libxfixes_5.0.1.orig.tar.gz 352057 SHA256:81b692856c0e7ab2778a34a32aa6b3f455b9b58cf388f009cba872ed933ae9c0
'http://deb.debian.org/debian/pool/main/libx/libxfixes/libxfixes_5.0.1-2.diff.gz' libxfixes_5.0.1-2.diff.gz 6564 SHA256:df62260744ac03e8354b004685d439c32588e826c9dc570b6109070447601ce0
```

Likely also available for browsing at:

- https://sources.debian.net/src/libxfixes/1:5.0.1-2/
- https://sources.debian.net/src/libxfixes/1:5.0.1-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libxi=2:1.7.4-1`

Binary Packages:

- `libxi6:amd64=2:1.7.4-1+b2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxi=2:1.7.4-1
'http://deb.debian.org/debian/pool/main/libx/libxi/libxi_1.7.4-1.dsc' libxi_1.7.4-1.dsc 2331 SHA256:c0ba57cce10f4edaf66302a25ce1503c687d373f562b64a272464f856d8ad380
'http://deb.debian.org/debian/pool/main/libx/libxi/libxi_1.7.4.orig.tar.gz' libxi_1.7.4.orig.tar.gz 574645 SHA256:ddf7c56bc0d7206308c22365f694c1a1f177eb3b801fc22d42ead378440aca54
'http://deb.debian.org/debian/pool/main/libx/libxi/libxi_1.7.4-1.diff.gz' libxi_1.7.4-1.diff.gz 18576 SHA256:b144fc2ae9665dbd2fa33a5008d32291378ecabb5c20a8a4b5d729e2aeb7763e
```

Likely also available for browsing at:

- https://sources.debian.net/src/libxi/2:1.7.4-1/
- https://sources.debian.net/src/libxi/2:1.7.4-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libxinerama=2:1.1.3-1`

Binary Packages:

- `libxinerama1:amd64=2:1.1.3-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxinerama=2:1.1.3-1
'http://deb.debian.org/debian/pool/main/libx/libxinerama/libxinerama_1.1.3-1.dsc' libxinerama_1.1.3-1.dsc 2198 SHA256:4cf9a3558bd7ce1b4f55a581175c05e4b4a172364458a21ff4b657b714688fbb
'http://deb.debian.org/debian/pool/main/libx/libxinerama/libxinerama_1.1.3.orig.tar.gz' libxinerama_1.1.3.orig.tar.gz 350141 SHA256:0ba243222ae5aba4c6a3d7a394c32c8b69220a6872dbb00b7abae8753aca9a44
'http://deb.debian.org/debian/pool/main/libx/libxinerama/libxinerama_1.1.3-1.diff.gz' libxinerama_1.1.3-1.diff.gz 15738 SHA256:2b1487e3511ddabfec666a62f6e5e8ac4f97536b0d53c51f7bf4cbe07508a130
```

Likely also available for browsing at:

- https://sources.debian.net/src/libxinerama/2:1.1.3-1/
- https://sources.debian.net/src/libxinerama/2:1.1.3-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libxml2=2.9.1+dfsg1-5+deb8u4`

Binary Packages:

- `libxml2:amd64=2.9.1+dfsg1-5+deb8u4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.1+dfsg1-5+deb8u4
'http://deb.debian.org/debian/pool/main/libx/libxml2/libxml2_2.9.1+dfsg1-5+deb8u4.dsc' libxml2_2.9.1+dfsg1-5+deb8u4.dsc 2760 SHA256:23f9a9935227718fd2921abb484c129617325e1306d8525b3dcec1611df01096
'http://deb.debian.org/debian/pool/main/libx/libxml2/libxml2_2.9.1+dfsg1.orig.tar.gz' libxml2_2.9.1+dfsg1.orig.tar.gz 3793894 SHA256:f3ec5256412192f74833286c4490672500b232ed1c9195214db2c641df064a28
'http://deb.debian.org/debian/pool/main/libx/libxml2/libxml2_2.9.1+dfsg1-5+deb8u4.debian.tar.xz' libxml2_2.9.1+dfsg1-5+deb8u4.debian.tar.xz 66756 SHA256:cda8374910db4e2a06b2515123dbe0b714f7f647532dc305f03c2a094175e706
```

Likely also available for browsing at:

- https://sources.debian.net/src/libxml2/2.9.1+dfsg1-5+deb8u4/
- https://sources.debian.net/src/libxml2/2.9.1+dfsg1-5+deb8u4/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libxmu=2:1.1.2-1`

Binary Packages:

- `libxmu6:amd64=2:1.1.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxmu=2:1.1.2-1
'http://deb.debian.org/debian/pool/main/libx/libxmu/libxmu_1.1.2-1.dsc' libxmu_1.1.2-1.dsc 2338 SHA256:63be1a0be054298bcde9455f8b728dcbcc62b932479645f1d176373f9112ff60
'http://deb.debian.org/debian/pool/main/libx/libxmu/libxmu_1.1.2.orig.tar.gz' libxmu_1.1.2.orig.tar.gz 469019 SHA256:e5fd4bacef068f9509b8226017205040e38d3fba8d2de55037200e7176c13dba
'http://deb.debian.org/debian/pool/main/libx/libxmu/libxmu_1.1.2-1.diff.gz' libxmu_1.1.2-1.diff.gz 6653 SHA256:7b5f0b0536c951cad486c89805b089f535ae357a44602267c787b234c8dcd78f
```

Likely also available for browsing at:

- https://sources.debian.net/src/libxmu/2:1.1.2-1/
- https://sources.debian.net/src/libxmu/2:1.1.2-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libxrandr=2:1.4.2-1`

Binary Packages:

- `libxrandr2:amd64=2:1.4.2-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxrandr=2:1.4.2-1
'http://deb.debian.org/debian/pool/main/libx/libxrandr/libxrandr_1.4.2-1.dsc' libxrandr_1.4.2-1.dsc 2091 SHA256:cdc60b31275d8a80c2aaf8105aa015e35e54368fc1fb435e728f1926720fa203
'http://deb.debian.org/debian/pool/main/libx/libxrandr/libxrandr_1.4.2.orig.tar.gz' libxrandr_1.4.2.orig.tar.gz 384543 SHA256:fdccecde43daf8caf5697884fe7855c6560e4804957c57f71f65439544b847d4
'http://deb.debian.org/debian/pool/main/libx/libxrandr/libxrandr_1.4.2-1.diff.gz' libxrandr_1.4.2-1.diff.gz 16357 SHA256:c2a1630e677713eab84e4e074aa0400bcc2558fb3b38dcccf1ba01190c5f595e
```

Likely also available for browsing at:

- https://sources.debian.net/src/libxrandr/2:1.4.2-1/
- https://sources.debian.net/src/libxrandr/2:1.4.2-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libxrender=1:0.9.8-1`

Binary Packages:

- `libxrender1:amd64=1:0.9.8-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxrender=1:0.9.8-1
'http://deb.debian.org/debian/pool/main/libx/libxrender/libxrender_0.9.8-1.dsc' libxrender_0.9.8-1.dsc 2161 SHA256:af7f6e3d257cc75eb70fc964d8db281d69eb204f0c9af7677419c8462a90e69f
'http://deb.debian.org/debian/pool/main/libx/libxrender/libxrender_0.9.8.orig.tar.gz' libxrender_0.9.8.orig.tar.gz 363551 SHA256:c3acffff4cd5c91585e8c4fdf1ec29fc234482f661ed548112b4d52db19963d1
'http://deb.debian.org/debian/pool/main/libx/libxrender/libxrender_0.9.8-1.diff.gz' libxrender_0.9.8-1.diff.gz 18898 SHA256:e3d0fe59c5bb680e0fd1e115c54a6cb2fa2c9fe208679b7fbe7b8de7040ffe16
```

Likely also available for browsing at:

- https://sources.debian.net/src/libxrender/1:0.9.8-1/
- https://sources.debian.net/src/libxrender/1:0.9.8-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libxshmfence=1.1-4`

Binary Packages:

- `libxshmfence1:amd64=1.1-4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxshmfence=1.1-4
'http://deb.debian.org/debian/pool/main/libx/libxshmfence/libxshmfence_1.1-4.dsc' libxshmfence_1.1-4.dsc 2125 SHA256:b4d136498a488b4c946871c2ec25c6df882558dce587be844d213a98fcdbce7d
'http://deb.debian.org/debian/pool/main/libx/libxshmfence/libxshmfence_1.1.orig.tar.gz' libxshmfence_1.1.orig.tar.gz 353601 SHA256:36a6c67c71c6f262be0f2f29349d33ad157ba1fea64a55acd35b90c3816a4cdc
'http://deb.debian.org/debian/pool/main/libx/libxshmfence/libxshmfence_1.1-4.diff.gz' libxshmfence_1.1-4.diff.gz 2483 SHA256:10f0926dd70c1cced73470c012e8b021c32d0badffecc2a3509b259c332aaf3c
```

Likely also available for browsing at:

- https://sources.debian.net/src/libxshmfence/1.1-4/
- https://sources.debian.net/src/libxshmfence/1.1-4/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libxslt=1.1.28-2+deb8u2`

Binary Packages:

- `libxslt1.1:amd64=1.1.28-2+deb8u2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxslt=1.1.28-2+deb8u2
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.28-2+deb8u2.dsc' libxslt_1.1.28-2+deb8u2.dsc 2529 SHA256:e5a1286006f7c9d136f1a2441e4993deb35551ed359d4cb7492d3128835f6f64
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.28.orig.tar.gz' libxslt_1.1.28.orig.tar.gz 3435907 SHA256:5fc7151a57b89c03d7b825df5a0fae0a8d5f05674c0e7cf2937ecec4d54a028c
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.28-2+deb8u2.debian.tar.xz' libxslt_1.1.28-2+deb8u2.debian.tar.xz 37564 SHA256:218aa08affb2a5c8b8935a8b44d09e7727cbf453576b4c3e0886fd86a966cca0
```

Likely also available for browsing at:

- https://sources.debian.net/src/libxslt/1.1.28-2+deb8u2/
- https://sources.debian.net/src/libxslt/1.1.28-2+deb8u2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libxt=1:1.1.4-1`

Binary Packages:

- `libxt6:amd64=1:1.1.4-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxt=1:1.1.4-1
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.1.4-1.dsc' libxt_1.1.4-1.dsc 2130 SHA256:2158838b3cc889d51bc267c2a1832b753a38a507b22274daa5b9341d88b2109e
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.1.4.orig.tar.gz' libxt_1.1.4.orig.tar.gz 950463 SHA256:823109a0d14dfaef7ede1b3fd28318078daa2cc2f005c439a21c33bdac3d3784
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.1.4-1.diff.gz' libxt_1.1.4-1.diff.gz 11246 SHA256:4414e80a2d36a7122de644d3fe67dadbd12a636d80366eda9b6840f1c7d328bc
```

Likely also available for browsing at:

- https://sources.debian.net/src/libxt/1:1.1.4-1/
- https://sources.debian.net/src/libxt/1:1.1.4-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libxtst=2:1.2.2-1`

Binary Packages:

- `libxtst6:amd64=2:1.2.2-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxtst=2:1.2.2-1
'http://deb.debian.org/debian/pool/main/libx/libxtst/libxtst_1.2.2-1.dsc' libxtst_1.2.2-1.dsc 2303 SHA256:92507fe81ab453ee4e9de52e3b638e33429f74f175ea496c310bffb8434e4b4d
'http://deb.debian.org/debian/pool/main/libx/libxtst/libxtst_1.2.2.orig.tar.gz' libxtst_1.2.2.orig.tar.gz 392569 SHA256:221838960c7b9058cd6795c1c3ee8e25bae1c68106be314bc3036a4f26be0e6c
'http://deb.debian.org/debian/pool/main/libx/libxtst/libxtst_1.2.2-1.diff.gz' libxtst_1.2.2-1.diff.gz 16977 SHA256:3f1ae4cee26b1d93d037610bb7397f324eb293a0520e2be5f5bd822c115cd639
```

Likely also available for browsing at:

- https://sources.debian.net/src/libxtst/2:1.2.2-1/
- https://sources.debian.net/src/libxtst/2:1.2.2-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `libxxf86vm=1:1.1.3-1`

Binary Packages:

- `libxxf86vm1:amd64=1:1.1.3-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxxf86vm=1:1.1.3-1
'http://deb.debian.org/debian/pool/main/libx/libxxf86vm/libxxf86vm_1.1.3-1.dsc' libxxf86vm_1.1.3-1.dsc 2094 SHA256:4b75f3b4f18f5c80a240e279e3edd222523b791e2ed2657a45716310fe7db430
'http://deb.debian.org/debian/pool/main/libx/libxxf86vm/libxxf86vm_1.1.3.orig.tar.gz' libxxf86vm_1.1.3.orig.tar.gz 354937 SHA256:26ffbb4baaee0256ef9cdd7b8631aa3fa7bbb32e87125cfdb37fa644a623570e
'http://deb.debian.org/debian/pool/main/libx/libxxf86vm/libxxf86vm_1.1.3-1.diff.gz' libxxf86vm_1.1.3-1.diff.gz 5115 SHA256:5b51cc770666430c2c40e9a58395c72d7591f81bc5e7fd494397bbaf794b38e2
```

Likely also available for browsing at:

- https://sources.debian.net/src/libxxf86vm/1:1.1.3-1/
- https://sources.debian.net/src/libxxf86vm/1:1.1.3-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `lp-solve=5.5.0.13-7`

Binary Packages:

- `lp-solve=5.5.0.13-7+b1`

Licenses: (parsed from: `/usr/share/doc/lp-solve/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris lp-solve=5.5.0.13-7
'http://deb.debian.org/debian/pool/main/l/lp-solve/lp-solve_5.5.0.13-7.dsc' lp-solve_5.5.0.13-7.dsc 2112 SHA256:4b53606f4b46259c136f0ec56154e452e5184b015e775fb7214a3e4fe5c016f2
'http://deb.debian.org/debian/pool/main/l/lp-solve/lp-solve_5.5.0.13.orig-docs.tar.gz' lp-solve_5.5.0.13.orig-docs.tar.gz 378518 SHA256:1d31b9b16f914372bc0e58c279fefabca279f3b665f21be8d83b418addd75509
'http://deb.debian.org/debian/pool/main/l/lp-solve/lp-solve_5.5.0.13.orig.tar.gz' lp-solve_5.5.0.13.orig.tar.gz 793437 SHA256:8714793ffc227c5d78b83acc8e409a68f6159d83bcf0af632a69887c97fe4155
'http://deb.debian.org/debian/pool/main/l/lp-solve/lp-solve_5.5.0.13-7.debian.tar.gz' lp-solve_5.5.0.13-7.debian.tar.gz 9140 SHA256:8d310fb4f08e62b2e96be176e8607ef70387ca69746f45489219afe8715a72b1
```

Likely also available for browsing at:

- https://sources.debian.net/src/lp-solve/5.5.0.13-7/
- https://sources.debian.net/src/lp-solve/5.5.0.13-7/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `lsb=4.1+Debian13+nmu1`

Binary Packages:

- `lsb-base=4.1+Debian13+nmu1`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=4.1+Debian13+nmu1
'http://deb.debian.org/debian/pool/main/l/lsb/lsb_4.1+Debian13+nmu1.dsc' lsb_4.1+Debian13+nmu1.dsc 2449 SHA256:ef70a3302cf4b50c02ad3cfb90d7997968dd509dc0dbb77562b76f23b617c254
'http://deb.debian.org/debian/pool/main/l/lsb/lsb_4.1+Debian13+nmu1.tar.xz' lsb_4.1+Debian13+nmu1.tar.xz 59880 SHA256:7f5fbd13c04de166d0f658c0b71ed97c3fe07e01e165f5c0bd68ff5977bee72d
```

Likely also available for browsing at:

- https://sources.debian.net/src/lsb/4.1+Debian13+nmu1/
- https://sources.debian.net/src/lsb/4.1+Debian13+nmu1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `lvm2=2.02.111-2.2+deb8u1`

Binary Packages:

- `dmsetup=2:1.02.90-2.2+deb8u1`
- `libdevmapper1.02.1:amd64=2:1.02.90-2.2+deb8u1`

Licenses: (parsed from: `/usr/share/doc/dmsetup/copyright`, `/usr/share/doc/libdevmapper1.02.1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris lvm2=2.02.111-2.2+deb8u1
'http://deb.debian.org/debian/pool/main/l/lvm2/lvm2_2.02.111-2.2+deb8u1.dsc' lvm2_2.02.111-2.2+deb8u1.dsc 2474 SHA256:9e67627d50ef43b88f29a42b5ff4d48b0bfeeb35d98c09da33c6ce51e99c5d96
'http://deb.debian.org/debian/pool/main/l/lvm2/lvm2_2.02.111.orig.tar.gz' lvm2_2.02.111.orig.tar.gz 1497626 SHA256:ff358054ee821503ada8a33b327688cd4d64a2fc448c667a85c332c545aae4f6
'http://deb.debian.org/debian/pool/main/l/lvm2/lvm2_2.02.111-2.2+deb8u1.debian.tar.xz' lvm2_2.02.111-2.2+deb8u1.debian.tar.xz 29476 SHA256:df657682e06f9559d04719c1543285e8bcb51fb4647f673b787538fb34ebe26f
```

Likely also available for browsing at:

- https://sources.debian.net/src/lvm2/2.02.111-2.2+deb8u1/
- https://sources.debian.net/src/lvm2/2.02.111-2.2+deb8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `mawk=1.3.3-17`

Binary Packages:

- `mawk=1.3.3-17`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.3-17
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.3-17.dsc' mawk_1.3.3-17.dsc 1801 SHA256:f98ce6e153e8ac1faf8165bbf77447a4279313f1c18f6bfeec0c5ce35e4b9c03
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.3.orig.tar.gz' mawk_1.3.3.orig.tar.gz 209942 SHA256:32649c46063d4ef0777a12ae6e9a26bcc920833d54e1abca7edb8d37481e7485
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.3-17.diff.gz' mawk_1.3.3-17.diff.gz 63506 SHA256:13cb66b6eb5ee654d5626621d5ef476ede6b0bebac18ce765516de810e58490c
```

Likely also available for browsing at:

- https://sources.debian.net/src/mawk/1.3.3-17/
- https://sources.debian.net/src/mawk/1.3.3-17/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `mesa=10.3.2-1+deb8u1`

Binary Packages:

- `libgl1-mesa-glx:amd64=10.3.2-1+deb8u1`
- `libglapi-mesa:amd64=10.3.2-1+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libgl1-mesa-glx/copyright`, `/usr/share/doc/libglapi-mesa/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris mesa=10.3.2-1+deb8u1
'http://deb.debian.org/debian/pool/main/m/mesa/mesa_10.3.2-1+deb8u1.dsc' mesa_10.3.2-1+deb8u1.dsc 5461 SHA256:f9b14951df390dc25aac9562e08237e162e06b9526b4136ac58e0df27bea7d36
'http://deb.debian.org/debian/pool/main/m/mesa/mesa_10.3.2.orig.tar.gz' mesa_10.3.2.orig.tar.gz 9649735 SHA256:e65f8e691f06f111c1aeb3a376b13c9cc88cb162bee2709e0e7e6b0e6628ca75
'http://deb.debian.org/debian/pool/main/m/mesa/mesa_10.3.2-1+deb8u1.diff.gz' mesa_10.3.2-1+deb8u1.diff.gz 82262 SHA256:e9d66405fe9b41a41a022ba452769a4627c97c289d92b1c27dca60c6dccea997
```

Likely also available for browsing at:

- https://sources.debian.net/src/mesa/10.3.2-1+deb8u1/
- https://sources.debian.net/src/mesa/10.3.2-1+deb8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `mhash=0.9.9.9-7`

Binary Packages:

- `libmhash2:amd64=0.9.9.9-7`

Licenses: (parsed from: `/usr/share/doc/libmhash2/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris mhash=0.9.9.9-7
'http://deb.debian.org/debian/pool/main/m/mhash/mhash_0.9.9.9-7.dsc' mhash_0.9.9.9-7.dsc 1947 SHA256:cb4349ff77c8ad7ecb0b5d02083d0a0f2d60f7e8dd6ce4735cbafc7b4dc63461
'http://deb.debian.org/debian/pool/main/m/mhash/mhash_0.9.9.9.orig.tar.gz' mhash_0.9.9.9.orig.tar.gz 577533 SHA256:73991e9e54bb392484a510943d4c5d395462181cc4abe53f863edec13c335403
'http://deb.debian.org/debian/pool/main/m/mhash/mhash_0.9.9.9-7.debian.tar.xz' mhash_0.9.9.9-7.debian.tar.xz 11120 SHA256:229076933ac07420e16f7ab76e820aba79158cd7c5f3204fd1adac4f048bbe5a
```

Likely also available for browsing at:

- https://sources.debian.net/src/mhash/0.9.9.9-7/
- https://sources.debian.net/src/mhash/0.9.9.9-7/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `mime-support=3.58`

Binary Packages:

- `mime-support=3.58`

Licenses: (parsed from: `/usr/share/doc/mime-support/copyright`)

- `Bellcore`
- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris mime-support=3.58
'http://deb.debian.org/debian/pool/main/m/mime-support/mime-support_3.58.dsc' mime-support_3.58.dsc 1604 SHA256:3279480870a7bd6c7e2a85f7f1e5deba50c3cb5edcbd6ce69a3cfc7fe0266284
'http://deb.debian.org/debian/pool/main/m/mime-support/mime-support_3.58.tar.gz' mime-support_3.58.tar.gz 34995 SHA256:3d9ca5115e93edb3ada3fb120cde88ac3d866903e18a41ca124428d77dd1721e
```

Likely also available for browsing at:

- https://sources.debian.net/src/mime-support/3.58/
- https://sources.debian.net/src/mime-support/3.58/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `mpdecimal=2.4.1-1`

Binary Packages:

- `libmpdec2:amd64=2.4.1-1`

Licenses: (parsed from: `/usr/share/doc/libmpdec2/copyright`)

- `BSD`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mpdecimal=2.4.1-1
'http://deb.debian.org/debian/pool/main/m/mpdecimal/mpdecimal_2.4.1-1.dsc' mpdecimal_2.4.1-1.dsc 1211 SHA256:c5f8ec23ca7fa98625c8da280e0771a41d4b26d2cc88b76873437c9806e63dc6
'http://deb.debian.org/debian/pool/main/m/mpdecimal/mpdecimal_2.4.1.orig.tar.gz' mpdecimal_2.4.1.orig.tar.gz 2254789 SHA256:da74d3cfab559971a4fbd4fb506e1b4498636eb77d0fd09e44f8e546d18ac068
'http://deb.debian.org/debian/pool/main/m/mpdecimal/mpdecimal_2.4.1-1.debian.tar.xz' mpdecimal_2.4.1-1.debian.tar.xz 5100 SHA256:770203cd68a7cfd33b2b4ba0c82f4e4a5e12cd37c58873eef26451ae76b70d4b
```

Likely also available for browsing at:

- https://sources.debian.net/src/mpdecimal/2.4.1-1/
- https://sources.debian.net/src/mpdecimal/2.4.1-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `mysql-connector-java=5.1.39-1~deb8u1`

Binary Packages:

- `libmysql-java=5.1.39-1~deb8u1`

Licenses: (parsed from: `/usr/share/doc/libmysql-java/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris mysql-connector-java=5.1.39-1~deb8u1
'http://deb.debian.org/debian/pool/main/m/mysql-connector-java/mysql-connector-java_5.1.39-1~deb8u1.dsc' mysql-connector-java_5.1.39-1~deb8u1.dsc 2355 SHA256:e4da6a322eb61235548dbe84157c00a4153d66f1e9fb8f136b01220bb70cfce0
'http://deb.debian.org/debian/pool/main/m/mysql-connector-java/mysql-connector-java_5.1.39.orig.tar.xz' mysql-connector-java_5.1.39.orig.tar.xz 979308 SHA256:53a661327b212840adce981136ad1adefd2431d83f807c0f895c28a45a576953
'http://deb.debian.org/debian/pool/main/m/mysql-connector-java/mysql-connector-java_5.1.39-1~deb8u1.debian.tar.xz' mysql-connector-java_5.1.39-1~deb8u1.debian.tar.xz 11692 SHA256:6d82b795d6e45f5030cce6bc7be9d33c25f4ba536f46a4b4c3235d74e44eaaea
```

Likely also available for browsing at:

- https://sources.debian.net/src/mysql-connector-java/5.1.39-1~deb8u1/
- https://sources.debian.net/src/mysql-connector-java/5.1.39-1~deb8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `mythes=2:1.2.4-1`

Binary Packages:

- `libmythes-1.2-0=2:1.2.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris mythes=2:1.2.4-1
'http://deb.debian.org/debian/pool/main/m/mythes/mythes_1.2.4-1.dsc' mythes_1.2.4-1.dsc 1858 SHA256:a981e6d497032adab6efc78adf84fea93a96e8870aa14dd9909de26446f7ccf2
'http://deb.debian.org/debian/pool/main/m/mythes/mythes_1.2.4.orig.tar.gz' mythes_1.2.4.orig.tar.gz 4910303 SHA256:1e81f395d8c851c3e4e75b568e20fa2fa549354e75ab397f9de4b0e0790a305f
'http://deb.debian.org/debian/pool/main/m/mythes/mythes_1.2.4-1.debian.tar.xz' mythes_1.2.4-1.debian.tar.xz 5036 SHA256:e8f6f8d0581e9cd20b5bd0f293ede37599e29089f6f8bc174e6d21e346b237dc
```

Likely also available for browsing at:

- https://sources.debian.net/src/mythes/2:1.2.4-1/
- https://sources.debian.net/src/mythes/2:1.2.4-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `ncurses=5.9+20140913-1`

Binary Packages:

- `libncurses5:amd64=5.9+20140913-1+b1`
- `libncursesw5:amd64=5.9+20140913-1+b1`
- `libtinfo5:amd64=5.9+20140913-1+b1`
- `ncurses-base=5.9+20140913-1`
- `ncurses-bin=5.9+20140913-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris ncurses=5.9+20140913-1
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_5.9+20140913-1.dsc' ncurses_5.9+20140913-1.dsc 3463 SHA256:c45d894baa8bd4814e41308edc573e2a5c0f14bdc849925a4a9281e0f3b3b640
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_5.9+20140913.orig.tar.gz' ncurses_5.9+20140913.orig.tar.gz 2987249 SHA256:c4247ad81ee9d743caba8a2db6dd96d36878530b2e76e376af1c00b067a2dec9
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_5.9+20140913-1.debian.tar.xz' ncurses_5.9+20140913-1.debian.tar.xz 51252 SHA256:ff102696241674e40cc0e525ae6cd4b10d249e29f2c77aa9c983af0bcebdd4ff
```

Likely also available for browsing at:

- https://sources.debian.net/src/ncurses/5.9+20140913-1/
- https://sources.debian.net/src/ncurses/5.9+20140913-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `neon27=0.30.1-1`

Binary Packages:

- `libneon27-gnutls=0.30.1-1`

Licenses: (parsed from: `/usr/share/doc/libneon27-gnutls/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris neon27=0.30.1-1
'http://deb.debian.org/debian/pool/main/n/neon27/neon27_0.30.1-1.dsc' neon27_0.30.1-1.dsc 2170 SHA256:bd4e868e95dbd0a4d3b0f007108e808fad689385aef800880f1d8a41b2f1dc4a
'http://deb.debian.org/debian/pool/main/n/neon27/neon27_0.30.1.orig.tar.gz' neon27_0.30.1.orig.tar.gz 911414 SHA256:00c626c0dc18d094ab374dbd9a354915bfe4776433289386ed489c2ec0845cdd
'http://deb.debian.org/debian/pool/main/n/neon27/neon27_0.30.1-1.debian.tar.xz' neon27_0.30.1-1.debian.tar.xz 9128 SHA256:e43215c3188d47968cb380d2e918c151caae1e7132e63526c5cd29487d733b0b
```

Likely also available for browsing at:

- https://sources.debian.net/src/neon27/0.30.1-1/
- https://sources.debian.net/src/neon27/0.30.1-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `netbase=5.3`

Binary Packages:

- `netbase=5.3`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=5.3
'http://deb.debian.org/debian/pool/main/n/netbase/netbase_5.3.dsc' netbase_5.3.dsc 1308 SHA256:fcb9c97fe55277f775fd5a39933ca0189b9a983c6cf1abc8184fc29b8e1d77cb
'http://deb.debian.org/debian/pool/main/n/netbase/netbase_5.3.tar.xz' netbase_5.3.tar.xz 31292 SHA256:81f6c69795044d62b8ad959cf9daf049d0545fd466c52860ad3f933b1e97b88b
```

Likely also available for browsing at:

- https://sources.debian.net/src/netbase/5.3/
- https://sources.debian.net/src/netbase/5.3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `nettle=2.7.1-5+deb8u2`

Binary Packages:

- `libhogweed2:amd64=2.7.1-5+deb8u2`
- `libnettle4:amd64=2.7.1-5+deb8u2`

Licenses: (parsed from: `/usr/share/doc/libhogweed2/copyright`, `/usr/share/doc/libnettle4/copyright`)

- `GAP`
- `GPL`
- `GPL-2`
- `GPL-2+`
- `LGPL`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1+`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris nettle=2.7.1-5+deb8u2
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_2.7.1-5+deb8u2.dsc' nettle_2.7.1-5+deb8u2.dsc 2078 SHA256:9169cedb90e4eb552f4383172b56107c4365a7a43769c9e6d113072abc975223
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_2.7.1.orig.tar.gz' nettle_2.7.1.orig.tar.gz 1558863 SHA256:bc71ebd43435537d767799e414fce88e521b7278d48c860651216e1fc6555b40
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_2.7.1-5+deb8u2.debian.tar.xz' nettle_2.7.1-5+deb8u2.debian.tar.xz 20496 SHA256:0edb103b1268e6b3e8909883c1e9c7416dd75a51c9116047ca60031377e01141
```

Likely also available for browsing at:

- https://sources.debian.net/src/nettle/2.7.1-5+deb8u2/
- https://sources.debian.net/src/nettle/2.7.1-5+deb8u2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `nspr=2:4.12-1+debu8u1`

Binary Packages:

- `libnspr4:amd64=2:4.12-1+debu8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris nspr=2:4.12-1+debu8u1
'http://deb.debian.org/debian/pool/main/n/nspr/nspr_4.12-1+debu8u1.dsc' nspr_4.12-1+debu8u1.dsc 1792 SHA256:421dcd3e6bf4c26793d7c06dddf28945d4cb46829b06160d80a07a8b26244563
'http://deb.debian.org/debian/pool/main/n/nspr/nspr_4.12.orig.tar.gz' nspr_4.12.orig.tar.gz 1135458 SHA256:e0b10a1e569153668ff8bdea6c7e491b389fab69c2f18285a1ebf7c2ea4269de
'http://deb.debian.org/debian/pool/main/n/nspr/nspr_4.12-1+debu8u1.debian.tar.xz' nspr_4.12-1+debu8u1.debian.tar.xz 14276 SHA256:d69e39fd076a58b4aab9809d7defe6505fc327edc421bdfc5b8348ff2d843cf3
```

Likely also available for browsing at:

- https://sources.debian.net/src/nspr/2:4.12-1+debu8u1/
- https://sources.debian.net/src/nspr/2:4.12-1+debu8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `nss=2:3.26-1+debu8u1`

Binary Packages:

- `libnss3:amd64=2:3.26-1+debu8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris nss=2:3.26-1+debu8u1
'http://deb.debian.org/debian/pool/main/n/nss/nss_3.26-1+debu8u1.dsc' nss_3.26-1+debu8u1.dsc 1907 SHA256:778a3f74cd338ef1ee41144bc20648ce0afa0507b8320516d53b98a363f0ade3
'http://deb.debian.org/debian/pool/main/n/nss/nss_3.26.orig.tar.gz' nss_3.26.orig.tar.gz 7386943 SHA256:91783a570ab953693eb977ce47c501f04c104cec287fa011c91bcc8970d1c564
'http://deb.debian.org/debian/pool/main/n/nss/nss_3.26-1+debu8u1.debian.tar.xz' nss_3.26-1+debu8u1.debian.tar.xz 24352 SHA256:b9512797152852d8bd7a71ea8cb6a6e4b77c8c8d98a541cdbf8d2ac78bac67d2
```

Likely also available for browsing at:

- https://sources.debian.net/src/nss/2:3.26-1+debu8u1/
- https://sources.debian.net/src/nss/2:3.26-1+debu8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `openjdk-8=8u121-b13-1~bpo8+1`

Binary Packages:

- `openjdk-8-jre-headless:amd64=8u121-b13-1~bpo8+1`

Licenses: (parsed from: `/usr/share/doc/openjdk-8-jre-headless/copyright`)

- `Apache-2.0`
- `GPL-2`
- `LGPL-2`
- `LGPL-2-1`

Source:

```console
$ apt-get source -qq --print-uris openjdk-8=8u121-b13-1~bpo8+1
'http://deb.debian.org/debian/pool/main/o/openjdk-8/openjdk-8_8u121-b13-1~bpo8+1.dsc' openjdk-8_8u121-b13-1~bpo8+1.dsc 4522 SHA256:ae40bb526fde162d14816d07ee1fecba2f2696feed07d01475a945d2dc721b0a
'http://deb.debian.org/debian/pool/main/o/openjdk-8/openjdk-8_8u121-b13.orig.tar.xz' openjdk-8_8u121-b13.orig.tar.xz 63884892 SHA256:78f64c05575fa36ae35e712e3d23b3ac139aaeb328eebca705705652b5985699
'http://deb.debian.org/debian/pool/main/o/openjdk-8/openjdk-8_8u121-b13-1~bpo8+1.debian.tar.xz' openjdk-8_8u121-b13-1~bpo8+1.debian.tar.xz 235396 SHA256:190d5b0ff30f6085aadccc38cf6d56ce91ba4185b0cb25ae6996c042b4066e34
```

Likely also available for browsing at:

- https://sources.debian.net/src/openjdk-8/8u121-b13-1~bpo8+1/
- https://sources.debian.net/src/openjdk-8/8u121-b13-1~bpo8+1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `openldap=2.4.40+dfsg-1+deb8u2`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.40+dfsg-1+deb8u2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.40+dfsg-1+deb8u2
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.40+dfsg-1+deb8u2.dsc' openldap_2.4.40+dfsg-1+deb8u2.dsc 2819 SHA256:fa6859696d15e6e2a40a940cb4f4356d0c04b5994faf02717f64c1e51517e877
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.40+dfsg.orig.tar.gz' openldap_2.4.40+dfsg.orig.tar.gz 4797667 SHA256:86c0326dc3dc5f1a9b3c25f7106b96f3eafcdf5da090b1fc586dec57d56e0e7f
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.40+dfsg-1+deb8u2.diff.gz' openldap_2.4.40+dfsg-1+deb8u2.diff.gz 179809 SHA256:aa5cb8c89c602c3625e121555de6dea53df051c811da49dc0f4487f4b859061a
```

Likely also available for browsing at:

- https://sources.debian.net/src/openldap/2.4.40+dfsg-1+deb8u2/
- https://sources.debian.net/src/openldap/2.4.40+dfsg-1+deb8u2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `openssl=1.0.1t-1+deb8u6`

Binary Packages:

- `libssl1.0.0:amd64=1.0.1t-1+deb8u6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.0.1t-1+deb8u6
'http://security.debian.org/pool/updates/main/o/openssl/openssl_1.0.1t-1+deb8u6.dsc' openssl_1.0.1t-1+deb8u6.dsc 2272 SHA256:c5d2624a9b9de16a8d173c852e84f175757ee838cd3b5efe44683b96a6aa927b
'http://security.debian.org/pool/updates/main/o/openssl/openssl_1.0.1t.orig.tar.gz' openssl_1.0.1t.orig.tar.gz 4556447 SHA256:4a6ee491a2fdb22e519c76fdc2a628bb3cec12762cd456861d207996c8a07088
'http://security.debian.org/pool/updates/main/o/openssl/openssl_1.0.1t-1+deb8u6.debian.tar.xz' openssl_1.0.1t-1+deb8u6.debian.tar.xz 108424 SHA256:670935107107c20c872174c96c0cd098ffc2c15cac17f5a104af63a1db69cf3a
```

Likely also available for browsing at:

- https://sources.debian.net/src/openssl/1.0.1t-1+deb8u6/
- https://sources.debian.net/src/openssl/1.0.1t-1+deb8u6/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `openssl=1.1.0e-1`

Binary Packages:

- `libssl1.1:amd64=1.1.0e-1`
- `openssl=1.1.0e-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.0e-1
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.0e-1.dsc' openssl_1.1.0e-1.dsc 2583 SHA256:8d813e7a52b4732e0af7cf8cab1436ae7f00e012594c26c401c1eec0e82cfe64
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.0e.orig.tar.gz' openssl_1.1.0e.orig.tar.gz 5202247 SHA256:57be8618979d80c910728cfc99369bf97b2a1abd8f366ab6ebdee8975ad3874c
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.0e.orig.tar.gz.asc' openssl_1.1.0e.orig.tar.gz.asc 455 SHA256:05ab4b1019da59963890509ad9ff3142c72df0b3baf4a38043392aff99e6a13d
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.0e-1.debian.tar.xz' openssl_1.1.0e-1.debian.tar.xz 52864 SHA256:3063329a11696c03f3330991089d4c028c5b0a61ccc3e31e5189ca3b96cd5b3c
```

Likely also available for browsing at:

- https://sources.debian.net/src/openssl/1.1.0e-1/
- https://sources.debian.net/src/openssl/1.1.0e-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `orc=1:0.4.22-1`

Binary Packages:

- `liborc-0.4-0:amd64=1:0.4.22-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris orc=1:0.4.22-1
'http://deb.debian.org/debian/pool/main/o/orc/orc_0.4.22-1.dsc' orc_0.4.22-1.dsc 2394 SHA256:f79dd273ebcd666392f3bd9231fac03bde1dd8cb275d6bffffbae2c7d7e6d235
'http://deb.debian.org/debian/pool/main/o/orc/orc_0.4.22.orig.tar.xz' orc_0.4.22.orig.tar.xz 445792 SHA256:04ca077f4b25f02cc13090effa55343bbfde986c8d663df430347992aa5cf935
'http://deb.debian.org/debian/pool/main/o/orc/orc_0.4.22-1.debian.tar.xz' orc_0.4.22-1.debian.tar.xz 4948 SHA256:a133f9186f2298c4acd9caaf44020dd0102364f31a71a1669158bdea9fabe0f7
```

Likely also available for browsing at:

- https://sources.debian.net/src/orc/1:0.4.22-1/
- https://sources.debian.net/src/orc/1:0.4.22-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `p11-kit=0.20.7-1`

Binary Packages:

- `libp11-kit0:amd64=0.20.7-1`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `This file is distributed under the same license as the debian`
- `This file is distributed under the same license as the p11-kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.20.7-1
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.20.7-1.dsc' p11-kit_0.20.7-1.dsc 2221 SHA256:459d56241f560163471eb5ec789eb5691ca97c5aa9a1bca98dabcf613a2d4bc3
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.20.7.orig.tar.gz' p11-kit_0.20.7.orig.tar.gz 986731 SHA256:68405492fe466b33927d461302aa98e703db3b8a596411585508bc33084484d2
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.20.7-1.debian.tar.xz' p11-kit_0.20.7-1.debian.tar.xz 14208 SHA256:515dfcc279d284bfbee4d172c9cf1db3befe52d55e6d3f50d024c8f72d56574d
```

Likely also available for browsing at:

- https://sources.debian.net/src/p11-kit/0.20.7-1/
- https://sources.debian.net/src/p11-kit/0.20.7-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `pam=1.1.8-3.1+deb8u2`

Binary Packages:

- `libpam-modules:amd64=1.1.8-3.1+deb8u2`
- `libpam-modules-bin=1.1.8-3.1+deb8u2`
- `libpam-runtime=1.1.8-3.1+deb8u2`
- `libpam0g:amd64=1.1.8-3.1+deb8u2`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.1.8-3.1+deb8u2
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.1.8-3.1+deb8u2.dsc' pam_1.1.8-3.1+deb8u2.dsc 2504 SHA256:0dcab55550af17b5f2779b5749930a69ea54302d8f8ef1bdd1a8dea3ed4e0619
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.1.8.orig.tar.gz' pam_1.1.8.orig.tar.gz 1892765 SHA256:4183409a450708a976eca5af561dbf4f0490141a08e86e4a1e649c7c1b094876
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.1.8-3.1+deb8u2.diff.gz' pam_1.1.8-3.1+deb8u2.diff.gz 134897 SHA256:84a455ce53c7701d2a536fc33909a6ce19c1a6b7c18e6be8d2d0fc2294260610
```

Likely also available for browsing at:

- https://sources.debian.net/src/pam/1.1.8-3.1+deb8u2/
- https://sources.debian.net/src/pam/1.1.8-3.1+deb8u2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `pango1.0=1.36.8-3`

Binary Packages:

- `libpango-1.0-0:amd64=1.36.8-3`
- `libpangocairo-1.0-0:amd64=1.36.8-3`
- `libpangoft2-1.0-0:amd64=1.36.8-3`

Licenses: (parsed from: `/usr/share/doc/libpango-1.0-0/copyright`, `/usr/share/doc/libpangocairo-1.0-0/copyright`, `/usr/share/doc/libpangoft2-1.0-0/copyright`)

- `LGPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris pango1.0=1.36.8-3
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.36.8-3.dsc' pango1.0_1.36.8-3.dsc 3169 SHA256:8a0e51c2c4a33e4136dd4cabe670b265e48cf92e740d6d9889623c2183940a1e
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.36.8.orig.tar.xz' pango1.0_1.36.8.orig.tar.xz 1033528 SHA256:18dbb51b8ae12bae0ab7a958e7cf3317c9acfc8a1e1103ec2f147164a0fc2d07
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.36.8-3.debian.tar.xz' pango1.0_1.36.8-3.debian.tar.xz 31668 SHA256:4249e9e29a186994abe8d5d57debc81c446916a6c7ea872171597c4df4d8f6ea
```

Likely also available for browsing at:

- https://sources.debian.net/src/pango1.0/1.36.8-3/
- https://sources.debian.net/src/pango1.0/1.36.8-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `pcre3=2:8.35-3.3+deb8u4`

Binary Packages:

- `libpcre3:amd64=2:8.35-3.3+deb8u4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.35-3.3+deb8u4
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.35-3.3+deb8u4.dsc' pcre3_8.35-3.3+deb8u4.dsc 1985 SHA256:862ee7365c8cc9916f58856617701e2e2f3dcd384a34375379ddfa52b642c649
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.35.orig.tar.gz' pcre3_8.35.orig.tar.gz 1996552 SHA256:1c9ee292943ba2737f127b481a3f72f44c13fbd09a7b5b4eb8fa58650cfa56a0
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.35-3.3+deb8u4.debian.tar.gz' pcre3_8.35-3.3+deb8u4.debian.tar.gz 38081 SHA256:93e38ad38d4cdb21d346226eebc7e2ad419cbfe0261b27d2910e8e5c3a946fb9
```

Likely also available for browsing at:

- https://sources.debian.net/src/pcre3/2:8.35-3.3+deb8u4/
- https://sources.debian.net/src/pcre3/2:8.35-3.3+deb8u4/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `pcsc-lite=1.8.13-1+deb8u1`

Binary Packages:

- `libpcsclite1:amd64=1.8.13-1+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libpcsclite1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-3`
- `GPL-3+`
- `ISC`

Source:

```console
$ apt-get source -qq --print-uris pcsc-lite=1.8.13-1+deb8u1
'http://deb.debian.org/debian/pool/main/p/pcsc-lite/pcsc-lite_1.8.13-1+deb8u1.dsc' pcsc-lite_1.8.13-1+deb8u1.dsc 2252 SHA256:325efa1f879f04a80447077b4fae1bcac2b6886cd9c7b3459ee22ca3050df268
'http://deb.debian.org/debian/pool/main/p/pcsc-lite/pcsc-lite_1.8.13.orig.tar.bz2' pcsc-lite_1.8.13.orig.tar.bz2 584083 SHA256:f315047e808d63a3262c4a040f77548af2e04d1fd707e0c2759369b926fbbc3b
'http://deb.debian.org/debian/pool/main/p/pcsc-lite/pcsc-lite_1.8.13-1+deb8u1.debian.tar.xz' pcsc-lite_1.8.13-1+deb8u1.debian.tar.xz 15700 SHA256:61e89cdd33e5f189de19ad3465d3bd40f2a5326c84dcc04e8d6519f7a74edf66
```

Likely also available for browsing at:

- https://sources.debian.net/src/pcsc-lite/1.8.13-1+deb8u1/
- https://sources.debian.net/src/pcsc-lite/1.8.13-1+deb8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `perl=5.20.2-3+deb8u6`

Binary Packages:

- `perl=5.20.2-3+deb8u6`
- `perl-base=5.20.2-3+deb8u6`
- `perl-modules=5.20.2-3+deb8u6`

Licenses: (parsed from: `/usr/share/doc/perl/copyright`, `/usr/share/doc/perl-base/copyright`, `/usr/share/doc/perl-modules/copyright`)

- `Artistic`
- `Artistic,`
- `Artistic-2`
- `BSD-3-clause`
- `BSD-3-clause-GENERIC`
- `BSD-4-clause`
- `BSD-4-clause-POWERDOG`
- `BZIP`
- `DONT-CHANGE-THE-GPL`
- `Expat`
- `GPL-1`
- `GPL-1+`
- `GPL-2+`
- `GPL-3+-WITH-BISON-EXCEPTION`
- `HSIEH-BSD`
- `HSIEH-DERIVATIVE`
- `LGPL-2.1`
- `REGCOMP`
- `REGCOMP,`
- `S2P`
- `SDBM-PUBLIC-DOMAIN`
- `TEXT-TABS`
- `Unicode`
- `ZLIB`

Source:

```console
$ apt-get source -qq --print-uris perl=5.20.2-3+deb8u6
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.20.2-3+deb8u6.dsc' perl_5.20.2-3+deb8u6.dsc 2322 SHA256:b7569ffa209fcd84bc4d487a9c242b21b0db591b3a9222ae0e1140bab67c6106
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.20.2.orig.tar.bz2' perl_5.20.2.orig.tar.bz2 13717128 SHA256:e5a4713bc65e1da98ebd833dce425c000768bfe84d17ec5183ec5ca249db71ab
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.20.2-3+deb8u6.debian.tar.xz' perl_5.20.2-3+deb8u6.debian.tar.xz 147848 SHA256:f6d31a96ea22b2f2626bb017c4960bcbdf1ac1e11e5639175cd9418fdccda812
```

Likely also available for browsing at:

- https://sources.debian.net/src/perl/5.20.2-3+deb8u6/
- https://sources.debian.net/src/perl/5.20.2-3+deb8u6/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `pixman=0.32.6-3`

Binary Packages:

- `libpixman-1-0:amd64=0.32.6-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pixman=0.32.6-3
'http://deb.debian.org/debian/pool/main/p/pixman/pixman_0.32.6-3.dsc' pixman_0.32.6-3.dsc 2002 SHA256:bc1090a051b5ce887976c06e8f1e389941f906bc6fc5b95f88a17cc2f5f887f1
'http://deb.debian.org/debian/pool/main/p/pixman/pixman_0.32.6.orig.tar.gz' pixman_0.32.6.orig.tar.gz 816702 SHA256:3dfed13b8060eadabf0a4945c7045b7793cc7e3e910e748a8bb0f0dc3e794904
'http://deb.debian.org/debian/pool/main/p/pixman/pixman_0.32.6-3.diff.gz' pixman_0.32.6-3.diff.gz 283461 SHA256:d7343e301c4c79a931d38cfb3fcf6189c50a6904b3a26ea484481cba4fdef13c
```

Likely also available for browsing at:

- https://sources.debian.net/src/pixman/0.32.6-3/
- https://sources.debian.net/src/pixman/0.32.6-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `procps=2:3.3.9-9`

Binary Packages:

- `libprocps3:amd64=2:3.3.9-9`
- `procps=2:3.3.9-9`

Licenses: (parsed from: `/usr/share/doc/libprocps3/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.9-9
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.9-9.dsc' procps_3.3.9-9.dsc 2052 SHA256:b4ee0cb8b2cfb6362bf5a9b6ad2ac1a921098638c8c396fae5823080a159935d
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.9.orig.tar.xz' procps_3.3.9.orig.tar.xz 560812 SHA256:00f0cb0fadf968ddf605b0ef119846af07386629244d4f3da711a2cecf4e8663
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.9-9.debian.tar.xz' procps_3.3.9-9.debian.tar.xz 35096 SHA256:d66ade0f2d1b44ef55404cc612e25c0f031e7ed2f05e5ab628a0de8c27ed19bf
```

Likely also available for browsing at:

- https://sources.debian.net/src/procps/2:3.3.9-9/
- https://sources.debian.net/src/procps/2:3.3.9-9/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `python3-defaults=3.4.2-2`

Binary Packages:

- `libpython3-stdlib:amd64=3.4.2-2`
- `python3=3.4.2-2`
- `python3-minimal=3.4.2-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.4.2-2
'http://deb.debian.org/debian/pool/main/p/python3-defaults/python3-defaults_3.4.2-2.dsc' python3-defaults_3.4.2-2.dsc 2739 SHA256:9e259f8755d6bd7f8c1a20d1110725248c416d09b9c4de7adc32c21e59703030
'http://deb.debian.org/debian/pool/main/p/python3-defaults/python3-defaults_3.4.2-2.tar.gz' python3-defaults_3.4.2-2.tar.gz 128541 SHA256:96ef5763cae104c181fcf530f84a16537b5727ebc41f1ae6482ce18775556bcf
```

Likely also available for browsing at:

- https://sources.debian.net/src/python3-defaults/3.4.2-2/
- https://sources.debian.net/src/python3-defaults/3.4.2-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `python3.4=3.4.2-1`

Binary Packages:

- `libpython3.4:amd64=3.4.2-1`
- `libpython3.4-minimal:amd64=3.4.2-1`
- `libpython3.4-stdlib:amd64=3.4.2-1`
- `python3.4=3.4.2-1`
- `python3.4-minimal=3.4.2-1`

Licenses: (parsed from: `/usr/share/doc/libpython3.4/copyright`, `/usr/share/doc/libpython3.4-minimal/copyright`, `/usr/share/doc/libpython3.4-stdlib/copyright`, `/usr/share/doc/python3.4/copyright`, `/usr/share/doc/python3.4-minimal/copyright`)

- `* Permission to use this software in any way is granted without`
- `By obtaining, using, and/or copying this software and/or its`
- `GPL-2`
- `Permission  is  hereby granted,  free  of charge,  to  any person`
- `Permission is hereby granted, free of charge, to any person obtaining`
- `Permission to use, copy, modify,`
- `Redistribution`
- `This software is provided 'as-is', without any express`
- `This software is provided as-is, without express`
- `binary forms, with`
- `distribute this software`
- `distribute this software and`
- `distribute this software for any`
- `implied`
- `its`
- `use in source`
- `without`

Source:

```console
$ apt-get source -qq --print-uris python3.4=3.4.2-1
'http://deb.debian.org/debian/pool/main/p/python3.4/python3.4_3.4.2-1.dsc' python3.4_3.4.2-1.dsc 2584 SHA256:339ada67a26d2fe70184294ee38bc85b5cfb79bb0b67707ed028853c869337ce
'http://deb.debian.org/debian/pool/main/p/python3.4/python3.4_3.4.2.orig.tar.gz' python3.4_3.4.2.orig.tar.gz 19380599 SHA256:29fe97d2e197ed25651beb233314121039477e96b4da5ec27cd317e9396a9d72
'http://deb.debian.org/debian/pool/main/p/python3.4/python3.4_3.4.2-1.diff.gz' python3.4_3.4.2-1.diff.gz 348260 SHA256:3b5ad5196a4b8e368a10c78e2c72ab0b06a5a9509da7ddf346d35dd9c1a40f2c
```

Likely also available for browsing at:

- https://sources.debian.net/src/python3.4/3.4.2-1/
- https://sources.debian.net/src/python3.4/3.4.2-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `raptor2=2.0.14-1`

Binary Packages:

- `libraptor2-0:amd64=2.0.14-1`

Licenses: (parsed from: `/usr/share/doc/libraptor2-0/copyright`)

- `Apache-2.0`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris raptor2=2.0.14-1
'http://deb.debian.org/debian/pool/main/r/raptor2/raptor2_2.0.14-1.dsc' raptor2_2.0.14-1.dsc 1455 SHA256:9cee0bfac55f8b7fe7d72e3780de235f4dd5309ca89e5afaed302dfed0e1221a
'http://deb.debian.org/debian/pool/main/r/raptor2/raptor2_2.0.14.orig.tar.gz' raptor2_2.0.14.orig.tar.gz 1877454 SHA256:cb447b7c684cbe60f1266d622691fd20fdcf7b91f4a470c6de5fc8e8961df1b2
'http://deb.debian.org/debian/pool/main/r/raptor2/raptor2_2.0.14-1.debian.tar.xz' raptor2_2.0.14-1.debian.tar.xz 7624 SHA256:2b13e72202c99570f225f378318cdceca38ee130e7a24e46881e7672ea2b8758
```

Likely also available for browsing at:

- https://sources.debian.net/src/raptor2/2.0.14-1/
- https://sources.debian.net/src/raptor2/2.0.14-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `rasqal=0.9.32-1`

Binary Packages:

- `librasqal3:amd64=0.9.32-1`

Licenses: (parsed from: `/usr/share/doc/librasqal3/copyright`)

- `Apache-2.0`
- `Apache-2.0+`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris rasqal=0.9.32-1
'http://deb.debian.org/debian/pool/main/r/rasqal/rasqal_0.9.32-1.dsc' rasqal_0.9.32-1.dsc 1360 SHA256:fd0ecaa94c86647ee855def087955b01f0bfe2933c8471c83d2094d7b60f84ce
'http://deb.debian.org/debian/pool/main/r/rasqal/rasqal_0.9.32.orig.tar.gz' rasqal_0.9.32.orig.tar.gz 1544623 SHA256:eeba03218e3b7dfa033934d523a1a64671a9a0f64eadc38a01e4b43367be2e8f
'http://deb.debian.org/debian/pool/main/r/rasqal/rasqal_0.9.32-1.debian.tar.xz' rasqal_0.9.32-1.debian.tar.xz 5888 SHA256:02c3a4303f0a5afb84de6a06303aac1684ed900eb49a5f517222734b3d0caea6
```

Likely also available for browsing at:

- https://sources.debian.net/src/rasqal/0.9.32-1/
- https://sources.debian.net/src/rasqal/0.9.32-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `readline6=6.3-8`

Binary Packages:

- `libreadline6:amd64=6.3-8+b3`
- `readline-common=6.3-8`

Licenses: (parsed from: `/usr/share/doc/libreadline6/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline6=6.3-8
'http://deb.debian.org/debian/pool/main/r/readline6/readline6_6.3-8.dsc' readline6_6.3-8.dsc 1941 SHA256:f7ab77b8580cbdb10b3906f40c3da12d0acc93bef786ff217c65aabc32973cec
'http://deb.debian.org/debian/pool/main/r/readline6/readline6_6.3.orig.tar.gz' readline6_6.3.orig.tar.gz 2468560 SHA256:56ba6071b9462f980c5a72ab0023893b65ba6debb4eeb475d7a563dc65cafd43
'http://deb.debian.org/debian/pool/main/r/readline6/readline6_6.3-8.debian.tar.xz' readline6_6.3-8.debian.tar.xz 30576 SHA256:c2b55fdd221136f46fa1e0cbf0bf2e37b70ddf97929312fbab6032e9129d58b5
```

Likely also available for browsing at:

- https://sources.debian.net/src/readline6/6.3-8/
- https://sources.debian.net/src/readline6/6.3-8/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `redland=1.0.17-1`

Binary Packages:

- `librdf0:amd64=1.0.17-1+b1`

Licenses: (parsed from: `/usr/share/doc/librdf0/copyright`)

- `Apache-2.0`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris redland=1.0.17-1
'http://deb.debian.org/debian/pool/main/r/redland/redland_1.0.17-1.dsc' redland_1.0.17-1.dsc 1633 SHA256:dc797129337f8cd75b85323ba700dbe7cff5cbbf182f7283b73d335e2e54c1f9
'http://deb.debian.org/debian/pool/main/r/redland/redland_1.0.17.orig.tar.gz' redland_1.0.17.orig.tar.gz 1621566 SHA256:de1847f7b59021c16bdc72abb4d8e2d9187cd6124d69156f3326dd34ee043681
'http://deb.debian.org/debian/pool/main/r/redland/redland_1.0.17-1.debian.tar.gz' redland_1.0.17-1.debian.tar.gz 9049 SHA256:525bbd9228fe81fff3abd515972c7e431d416699411aaf7391c54a6fee178008
```

Likely also available for browsing at:

- https://sources.debian.net/src/redland/1.0.17-1/
- https://sources.debian.net/src/redland/1.0.17-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `rtmpdump=2.4+20150115.gita107cef-1`

Binary Packages:

- `librtmp1:amd64=2.4+20150115.gita107cef-1`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20150115.gita107cef-1
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4+20150115.gita107cef-1.dsc' rtmpdump_2.4+20150115.gita107cef-1.dsc 2257 SHA256:acfa72b9e6e0a96b4a514201b2e11e8ec9ae3173596f0467f6a5eb300d5fecdd
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4+20150115.gita107cef.orig.tar.gz' rtmpdump_2.4+20150115.gita107cef.orig.tar.gz 142030 SHA256:d47ef3a07815079bf73eb5d053001c4341407fcbebf39f34e6213c4b772cb29a
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4+20150115.gita107cef-1.debian.tar.xz' rtmpdump_2.4+20150115.gita107cef-1.debian.tar.xz 7004 SHA256:68d430d4f97be9767674920fb0a7821761ad1633578aa3cd6144b919ebbfcca4
```

Likely also available for browsing at:

- https://sources.debian.net/src/rtmpdump/2.4+20150115.gita107cef-1/
- https://sources.debian.net/src/rtmpdump/2.4+20150115.gita107cef-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `sed=4.2.2-4+deb8u1`

Binary Packages:

- `sed=4.2.2-4+deb8u1`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris sed=4.2.2-4+deb8u1
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.2.2-4+deb8u1.dsc' sed_4.2.2-4+deb8u1.dsc 1495 SHA256:c8f47bac04e1b1d59fc433de2f977c6d08e40eefbdb10cabb7650297c0c12929
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.2.2.orig.tar.bz2' sed_4.2.2.orig.tar.bz2 1059414 SHA256:f048d1838da284c8bc9753e4506b85a1e0cc1ea8999d36f6995bcb9460cddbd7
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.2.2-4+deb8u1.debian.tar.xz' sed_4.2.2-4+deb8u1.debian.tar.xz 57724 SHA256:ba9b84ebb251edc7c78b3b4c715cfacc6fdd263997a92269a0282469d226557d
```

Likely also available for browsing at:

- https://sources.debian.net/src/sed/4.2.2-4+deb8u1/
- https://sources.debian.net/src/sed/4.2.2-4+deb8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `sensible-utils=0.0.9`

Binary Packages:

- `sensible-utils=0.0.9`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.9
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.9.dsc' sensible-utils_0.0.9.dsc 1405 SHA256:390c29b31a09ab7f31f8b5fc0fd82e47c25f15b22b17c614fb87f12d3b091070
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.9.tar.gz' sensible-utils_0.0.9.tar.gz 74331 SHA256:6fcb5cc0f7f1cf80421840cfa17b1b3fa5afaf3fe852dc984a789023af2f70c6
```

Likely also available for browsing at:

- https://sources.debian.net/src/sensible-utils/0.0.9/
- https://sources.debian.net/src/sensible-utils/0.0.9/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `shadow=1:4.2-3+deb8u3`

Binary Packages:

- `login=1:4.2-3+deb8u3`
- `passwd=1:4.2-3+deb8u3`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.2-3+deb8u3
'http://security.debian.org/pool/updates/main/s/shadow/shadow_4.2-3+deb8u3.dsc' shadow_4.2-3+deb8u3.dsc 2492 SHA256:95e6fd479bc7721f71b2e3cbfe65776f021d1338cc4906ad880e5383129a096a
'http://security.debian.org/pool/updates/main/s/shadow/shadow_4.2.orig.tar.xz' shadow_4.2.orig.tar.xz 1088696 SHA256:c5bd72c4ecb438b99289e4630b22ea0626987a378d084910dbe59eceaa34be1d
'http://security.debian.org/pool/updates/main/s/shadow/shadow_4.2-3+deb8u3.debian.tar.xz' shadow_4.2-3+deb8u3.debian.tar.xz 498396 SHA256:2d4b93667a1f09433725e457c74b6215d31386e2e42bd192c26d34d3592444be
```

Likely also available for browsing at:

- https://sources.debian.net/src/shadow/1:4.2-3+deb8u3/
- https://sources.debian.net/src/shadow/1:4.2-3+deb8u3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `shared-mime-info=1.3-1`

Binary Packages:

- `shared-mime-info=1.3-1`

Licenses: (parsed from: `/usr/share/doc/shared-mime-info/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris shared-mime-info=1.3-1
'http://deb.debian.org/debian/pool/main/s/shared-mime-info/shared-mime-info_1.3-1.dsc' shared-mime-info_1.3-1.dsc 2265 SHA256:76ca2921de722cd4e17bcffadbb55f74e4730e99d8fe5cff13ad05178785c691
'http://deb.debian.org/debian/pool/main/s/shared-mime-info/shared-mime-info_1.3.orig.tar.xz' shared-mime-info_1.3.orig.tar.xz 517420 SHA256:4fd49c8c7ca9ecb10c59845094a18dbb73b69c72b4bad3db5e864f2111cb323a
'http://deb.debian.org/debian/pool/main/s/shared-mime-info/shared-mime-info_1.3-1.debian.tar.xz' shared-mime-info_1.3-1.debian.tar.xz 10060 SHA256:ba82b382b1fcf6a27bb410155f11b7e7d6499c3302781990e9b747b342c2e7d8
```

Likely also available for browsing at:

- https://sources.debian.net/src/shared-mime-info/1.3-1/
- https://sources.debian.net/src/shared-mime-info/1.3-1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `slang2=2.3.0-2`

Binary Packages:

- `libslang2:amd64=2.3.0-2`

Licenses: (parsed from: `/usr/share/doc/libslang2/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris slang2=2.3.0-2
'http://deb.debian.org/debian/pool/main/s/slang2/slang2_2.3.0-2.dsc' slang2_2.3.0-2.dsc 2329 SHA256:2d6ede702782aec9758a3fb6001837ef6d2191d3989db63aa55333da74d5b05e
'http://deb.debian.org/debian/pool/main/s/slang2/slang2_2.3.0.orig.tar.xz' slang2_2.3.0.orig.tar.xz 1250392 SHA256:cdd5b9582959b3afdae403ee6f4be9de8efc7e205e4a7de18c1a847ea5ef0472
'http://deb.debian.org/debian/pool/main/s/slang2/slang2_2.3.0-2.debian.tar.xz' slang2_2.3.0-2.debian.tar.xz 21864 SHA256:8b088f54be2a284eedee56d74968feb4cc662410d352280a7e351cc02bef57b2
```

Likely also available for browsing at:

- https://sources.debian.net/src/slang2/2.3.0-2/
- https://sources.debian.net/src/slang2/2.3.0-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `sqlite3=3.8.7.1-1+deb8u2`

Binary Packages:

- `libsqlite3-0:amd64=3.8.7.1-1+deb8u2`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.8.7.1-1+deb8u2
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.8.7.1-1+deb8u2.dsc' sqlite3_3.8.7.1-1+deb8u2.dsc 2540 SHA256:a99074d920a3b6c95bbc55402ff62ccddbfeed2f1a0ed63423bf79e7e4faeff9
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.8.7.1.orig-www.tar.bz2' sqlite3_3.8.7.1.orig-www.tar.bz2 3337784 SHA256:e642657752f20144f42d002895510ea635e0384b14f276f1a2f281b73252bc64
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.8.7.1.orig.tar.bz2' sqlite3_3.8.7.1.orig.tar.bz2 4082068 SHA256:2632a999feba925aa0f1828fa669a091b165a719676765fb542f538345bfa7b9
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.8.7.1-1+deb8u2.debian.tar.xz' sqlite3_3.8.7.1-1+deb8u2.debian.tar.xz 20428 SHA256:e3ef272994d4423c0dbed82c1171d774d7c0a459db44eb1750a4a61d719fbbd2
```

Likely also available for browsing at:

- https://sources.debian.net/src/sqlite3/3.8.7.1-1+deb8u2/
- https://sources.debian.net/src/sqlite3/3.8.7.1-1+deb8u2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `startpar=0.59-3`

Binary Packages:

- `startpar=0.59-3`

Licenses: (parsed from: `/usr/share/doc/startpar/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris startpar=0.59-3
'http://deb.debian.org/debian/pool/main/s/startpar/startpar_0.59-3.dsc' startpar_0.59-3.dsc 1496 SHA256:f8fdfac7902c1b0cf5d627421893deaa8e041e9e23096ae60a33fe84464526ff
'http://deb.debian.org/debian/pool/main/s/startpar/startpar_0.59.orig.tar.bz2' startpar_0.59.orig.tar.bz2 22747 SHA256:30a30c8d27a694e3743c1839fb6f60563b2882cddf0e61c698120c4cbde1d7b9
'http://deb.debian.org/debian/pool/main/s/startpar/startpar_0.59-3.debian.tar.xz' startpar_0.59-3.debian.tar.xz 38428 SHA256:abd4650e507cd4e63e7caf2199972b6ee5367aea34ae8f53a19caf126bd2248c
```

Likely also available for browsing at:

- https://sources.debian.net/src/startpar/0.59-3/
- https://sources.debian.net/src/startpar/0.59-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `suitesparse=1:4.2.1-3`

Binary Packages:

- `libcolamd2.8.0:amd64=1:4.2.1-3`

Licenses: (parsed from: `/usr/share/doc/libcolamd2.8.0/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL, GPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris suitesparse=1:4.2.1-3
'http://deb.debian.org/debian/pool/main/s/suitesparse/suitesparse_4.2.1-3.dsc' suitesparse_4.2.1-3.dsc 2841 SHA256:81499792d7fd28abc5b8e76a2b87a87c80ca291581e05af66f0dab57373a645b
'http://deb.debian.org/debian/pool/main/s/suitesparse/suitesparse_4.2.1.orig.tar.gz' suitesparse_4.2.1.orig.tar.gz 22544250 SHA256:7ec70a8b65576559daae3bbe61fb29be4ccb5dbb765c43d66a0ee9a42df68b5f
'http://deb.debian.org/debian/pool/main/s/suitesparse/suitesparse_4.2.1-3.debian.tar.gz' suitesparse_4.2.1-3.debian.tar.gz 23261 SHA256:64e413d09425bf2dd6d64272fdfb652d14d6cc0760ab84077a7342e7ae757622
```

Likely also available for browsing at:

- https://sources.debian.net/src/suitesparse/1:4.2.1-3/
- https://sources.debian.net/src/suitesparse/1:4.2.1-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `systemd=215-17+deb8u6`

Binary Packages:

- `libsystemd0:amd64=215-17+deb8u6`
- `libudev1:amd64=215-17+deb8u6`
- `systemd=215-17+deb8u6`
- `systemd-sysv=215-17+deb8u6`
- `udev=215-17+deb8u6`

Licenses: (parsed from: `/usr/share/doc/libsystemd0/copyright`, `/usr/share/doc/libudev1/copyright`, `/usr/share/doc/systemd/copyright`, `/usr/share/doc/systemd-sysv/copyright`, `/usr/share/doc/udev/copyright`)

- `Expat`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris systemd=215-17+deb8u6
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_215-17+deb8u6.dsc' systemd_215-17+deb8u6.dsc 4149 SHA256:2cdd3d1dec1d772d6a7e0c5be9c750ea2d24fd59382f889112302dbfd10d1ddc
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_215.orig.tar.xz' systemd_215.orig.tar.xz 2888652 SHA256:ce76a3c05e7d4adc806a3446a5510c0c9b76a33f19adc32754b69a0945124505
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_215-17+deb8u6.debian.tar.xz' systemd_215-17+deb8u6.debian.tar.xz 221404 SHA256:b44d9676923cccb9f10b1c6385fd3e1d080621760c9ccb43c898b8b03096ee76
```

Likely also available for browsing at:

- https://sources.debian.net/src/systemd/215-17+deb8u6/
- https://sources.debian.net/src/systemd/215-17+deb8u6/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `sysvinit=2.88dsf-59`

Binary Packages:

- `initscripts=2.88dsf-59`
- `sysv-rc=2.88dsf-59`
- `sysvinit-utils=2.88dsf-59`

Licenses: (parsed from: `/usr/share/doc/initscripts/copyright`, `/usr/share/doc/sysv-rc/copyright`, `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.88dsf-59
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.88dsf-59.dsc' sysvinit_2.88dsf-59.dsc 2467 SHA256:0201f6d34c1be692ac0e594a4006e7e0b921eda7ffb37b4373abc949bf7181b2
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.88dsf.orig.tar.gz' sysvinit_2.88dsf.orig.tar.gz 125330 SHA256:b016f937958d2809a020d407e1287bdc09abf1d44efaa96530e2ea57f544f4e8
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.88dsf-59.debian.tar.xz' sysvinit_2.88dsf-59.debian.tar.xz 152316 SHA256:cfd1ff3423b7cfb2239f2311088eba8e5b8abde1835cb25806fb0983d159635f
```

Likely also available for browsing at:

- https://sources.debian.net/src/sysvinit/2.88dsf-59/
- https://sources.debian.net/src/sysvinit/2.88dsf-59/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `tar=1.27.1-2+deb8u1`

Binary Packages:

- `tar=1.27.1-2+deb8u1`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.27.1-2+deb8u1
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.27.1-2+deb8u1.dsc' tar_1.27.1-2+deb8u1.dsc 2049 SHA256:e42e96a9cdf325d7f030306735a1380276670deb72541a7f97ffe59a1e32e67b
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.27.1.orig.tar.xz' tar_1.27.1.orig.tar.xz 1704252 SHA256:58169c5a03c04be20d3fb91010b01e822c6a58060a96e7cf2f9c1944de0151ab
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.27.1-2+deb8u1.debian.tar.xz' tar_1.27.1-2+deb8u1.debian.tar.xz 32632 SHA256:dc2e495770f6c1c79a4e299d4008c8cb1f91a48e823751bc95d7f26ae498f995
```

Likely also available for browsing at:

- https://sources.debian.net/src/tar/1.27.1-2+deb8u1/
- https://sources.debian.net/src/tar/1.27.1-2+deb8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `tiff=4.0.3-12.3+deb8u2`

Binary Packages:

- `libtiff5:amd64=4.0.3-12.3+deb8u2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tiff=4.0.3-12.3+deb8u2
'http://security.debian.org/pool/updates/main/t/tiff/tiff_4.0.3-12.3+deb8u2.dsc' tiff_4.0.3-12.3+deb8u2.dsc 2240 SHA256:6a2dd52c52bccdc8404be32a55c2e26fa0077736a5d8e3644123e6155866ac45
'http://security.debian.org/pool/updates/main/t/tiff/tiff_4.0.3.orig.tar.gz' tiff_4.0.3.orig.tar.gz 2051630 SHA256:ea1aebe282319537fb2d4d7805f478dd4e0e05c33d0928baba76a7c963684872
'http://security.debian.org/pool/updates/main/t/tiff/tiff_4.0.3-12.3+deb8u2.debian.tar.xz' tiff_4.0.3-12.3+deb8u2.debian.tar.xz 43512 SHA256:0f5eb5da8fd6c9b334db2cb715e9c747e1173e5f9288daeb2036108f9cfefb90
```

Likely also available for browsing at:

- https://sources.debian.net/src/tiff/4.0.3-12.3+deb8u2/
- https://sources.debian.net/src/tiff/4.0.3-12.3+deb8u2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `tzdata=2017a-0+deb8u1`

Binary Packages:

- `tzdata=2017a-0+deb8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!


### `dpkg` source package: `ucf=3.0030`

Binary Packages:

- `ucf=3.0030`

Licenses: (parsed from: `/usr/share/doc/ucf/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ucf=3.0030
'http://deb.debian.org/debian/pool/main/u/ucf/ucf_3.0030.dsc' ucf_3.0030.dsc 1300 SHA256:7e1861964217317a6be7fe83c1baaeb578e27a33850c33f14d168e40811b9115
'http://deb.debian.org/debian/pool/main/u/ucf/ucf_3.0030.tar.xz' ucf_3.0030.tar.xz 63524 SHA256:65b681c509f49bca586f12d57c5244ad93cf0d047f886e307fb2018abf3d802d
```

Likely also available for browsing at:

- https://sources.debian.net/src/ucf/3.0030/
- https://sources.debian.net/src/ucf/3.0030/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `unzip=6.0-16+deb8u2`

Binary Packages:

- `unzip=6.0-16+deb8u2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-16+deb8u2
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0-16+deb8u2.dsc' unzip_6.0-16+deb8u2.dsc 1685 SHA256:846d77076dffaa675160c98678919ce3f8a5e1c4e3c1652a197af94b95f7f2c1
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA256:036d96991646d0449ed0aa952e4fbe21b476ce994abc276e49d30e686708bd37
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0-16+deb8u2.debian.tar.xz' unzip_6.0-16+deb8u2.debian.tar.xz 15448 SHA256:121816256cf3d7064558c67ce071343699272a04bf65f4d133f0b889a2274aae
```

Likely also available for browsing at:

- https://sources.debian.net/src/unzip/6.0-16+deb8u2/
- https://sources.debian.net/src/unzip/6.0-16+deb8u2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `ustr=1.0.4-3`

Binary Packages:

- `libustr-1.0-1:amd64=1.0.4-3+b2`

Licenses: (parsed from: `/usr/share/doc/libustr-1.0-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris ustr=1.0.4-3
'http://deb.debian.org/debian/pool/main/u/ustr/ustr_1.0.4-3.dsc' ustr_1.0.4-3.dsc 1992 SHA256:ca6043d523fd9f677446b6cac95ce5263768f3ccc5ee38ef10e1551b2cf1c00a
'http://deb.debian.org/debian/pool/main/u/ustr/ustr_1.0.4.orig.tar.gz' ustr_1.0.4.orig.tar.gz 301345 SHA256:4d293b6b9d9fe51d58441f4b09b1f0005fcad8256ae8048587789bf5dbefb62e
'http://deb.debian.org/debian/pool/main/u/ustr/ustr_1.0.4-3.diff.gz' ustr_1.0.4-3.diff.gz 11415 SHA256:8349cbdef416e9b919d434c6a88c7e29700a00df3e81f21b7d8127ffd7e4945a
```

Likely also available for browsing at:

- https://sources.debian.net/src/ustr/1.0.4-3/
- https://sources.debian.net/src/ustr/1.0.4-3/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `util-linux=2.25.2-6`

Binary Packages:

- `bsdutils=1:2.25.2-6`
- `libblkid1:amd64=2.25.2-6`
- `libmount1:amd64=2.25.2-6`
- `libsmartcols1:amd64=2.25.2-6`
- `libuuid1:amd64=2.25.2-6`
- `mount=2.25.2-6`
- `util-linux=2.25.2-6`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`)

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

Source:

```console
$ apt-get source -qq --print-uris util-linux=2.25.2-6
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.25.2-6.dsc' util-linux_2.25.2-6.dsc 3443 SHA256:742a9c6378132c30d4bfc31722904e73a608c2fee1eab89d1d832c5e5672a82f
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.25.2.orig.tar.xz' util-linux_2.25.2.orig.tar.xz 3703644 SHA256:e0457f715b73f4a349e1acb08cb410bf0edc9a74a3f75c357070f31f70e33cd6
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.25.2-6.debian.tar.xz' util-linux_2.25.2-6.debian.tar.xz 304292 SHA256:b500d70a60f2814d6552492cee5f40c27063029ef74ddea53bc713503680527b
```

Likely also available for browsing at:

- https://sources.debian.net/src/util-linux/2.25.2-6/
- https://sources.debian.net/src/util-linux/2.25.2-6/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `wget=1.16-1+deb8u1`

Binary Packages:

- `wget=1.16-1+deb8u1`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.16-1+deb8u1
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.16-1+deb8u1.dsc' wget_1.16-1+deb8u1.dsc 1769 SHA256:b3f36055616985f0d92b43ed6f3a51c8bee585ff84a475e93fe9c38eed32e276
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.16.orig.tar.gz' wget_1.16.orig.tar.gz 3325041 SHA256:b977fc10ac7a72d987d48136251aeb332f2dced1aabd50d6d56bdf72e2b79101
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.16-1+deb8u1.debian.tar.xz' wget_1.16-1+deb8u1.debian.tar.xz 21696 SHA256:39322969ff614d2a7416d5e9695bb87a09bda99a510d26f536ef3bdda7739bcd
```

Likely also available for browsing at:

- https://sources.debian.net/src/wget/1.16-1+deb8u1/
- https://sources.debian.net/src/wget/1.16-1+deb8u1/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `xorg=1:7.7+7`

Binary Packages:

- `x11-common=1:7.7+7`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+7
'http://deb.debian.org/debian/pool/main/x/xorg/xorg_7.7+7.dsc' xorg_7.7+7.dsc 1934 SHA256:fdba3ef7ef9309f4d038d56b028935d3a2e06c2f68f4168d8f27683c9279da3c
'http://deb.debian.org/debian/pool/main/x/xorg/xorg_7.7+7.tar.gz' xorg_7.7+7.tar.gz 919132 SHA256:ac9dd34ee30176e71a954bc1b922f7ccb81d759bd57674d1972bc14a93916667
```

Likely also available for browsing at:

- https://sources.debian.net/src/xorg/1:7.7+7/
- https://sources.debian.net/src/xorg/1:7.7+7/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `xz-utils=5.1.1alpha+20120614-2`

Binary Packages:

- `liblzma5:amd64=5.1.1alpha+20120614-2+b3`
- `xz-utils=5.1.1alpha+20120614-2+b3`

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
$ apt-get source -qq --print-uris xz-utils=5.1.1alpha+20120614-2
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.1.1alpha+20120614-2.dsc' xz-utils_5.1.1alpha+20120614-2.dsc 2325 SHA256:d7d87c6c7aa6d2fe45d8d55a8929ab12f0688f7f17bcfc6233ecfa94f6f7a298
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.1.1alpha+20120614.orig.tar.gz' xz-utils_5.1.1alpha+20120614.orig.tar.gz 556454 SHA256:b168e63400db449a6e7b3a06e668f557ca27e3d70accbd29d2b5a98e15c00fee
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.1.1alpha+20120614-2.debian.tar.gz' xz-utils_5.1.1alpha+20120614-2.debian.tar.gz 154298 SHA256:4e2873ab7b1ee44b7d580caf2a5ca761b10cb2725691b2c2a9b21edb0d771f39
```

Likely also available for browsing at:

- https://sources.debian.net/src/xz-utils/5.1.1alpha+20120614-2/
- https://sources.debian.net/src/xz-utils/5.1.1alpha+20120614-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `yajl=2.1.0-2`

Binary Packages:

- `libyajl2:amd64=2.1.0-2`

Licenses: (parsed from: `/usr/share/doc/libyajl2/copyright`)

- `ISC`

Source:

```console
$ apt-get source -qq --print-uris yajl=2.1.0-2
'http://deb.debian.org/debian/pool/main/y/yajl/yajl_2.1.0-2.dsc' yajl_2.1.0-2.dsc 1983 SHA256:bb0952d3d1c246cb6ffd920cd14c65e6d2e034c31dda792deca2d80b25841fd0
'http://deb.debian.org/debian/pool/main/y/yajl/yajl_2.1.0.orig.tar.gz' yajl_2.1.0.orig.tar.gz 83997 SHA256:3fb73364a5a30efe615046d07e6db9d09fd2b41c763c5f7d3bfb121cd5c5ac5a
'http://deb.debian.org/debian/pool/main/y/yajl/yajl_2.1.0-2.debian.tar.xz' yajl_2.1.0-2.debian.tar.xz 5480 SHA256:e68e0f76f7fc174a1eab3bc05e5549184669458dc78526a7b06aef2d9036a95f
```

Likely also available for browsing at:

- https://sources.debian.net/src/yajl/2.1.0-2/
- https://sources.debian.net/src/yajl/2.1.0-2/debian/copyright (for direct copyright/license information)

### `dpkg` source package: `zlib=1:1.2.8.dfsg-2`

Binary Packages:

- `zlib1g:amd64=1:1.2.8.dfsg-2+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)
  If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.8.dfsg-2
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.8.dfsg-2.dsc' zlib_1.2.8.dfsg-2.dsc 2458 SHA256:5dddd28d2b15fc0881177d720a3b5bf41a87eee7aaec296e4b20719a9fe18b7e
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.8.dfsg.orig.tar.gz' zlib_1.2.8.dfsg.orig.tar.gz 361943 SHA256:2caecc2c3f1ef8b87b8f72b128a03e61c307e8c14f5ec9b422ef7914ba75cf9f
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.8.dfsg-2.debian.tar.xz' zlib_1.2.8.dfsg-2.debian.tar.xz 14768 SHA256:39af7ea4b264c229f856ed342bb316a796cb2f1e1278a059f2dc5a4f3ffc9f31
```

Likely also available for browsing at:

- https://sources.debian.net/src/zlib/1:1.2.8.dfsg-2/
- https://sources.debian.net/src/zlib/1:1.2.8.dfsg-2/debian/copyright (for direct copyright/license information)
