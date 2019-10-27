FROM ubuntu

RUN apt-get update && apt-get upgrade
RUN apt-get install vim
ONBUILD COPY .vimrc ~/

ENTRYPOINT vim