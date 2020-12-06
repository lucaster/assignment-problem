FROM node:14

WORKDIR /app

COPY package.json .
COPY package-lock.json .

RUN npm ci

COPY . .

EXPOSE 3000

CMD node server.js

#docker build node-app -t lucaster/assignment1_nodeapp:1
#docker run -p 3000:3000 --name assignment1_nodeapp_1 --rm lucaster/assignment1_nodeapp