FROM pilwon/base

RUN \
  apt-get update && \
  apt-get -y install libfreetype6 libfontconfig && \
  wget -qO - https://bitbucket.org/ariya/phantomjs/downloads/phantomjs-1.9.8-linux-x86_64.tar.bz2 | tar xjC /opt && \
  ln -s /opt/phantomjs-1.9.8-linux-x86_64/bin/phantomjs /bin && \
  rm -rf /var/lib/apt/lists/*

CMD ["phantomjs", "--webdriver", "8910"]

EXPOSE 8910
