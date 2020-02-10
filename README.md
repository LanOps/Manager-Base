# Base image with PHP & Nginx


docker buildx is require to build multiple archs

```docker buildx build --platform linux/amd64,linux/arm/v7 --no-cache --push -t th0rn0/php-nginx-base:latest .```

Notes:

Some weird stuff going on with the builds. Need to investigate.

```docker run --rm --privileged docker/binfmt:820fdd95a9972a5308930a2bdfb8573dd4447ad3```
```systemctl status systemd-binfmt```
