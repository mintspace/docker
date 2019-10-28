# vim with .rc_file

FROM ubuntu

RUN apt-get update && apt-get upgrade
RUN apt-get install vim -y
COPY .vimrc /usr/bin

WORKDIR /usr/bin/
RUN touch test.c

ENTRYPOINT ./vim -S .vimrc test.c

# docker run -it ubuntu bash // run ubuntu