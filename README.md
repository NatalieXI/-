# 委托代征项目关键技术
## 记录委托代征项目使用到的关键技术
### 前端技术（web端，移动端）
1. web端

Jquery、JqGrid、Datatables、NiceValidator、Viwer、Echarts

2. 移动端（微信公众号）

Vue、Webpack、Nodejs、SUI、Esline

### 后台技术

Spring、Strtus、Ibatis、WebService、QuartZ、Log4j、POI、Dom4j、SAXReader、EhCache(缓存)

### 数据库技术

Oracle、Redis、MySql、触发器、存储过程、kettle

### 服务器技术

Tomcat、Weblogic、Jenkins、Apache、Linux、Shell脚本、正则表达式

### 项目构建 版本控制

Maven、Ivy、Svn

### JAVA

数据结构（List、Map、Set）、

### 安全

1. 前端
问题一 基于DOM的跨站点脚本编制(分析客户端代码并清理其输入源代码)

问题二 已解密的登录请求(高发送敏感信息时，始终使用 SSL 和 POST（主体）参数)

问题三 使用HTTP动词篡改的认证旁路(将您的服务器配置为仅允许所需 HTTP 方法)

问题四 跨站点请求伪造(验证“Referer”头的值，并对每个提交的表单使用 one-time-nonce)

问题五 检测到隐藏目录(对禁止的资源发布“404 - Not Found”响应状态代码，或者将其完全除去)

问题六 缺少“Content-Security-Policy”头、缺少“X-Content-Type-Options”头、缺少“X-XSS-Protection”头
```
将您的服务器配置为使用“Content-Security-Policy”头
将您的服务器配置为使用“X-Content-Type-Options”头
将您的服务器配置为使用“X-Frame-Options”头
将您的服务器配置为使用“X-XSS-Protection”头
```
问题七 HTML注释敏感信息泄露(除去 HTML 注释中的敏感信息)

问题八 客户端（JavaScript）Cookie 引用(除去客户端中的业务逻辑和安全逻辑)

2. 后台程序
问题一 短信验证码无限发送（解决方法：对同一个IP发送短信的次数、频率进行限制） 

问题二 不传参数能查出所有信息（解决方法：isnotnull别瞎用 涉及到使用用户信息来查询的从session中获取）

问题三 SQL注入获取数据库名（解决方法：除非特殊需求传递参数的时候不要用$符号改用#号）




