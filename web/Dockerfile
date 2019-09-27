# develop stage
FROM node:11.1-alpine as develop-stage
WORKDIR /usr/src/web
COPY package*.json ./
RUN npm install
COPY . .

# build stage
FROM develop-stage as build-stage
CMD ["npm", "run", "build"]

# production stage
# TODO
