# 快速上手

如果需要搭建 QQ 机器人，HYBot 需要搭配 go-cqhttp 使用。

现在请给我们几分钟的时间让您快速体会到自己定制机器人的乐趣。

## 安装 HYBot 与依赖项

HYBot 有三种安装方式：基于源代码构建、使用自动构建版本启动与使用无依赖源代码启动。**如果您是新手，请使用自动构建版本启动。**

### 基于源代码构建

首先从 Github 上下载该项目的全部文件，然后启动您的 Node.JS 与 npm。（国内用户可使用 cnpm）

输入以下代码开始初始化 HYBot：

```sh
npm i
node run
```

当您的依赖已经全部安装时，您可以直接输入以下代码启动 HYBot：

```sh
node run
```

### 使用自动构建版本启动

首先从 Github Realease 上下载自动构建版本（请根据您的操作系统与硬件架构选择构建的版本，如windows系统则请选择.exe后缀的）

然后用您喜欢的方式启动这个程序（如windows系统则直接双击或以管理员身份运行）

这里的构建基于 npm 上的开源库 pkg。

### 使用无依赖源代码启动

首先从 Github Realease 上下载无依赖源代码版本（名称为 go.js）

然后输入以下代码开始启动 HYBot

```sh
node go
```

## [OneBot 用户] 安装 go-cqhttp

请到 [这里](https://github.com/Mrs4s/go-cqhttp/releases) 下载 go-cqhttp 的指定版本，然后根据 [这里](https://docs.go-cqhttp.org/) 的提示自行配置您的机器人。

**注意，HYBot 不是 go-cqhttp。如果您在使用 go-cqhttp 中遇到任何疑问，请向 go-cqhttp 官方寻求帮助。HYBot 开发者没有义务帮助您解决此问题。**

## 配置 HYBot

一般来说，如果您的 go-cqhttp 安装在 HYBot 目录下，则不需要任何配置，HYBot 会自动读取您的 go-cqhttp 配置并自动处理。

以下是不同机器人平台的配置格式，请复制此内容到 ./config/bot.yml 中：

### OneBot

```yaml
QQ:
  enable: 
  APIServer: 
  port: 
```

| 对应键    | 对应值                | 功能与作用                                                   |
| --------- | --------------------- | ------------------------------------------------------------ |
| enable    | enable/disable        | 此协议是否启用                                               |
| APIServer | http://你的服务器地址 | 发送消息的 API 服务器，可在 go-cqhttp 里面设置               |
| port      | 一个正整数            | 监听 WebHook 的端口，只要是空闲的就可以了，会自动应用到 go-cqhttp里面 |

### Telegram

```yaml
TG:
  enable: 
  APIServer: 
  proxy: 
  token: 
  port: 
```

| 对应键    | 对应值                | 功能与作用                                                   |
| --------- | --------------------- | ------------------------------------------------------------ |
| enable    | enable/disable        | 此协议是否启用                                               |
| APIServer | http://你的服务器地址 | 发送消息的 API 服务器                                        |
| proxy     | noProxy/你的代理地址  | 如果需要代理连接，就输入代理地址，否则输入noProxy            |
| token     | 你 Bot 的 Token       | 没它啥事都干不了，从 @BotFather 处获取                       |
| port      | 一个正整数            | 监听 WebHook 的端口，只要是空闲的就可以了，会自动向服务器提交请求 |

关于 APIServer：这个服务器地址可以选择以下内容：

| 名称             | 服务器地址                   | 备注                           |
| ---------------- | ---------------------------- | ------------------------------ |
| 官方服务器       | https://api.telegram.org     | 安全，但国内需要代理           |
| HYBot 免代服务器 | https://tg.hanye.workers.dev | 安全免代，但是需要授权         |
| Telegram Rest    | https://telegram.rest        | 免代，不确定安全性，作者没用过 |

关于 HYBot 免代服务器的授权，请加 imyMuyang 的 QQ 好友（2121683039）发送 Bot 用途与 Token 就可以了。

**免滥用提示：数据流量有限，为防止滥用 API 所以需要授权，作者不会随意使用您的 Bot Token 进行乱七八糟的操作。**

