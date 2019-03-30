# pi-hole in docker

I am pulling the pi-hole image from https://hub.docker.com/r/pihole/pihole/

More info at https://github.com/pi-hole/docker-pi-hole/ and https://docs.pi-hole.net/

## Quickstart

    docker volume create pihole-etc
    docker volume create pihole-dnsmasq
    docker-compose up

## Proxy

I run this container behind a reverse proxy.

