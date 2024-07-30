FROM node:14

WORKDIR /app

RUN npm config set registry https://registry.npmmirror.com

COPY package.json .

RUN npm install

COPY . .

ARG DEFAULT_PORT=80

ENV PORT $DEFAULT_PORT

EXPOSE $PORT

CMD [ "npm", "start" ]