---
layout: post
section-type: post
title: Javascript小技巧
category: Tech
tags: [ 'front-end', 'javascript' ]
---

### 一点点惊喜
`!!`

当你看到代码里的!!或者!!!，你有没有一脸懵比过？JS的弱类型就是让你看到各种灵活的代码，仔细分析下，!表示结果是false或者true，再加一个!无非是取反，那么纠结在于第一个!后面跟着是什么，如果是undefine，则!后为true，如果是正常对象，则为false。

少点废话，其实!!obj就是Boolean(obj).

`<i>`

你会不会经常看到大家用它写icon，可是！他难道不是表示<i>斜体</i>的吗？！对的，写成这样是想语义化，然而这样其实不合标准。可以看[解答](https://www.zhihu.com/question/26880548)。

`with`

用于设置代码在特定对象中的作用域。最主要的问题：依赖运行时语义，影响优化，易出错，易泄漏全局变量。