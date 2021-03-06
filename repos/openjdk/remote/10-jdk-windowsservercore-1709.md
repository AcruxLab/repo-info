## `openjdk:10-jdk-windowsservercore-1709`

```console
$ docker pull openjdk@sha256:98fce7353e5ba19e2c9a70aa9a3daaf4c19dbf2e52b462f4db4e76e6239cb270
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.16299.492; amd64

### `openjdk:10-jdk-windowsservercore-1709` - windows version 10.0.16299.492; amd64

```console
$ docker pull openjdk@sha256:c8300712b583fe3de2f0c3f0f528d421922d766d9e65b81635e9152cc465983a
```

-	Docker Version: 17.10.0-ee-preview-3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 GB (3381658683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:225959815e5c871d7413017170706a6f172bfdb5375ae47669ffe7f8d428f1b1`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Mon, 11 Jun 2018 20:38:48 GMT
RUN Install update 10.0.16299.492
# Sat, 16 Jun 2018 10:25:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 16 Jun 2018 10:25:11 GMT
ENV JAVA_HOME=C:\ojdkbuild
# Sat, 16 Jun 2018 10:27:13 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath;
# Sat, 16 Jun 2018 10:27:14 GMT
ENV JAVA_VERSION=10.0.1
# Sat, 16 Jun 2018 10:27:15 GMT
ENV JAVA_OJDKBUILD_VERSION=10.0.1-1
# Sat, 16 Jun 2018 10:27:16 GMT
ENV JAVA_OJDKBUILD_ZIP=java-10-openjdk-10.0.1-1.b10.ojdkbuild.windows.x86_64.zip
# Sat, 16 Jun 2018 10:27:17 GMT
ENV JAVA_OJDKBUILD_SHA256=64664f2e28db55022d90beefd097779c59f843cacf1afeed8a7456ee64c603f1
# Sat, 16 Jun 2018 10:29:59 GMT
RUN $url = ('https://github.com/ojdkbuild/ojdkbuild/releases/download/{0}/{1}' -f $env:JAVA_OJDKBUILD_VERSION, $env:JAVA_OJDKBUILD_ZIP); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'ojdkbuild.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_OJDKBUILD_SHA256); 	if ((Get-FileHash ojdkbuild.zip -Algorithm sha256).Hash -ne $env:JAVA_OJDKBUILD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive ojdkbuild.zip -DestinationPath C:\; 		Write-Host 'Renaming ...'; 	Move-Item 		-Path ('C:\{0}' -f ($env:JAVA_OJDKBUILD_ZIP -Replace '.zip$', '')) 		-Destination $env:JAVA_HOME 	; 		Write-Host 'Verifying install ...'; 	Write-Host '  java -version'; java -version; 	Write-Host '  javac -version'; javac -version; 		Write-Host 'Removing ...'; 	Remove-Item ojdkbuild.zip -Force; 		Write-Host 'Complete.';
# Sat, 16 Jun 2018 10:30:01 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b9c63e313c8b374d5767c602fd6f2b947a3f1df9a8f8c5fcecb2fa6b1cfa968`  
		Last Modified: Wed, 13 Jun 2018 01:11:53 GMT  
		Size: 823.6 MB (823576248 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c64dfe6152b178e35770ab15c53bfcc70f8dd47d8a0551e325ccfa665416b738`  
		Last Modified: Sat, 16 Jun 2018 10:43:33 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432e0357edec73d47a9a9f0d45df806096b0d2124cc3495b64f0c8853e397da8`  
		Last Modified: Sat, 16 Jun 2018 10:43:33 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2fd923a3d34ae42ef6116f39e4e034e6b2e37b054bbc301d44ed5bb0f66edf`  
		Last Modified: Sat, 16 Jun 2018 10:43:34 GMT  
		Size: 4.7 MB (4704668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2799b8a40679a2501fff0b94d19a95dea0dc15188129bbb8d05e690c339b5a11`  
		Last Modified: Sat, 16 Jun 2018 10:43:32 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a92b536a0c41a30edd2bb83f5cf3ebaf4260d8f7c81310f431414468d01594`  
		Last Modified: Sat, 16 Jun 2018 10:43:30 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4488a56465a47653d0acca2a04099cfef21fbebf38ac3562e8fb71184368ff38`  
		Last Modified: Sat, 16 Jun 2018 10:43:30 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3817bb95063a9fd7582115d5bb3c233e610442abe2c094574db8673f9c24fc`  
		Last Modified: Sat, 16 Jun 2018 10:43:30 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150c83c5ae3877ff8c01d49d855ff58c532648260ae583ac855b00425eebfa0b`  
		Last Modified: Sat, 16 Jun 2018 10:44:04 GMT  
		Size: 279.1 MB (279068832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f259caa057f2d400b44350a7288289ae191af29578e0f97217f6c58bf78c0750`  
		Last Modified: Sat, 16 Jun 2018 10:43:30 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
