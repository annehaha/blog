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

### 流程
怕越往后记忆越模糊，意识到记录大公司开发流程、测试流程、发布流程、运营流程时，为时已晚。趁现在记录一下。

参与过大大小小的项目开发到上线，从实验室项目到公司实习的项目，从小范围使用产品到过亿用户使用的互联网产品，发觉当中的运作模式不尽相同。

从最“low”的开始介绍吧，实验室项目：政府内部使用，要求上不如千万级用户的高品质追求，开发协作使用git完成，git仓库选用一些有稳定的就好，此处用Bitbucket，发布则放在云服务器上，服务器上也需要同步git，有新的代码直接拉取即可更新上线。

Intel：开发的SDK产品属于小范围使用型企业级产品，开发协作也是git，仓库Teamforge，通过gerrit平台提交代码，由于SDK对于代码质量要求较高，提交的时候需要走几个步骤：1.自动化测试，需要所有测试脚本全部通过 2.review环节，最高权力者或者两个审查者打勾才可以将代码合入分支。测试流程，有专门的测试人员编写测试脚本，发布时运行测试脚本，并打包。

阿里：互联网产品的用户数量庞大，整个流程都要走完全。开发用gitlab协作，对于代码的质量要求并没有特别高，连lint都没有用，主要是功能能用就好。测试耦合低，以功能测试为主，并没有见到脚本，压测什么的没有参与过。发布非常严格，从集团内灰到部分区域内灰最后全量发行，走的也是内部的雨燕平台，这个平台一直在完善中，当时也没有权限操作，在旁边看了看，谨慎发行是为了早期暴露bug能及时修复。另外，在发布过程中，有操作中心的专门人员操作可见面积，这点比较坑，走的时候他们仍然没解决这个最容易出错的环节。运营，阿里运营强大之处体现出来，凤蝶平台是专门给运营和开发搭建的桥梁，很好很强大。




