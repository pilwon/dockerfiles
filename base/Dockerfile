FROM debian:wheezy

RUN \
  echo "deb http://http.debian.net/debian wheezy-backports main" >> /etc/apt/sources.list && \
  apt-get update && \
  apt-get -y upgrade && \
  apt-get -y install build-essential curl dstat less htop man procps sysstat unzip vim wget zip && \
  apt-get -y install -t wheezy-backports byobu git iotop && \
  rm -rf /var/lib/apt/lists/*

ADD init /root/.init

RUN /root/.init/setup

ENV HOME /root

WORKDIR /root
