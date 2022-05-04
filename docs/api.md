# API 列表

这里是 HYBot 提供的 API 列表。开发者可以使用这些 API 来简化开发流程。

## imyMuyang@API

imyMuyang开发的通用API，包含一个 Logger 和其他小功能。

### Logger

| 函数名称 | 函数作用                   |
| -------- | -------------------------- |
| info     | 普通消息                   |
| error    | 普通报错消息               |
| warn     | 提示消息                   |
| fatal    | 致命消息（调用会结束运行） |
| act      | 操作消息                   |
| confirm  | 确认消息                   |

### 其他小功能

| 函数名称     | 函数名称                                              |
| ------------ | ----------------------------------------------------- |
| getConfig    | 通过指定配置文件名，获取用户配置                      |
| quickReplace | 快速替换指定内容，就如console.log里面的字符串替换一样 |

## imyMuyang@menuText

imyMuyang开发的菜单文本API，可以快速生成菜单文本供用户使用。