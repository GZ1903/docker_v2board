## 一键部署docker_v2board

### 支持多版本系统

![](https://cdn.jsdelivr.net/gh/gz1903/tu/007.png)

| 系统   | 版本                |
| ------ | ------------------- |
| Centos | 7 或更高版本的系统  |
| Ubuntu | 16 或更高版本的系统 |
| Debian | 8 或更高版本的系统  |

#### 一键安装

```shell
yum -y install git && git clone https://github.com/GZ1903/docker_v2board.git /usr/local/src/docker_v2board && cd /usr/local/src/docker_v2board && chmod +x docker_v2board.sh && ./docker_v2board.sh
```

`该脚本适应纯净系统安装，若已安装Docker环境，参照：https://hub.docker.com/r/gz1903/v2board`
