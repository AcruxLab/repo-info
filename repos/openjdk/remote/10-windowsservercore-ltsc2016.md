## `openjdk:10-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:42d497528ef9d2e21523a667fae9c478fa9f68020fbed1318a0e8af8cfd2fcfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.2312; amd64

### `openjdk:10-windowsservercore-ltsc2016` - windows version 10.0.14393.2312; amd64

```console
$ docker pull openjdk@sha256:4ce143c88aa8699ad65bc09f5858622f6958f6b7d270eb578132b4de93daf144
```

-	Docker Version: 17.10.0-ee-preview-3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5768672690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:525705ff8b15bfe3fa1585856ae5f5a898c513dd61746470c4521968235152fe`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Wed, 13 Jun 2018 00:36:30 GMT
RUN Install update 10.0.14393.2312
# Sat, 16 Jun 2018 10:18:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 16 Jun 2018 10:18:58 GMT
ENV JAVA_HOME=C:\ojdkbuild
# Sat, 16 Jun 2018 10:21:51 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath;
# Sat, 16 Jun 2018 10:21:52 GMT
ENV JAVA_VERSION=10.0.1
# Sat, 16 Jun 2018 10:21:53 GMT
ENV JAVA_OJDKBUILD_VERSION=10.0.1-1
# Sat, 16 Jun 2018 10:21:54 GMT
ENV JAVA_OJDKBUILD_ZIP=java-10-openjdk-10.0.1-1.b10.ojdkbuild.windows.x86_64.zip
# Sat, 16 Jun 2018 10:21:55 GMT
ENV JAVA_OJDKBUILD_SHA256=64664f2e28db55022d90beefd097779c59f843cacf1afeed8a7456ee64c603f1
# Sat, 16 Jun 2018 10:24:56 GMT
RUN $url = ('https://github.com/ojdkbuild/ojdkbuild/releases/download/{0}/{1}' -f $env:JAVA_OJDKBUILD_VERSION, $env:JAVA_OJDKBUILD_ZIP); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'ojdkbuild.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_OJDKBUILD_SHA256); 	if ((Get-FileHash ojdkbuild.zip -Algorithm sha256).Hash -ne $env:JAVA_OJDKBUILD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive ojdkbuild.zip -DestinationPath C:\; 		Write-Host 'Renaming ...'; 	Move-Item 		-Path ('C:\{0}' -f ($env:JAVA_OJDKBUILD_ZIP -Replace '.zip$', '')) 		-Destination $env:JAVA_HOME 	; 		Write-Host 'Verifying install ...'; 	Write-Host '  java -version'; java -version; 	Write-Host '  javac -version'; javac -version; 		Write-Host 'Removing ...'; 	Remove-Item ojdkbuild.zip -Force; 		Write-Host 'Complete.';
# Sat, 16 Jun 2018 10:24:58 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8e9da9bbe3af2118a0b5eef7a3d649367557d0d3992ed0213c79857b23b4140e`  
		Last Modified: Wed, 13 Jun 2018 00:36:30 GMT  
		Size: 1.4 GB (1414319443 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f081cda9e78f379ae3f7a2238f310ca91bbbac2c32d6e990eb6b15df6c2df4b`  
		Last Modified: Sat, 16 Jun 2018 10:42:21 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d735f69af604295b7f6269c8995a8a00c86ac47630ed93a86d8569c5630bb13a`  
		Last Modified: Sat, 16 Jun 2018 10:42:21 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ad5c8c2e88d71e74046a3265a344d6cdd729f89cf9dbad61cef87b36117ed3`  
		Last Modified: Sat, 16 Jun 2018 10:42:23 GMT  
		Size: 5.0 MB (5009235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a0fe4f6b5673d8db880b3f59acdb6368c378b97913ee48d9c56b0288c69c47`  
		Last Modified: Sat, 16 Jun 2018 10:42:21 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d89e698be000bd495bd82ae82a794200a306019eb9573046dea22d4ee984b7`  
		Last Modified: Sat, 16 Jun 2018 10:42:18 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46395c72416b126d04e0cd78318266702f91057e144e3cdcdaa2abf039c33ea4`  
		Last Modified: Sat, 16 Jun 2018 10:42:18 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145d14e15ce2f9fdfbb9f8453a23ebfdeacf00cdb65f9d2b66f7ac5d4e683f0c`  
		Last Modified: Sat, 16 Jun 2018 10:42:18 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea88374d63be46f42d544250d177d806eabfccffcde4f216f66a05890649c3ee`  
		Last Modified: Sat, 16 Jun 2018 10:42:52 GMT  
		Size: 279.3 MB (279349763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58f64be4186d2679f7b3066276f768789f33a3f85946419948919cf9ccab76c`  
		Last Modified: Sat, 16 Jun 2018 10:42:18 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
