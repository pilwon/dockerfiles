FROM pilwon/base

# Node.js
RUN \
  curl -sL https://deb.nodesource.com/setup | bash - && \
  apt-get -y install nodejs && \
  rm -rf /var/lib/apt/lists/* && \
  npm install -g bower grunt-cli nodemon serve && \
  echo '\n# Node.js\nexport PATH="node_modules/.bin:$PATH"' >> /root/.bashrc

# Python
RUN \
  apt-get update && \
  apt-get -y install python-dev python-pip && \
  rm -rf /var/lib/apt/lists/*
