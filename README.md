# docker-env
快速启动各种 docker 环境

### nginx + php
```
cd nginx-php
docker compose up
```

### nginx + php + mysql

```
cd nginx-php-mysql
docker compose up
```

+ 如果需要最新版本 php，则将 `Dockerfile` 里面的 `php:5.6.19-fpm-alpine` 修改成 `php:fpm-alpine` 即可
+ php-fpm 中 启用了 `pdo` `pdo_mysql` `mysql` `mysqli` `sockets` 几个常用的拓展
+ mysql 中将默认变量中的 `NO_ZERO_DATE` 和 `NO_ZERO_IN_DATE` 去掉了

