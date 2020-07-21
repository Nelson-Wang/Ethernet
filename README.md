# Ethernet
ETH测试基础知识补充

## 以太网口的工作模式
1. 10M半双工
2. 10M全双工
3. 100M半双工
4. 100M全双工
5. 自协商模式
  * 自协商功能完全由物理层芯片设计实现，因此并不使用专用数据包或带来任何高层协议开销
  * 以太口两端，若果一端设置为固定模式，另一端为自协商，那么自协商那一段职能工作在半双工模式
  * 一端全双工，一端半双工，在
  


## MTU
### MTU-数据链路层协议
在7层网络协议中，MTU是数据链路层的概念。MTU限制的是数据链路层的payload，也就是上层协议的大小，例如IP，ICMP等。
* OSI中的层------------------------功能----------------------------------TCP/IP协议族
 * 应用层--------文件传输、电子邮件、文件服务、虚拟终端---------TFTP、HTTP、SNMP、FTP、SMTP、DNS、Telnet
 * 表示层----------数据格式化，代码转换，数据加密----------------------------无协议
 * 会话层-----------解除或建立与别的接点的联系-------------------------------无协议
 * 传输层-----------------提供端对端的接口----------------------------------TCP、UDP
 * 网络层-----------------为数据包选择路由-----------------------IP，ICMP，RIP，OSPF，BGP，IGMP
 * 数据链路层--------传输有地址的帧以及错误检测功能----------------SLIP，CSLIP，PPP，ARP，RARP，MTU
 * 物理层-----------以二进制数据形式在物理媒体上传输数据------------ISO2110，IEEE802，IEEE802.2

### MTU作用
