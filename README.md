# docker-serviio

[![](http://serviio.org/images/serviio.png)](http://serviio.org/)

Link on github: [dfuchslin/docker-serviio](https://github.com/dfuchslin/docker-serviio)

!!! > THIS IS A FORK OF [riftbit/docker-serviio](https://github.com/riftbit/docker-serviio) < !!!

### Build Args

 - `VERSION` = 2.2.1 - serviio version
 - `FFMPEG_VERSION` = 5.0


### Exposed Ports

 - `1900:1900/udp`
 - `8895:8895/tcp`
 - `23423:23423/tcp` - HTTP/1.1 /console /rest
 - `23523:23523/tcp` - HTTPS/1.1 /console /rest
 - `23424:23424/tcp` - HTTP/1.1 /cds /mediabrowser
 - `23524:23524/tcp` - HTTPS/1.1 /cds /mediabrowser

### Recomended Volumes (no auto mounting now)
 - `/opt/serviio/config`
 - `/opt/serviio/library`
 - `/opt/serviio/plugins`
 - `/opt/serviio/log`
 - `/media/serviio` - put media content here and add in serviio gui this path


### Container Changelog (dd.mm.yy)
 - **05.02.2022** - Update Serviio version to 2.2.1, alpine to 3.15, ffmpeg to 5.0, dcraw to latest official
 - **01.10.2021** - Update Serviio version to 2.2
 - **19.03.2021** - Update FFMPEG to 4.3.2, add healthcheck (PR #19), cleanup volumes (mount only if you need it)
 - **07.12.2020** - Update alpine to 3.12, fix dcraw.c build (add jasper build from source), removed config volume
 - **28.05.2020** - Update Serviio version to 2.1, alpine to 3.11, ffmpeg to 4.2, fix dcraw.c path
 - **27.05.2019** - Update Serviio version to 2.0 and alpine to latest on build date
 - **19.12.2018** - Update Serviio version to 1.10.1 and ffmpeg to 4.1 and alpine to latest on build date
 - **09.05.2018** - Update Serviio version from 1.9.1 to 1.9.2
 - **02.03.2018** - Update Serviio version from 1.9 to 1.9.1
 - **12.01.2018** - dcraw now supported. dockerfile cleanups. many fixes and updates
