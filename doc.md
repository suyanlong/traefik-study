# 测试traefik

## 注意事项

* 编写配置文件，在编写规则时，需要注意规则的语法规范，否则无法负载均衡。

* 每一个模块的说明都不一样，需要查看帮助文档以及使用实例。 

* 配置文件的编写比较麻烦，但是建议学会用配置文件的形式启动traefik实例。

## 启动traefik

traefik -c traefil.toml

## 镜像启动
docker run -d -p 8080:8080 -p 80:80 -v $PWD/traefik.toml:/etc/traefik/traefik.toml traefik

## 帮助文档
https://docs.traefik.io

## 学习心得

其实搭建环境还比较方便的，就一个二进制程序，运行制定参数就行了，主要麻烦的地方是，traefik参数比较多，每一个参数的意义需要明白，因此，建议熟读帮助文档，多事件操作。
