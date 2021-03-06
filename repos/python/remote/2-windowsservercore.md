## `python:2-windowsservercore`

```console
$ docker pull python@sha256:0a8c46b161a9ef8f4d1fa708701543901fc93ec8d4645571ce6a0cadc289ebd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.2248; amd64
	-	windows version 10.0.16299.431; amd64

### `python:2-windowsservercore` - windows version 10.0.14393.2248; amd64

```console
$ docker pull python@sha256:3791296b5bcc0964afb69dd86f69f0ecfd8c1c1c80a910af3cd1b523d1df83af
```

-	Docker Version: 17.10.0-ee-preview-3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 GB (5520713839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4c9c85395f0f24310322c079be6a2746e08fe5c1106d6ede8c7173339a49c4f`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 07 May 2018 18:12:28 GMT
RUN Install update 10.0.14393.2248
# Thu, 10 May 2018 09:39:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 24 May 2018 09:33:59 GMT
ENV PYTHON_VERSION=2.7.15
# Thu, 24 May 2018 09:34:00 GMT
ENV PYTHON_RELEASE=2.7.15
# Thu, 24 May 2018 09:36:29 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}.amd64.msi' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.msi'; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'python.msi', 			'/quiet', 			'/qn', 			'TARGETDIR=C:\Python', 			'ALLUSERS=1', 			'ADDLOCAL=DefaultFeature,Extensions,TclTk,Tools,PrependPath' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.msi -Force; 		Write-Host 'Complete.';
# Thu, 24 May 2018 09:36:30 GMT
ENV PYTHON_PIP_VERSION=10.0.1
# Thu, 24 May 2018 09:38:15 GMT
RUN Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri 'https://bootstrap.pypa.io/get-pip.py' -OutFile 'get-pip.py'; 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.';
# Thu, 24 May 2018 09:39:29 GMT
RUN pip install --no-cache-dir virtualenv
# Thu, 24 May 2018 09:39:30 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ace98111594c5bc232640988045037489d2adc214b3a14e07a8a9e9d30442cef`  
		Last Modified: Mon, 07 May 2018 18:12:28 GMT  
		Size: 1.4 GB (1395367096 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3fef3bd83b7c0eb06ccae001ea0bfed47b7258d9a1c5d593913034b18f7fd8c0`  
		Last Modified: Thu, 10 May 2018 10:17:55 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689c393c4187201da582c5c42c961fff7e6941661a04b677469c9bddd64183d5`  
		Last Modified: Thu, 24 May 2018 09:48:47 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d5546b9aabaf325f9f1004bb94474c56a5c4779050971060fcb198e9942fc2`  
		Last Modified: Thu, 24 May 2018 09:48:44 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3923fa014212a6f69307600e6e9616458ee3f2ee3b2f9831a14f186dd80fbbf`  
		Last Modified: Thu, 24 May 2018 09:49:02 GMT  
		Size: 38.9 MB (38933340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e1e6c784f84106bb9dc95b561490aa5e2cabcd3f103dbbf654c2c2a25bcb37`  
		Last Modified: Thu, 24 May 2018 09:48:41 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4807826c1539a1ae6733acd6182b2331bbaa1599f84b8fd611a618ddcfefe1d6`  
		Last Modified: Thu, 24 May 2018 09:48:48 GMT  
		Size: 9.5 MB (9452737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4c539b8f541c330595cc760913bb8d5b58f918a8b2d62c7395bed51fc23e30`  
		Last Modified: Thu, 24 May 2018 09:48:43 GMT  
		Size: 7.0 MB (6968777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79556ff3e9f3a75bc9918054e7a965ed1640b97d205a037dfaccee7ff9682891`  
		Last Modified: Thu, 24 May 2018 09:48:41 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:2-windowsservercore` - windows version 10.0.16299.431; amd64

```console
$ docker pull python@sha256:ec31a901d316b4e56194872d2fdc59fcfbd6c51f89d7ddd03dca6fc57f05347c
```

-	Docker Version: 17.10.0-ee-preview-3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3134766623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32a18decfb9088fb8b9923f1007735b912ad0ed17761a8dfd6390fc59ff7932b`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 05 May 2018 14:37:10 GMT
RUN Install update 10.0.16299.431
# Thu, 10 May 2018 09:50:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 24 May 2018 09:39:42 GMT
ENV PYTHON_VERSION=2.7.15
# Thu, 24 May 2018 09:39:42 GMT
ENV PYTHON_RELEASE=2.7.15
# Thu, 24 May 2018 09:41:44 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}.amd64.msi' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.msi'; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'python.msi', 			'/quiet', 			'/qn', 			'TARGETDIR=C:\Python', 			'ALLUSERS=1', 			'ADDLOCAL=DefaultFeature,Extensions,TclTk,Tools,PrependPath' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.msi -Force; 		Write-Host 'Complete.';
# Thu, 24 May 2018 09:41:45 GMT
ENV PYTHON_PIP_VERSION=10.0.1
# Thu, 24 May 2018 09:43:23 GMT
RUN Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri 'https://bootstrap.pypa.io/get-pip.py' -OutFile 'get-pip.py'; 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.';
# Thu, 24 May 2018 09:44:24 GMT
RUN pip install --no-cache-dir virtualenv
# Thu, 24 May 2018 09:44:25 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:af675e5054a0dfb3eb70b140f566a5dbe612b5212e4a4ef2a2991308740d1006`  
		Last Modified: Tue, 08 May 2018 18:45:22 GMT  
		Size: 805.9 MB (805944217 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b0d3f2c48ca5c41c53fe84071bb55725c2d6c36c8840dcef5297cc048ffe39aa`  
		Last Modified: Thu, 10 May 2018 10:18:48 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97802b47cdb8590a8fdba60c612176de07cea1a9f0db9a442383ab1aa51c425`  
		Last Modified: Thu, 24 May 2018 09:49:21 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11d607860a599a80eb3a7b7faa2047fca09b6c3456d401c3eb0a0837745ddde`  
		Last Modified: Thu, 24 May 2018 09:49:21 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09942d7565c40e06feb7946cfc5ffe467c5b50329eb25a5b49b132a44698808`  
		Last Modified: Thu, 24 May 2018 09:49:38 GMT  
		Size: 38.7 MB (38668076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdcef41569738c9194aed9274abda0afc9cef9fd629fb512074b12e14be6e00`  
		Last Modified: Thu, 24 May 2018 09:49:17 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a9d3c561abf424b009a2700d053797f4087f45e1b7f87f13b6b14c45d38457`  
		Last Modified: Thu, 24 May 2018 09:49:26 GMT  
		Size: 9.2 MB (9157625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2ae2c8c31c2716baf5101885451cfa0205076789eaa367110b5083f0fcf596`  
		Last Modified: Thu, 24 May 2018 09:49:20 GMT  
		Size: 6.7 MB (6690175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206329f5a61797ccb7ed90421505325c549180fbff5c0ea42e8f1b40551bd963`  
		Last Modified: Thu, 24 May 2018 09:49:17 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
