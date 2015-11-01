This is a Dockerfile setup for deluge - http://deluge-torrent.org/

To run:

```
docker build -t butters16/deluge .
docker run -d --name=deluge --restart=always -v /path_to_config/:/config -v /path_to_torrents/:/torrents -v /path_to_temp/:/temp -v /path_to_storage/:/done -v /etc/localtime:/etc/localtime:ro -p 8112:8112 -p 58846:58846 butters16/deluge
```
