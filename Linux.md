# Linux命令

### httpd的启动和停止

```shell
systemctl start httpd.service 			#启动httpd服务
systemctl stop httpd.service 			#关闭httpd服务
systemctl status httpd					#查看httpd状态

```

### firewalld防火墙

```
firewall-cmd --state
systemctl status firewalld		#查看防火墙状态
systemctl stop firewalld 		#关闭防火墙
systemctl start firewalld 		#开启防火墙
#重启防火墙
firewall-cmd --reload


#开启80端口
firewall-cmd --zone=public --add-port=80/tcp --permanent

#关闭80端口
firewall-cmd --zone=public --remove-port=80/tcp --permanent

#查询80端口是否开启
firewall-cmd --query-port=80/tcp

#查询开放列表
firewall-cmd --list-port


```

