ARG ARCH=amd64/
FROM ${ARCH}node:16.11.1-bullseye
RUN npm config set registry https://registry.npmmirror.com && npm i -g pnpm && pnpm config set registry https://registry.npmmirror.com
