# Remote Control Server

This is the server of RemoteTouch, you should do the following steps to setup the server.
- 1.Prepare a server(Recommend CentOS) with public IP address and Java 17 environment.
- 2.Build the project and generate artifacts(rt.jar), then upload the rt.jar file to the server.
- 3.Grant permissions to rt.jar.
```
chmod 777 rt.jar
```
- 4.Ensure these four network ports(6899, 4245, 6898, 4244) are available, then run the following script.
```
nohup java -jar rt.jar &
```

OK, that's all.

## Notice
For some VPS, there are public IP and private IP at the same time, you may create ip_public.txt(Content is public IP address) and ip_private.txt(Content is private IP address) in the same directory as rt.jar, reboot and run the rt.jar again.
