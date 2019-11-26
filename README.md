### Redis-config



### windows版本

- 注册服务

1. 启动

    运行
    redis-server.exe redis.windows.conf 
    就启动了redis

2. 测试
    另启一个cmd窗口，原来的cmd窗口不可关闭，不然Redis服务端就关闭了。

    运行redis-cli.exe -h 127.0.0.1 -p 6379 

    设置键值对 set key1 123
    取出键值对 get key2
    得到123说明测试成功

3. 安装成Windows服务—开机自启
    另启一个cmd窗口(管理员身份)

    运行redis-server --service-install redis.windows.conf

4. 输入：redis-server --service-start ( 启动服务 )

5. 输入：redis-server --service-stop （停止服务）

6. 启动指定的配置文件redis-server --service-start redis.windows-service.conf