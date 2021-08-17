# 认识一下 HYBot

一个免费开源的 **Javascript** 异步机器人开发框架。

HYBot 音同 *Hi, Bot* ，意在表达“与你的机器人说 Hi”之意。

## 有什么用

1. 在几分钟内搭建自己的机器人。
2. 使用 Javascript 为机器人的功能添砖加瓦。
3. 与朋友们使用机器人，增进友情 & 自己使用机器人，提升效率。

## 特性

这里介绍一些 HYBot 不同于其他 Bot 框架的特性。

### 使用 Javascript 编写插件

有些框架使用 Python、Java、Kotlin 抑或是易语言开发插件，存在一些不能跨平台或需要安装各种各样的支持库的问题，对于要立刻尝鲜的用户并不是一个好主意。得益于 Javascript 依赖程度低的特性，HYBot 可以在各种系统下自由使用，尽力减小用户的使用困难度。（防喷提示：不是指用这些语言不好，而是说这些语言相对于 JS 来说依赖度更高一些）

### 多协议支持

HYBot 并不仅限于 QQ，下面列表是我们支持的协议：

| 协议平台 | 协议版本    | 通信方式           |
| -------- | ----------- | ------------------ |
| QQ       | OneBot v11  | WebHook + HTTP GET |
| Telegram | Bot API 5.3 | WebHook + HTTP GET |
| Telegram | Bot API 5.3 | 长轮询 + HTTP GET  |

注：其中 **通信方式** 字段中，加号前面的为接收信息的方式，加号后面的为发送信息的方式。

## 后续实现功能

- [ ] 插件权限申请（类似酷Q）
- [ ] 官方插件管理器（与插件授权 API 互联的通道）imyMuyang@pluginCenter.HY.js
- [ ] Plugin Config & Database API
- [ ] 补充完整 API、事件与文档
- [ ] 更安全的 API 授权调用
- [ ] 同协议多 Bot 部署
