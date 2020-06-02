FROM node:latest

RUN apt-get update && apt-get install -y ffmpeg imagemagick git
RUN mkdir -vp media/_thumbnails

RUN git clone https://github.com/colloqi/pisignage-server /pisignage/app

WORKDIR /pisignage/app

RUN npm install

COPY .env.js config/env/docker.js

ENV NODE_ENV docker
ENV MONGO_URI mongodb://mongodb/pisignage-server
ENV PORT 3000
EXPOSE 3000

CMD node server.js
