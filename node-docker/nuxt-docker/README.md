NODE version: 12.1.0
```bash
# eg
$ docker build -t nuxt-docker docker-path
$ docker run -dit -p localhost/8080:3000 -v localhost:/apps nuxt-docker
```
**目前**的想法是让开发的应用运行在各自独立的环境中，抛出接口信息给主机来访问。

**这样**也不会因为应用的重复默认端口而报错，从而需要修改配置来运行多个开发应用。

**还有**个好处是可以直接模拟线上环境。

**相比**之前自己的php使用docker创建一个lamp环境，使用nginx反向代理到主机，还要修改本机hosts来说，更佳高效，开箱即用。

**可以**代替pm2类似的守护进程来维护程序