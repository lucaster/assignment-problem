FROM node:14

WORKDIR /app

COPY package.json .
COPY package-lock.json .

RUN npm ci

COPY . .

EXPOSE 3000

CMD node server.js

#docker build node-app -t assignment1:nodeapp
#docker run -p 3000:3000 --name assignment1_nodeapp_1 --rm assignment1:nodeapp