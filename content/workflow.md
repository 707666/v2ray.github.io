# 工作机制

## 个人使用
你需要至少两个 V2Ray Server（设为 A、B）才可以正常穿墙。以网页浏览为例，你的浏览器和 A 以 Socks 5 协议通信，
B 和目标网站之间以 HTTP 协议通信，A 和 B 之间使用 V2Ray 的自有协议 [VMess](#a=vmess-zh-cn) 通信，如下图：

![](/content/v2ray.png)

通常 Server A 运行在你自己的电脑，Server B 运行在一台海外的 VPS 中。

上述的架构是一个简单的客户端 / 服务器架构。Server A 充当客户端，用于加密并发送网络请求；Server B 充当服务器，
用于解密并响应网络请求。

## 多人共享
V2Ray 也可被部署成多服务器模式……（未完待续）
