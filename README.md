# Workflow
## cd to dir
```bash
cd nginx
```
## build docker image
```bash
docker build . -t yinzhenyu87/nginx:latest
```
## push image to hub.docker.com
```bash
docker login
docker tag image_id yinzhenyu87/nginx:latest
docker push yinzhenyu87/nginx:latest
```

## buildx platform
```bash
docker buildx build \
--push \
--platform linux/arm/v7,linux/arm64/v8,linux/amd64 \ --tag yinzhenyu87/nginx:latest .
```