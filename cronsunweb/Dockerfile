FROM ubuntu:latest
MAINTAINER hongjack
WORKDIR cronsun
ADD cronsun-v0.3.5 /cronsun/
VOLUME ["/var/run/cronsun/","/etc/cronsun/"]
RUN chmod +x /cronsun/cronweb
ENTRYPOINT ["/cronsun/cronweb","--conf=/cronsun/conf/base.json"]
EXPOSE 7079
