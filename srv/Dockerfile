FROM node:lts-alpine

WORKDIR /usr/src/srv

COPY package*.json ./

RUN npm install

COPY . .

CMD ["npm", "run", "start"]