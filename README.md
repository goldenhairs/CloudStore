# 云储存

- oss - 阿里云云存储
- cos - 腾讯云云存储
- bos - 百度云云存储
- qiniu - 七牛云存储
- upyun - 又拍云存储

- ~~obs - 华为云云存储~~
- ~~local - 本地化存储~~

## 为什么要有这个项目？

自己开源的两个项目 [BookStack](https://github.com/TruthHun/BookStack)、
[DocHub](https://github.com/TruthHun/DocHub) 使用到云存储，
但是各个云存储服务商的接口都各不相同，使用起来非常麻烦，所以直接弄了这么一个云存储的集合，
设计统一的接口规范，以方便使用。

你不需要看各大云存储的文档，只需要看这里的集成，统一使用各大云存储

目前只是对云存储做一个简单的集成，更多功能集成，有待不断升级迭代.

## 目前实现的接口
以`bucket`为操作单位
- 上传文件对象（同时返回文件信息，如文件大小等）
- 获取文件对象链接地址 (分内网和外网以及签名链接地址)
- 获取文件对象基本信息 (文档大小、扩展名、更新时间)
- 获取文件对象列表
- `header` 设置 （仅对云存储邮箱）
- 删除文件对象
- 下载文件到云存
