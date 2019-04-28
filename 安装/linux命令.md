#一、服务开闭，以防火墙为例

##1、开闭防火墙命令的基本使用
启动：service firewalld start

关闭:service firewalld stop

重启:service firewalld restart

查看状态 service firewalld status 

service命令是centos7 之前的系统服务管理命令，从centos7开始使用
systemctl 

##2、systemctl 命令开闭防火墙
启动：systemctl start firewalld.service

关闭：systemctl stop firewalld.service

重启：systemctl restart firewalld.service

查看状态：systemctl status firewalld.service

##3、开机启动设置
开机启动：systemctl enable firewalld.service

开机不启动:systemctl disable firewalld.service

查看是否开机启动:systemctl is-enabled firewalld.service

##4、特殊用法
查看服务是否运行: systemctl is-active firewalld.service





	