# docker-os

Building
====================

Normal:

```
docker build -f debian/buster/Dockerfile -t xduooo/debian:buster .
```
```
docker build -f debian/buster/slim/Dockerfile -t xduooo/debian:buster-slim .
```
```
docker build -f centos/Dockerfile -t xduooo/centos:8 .
```
```
docker build -f alpine/Dockerfile -t xduooo/alpine:3.14 .
```

With ARGs:

```
docker build -f debian/buster/Dockerfile -t xduooo/debian:buster --build-arg TIMEZONE="Asia/Shanghai" .
```

Building ARGs
====================

| Key | Default | Description |
:----- | :-----: |:----------- |
|TIMEZONE  | "Asia/Shanghai" | The timezone. |