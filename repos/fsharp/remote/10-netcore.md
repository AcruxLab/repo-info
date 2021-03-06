## `fsharp:10-netcore`

```console
$ docker pull fsharp@sha256:2be097c683813a824f8fd01e398598843a1b6b5b0d234d2af6769a92fc00dccb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:10-netcore` - linux; amd64

```console
$ docker pull fsharp@sha256:ad7249faec50915ec5501568fe7e85baf6eb971f8afcc57a95b8c87a8cc8ca23
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **627.8 MB (627813113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95f41fa966fc655b516da87e68e707cce85a82c53255990bb995e491b776bf84`
-	Default Command: `["fsharpi"]`

```dockerfile
# Sat, 28 Apr 2018 07:09:59 GMT
ADD file:ec5be7eec56a749752ca284359ece04f5eb0b981eac08b8855454c6b16e3893c in / 
# Sat, 28 Apr 2018 07:09:59 GMT
CMD ["bash"]
# Wed, 06 Jun 2018 00:04:56 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Wed, 06 Jun 2018 00:04:56 GMT
ENV MONO_THREADS_PER_CPU=50
# Wed, 06 Jun 2018 00:20:09 GMT
RUN MONO_VERSION=5.8.0.127 &&     FSHARP_VERSION=10.0.2 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr &&     apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stretch/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get install -y apt-transport-https &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Wed, 06 Jun 2018 00:20:10 GMT
WORKDIR /root
# Wed, 06 Jun 2018 00:20:10 GMT
CMD ["fsharpi"]
# Wed, 06 Jun 2018 00:46:38 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Wed, 06 Jun 2018 00:46:38 GMT
ENV FrameworkPathOverride=/usr/lib/mono/4.6.2-api/
# Wed, 06 Jun 2018 00:46:38 GMT
ENV NUGET_XMLDOC_MODE=skip
# Wed, 06 Jun 2018 00:46:50 GMT
RUN apt-get update &&     apt-get --no-install-recommends install -y     curl     libunwind8     gettext     apt-transport-https     libc6     libcurl3     libgcc1     libgssapi-krb5-2     libicu57     liblttng-ust0     libssl1.0.2     libstdc++6     libunwind8     libuuid1     zlib1g &&     rm -rf /var/lib/apt/lists/*
# Wed, 06 Jun 2018 00:47:47 GMT
RUN DOTNET_SDK_VERSION=2.1.104 &&     DOTNET_SDK_DOWNLOAD_URL=https://dotnetcli.blob.core.windows.net/dotnet/Sdk/$DOTNET_SDK_VERSION/dotnet-sdk-$DOTNET_SDK_VERSION-linux-x64.tar.gz &&     DOTNET_SDK_DOWNLOAD_SHA=813334694667f8c1389d88cd3128a7749f4f65b13a0a8e2cb47380823849b8fe7f4816ab66c2d77e589fac9cb5748390b262beae9673aef86cad5a3d8f24986e &&     curl -SL $DOTNET_SDK_DOWNLOAD_URL --output dotnet.tar.gz &&     echo "$DOTNET_SDK_DOWNLOAD_SHA dotnet.tar.gz" | sha512sum -c - &&     mkdir -p /usr/share/dotnet &&     tar -zxf dotnet.tar.gz -C /usr/share/dotnet &&     rm dotnet.tar.gz &&     ln -s /usr/share/dotnet/dotnet /usr/bin/dotnet
# Wed, 06 Jun 2018 00:47:47 GMT
ENV DOTNET_CLI_TELEMETRY_OPTOUT=1
# Wed, 06 Jun 2018 00:48:25 GMT
RUN mkdir warmup &&     cd warmup &&     dotnet new &&     cd - &&     rm -rf warmup /tmp/NuGetScratch
# Wed, 06 Jun 2018 00:48:27 GMT
WORKDIR /root
```

-	Layers:
	-	`sha256:f2aa67a397c49232112953088506d02074a1fe577f65dc2052f158a3e5da52e8`  
		Last Modified: Sat, 28 Apr 2018 09:31:20 GMT  
		Size: 22.5 MB (22496029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc0279cf2a50e81ffca186bbdab1bd75e4259284898104859d3211a3754a5b7`  
		Last Modified: Wed, 06 Jun 2018 00:49:36 GMT  
		Size: 132.5 MB (132512705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fb4733cd0253f432d89b4bf412cf27ed9750d2729b18144ded19e74f3f3a97`  
		Last Modified: Wed, 06 Jun 2018 00:51:58 GMT  
		Size: 18.0 MB (17997675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef610066105ecac5a7045460b3d58290804f529bac6c5f3c0c723770f7bb418`  
		Last Modified: Wed, 06 Jun 2018 00:52:44 GMT  
		Size: 164.3 MB (164322430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada94ecae16ff06f58b38b51ad56056f054ea86c5ec2d0de05d8297c28b75046`  
		Last Modified: Wed, 06 Jun 2018 00:53:20 GMT  
		Size: 290.5 MB (290484274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
