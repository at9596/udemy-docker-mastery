FROM node:25-alpine

EXPOSE 3000

RUN apk add --update  tini

RUN mkdir -p /user/src/app

WORKDIR /user/src/app

COPY package.json  package.json

RUN npm install && npm cache clean --force

COPY . .

CMD [ "tini", "--", "./bin/www" ]