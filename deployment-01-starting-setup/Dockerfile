FROM node:14-alpine

WORKDIR /app

COPY package.json .

# 配置 npm 使用国内镜像源
RUN npm config set registry https://registry.npmmirror.com

RUN npm install

COPY . .

EXPOSE 80

CMD ["node", "app.js"]