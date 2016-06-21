---
layout: post
section-type: post
title: 实习伊始
category: Tech
tags: [ 'internship', 'front-end' ]
---

### 初进蚂蚁
报道那天进了支付宝大楼，发现只需要工牌和手机就可以在这里存活下去，支付宝渗透了方方面面，阿里内部还有很多app，方便的飞起，比如有个app的功能是可以控制会议室的空调和灯，像我这种想做小透明的人再也不需要尴尬的站起身了。

### 环境部署
阿里前端用了不少封装的UI，他们用的tnpm也是npm的镜像部分内容对内使用，Ant－tool是自己做的脚手架工具。除此之外，各种配置文档写的挺清晰，按照代码框里面的步骤走，基本不看其他说明也能快速成功，如果要我提意见找bug，就需要细心来吹毛求疵了。阿里前端的开发构建如此成熟，还是挺开眼的。
接下来会持续更新一些收获。

### 工具小结
[npm](https://www.npmjs.com/) : npm的全称是Node Package Manager, 是一个NodeJS包管理和分发工具。

tnpm : 阿里内部 npm 及 源 npm 镜像，完整 npmjs.org 镜像，同步频率目前为 10分钟 一次以保证尽量与官方服务同步。

React :React 是一个 Facebook 和 Instagram 用来创建用户界面的 JavaScript 库。 React 是为了解决一个问题：构建随着时间数据不断变化的大规模应用程序.

React Native :React Native 结合了 Web 应用和 Native 应用的优势，可以使用 JavaScript 来开发 iOS 和 Android 原生应用。在 JavaScript 中用 React 抽象操作系统原生的 UI 组件，代替 DOM 元素来渲染等。

Flux :Flux是Facebook用来构建用户端的web应用的应用程序体系架构。它通过利用数据的单向流动为React的可复用的视图组件提供了补充。相比于形式化的框架它更像是一个架构思想，不需要太多新的代码你就可以马上使用Flux构建你的应用。

antd :Ant Design 是面向中后台的 UI 设计语言。Ant Design 在蚂蚁金服中后台产品线迅速推广，对接多条业务线，覆盖系统 40 个以上。定位于中后台业务的 Ant Design 兼顾专业和非专业的设计人员，具有学习成本低、上手速度快、实现效果好等特点，并且提供从界面设计到前端开发的全链路生态，可以大大提升设计和开发的效率。

Roof : 在 React 中，组件间的数据交互往往是一件比较麻烦的事。
Roof 给出了一种解决这个问题的办法。

Anima : Anima是面向于H5移动Web开发的一套整体解决方案。她继承了Arale家族的光荣传统，立足于支付宝的H5移动Web前端需求，致力于更 轻、更 小、更 美的架构设计，包含了一整套构建、编码、调试、打包的开发体系，完全遵循CommonJS规范并以最开放的态度打造模块生态圈，是一套开放、简单、易用的H5移动Web前端解决方案。

[Yocto](http://gitlab.alibaba-inc.com/animajs/yocto)基于Zepto核心，绝大多数API与Zepto保持一致，不一致的部分Yocto也提供shim机制抹平差异。
Yocto的core精简了不常用的API，去除不必要的逻辑，深度优化了性能。
Yocto采用spm模块化方案，可以灵活组装和拆解，从而保证体积最小和性能最佳。
Yocto提供touch的完整解决方案，解决click的300ms延迟，解决了Zepto一直没有解决的tap事件的穿透问题。

[HPM](http://hpm.h5.alipay.net/):Hybrid-App package manager and developing kit,HPM调试[H5](http://h5.alipay.net/portal/article/151)

凤蝶： 支付宝的运营内容管理平台。

[babel](https://babeljs.io/): 可以把符合 ECMAScript 6 标准的代码完美地转换为 ECMAScript 5 标准的代码，并且可以确保良好地运行在所有主流 JavaScript 引擎中。

[atool-build](https://github.com/ant-tool/atool-build) :基于 webpack 实现,支持通过 webpack.config.js 进行扩展 webpack 的配置项,支持 stage-0, es2015, react 和 less
支持 hash 模式的构建, 并生成映射表 map.json,支持 typescript

[dora](https://github.com/dora-js/dora) : dora将编译的过程放在自己起server的生命周期中，只要一个命令就完成build watch server的阶段。不需要多个terminal或者多个命令，只要一键配成，傻瓜式。

### 其它工具
图片压缩： <https://tinypng.com/>

编辑器：Sublime, WebStorm, Atom

调试工具 ： weinre chrome safari

### 翻墙
又一免费翻墙方法：
[ihost](http://ihost.alibaba.net/) ＋ [racaljk/hosts](https://github.com/racaljk/hosts)
