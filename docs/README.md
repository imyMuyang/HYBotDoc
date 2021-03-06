# 认识一下 HYBot

一个免费开源的 **Javascript** 聊天机器人开发框架。

现行版本为 **v2**（因为 v1 被屎山代码搞垮了，故全部重写开发）


## 有什么用

1. 在几分钟内搭建自己的机器人。
2. 借助 Packer 和 Plugin 自定义机器人功能。
3. 为自己 / 群友 / 公众提供形式多样，简介便利的服务。

## 特性

这里介绍一些 HYBot 不同于其他 Bot 框架的特性。

### 多系统支持

得益于 Node.JS 与 go-cqhttp 极为良好的多系统支持，HYBot 可以在任何支持运行依赖库上的系统运行。

### 插件高效能

采用 Node.JS 自带的插件机制，所有插件都可以与 HYBot 契合，组件化设计让后续代码维护更加简单，极大化减少阻塞情况。

### 高度自定义

从各种协议收到消息的第一刻起，我们把所有操作全部交给插件处理，在官方提供的各种功能全面丰富的插件与包装器外，您可以自由决定消息的处理机制。自定义的消息内容？个性化的处理机制？都由你来决定！

## 后续实现功能

- [ ] 插件权限申请
- [ ] 插件管理器
- [ ] Plugin Config & Database API
- [ ] 完整 API、事件与文档
- [ ] 同协议多 Bot 部署

---

准备好了？那我们就 [开始](/getStarted?id=%e5%bf%ab%e9%80%9f%e4%b8%8a%e6%89%8b) 吧！