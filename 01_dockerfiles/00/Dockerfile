FROM alpine

RUN apk update
RUN	apk upgrade
RUN apk add vim

ENTRYPOINT vim

# to start machine: docker-machine start Char
# eval $(docker-machine env Char)
# docker run --rm -it alpine

# docker build -t task_01:v1 . // build
# docker images - check for task_01 image
# docker run task_01:v1