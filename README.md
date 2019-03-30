# pi-hole in docker

I am pulling the pi-hole image from https://hub.docker.com/r/pihole/pihole/

More info at https://github.com/pi-hole/docker-pi-hole/ and https://docs.pi-hole.net/

## Quickstart

    docker volume create pihole-etc
    docker volume create pihole-dnsmasq
    docker-compose up

## Proxy

I run this container behind a reverse proxy.

To make it work with my proxy (brian32768/docker-proxy), I made these changes:

1. define VIRTUAL_HOST as pihole.wildsong.biz
2. add network "proxy_net" so the proxy container can see into this network
3. expose port 80

