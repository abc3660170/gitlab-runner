# 使用官方 nginx 1.27.2 镜像作为基础镜像
FROM nginx:1.29.0

# 安装 Node.js 22
RUN apt-get update && \
    apt-get install -y curl && \
    curl -fsSL https://deb.nodesource.com/setup_22.x | bash - && \
    apt-get install -y nodejs && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

# 验证 Node.js 和 npm 安装
RUN node -v && npm -v

# 设置工作目录
WORKDIR /usr/src/app

# 复制 nginx 配置文件（如果需要自定义）
# COPY nginx.conf /etc/nginx/nginx.conf

# 暴露端口
EXPOSE 80

# 启动 nginx
# CMD ["nginx", "-g", "daemon off;"]
CMD []