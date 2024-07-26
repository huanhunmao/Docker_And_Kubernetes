# 使用官方 Node.js 镜像作为基础镜像
FROM node:14

# 设置工作目录为 /app
WORKDIR /app

# 配置 npm 使用国内镜像源
RUN npm config set registry https://registry.npmmirror.com

# 复制 package.json 和 package-lock.json 到工作目录
COPY package*.json ./

# 安装依赖
RUN npm install

# 将当前目录下的所有文件复制到容器的 /app 目录中
COPY . .

# 指定容器会监听的端口号为 80
EXPOSE 80

# 容器启动时执行的命令
CMD ["node", "server.js"]
