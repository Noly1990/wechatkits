# Node.js 微信公众号后台通用工具箱

> 做一个简单通用的微信相关的工具箱

## 提示

模块还未可用，请勿下载使用

## 前言

经过简单的接触了下微信公众号后台的node.js相关的看发，最初是不愿意写这样一个工具包的，因为就一个原因，微信的开发文档太烂了，当中踩了一些坑都不是因为自己失误或无知，而是自己太天真，以为一些参数和接口比较标准，没想到光光参数大小写尴尬场景都遇到很多次，但后续想一想，以后保不齐还拜托不了开发微信相关的东西，就下定决心手撸一个出来，开始一定比较粗糙，有看到的看官莫见笑

## 开发进度

1. 主模块开发 <-
2. 附属部分
3. 测试部分

## 预计功能列表

- 用户授权登陆
- wxJSsdk相关
- 微信支付
- 消息回复
- 公众平台的其他可实现功能

## 使用前熟读

- [微信支付文档](https://pay.weixin.qq.com/wiki/doc/api/index.html)
- [签名校验工具](https://pay.weixin.qq.com/wiki/doc/api/jsapi.php?chapter=20_1)

## Installation

(功能还未可用，马上跟进开发，看到的请不要使用谢谢)npm上已经有一个co-wechat-api看了下还不错，但决定还是自己造个轮子，会逐步写下自己的思考过程和开发过程，放心不会偷看抄袭的，我就是自己写着玩，不求其他


## 开发思路

本工具箱，并不限定使用具体的某一个后台框架，但会对主流框架集成做一定的优化，不限制使用者的自由

同时也会对开发环境的需求做相应的设计，以满足具体情况下的高可用

微信相关的开发比较麻烦的点就在签名校验，主要实现通用的签名算法， 初步先实现MD5版本的加密签名，后续再跟进sha256的

## 实现列表

- 统一下单API => https://api.mch.weixin.qq.com/pay/unifiedorder
- JSsdk签名API