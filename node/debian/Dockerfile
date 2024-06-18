ARG ARCH=amd64/
FROM ${ARCH}node:18.20.3-slim
RUN npm config set registry https://registry.npmmirror.com \
  && sed -i 's/deb.debian.org/mirrors.tuna.tsinghua.edu.cn/g' /etc/apt/sources.list.d/debian.sources \
  && apt update \
  && apt install -y curl zip unzip git