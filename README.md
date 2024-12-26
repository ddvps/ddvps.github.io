# 使用教程：
阿里云DD安装Windows用27、31
安装重装系统的前提组件:

Debian/Ubuntu:


```
apt-get install -y xz-utils openssl gawk file wget screen && screen -S os
```

RedHat/CentOS:


```
yum install -y xz openssl gawk file glibc-common wget screen && screen -S os
```



如果出现异常，请刷新Mirrors缓存或更换镜像源。

RedHat/CentOS:


```
yum makecache && yum update -y
```



Debian/Ubuntu:


```
apt update -y && apt dist-upgrade -y
```


（ipv4忽略，NATipv6使用）快速使用一键设置NAT64地址


```
mv /etc/resolv.conf /etc/resolv.conf.bak && echo -e "nameserver 2001:67c:2b0::4\nnameserver 2001:67c:2b0::6" > /etc/resolv.conf
```


使用:


```
wget --no-check-certificate -O NewReinstall.sh https://git.io/newbetags && chmod a+x NewReinstall.sh && bash NewReinstall.sh
```



如为CN主机(部分主机商已不能使用)，可能出现报错或不能下载脚本的问题，可执行以下命令开始安装.


```
wget --no-check-certificate -O NewReinstall.sh https://jsd.onmicrosoft.cn/gh/a21922/ddos@master/NewReinstall.sh && chmod a+x NewReinstall.sh && bash NewReinstall.sh
```


41合1的系统一键DD选择界面，输入99则使用自定义镜像。 以上系统密码不为默认密码的均为网络收集，如有疑虑使用自己的自定义镜像。
41合一系统密码：


```
1、CentOS 7.7 (已关闭防火墙及SELinux，默认密码Pwd@CentOS)
2、CentOS 7 (默认密码cxthhhhh.com)
3、CentOS 7 (支持ARM64、UEFI，默认密码cxthhhhh.com)
4、CentOS 8 (默认密码cxthhhhh.com)
5、Rocky 8 (默认密码cxthhhhh.com)
6、Rocky 8 (支持UEFI，默认密码cxthhhhh.com)
7、Rocky 8 (支持ARM64、UEFI，默认密码cxthhhhh.com)
8、CentOS 9 (默认密码cxthhhhh.com)
9、CentOS 6 (官方源原版，默认密码Minijer.com)
10、Debian 11 (官方源原版，默认密码Minijer.com)
11、Debian 10 (官方源原版，默认密码Minijer.com)
12、Debian 9 (官方源原版，默认密码Minijer.com)
13、Debian 8 (官方源原版，默认密码Minijer.com)
14、Ubuntu 20.04 (官方源原版，默认密码Minijer.com)
15、Ubuntu 18.04 (官方源原版，默认密码Minijer.com)
16、Ubuntu 16.04 (官方源原版，默认密码Minijer.com)
17、Windows Server 2022 (默认密码cxthhhhh.com)
18、Windows Server 2022 (支持UEFI，默认密码cxthhhhh.com)
19、Windows Server 2019 (默认密码cxthhhhh.com)
20、Windows Server 2016 (默认密码cxthhhhh.com)
21、Windows Server 2012 (默认密码cxthhhhh.com)
22、Windows Server 2008 (默认密码cxthhhhh.com)
23、Windows Server 2003 (默认密码cxthhhhh.com)
24、Windows 10 LTSC (默认密码Teddysun.com)
25、Windows 10 LTSC (支持UEFI，默认密码Teddysun.com)
26、Windows 7 x86 Lite (默认密码nat.ee)
27、Windows 7 x86 Lite (阿里云专用，默认密码nat.ee)
28、Windows 7 x64 Lite (默认密码nat.ee)
29、Windows 7 x64 Lite (支持UEFI，默认密码nat.ee)
30、Windows 10 LTSC Lite (默认密码nat.ee)
31、Windows 10 LTSC Lite (阿里云专用，默认密码nat.ee)
32、Windows 10 LTSC Lite (支持UEFI，默认密码nat.ee)
33、Windows Server 2003 Lite (C盘默认10G，默认密码WinSrv2003x86-Chinese)
34、Windows Server 2008 Lite (默认密码nat.ee)
35、Windows Server 2008 Lite (支持UEFI，默认密码nat.ee)
36、Windows Server 2012 Lite (默认密码nat.ee)
37、Windows Server 2012 Lite (支持UEFI，默认密码nat.ee)
38、Windows Server 2016 Lite (默认密码nat.ee)
39、Windows Server 2016 Lite (支持UEFI，默认密码nat.ee)
40、Windows Server 2022 Lite (默认密码nat.ee)
41、Windows Server 2022 Lite (支持UEFI，默认密码nat.ee)
99、自定义镜像
```


