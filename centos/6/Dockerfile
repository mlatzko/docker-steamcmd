FROM centos:6

MAINTAINER wilkesystems <developer@wilke.systems>

ADD steamcmd.tar.xz /

RUN yum -y install glibc.i686 libstdc++.i686; \
steamcmd +quit; rm -rf /root/.steam/logs/* /tmp/*

CMD ["steamcmd"]