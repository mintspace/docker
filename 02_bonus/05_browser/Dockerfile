# console browser

FROM ubuntu

RUN apt-get update && apt-get upgrade
RUN apt-get install apt-utils -y
RUN apt-get install elinks -y

WORKDIR /usr/bin/

ENTRYPOINT ./elinks www.google.com

# docker run -it ubuntu bash // run ubuntu