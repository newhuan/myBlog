# 管理后台第一阶段总结
做了什么，怎么做的，做出来的效果是什么样的，过程中遇到的问题和收获。
下一阶段还要做什么。

## 做了什么

轻流运营支撑系统，实现工作区的新购，续费和升级，以及数据叠加包的购买。

一门式管理后台，实现了一套JA管理后台专用的帐号体系以及工作区同步到sjtu的管理。

## 怎么做的

### 需求调研
https://shimo.im/docs/BMmbShHVnaMgpv8w

主要和市场的同事确认他们需要哪些功能，功能需要达到什么效果，各个功能之间的优先级

### 排期

轻流： https://shimo.im/sheet/bOIgDhR0AFscVPtH/RIDOC
每周安排一天的时间专门去做，排期包括确定方案，设计稿的实现

### 产品方案

轻流： https://shimo.im/docs/j7WAI8CgLWQwWBzj

JA： https://shimo.im/docs/4YbNrdthPX0nH4JX

### 前端

基于ant design pro 并做了多版本拓展

###### 多版本

- router
- webpackConfig
- index.html
- ico
- environment file

### 后端

首先感谢王臻、大哥、婷婷的帮助和指导。

- 轻流: @大哥

工作区续费，升级，新购，叠加包购买等一整套逻辑

- JA： @王臻 @oldFox

后端多项目实现，管理后台新的帐号体系，ja工作区同步到sjtu

## 做出来的效果

轻流： http://localhost:4202/user/login

JA： http://localhost:8000/sync-ws

## 问题和收获
###### 问题
- 前端多版本管理还是有点复杂，配置文件比较分散，看有没有办法每个版本只添加一个配置文件，而且index.html的多版本这块做的还是不太好，需要继续优化
- 前端因为比较赶，很多地方做的比较乱，需要整理
- 实现过程中没有和产品沟通就直接改了实现，需要对大红道个歉
- 后端感觉还有很多情况没有考虑到，比如错误处理，重置密码的次数限制等。

###### 收获
- 做了一次需求调研，了解了一下技术部门可以从技术方面协助市场做的事情。
- 尝试着做了一些交互和功能的设计
- 前端多版本控制理解更深了，需要做什么，需要怎么做也更加清晰。
- 后端有了一个开头，对在spring框架下的项目结构有了一定的了解。


## 下一阶段展望

先和市场和产品再次确定功能优先级，和产品确定实现方案和方式，确定每周安排的时间和排期。