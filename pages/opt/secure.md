## 6.13 安全管理

### 6.13.1 伪IP防护

内网只允许列表内的IP通过路由

![](http://static.toughcloud.net/toughsms/xs_2018-12-25_003154.png)


### 6.13.2 攻击防范

![](http://static.toughcloud.net/toughsms/xs_2018-12-25_003220.png)


### 6.13.3 连接数控制

通过策略限制TCP、UDP、ICMP、总连接数

![](http://static.toughcloud.net/toughsms/xs_2018-12-25_003253.png)

新增连接数控制策略

![](http://static.toughcloud.net/toughsms/xs_2018-12-25_003335.png)

- 策略优先级：策略执行的优先顺序，数字小，优先执行，范围1-65535
- 策略名称：标识策略名称
- VLAN：策略匹配条件，指定的外层VLAN标签
- 内层VLAN：策略匹配条件，指定的内层VLAN标签
- 内网数据线路：策略匹配条件，可以选择内网线路，默认全部内网线路
- 内网地址类型：策略匹配条件，数据包的源IP地址，可以指定IP群组
- 内网端口：策略匹配条件，数据包的源端口
- 外网地址类型：策略匹配条件，数据包的目的IP地址，可以指定IP群组
- 外网端口：策略匹配条件，数据包的目的端口
- 传输协议：策略匹配条件，可以选择TCP、UDP、ICMP，默认是所有传输协议
- 应用协议：策略匹配条件，可以选择协议或者自定义协议组

![](http://static.toughcloud.net/toughsms/xs_2018-12-25_003458.png)

- 每IP最大TCP连接数：每个IP最大的TCP连接数，默认0不限制
- 每IP最大UDP连接数：每个IP最大的UDP连接数，默认0不限制
- 每IP最大ICMP连接数：每个IP最大的ICMP连接数，默认0不限制
- 每IP最大连接数：每个IP最大的连接数，默认0不限制
- 生效时间：选择创建好的时间组，不填表示全部时间


### 6.13.4 IP-MAC绑定

绑定IP和MAC地址，预防ARP攻击

![](http://static.toughcloud.net/toughsms/xs_2018-12-25_003611.png)


### 6.13.5 MAC访问控制

通过MAC地址加入黑名单和白名单控制访问路由

![](http://static.toughcloud.net/toughsms/xs_2018-12-25_003648.png)


