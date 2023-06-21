FROM mcr.microsoft.com/vscode/devcontainers/base:debian-11

# install fish terminal
RUN apt-get update && apt-get install -y \
    fish \
    && rm -rf /var/lib/apt/lists/*

# install nodejs
USER root
ARG NODE_VERSION=v18.16.1
RUN set -x \
    && mkdir -p /usr/local/lib/nodejs \
    && curl -fsSL "https://nodejs.org/dist/${NODE_VERSION}/node-${NODE_VERSION}-linux-x64.tar.xz" | tar xJ -C /usr/local/lib/nodejs
ENV PATH $PATH:/usr/local/lib/nodejs/node-${NODE_VERSION}-linux-x64/bin

# install yarn
RUN npm install -g yarn
