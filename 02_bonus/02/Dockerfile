#tetris

FROM ubuntu

RUN apt-get update && apt-get upgrade
RUN apt-get install bastet -y

WORKDIR /usr/games/

ENTRYPOINT ./bastet

# docker build -t  tetris .
# docker run tetris
# docker run -it ubuntu bash // run ubuntu
