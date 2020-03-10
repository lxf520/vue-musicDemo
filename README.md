# lxf-music

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

linux 系列的ubuntu 
### 基本命令 
ls  list 查看当前目录结构
ls -all  查看所有目录

连接服务器 
改完密码重启一下服务器
1. ssh 命令 (xshell)
```
ssh root@123.56.91.78
回车输入密码 
```
2. ftp协议上传文件  fz (fileZilla)

apt-get 用来在ubutun 系统安装软件
apt-get  update  更新远程仓库 
apt-get  install  软件的名字
apt-get  remove  软件的名字

#### 网页上线
所有的人在外网的情况下访问网页
apt-get  install nginx

nginx 命令启动
nginx -s stop 停止
nginx -s relod 重载

打开阿里云的80端口，不然访问不了

/etc/nginx  nginx 软件所在目录
/var/www ...   nginx 默认的www目录

#### nginx 代理转发
vue项目中的开发环境 有node服务器可以做代理跨域
打包上线之后没有node开发环境 代理全部失效
服务器下 配置文件
```
/etc/nginx/sites-enabled/default 
location ^~/小暗号/{
  proxy_pass  转发路径/;
}
```
