# 单网卡配置多个ip地址

```bash
# 进入网卡配置
vi /etc/network/interfaces
auto lo
iface lo inet loopback
auto eth0
iface eth0 inet static
address 172.18.156.97
netmask 255.255.240.0                                                                      
up route add -net 0.0.0.0 netmask 0.0.0.0 gw 172.18.159.253 dev eth0

auto eth0:1
iface eth0:1 inet static
address 192.168.0.1
netmask 255.255.240.0

auto eth0:2
iface eth0:2 inet static
address 192.168.0.2
netmask 255.255.240.0

# 重启网络
service networking restart

# 测试新增加的ip地址是否有效
ping 192.168.0.1
ping 192.168.0.2
```
