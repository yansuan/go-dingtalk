# 介绍

`go-dingtalk`是用Golang编写的钉钉开放平台服务端SDK，着重解决了开发者面临的一些问题，如：

- `access_token` 续期过期管理
- `TOP API` 生成签名
- 回调消息加解密
- SSO，SNS，企业免登处理

... 上述的举例仅仅涉及到一部分，在使用的过程中，你会发现使用`go-dingtalk`SDK开发基于钉钉的服务，变的那么简单，易用。

## 运行原理

`go-dingtalk`实际上是基于go标准库`net/http`开发的一套Api，一个Api的使用就像输入输出式的简单，在输入参数和输出结果上，定义了大量的结构体，你只需要遵循规则，就能很方便的进行开发，而无须关注实现细节。

## 已支持

- 企业`access_token`的续期过期管理以及免登流程
- 企业`sso_access_token`的续期过期管理以及免登流程
- 企业`sns_access_token`的续期过期管理以及免登流程
- 支持对钉钉事件回调消息签名的加解密
- 支持全部 Open api
- 支持全部 Top api，并且自动处理生成加密签名

## 待支持

- ISV`access_token`的续期过期管理以及免登流程
- 小程序`access_token`的续期过期管理以及免登流程