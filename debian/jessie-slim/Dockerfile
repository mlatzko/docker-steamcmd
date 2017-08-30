FROM debian:jessie-slim

MAINTAINER wilkesystems <developer@wilke.systems>

ENV DEBIAN_FRONTEND=noninteractive

ADD steamcmd.tar.xz /

RUN apt-get dpkg --add-architecture i386; update; \
apt-get install -y binutils ca-certificates lib32gcc1 lib32stdc++6 libterm-ui-perl locales locales-all net-tools; \
steamcmd +quit; rm -rf /root/.steam/logs/* /var/lib/apt/lists/* /tmp/*

CMD ["steamcmd"]