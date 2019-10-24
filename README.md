# home-server

Create and run a Docker-based home server.  
The following services are included:

| Service                                           | Description                | Port  |
| ------------------------------------------------- | -------------------------- | ----- |  
| [Portainer](https://www.portainer.io/)            | 🐋 Docker web UI           | 9000  |  
| [Organizr](https://github.com/causefx/Organizr)   | 📑 HTPC services organiser | 9001  |  
| [Transmission](https://transmissionbt.com/)       | 🌊 BitTorrent client       | 9091  |  
| [Radarr](https://radarr.video/)                   | 🎬 Movies downloader       | 7878  |  
| [Sonarr](https://sonarr.tv/)                      | 📺 TV shows downloader     | 8989  |  
| [Plex](http://plex.tv/)                           | 🎟 Media server            | 32400 |  


## Prerequisites
- [Docker Engine](https://docs.docker.com/install/linux/docker-ce/ubuntu/).
- [Docker Compose](https://docs.docker.com/compose/install/).

**Tested on Ubuntu Server 18.04.3.**

## Setup
```
$ ./init
$ ./up
```
## Scripts
- `init` - Create required folders and `.env` file (should be run once).
- `services` - list Docker services
- `logs <service>` - show logs of specific service.
- `logs` - show logs of all services.
- `up` - Bring up services.
- `down` - Take down services.
- `login <service>` - Shell login to specific service.

## TODO
- [ ] Add [Jackett](https://hub.docker.com/r/linuxserver/jackett/).  
- [ ] Read ports from .env file.  

## Credits
Inspired by the [awesome tutorial](https://www.smarthomebeginner.com/docker-home-media-server-2018-basic/) written by [@htpcBeginner](https://github.com/htpcBeginner).
