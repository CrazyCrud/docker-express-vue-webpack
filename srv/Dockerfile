FROM node:lts-alpine

WORKDIR /usr/src/srv

COPY package*.json ./

RUN npm install -g nodemon

RUN npm install

COPY . .