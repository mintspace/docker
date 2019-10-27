FROM debian

ENV TS3SERVER_LICENSE=accept

RUN apt-get update
RUN	apt-get upgrade
RUN apt-get install -y wget bzip2
RUN wget http://dl.4players.de/ts/releases/3.0.13.8/teamspeak3-server_linux_amd64-3.0.13.8.tar.bz2
RUN tar xfv teamspeak3-server_linux_amd64-3.0.13.8.tar.bz2

WORKDIR /teamspeak3-server_linux_amd64
ENTRYPOINT sh ts3server_minimal_runscript.sh

# docker-machine ip Char

# docker run -it debian bash

# docker build -t ts:v1 . // build
# docker images - check for teamspeak image
# docker run ts:v1