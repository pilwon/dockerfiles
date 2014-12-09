FROM pilwon/base

RUN \
  curl -sL https://deb.nodesource.com/setup | bash - && \
  apt-get -y install nodejs && \
  rm -rf /var/lib/apt/lists/* && \
  npm install -g npm && \
  npm install -g bower grunt-cli nodemon serve && \
  echo -e '\n# Node.js\nexport PATH="node_modules/.bin:$PATH"' >> /root/.bashrc
