

# 环境搭建

## 安装nodejs

`apt-get install nodejs`

```
boeving@mint19:~$ nodejs -v
v8.10.0
boeving@mint19:~$ npm -v
3.5.2
boeving@mint19:~$ 
```

## 配置npm仓库

因为国内的网络环境，直接从npm官方源安装软件包速度会比较慢，甚至导致安装不成功。
我们可以安装nrm工具，用于管理软件源。

`$ sudo npm install -g nrm`

安装完成之后，列出可用的软件源
```
$ nrm ls
* npm ---- https://registry.npmjs.org/
  cnpm --- http://r.cnpmjs.org/
  taobao - https://registry.npm.taobao.org/
  nj ----- https://registry.nodejitsu.com/
  rednpm - http://registry.mirror.cqupt.edu.cn/
  npmMirror  https://skimdb.npmjs.com/registry/
  edunpm - http://registry.enpmjs.org/
```

在国内，我们可以使用taobao的源，速度还相对不错。

```
$ nrm use taobao
                        
Registry has been set to: https://registry.npm.taobao.org/
```


配置代理

另外，如果在特定网络环境下需要配置代理的话，可以使用如下命令配置。

```
$ npm config set proxy http://127.0.0.1:3128
$ npm config set http-proxy http://127.0.0.1:3128
$ npm config set https-proxy https://127.0.0.1:3128
```


## 搭建vue 开发环境 

安装 vue的脚



