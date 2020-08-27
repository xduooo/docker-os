FROM alpine:3.12

ARG TIMEZONE="Asia/Shanghai"

RUN sed -i "s/dl-cdn.alpinelinux.org/mirrors.aliyun.com/g" /etc/apk/repositories \
    && apk update && apk add --no-cache tzdata \
    && cp /usr/share/zoneinfo/${TIMEZONE} /etc/localtime \
    && echo ${TIMEZONE} > /etc/timezone \
    && apk del tzdata \
    && rm -rf /var/cache/apk/*