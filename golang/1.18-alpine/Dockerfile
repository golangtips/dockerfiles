FROM golang:1.18-alpine
LABEL maintainer="hopher.hong@qq.com"


# 查询 alpine 版本 && 设置镜像源
RUN source /etc/os-release && printf "\
http://mirrors.aliyun.com/alpine/v${VERSION_ID%.*}/main\n\
http://mirrors.aliyun.com/alpine/v${VERSION_ID%.*}/community\n\
" > /etc/apk/repositories

# 更新源
RUN apk update --no-cache

# 时区设置 (date 命令可验证结果)
ENV TZ Asia/Shanghai
RUN apk add --no-cache tzdata \
    && ln -snf /usr/share/zoneinfo/$TZ /etc/localtime \
    && echo $TZ > /etc/timezone


# 环境变量设置
ENV GO111MODULE on
ENV CGO_ENABLED 0
ENV GOOS linux
ENV GOPROXY https://goproxy.cn,direct