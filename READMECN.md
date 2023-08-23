# Remote Control Server

这是远程控制的服务器端，执行以下步骤让服务器跑起来。

1.准备一个有公网IP的服务器，安装JDK 17;

2.下载源码编译rt.jar并上传到服务器，或者你可以到[已发布版本](https://github.com/miekir163/RemoteControlOutput/tree/main/release)里下载；

3.授权读写；
```
chmod 777 rt.jar
```

4.确保端口已打开：6899, 4245, 6898, 4244，然后执行：
前台运行：
```
java -jar rt.jar
```

后台运行：
```
nohup java -jar rt.jar &
```

可以直接下载[客户端APK](https://github.com/miekir163/RemoteControlOutput/blob/main/release/V1.0/rt_realease_v1.0.apk) 和 [服务端JAR](https://github.com/miekir163/RemoteControlOutput/blob/main/release/V1.0/rt.jar) 进行体验！

## 注意事项
 - 阿里云的端口需要在阿里控制面板自行开放（出和入方向都要开放）；
 - 如果安装了宝塔面板，还要在宝塔开放端口；
 - 对于国内部分VPS，比如阿里云这些既有私网IP又有公网IP的服务器，你需要在rt.jar同一目录创建ip_public.txt（内容是公网IP） 和 ip_private.txt（内容是私网IP），然后重启服务器，再次执行其他rt.jar的命令。

## 支持作者
如果本项目有给你带来一些帮助，就请我喝杯咖啡吧。

[支付宝](https://github.com/miekir163/RemoteControlOutput/blob/main/image/alipay.jpg?raw=true){:target="_blank"}

[微信](https://github.com/miekir163/RemoteControlOutput/blob/main/image/wechat.jpg?raw=true){:target="_blank"}
