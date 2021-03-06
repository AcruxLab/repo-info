## `python:3-windowsservercore-ltsc2016`

```console
$ docker pull python@sha256:f94b4fbb97c62d3f3ffb0040d0e16776bf948883b3d5f5396489b5a76a9e9615
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.2248; amd64

### `python:3-windowsservercore-ltsc2016` - windows version 10.0.14393.2248; amd64

```console
$ docker pull python@sha256:f6dba05b0eab12d3a45de12dff4599b9a5bd5caa38a35d0096984c6cfe364d58
```

-	Docker Version: 17.10.0-ee-preview-3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 GB (5527699765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76e090eb896cafb70ad65825f9e63420080798eeb2f1779d5de06b27928e3f1`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 07 May 2018 18:12:28 GMT
RUN Install update 10.0.14393.2248
# Thu, 10 May 2018 09:39:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 24 May 2018 09:24:50 GMT
ENV PYTHON_VERSION=3.6.5
# Thu, 24 May 2018 09:24:52 GMT
ENV PYTHON_RELEASE=3.6.5
# Thu, 24 May 2018 09:27:47 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.';
# Thu, 24 May 2018 09:27:48 GMT
ENV PYTHON_PIP_VERSION=10.0.1
# Thu, 24 May 2018 09:29:33 GMT
RUN Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri 'https://bootstrap.pypa.io/get-pip.py' -OutFile 'get-pip.py'; 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.';
# Thu, 24 May 2018 09:29:34 GMT
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
	-	`sha256:83799b1ca7ab30fdc8d26d388f137502d8617faa274cb5d306cb800876634bbe`  
		Last Modified: Thu, 24 May 2018 09:47:17 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be6483f40c97ced8da645bf54531aabc41df2266e24d618d31a7d1b1be4f1c0`  
		Last Modified: Thu, 24 May 2018 09:47:14 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4ac4931478c09b610a3b4a2954572a8661f80465d9a8e9799b4b9299bf0d7e`  
		Last Modified: Thu, 24 May 2018 09:47:39 GMT  
		Size: 52.5 MB (52518839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d8a45a5ac32126a12474569fdc30f568d351a65fe139b96424c9a577cd1db6`  
		Last Modified: Thu, 24 May 2018 09:47:13 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08853acb649fc056b864071eb6ed105292f632c1eabf915fed12b27a2942de3c`  
		Last Modified: Thu, 24 May 2018 09:47:25 GMT  
		Size: 9.8 MB (9821961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96c7c30e6f2ee7fb4ffb97f7ea0397a21a679b1d7c64bab6caf3e1f3500bc82`  
		Last Modified: Thu, 24 May 2018 09:47:13 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
