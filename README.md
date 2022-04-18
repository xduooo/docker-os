# docker-os

# Building

Normal:

```
docker build -f debian/bullseye/Dockerfile -t xduooo/debian:bullseye .
```

```
docker build -f debian/bullseye/slim/Dockerfile -t xduooo/debian:bullseye-slim .
```

```
docker build -f alpine/Dockerfile -t xduooo/alpine:3.15 .
```

With ARGs:

```
docker build -f debian/bullseye/Dockerfile -t xduooo/debian:bullseye --build-arg TIMEZONE="Asia/Shanghai" .
```

# Building ARGs

| Key      |     Default     | Description   |
| :------- | :-------------: | :------------ |
| TIMEZONE | "Asia/Shanghai" | The timezone. |
