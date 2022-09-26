# dockerfiles

常用团队docker镜像，方便维护、升级。


## 各系统软件源

### Ubuntu

| 系统代号 | 版本  |
| -------- | ----- |
| precise  | 12.04 |
| trusty   | 14.04 |
| vivid    | 15.04 |
| xenial   | 16.04 |
| zesty    | 17.04 |

### Debian

| 系统代号 | 版本 |
| -------- | ---- |
| squeeze  | 6.x  |
| wheezy   | 7.x  |
| jessie   | 8.x  |
| stretch  | 9.x  |
| buster   | 10.x |

**查询Linux版本**

方法一

    cat /etc/issue

方法二

    source /etc/os-release
    echo $VERSION_ID
    echo ${VERSION_ID%.*}


##  参考资料
- [[官方文档] Docker Documentation](https://docs.docker.com/)
- [[镜像] mysql 镜像说明](https://hub.docker.com/_/mysql/)
- [[镜像] php 镜像说明](https://hub.docker.com/_/php/)
- [[镜像站] 阿里云开源镜像站](https://opsx.alibaba.com/mirror)
- [[镜像站] 腾讯开源镜像站](https://mirrors.cloud.tencent.com/index.html)
- [[镜像站] 网易开源镜像站](http://mirrors.163.com/)
- [[镜像站] 清华大学开源软件镜像站](https://mirrors.tuna.tsinghua.edu.cn/help/debian/)
- [[镜像加速] 阿里云](https://cr.console.aliyun.com/)
- [alpine 包查找](https://pkgs.alpinelinux.org/packages)
- [php 扩展包查找](https://pecl.php.net/)