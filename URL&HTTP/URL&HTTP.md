## 域名是什么

#### 域名就是对 IP 的别称

1. 如何得到某个网站对应的域名
   ![](得到域名.png)
   `ping 网址`
2. 知识点
   - 一个域名可以对应不同的 IP,这叫做负载均衡，放置一台机器扛不住
   - 一个 IP 可以对应不同域名，这个叫做共享主机，穷开发者会这么做

#### 域名和 IP 是怎么对应起来的

1. DNS 的定义
   - Domain Name System，DNS）是互联网的一项服务。 它作为将域名和 IP 地址相互映射的一个分布式数据库，能够使人更方便地访问互联网。 DNS 使用 TCP 和 UDP 端口 53。
2. 当输入www.baidu.com
   - 浏览器向电信/联通提供的 DNS 服务器询问www.baidu.com对应的什么IP
   - 电信/联通会回答一个 IP
   - 然后浏览器会向对应 IP 的 80/443 端口发送请求
   - 请求内容是查看www.baidu.com的首页
3. 为什么是 80 或 443 端口
   - 服务器默认用 80 提供 http 服务
   - 服务器默认用 443 提供 https 无法
4. `www.baidu.com`和`baidu.com`不是同一个域名
   - com 是顶级域名
   - `baidu.com`是二级域名（俗称一级域名）
   - `www.baidu.com`是三级域名（俗称二级域名）
   - `baidu.com`和`www.baidu.com`是父子关系
   - www 是多余的，一般不用

## 路径

#### 如何请求不同的页面

1. 路径可以做到
   - `https://developer.mozilla.org/zh-CN/docs/Web/HTML`
   - `https://developer.mozilla.org/zh-CN/docs/Web/CSS`
2. 工具
