# Remote Control Server

## [中文文档](https://github.com/miekir163/RemoteControlServer/blob/main/READMECN.md)

This is the server of RemoteTouch, you should do the following steps to setup the server.
- 1.Prepare a server(Recommend CentOS) with public IP address and Java 17 environment.
- 2.Build the project and generate artifacts(rt.jar), or download rt.jar from [RELEASE](https://github.com/miekir163/RemoteControlOutput/tree/main/release), then upload the rt.jar file to the server.
- 3.Grant permissions to rt.jar.
```
chmod 777 rt.jar
```
- 4.Ensure these four network ports(6899, 4245, 6898, 4244) are available, then run the following scripts.
For foreground:
```
java -jar rt.jar
```

For background:
```
nohup java -jar rt.jar &
```

OK, that's all.

Download [Client APK](https://github.com/miekir163/RemoteControlOutput/blob/main/release/V1.0/rt_realease_v1.0.apk) and [Server JAR](https://github.com/miekir163/RemoteControlOutput/blob/main/release/V1.0/rt.jar) to start your trail!

## Notice
For some VPS, there are public IP and private IP at the same time, you may create ip_public.txt(Content is public IP address) and ip_private.txt(Content is private IP address) in the same directory as rt.jar, reboot and run the rt.jar again.
