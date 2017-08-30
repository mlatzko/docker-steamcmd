FROM debian:wheezy-slim

MAINTAINER wilkesystems <developer@wilke.systems>

ENV DEBIAN_FRONTEND=noninteractive

ADD steamcmd.tar.xz /

RUN dpkg --add-architecture i386; apt-get update; \
apt-get install -y binutils ca-certificates lib32gcc1 lib32stdc++6 locales locales-all net-tools; \
steamcmd +quit; rm -rf /root/.steam/logs/* /var/lib/apt/lists/* /tmp/*

CMD ["steamcmd"]