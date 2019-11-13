FROM ubuntu:latest
MAINTAINER hongjack
WORKDIR cronsun
ADD cronsun-v0.3.5 /cronsun/
VOLUME ["/var/run/cronsun/","/etc/cronsun/"]
RUN chmod +x /cronsun/cronnode
ENTRYPOINT ["/cronsun/cronnode","--conf=/cronsun/conf/base.json"]
