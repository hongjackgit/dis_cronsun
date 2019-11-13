FROM ubuntu:latest
MAINTAINER hongjack
LABEL image_version = "1.0"
LABEL etcd_version = "3.3.13"
WORKDIR etcd 
ADD etcd-v3.3.13-linux-amd64.tar-3.gz /etcd/
RUN cd etcd-v3.3.13-linux-amd64
VOLUME ["/etc/data/"]
ENTRYPOINT ["etcd-v3.3.13-linux-amd64/etcd","--listen-client-urls=http://0.0.0.0:2379","--advertise-client-urls=http://0.0.0.0:2379","--data-dir=/etcd/data"]
EXPOSE 2379 2380 4001
