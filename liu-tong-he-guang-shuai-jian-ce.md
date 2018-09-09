流量统计：

流定义：

acl number 3005

rule 0 permit icmp source 10.204.32.13 0 destination 10.204.6.166 0

rule 1 permit icmp source 10.204.6.166 0 destination 10.204.32.13 0

定义类：

traffic classifier classifier\_1

if-match acl 3005

流行为：

traffic behavior behavior\_1

accounting

定义策略：

qos policy policy

classifier classifier\_1 behavior behavior\_1

interface gigabitethernet 1/0/1

qos apply policy policy inbound



H3C光衰检测命令：

display transceiver interface GigabitEthernet 1/1/1   //查看光模块的参数

display transceiver diagnosis interface GigabitEthernet 1/1/1   //查看光模块的收发光功率值。

