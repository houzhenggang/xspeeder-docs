## 6.14 系统管理


### 管理接口

配置查看路由管理口的地址

![](http://static.toughcloud.net/toughsms/xs_2018-12-25_001010.png)


### 认证信息

如无授权、授权过期、授权不可用，会限制并发数在10000，而且DNS策略和DPI功能无法使用

![](http://static.toughcloud.net/toughsms/xs_2018-12-25_001054.png)

### 备份还原

当前路由的配置和程序都保存下来，将备份下来的包还原到路由上，会重启路由

![](http://static.toughcloud.net/toughsms/xs_2018-12-25_001142.png)


### 定时邮件发送

填写SMTP邮件发送服务器信息，开启后定时每天05:01发送到指定的接收邮箱

![](http://static.toughcloud.net/toughsms/xs_2018-12-25_001226.png)


### 系统升级

从官网获取的升级包升级路由

![](http://static.toughcloud.net/toughsms/xs_2018-12-25_001322.png)


### 重启服务

路由程序控制重启，路由设备重启和关闭路由设备，需要验证admin的密码


![](http://static.toughcloud.net/toughsms/xs_2018-12-25_001419.png)


### 系统参数

![](http://static.toughcloud.net/toughsms/xs_2018-12-25_001458.png)

- 开启DPI：是否开启深度包识别
- 开启DFI：是否开启流识别功能
- 开启硬件校验和：是否开启网卡的硬件校验和
- 开启流控增强：是否开启TCP的强制流控功能
- 路由组播：桥模式下是否转发组播信号
- 处理内网IP分片：是否开启内网IP分片包处理，默认开启
- 处理外网IP分片：是否开启外网IP分片包处理，默认开启
- 主动检测IP分片超时：开启IP分片超时机制
- 线路负载附加轮询：线路群组增强分配
- 流量记录到内存：将后台流量数据记录在内存，重启机器后，会丢失流量记录
- 实时流量记录到内存：将实时流量记录在内存，降低磁盘开销
- 开启IP协议流量记录：是否开启IP协议记录到文件，不开启无法展示协议应用情况
- 开启IP流量记录：是否开启IP流量记录到文件，不开启无法展示线路速率情况
- 开启GPS信息记录：是否开启GPS记录
- 只统计有效IP：只统计有内外网交互的IP地址
- 防运营商共享检测：通过改变流特征防止运营商检测NAT
- 开启智能节电：是否开启路由智能节电
- 多维缓存命中牵引：开启针对多维缓存的牵引模式
- 协议追踪无限制：勾上表示去除根据内存来追踪IP的机制，如内存不够可能会造成程序因内存不足崩溃
- 默认允许wan2wan：不勾上则允许路由上的wan线路之间互通，勾上则不允许路由上的wan线路之间互通，默认允许路由上的wan线路之间互通

![](http://static.toughcloud.net/toughsms/xs_2018-12-25_001622.png)

- NATtry：默认20
- DNS代理：开启DNS代理功能，默认0关闭
- DNS TTL：DNS缓存生存时间
- 虚拟网卡允许端口：允许访问路由的指定端口，如全部关闭，则路由只能通过管理口访问
- RSS mode：网卡多队列处理模式,数值范围0-2，默认1，参考监控中心-RSS信息来修改
- QOS流控限速微调：QOS里限速微调
- TCP MSS：可指定TCP的MSS数值，默认0，根据线路的MTU计算

### 用户管理


#### 角色管理

![](http://static.toughcloud.net/toughsms/xs_2018-12-25_001800.png)

![](http://static.toughcloud.net/toughsms/xs_2018-12-25_001825.png)

授权操作，可以指定角色可以操作的菜单列表

![](http://static.toughcloud.net/toughsms/xs_2018-12-25_001915.png)


#### 用户管理

![](http://static.toughcloud.net/toughsms/xs_2018-12-25_001952.png)

新增后台用户

![](http://static.toughcloud.net/toughsms/xs_2018-12-25_002022.png)








