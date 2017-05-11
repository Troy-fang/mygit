# mygit
linux服务器运维课程：
一，服务器网络管理:
1.网卡管理：
/etc/sysconfig/network-scripts/ifcfg-eth0    网卡配置文件（centos6）
NetworkManager 是网络图标 （centos6里对服务的开机自动开启和关闭通过chkconfig来实现）chkconfig network off/on
centos7中开机自动启动和关闭命令：systemctl disable XXXXX
bash-completion  命令自动补全包
systemctl mask XXXXX    centos7中对服务进行锁定  （unmask 解锁）
ifconfig lo 1.1.1.1 netmask 255.255.255.0 up  命令行配置网卡
ip link show lo     查看网卡两层信息
ip addr show lo     查看网卡三层信息
ifdown lo           关闭网卡
ifup lo             开启网卡
ip link set down lo 关闭网卡二层
ip addr add xx.xx.xx.xx/24 lo del lo：1 
traceroute www.baidu.com   查询路由
tcpdump -i eth0      抓包命令
nslookup www.baidu.com dns解析地址
elinks    字符串浏览器
nc  万能工具
nmcli connection show --active 查看激活的网卡
2.网络桥接：
