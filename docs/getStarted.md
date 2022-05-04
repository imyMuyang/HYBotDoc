# 快速上手

如果需要搭建 QQ 机器人，HYBot 需要搭配 go-cqhttp 使用。

现在请给我们几分钟的时间让您快速体会到自己定制机器人的乐趣。

## 下载与初始化

HYBot 可以通过源代码进行使用。

### 使用教程

首先从 Github 上下载该项目的全部文件，然后启动您的 Node.JS 与 npm。（国内用户可使用 cnpm）

输入以下代码开始初始化 HYBot：

```sh
npm install
node .
```

当您的依赖已经全部安装时，您可以直接输入以下代码启动 HYBot：

```sh
node .
```

## OneBot 用户： 安装 go-cqhttp

到 [这里](https://github.com/Mrs4s/go-cqhttp/releases) 下载 go-cqhttp 的指定版本，然后根据 [这里](https://docs.go-cqhttp.org/) 的提示自行配置机器人。

## 配置与运行

一般来说，如果您的 go-cqhttp 安装在 HYBot 目录下，则不需要任何配置，HYBot 会自动读取您的 go-cqhttp 配置并自动处理。

以下是不同机器人平台的配置格式，请复制此内容到 config.js 中：

### OneBot

```js
module.exports = {
  QQ: {
    enable: true, 
    ws: 'ws://127.0.0.1:6700', 
    APIServer: 'http://127.0.0.1:8080', 
  },
};
```

**如果您是新手，并且还没有对go-cqhttp进行其他自定义，则请直接复制此内容即可！**

| 对应键    | 对应值                | 功能与作用                                                   |
| --------- | --------------------- | ------------------------------------------------------------ |
| enable    | true/false        | 是否启用                                               |
| ws      | ws://你的服务器地址            | 正向 WebSocket 服务器，可在 go-cqhttp 里面设置 |
| APIServer | http://你的服务器地址 | 发送消息的 API 服务器，可在 go-cqhttp 里面设置               |

## 世界，你好

如果您看到了 ``已连接到 ws://……`` 的字样，并且没有出现报错，则说明 HYBot 已经成功运行了。此时系统默认启用了样例插件，其中包含了对 Hello World 私聊消息的反馈。请移步到 QQ 私聊机器人，发送以下信息：``Hello World`` 。

``Hello World from HYBot v2!`` 此消息会被机器人发送回您的设备上。如果您的机器人响应正常，则 HYBot 没有被风控，您可以继续下一步的操作了。