# 1、点击浏览器请求过程

![image-20210120214559666](geekTime-http.assets/image-20210120214559666.png)



# 2、IP是怎么来的 DHCP

## 网络请求过程相同网段和不同网段

1. <font color=red size=5x>**网络请求首先检查是否是相同网段,如果是相同网段,会发送ARP请求,获取mac地址**</font>

2. <font color=r size=5x>**如果不是同一网段回请求网关,如果没配置网关,根本发不出去**</font>

<font color=red size=5x></font>



## 动态主机配置DHCP

动态主机配置协议（Dynamic Host Configuration Protocol），简称 DHCP。

1. <font color=red size=5x>**请求地址发送0.0.0.0的广播包,目标地址为255.255.255.255,广播包封装了 UDP，UDP 封装了 BOOTP。其实 DHCP 是 BOOTP 的增强版**</font>

2. <font color=r size=5x>**即使有多个DHCP服务器,总会有第一个去响应,给出ip**</font>

3. <font color=red size=5x>**请求的ip收到后,回应DHCP收到,==DHCP服务器收到后回应ACK,客户机表示收到,并将信息存储==**</font>

4. <font color=red size=5x>**客户机会在过去50%的时候去续租,根据新的回应跟新配置信息**</font>



















































































