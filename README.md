# 搭建轻量级的开源 npm 私有部署仓库

### 1、查看你的系统是否已安装 docker 及 docker-compose

```
docker -v 或 docker version
docker-compose version
```

[docker 安装教程](https://www.runoob.com/docker/docker-tutorial.html)

### 2、设置目录及文件所有者和文件关联组（否则没有操作权限）

```
sudo chown -R 10001:65533 storage
sudo chown -R 10001:65533 plugins
sudo chown 10001:65533 htpasswd
```

### 3、启动

```
docker-compose up -d --build
```

使用详情请查看官方文档 [Verdaccio 官网](https://verdaccio.org)
