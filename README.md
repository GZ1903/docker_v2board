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
git clone https://github.com/GZ1903/docker_v2board.git /usr/local/src/docker_v2board && cd /usr/local/src/docker_v2board && chmod +x docker_v2board.sh && ./docker_v2board.sh
```

`该脚本适应纯净系统安装，若已安装Docker环境，参照：https://hub.docker.com/r/gz1903/v2board`

### 如何管理？

#### 帐户密码

| MySQL_Default_USER | root                                    |
| ------------------ | --------------------------------------- |
| MySQL_Default_PASS | [v2board@qq.com](mailto:v2board@qq.com) |

| V2Board_Admin_USER | [v2board@qq.com](mailto:v2board@qq.com) |
| ------------------ | --------------------------------------- |
| V2Board_Admin_PASS | [v2board@qq.com](mailto:v2board@qq.com) |

#### 进入v2board容器管理

```shell
docker exec -it v2board /bin/bash
```

`exit退出容器`

#### 关键文件目录，支持更多扩展

Nginx_conf：`/etc/nginx/`

Nginx_html：`/usr/share/nginx/html/v2board/`

PHP_ini：`/etc/php.ini`

MySQL_conf：`/etc/my.cnf`

MySQL_date：`/var/lib/mysql`

MySQL_log：`/var/log/mysqld.log`

MySQL_Database：`v2board`

Supervisord_ini：`/etc/supervisord.d/v2board.ini`
