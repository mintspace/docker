FROM ubuntu

RUN apt-get update
RUN	apt-get upgrade -y
RUN	apt-get install -y ca-certificates openssh-server wget postfix

RUN wget https://packages.gitlab.com/install/repositories/gitlab/gitlab-ce/script.deb.sh && \
	chmod 777 script.deb.sh && \
	./script.deb.sh && \
	apt-get install -y gitlab-ce

RUN apt update && apt install -y tzdata
RUN	apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

EXPOSE 443 80 22

ENTRYPOINT (/opt/gitlab/embedded/bin/runsvdir-start &) && sleep 2 && gitlab-ctl reconfigure && tail -f /dev/null

# docker run -it --rm -p 8080:80 -p 8022:22 -p 8443:443 --privileged ex03