FROM node

WORKDIR /app

# 配置 npm 使用国内镜像源
RUN npm config set registry https://registry.npmmirror.com

COPY package.json .

RUN npm install

COPY . .

CMD ["node", "app.js"]