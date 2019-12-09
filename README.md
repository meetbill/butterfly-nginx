# butterfly_nginx
butterfly  nginx 部署

```
webserver
├── cache
│   ├── client_body
│   ├── fastcgi
│   ├── proxy
│   ├── scgi
│   └── uwsgi
├── conf
│   ├── mime.types
│   └── nginx.conf
├── logs
│   ├── butterfly.access.log
│   ├── error.log
│   └── nginx.pid
├── run.sh
├── sbin
│   └── nginx
└── __stdout
```

## 操作

> * (1) [编译 nginx](https://github.com/meetbill/op_practice_book/blob/master/doc/web/nginx.md)
> * (2) 将编译后的 nginx 放到 webserver/sbin 目录
> * (3) 将 webserver 放到 butterfly 目录中，即

```
butterfly
├── conf
├── handlers
├── logs
├── main.py
├── run.sh
├── static
├── __stdout
├── templates
├── test
├── test_handler.py
├── third
├── webserver -------------------------- 将 webserver 放到 butterfly 项目目录下
├── wsgiapp.py
└── xlib
```

> * (4) 配置：配置 webserver/conf/nginx.conf 修改端口
> * (5) 启动：cd webserver/ & bash run.sh start
