FROM node:14

WORKDIR /app

# 配置 npm 使用国内镜像源
RUN npm config set registry https://registry.npmmirror.com

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

# ENV MONGO_INITDB_ROOT_USERNAME=marxu
# ENV MONGO_INITDB_ROOT_PASSWORD=123

CMD [ "npm", "start" ]

