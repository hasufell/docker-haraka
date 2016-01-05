# VERSION           0.0.1
# DOCKER-VERSION    1.2.0

FROM hasufell/gentoo-haraka:latest
MAINTAINER Julian Ospald <hasufell@posteo.de>

# copy everything as we cannot guarantee, that package.json, docs,
# plugins or config is present. use .dockerignore to exclude other
# files.
#ONBUILD COPY package.json /app/package.json
#ONBUILD COPY plugins /app/plugins
#ONBUILD COPY config /app/config
#ONBUILD COPY docs /app/docs
ONBUILD COPY . /app
ONBUILD RUN npm install
