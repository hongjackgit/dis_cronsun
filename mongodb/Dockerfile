FROM ubuntu:latest
MAINTAINER hongjack
WORKDIR mongodb
RUN apt-get update
RUN apt-get install -y mongodb
VOLUME ["/mongodb/data"]
ENTRYPOINT ["mongod","--bind_ip=0.0.0.0","--dbpath=/mongodb/data","--logpath=/mongodb/log","--logappend"]
