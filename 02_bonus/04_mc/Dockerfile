# mc

FROM ubuntu

RUN apt-get update && apt-get upgrade
RUN apt-get install mc -y

WORKDIR /usr/bin/

ENTRYPOINT ./mc

# docker run -it ubuntu bash // run ubuntu