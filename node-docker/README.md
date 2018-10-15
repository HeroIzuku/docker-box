```bash
$ docker build -t docker-name docker-path
$ docekr run -dit -p host/8080:container/3000 -v host/apps:container/apps docker-name
```
**目前**的想法是让开发的应用运行在各自独立的环境中，抛出接口信息给主机来访问。

**这样**也不会因为应用的重复默认端口而报错，从而需要修改配置来运行多个开发应用。

**还有**个好处是可以直接模拟线上环境。

**相比**之前自己的php使用docker创建一个lamp环境，使用nginx反向代理到主机，还要修改本机hosts来说，更佳高效，开箱即用。

**可以**代替pm2类似的守护进程来维护程序