# home-server

## Setup
### Create `.env` file
```
PUID=<user id, id -u $USER>
PGID=<docker group id, cut -d: -f3 < <(getent group docker)>
TZ=<time zone, https://en.wikipedia.org/wiki/List_of_tz_database_time_zones>
USERDIR=<user home dir, $HOME>
PLEX_CLAIM=<plex server claim, https://www.plex.tv/claim/>
SERVER_ADDR=<server's IP>
```
