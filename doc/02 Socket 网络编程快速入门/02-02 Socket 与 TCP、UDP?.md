# Socket 与 TCP、UDP

> 概念

* 简单来说是 IP 地址与端口的结合协议（RFC 793）
* 一种地址与端口的结合描述协议
* TCP/IP 协议的相关 API 的总称，是网络 Api 的集合实现
* 涵盖了：Stream Socket/Datagram Socket

> 作用与组成

* 在网络传输中用于唯一标识两个端点上的连接
* 端点：包括（IP + Port）
* 4 个要素：客户端地址、客户端端口、服务器地址、服务器端口
* IP Address + Port number = Socket

> Socket 之 TCP

* TCP 是面向连接的通信
* 通过三次握手建立连接，通讯完成时要拆除连接
* 由于 TCP 是面向连接的，所以只能用于端到端的通信
* TCP 传输
   * A --> TCP DATA --> B
   * A <-- TCP ACK -- B 

> Socket 之 UDP

* UDP 是面向无连接的通讯协议
* UDP 数据包括目的端口号和源端口号信息
* 由于通讯不需要连接，所以可以实现广播发送，并不局限于端到端
* UDP 传输
    * A --> UDP DATA --> B
    * A --> UDP DATA --> C

> Client-Server Application

* TCP/IP 协议中，两个进程间通信的主要模式为：CS 模型
* 主要目的：协同网络中的计算机资源、服务模式、进程间数据共享
* 常见的：FTP、SMTP、HTTP
