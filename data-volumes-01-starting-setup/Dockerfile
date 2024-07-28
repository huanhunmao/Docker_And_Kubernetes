FROM node:14

WORKDIR /app

RUN npm config set registry https://registry.npmmirror.com

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

CMD [ "node", "server.js" ]