# Docker Container: Logitech Media Server for armhf (Raspberry Pi, ...)

As previous repo is not updated anymore, this is meant to be a fork for the latest version of the LMS.

Current version LMS: 7.9.2 nightly

Based on https://github.com/mrtestone/armhf-lms

Folders to map (for permanent data):
/var/log/squeezeboxserver
/var/lib/squeezeboxserver

Ports to map:
3483/tcp
3483/udp
9000/tcp
9090/tcp

example run:
```
docker run -d \
  -p 9090:9090 \
  -p 9000:9000 \
  -p 3483:3483 \
  -p 3483:3483/udp \
  mrtestone/armhf-lms
```
