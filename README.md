Docker container built with debian:stable-slim image.
Contains Apache (mod rewrite, header and http2 enabled), 
and PHP with a few extentions.

Remove (leave container in timezone UTC) or edit files/etc/cont-init.d/11-timezone to your preference

To keep data persistent mount ´/var/www/html´ ex:
[...]-v ./appdata/webapp:/var/www/html[...]

Set userid and groupid of container with environment vars
PUID=<uid(userid)>
PGID=<gid(groupid)>

S6-Overlay Version v1.21.4.0 (https://github.com/just-containers/s6-overlay)
