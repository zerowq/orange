### v0.5.0 2016.10.04

- 添加`Makefile`安装方式
- 支持通过命令行`orange store`初始化数据库
- 添加resty-cli支持
    - 支持orange start/stop/restart/reload/store等命令
- Break Change: 将*.conf配置移动到conf目录下


### v0.4.0 2016.09.24

- [x] 删除examples
- [x] 添加key auth插件
- [x] 限流插件rate limiting
- [ ] 防重提交机制（delay）
- [x] 补全新插件API文档

### v0.3.0 2016.07.21

- 添加HTTP Basic Auth插件

### v0.2.0

- API Server支持HTTP Basic Authorization
- 变量提取模块增加新类型
	- URL提取器支持一次提取多值
	- 以模板方式使用变量，格式为{{extractor.key}}
- 去除file store支持
- 提供Restful API及详细描述文档
- 分离内置的Dashboard，减少与API的耦合

### v0.1.1 2016.05.09

- 在使用MySQL作为存储时，为dashboard控制台添加账户系统


### v0.1.0 2016.05.04

特性:

- 配置项支持文件存储和MySQL存储
- 通过MySQL存储来简单支持集群部署
- 支持通过自定义插件方式扩展功能
- 默认内置六个插件
	- 全局状态统计
	- 自定义监控
	- URL重写
	- URI重定向
	- 简单防火墙
	- 代理、ABTesting、分流
- 提供管理界面用于管理内置插件

### v0.0.2

 - 完成监控、redirect/rewrite、WAF、分流等几个插件
 - 仍不推荐生产使用
