---
layout: post
section-type: post
title: 帧动画
category: tech
tags: [ 'frontend', 'css3' ]
---

## 实现方式
js实现，通用动画库。
需求分析

* 设计接口：
loadImage(img)
changePos(ele,positions,imgURL)
changeSrc();
repeat(times);
repeatForever()
wait(time)
start(interval)//执行动画间隔
pause()
dispose()
支持链式调用
requestAnimationFrame
cancelAnimationFrame

几种异步方式：

* defer，仅ie能用
* async（H5新）
* promise

* jquery deferred

* q.js,c和s共用

* koajs

详细整理每个部分的实现，待续。


# 插播
关于[滴滴wepApp](https://github.com/DDFE/DDFE-blog/issues/4)的分享一点感想

有时业务压力大，专注于实现功能，缺乏思考，长期以来很危险。程序员真的不能只是埋头苦干，其实各行各业都是，看到这篇总结有些感同身受，结合蚂蚁实习的经历来说，有些地方简直说到痛点。话又说回来，道理我都懂，只是究竟怎么做的问题。还记得在离职前，疯狂的看ATA的文章，因为走了就没得看了，那段时间不长却开了不少眼界，比如淘宝首页的优化等等隐藏数据，还有好多好多，看别人的总结都是安逸的，不过不记下来还真的会忘记。

移动端click事件延迟300ms，这回事是为了给doubleClick腾出时间。