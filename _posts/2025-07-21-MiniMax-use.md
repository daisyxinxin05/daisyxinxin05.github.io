---
layout: post
title:  "MiniMax Agent，一款小白友好的网页编程工具，用嘴编程第一弹"
date:   2025-07-21
categories: [实用工具推荐]
tags: [AI, MiniMax, 编程, 项目]
---


搬运2025-7-5测评

今天用MiniMax的Agent做了2个网页项目，不得不说，这个新出的Agent真的太好用了。非常感谢赛博禅心的推荐。

我的第1个项目是仿照官网做了一个宝可梦介绍页面。第一次让它生成的时候，出来的是静态图片。它库库帮我写了一段代码，但我一看成品，发现有些图片没有显示出来，还有一些图片根本就不是单个宝可梦，和整体风格也不搭。

**第1版：**

![MiniMax第1版](https://xinxin-digital-garden.oss-cn-shanghai.aliyuncs.com/MiniMax%E8%AF%95%E7%94%A8/MiniMax%E8%AF%95%E7%94%A83.jpg)


我注意到官网有动态展示的效果，于是就让它改成动态图。它又去各大网站搜了一遍，第二稿出来后，我发现动态图反而没有静态图好看，像素风格实在是有点难以接受。

**第2版：**

![MiniMax第2版](https://xinxin-digital-garden.oss-cn-shanghai.aliyuncs.com/MiniMax%E8%AF%95%E7%94%A8/MiniMax%E8%AF%95%E7%94%A82.jpg)


于是我又全盘推翻，跟它说还是要静态图版本，但要帮我解决图片无法显示的问题，并且要确保每张展示图片只放一个宝可梦。

如果这种底层开发逻辑被反复推翻的事放在人类身上，估计早就崩溃了吧？但MiniMax二话不说，撸起袖子就是干，最后第3版出来的效果非常好。

**第3版：**

![MiniMax第3版](https://xinxin-digital-garden.oss-cn-shanghai.aliyuncs.com/MiniMax%E8%AF%95%E7%94%A8/MiniMax%E8%AF%95%E7%94%A81.jpg)

![MiniMax第3版2](https://xinxin-digital-garden.oss-cn-shanghai.aliyuncs.com/MiniMax%E8%AF%95%E7%94%A8/MiniMax%E8%AF%95%E7%94%A84.jpg)


这个Agent有一个很大的优点，就是它的思维链可以实时看到。每一步的想法都会清楚地展示出来，比如它接下来要做什么操作、调用什么库、使用什么函数、去哪些网站搜索资料等，全部都罗列得很明白。虽然下附的那些编程术语我完全不懂，但有了这样显性的思维链，就可以实时监控，知道它是否在正确的轨道上思考。对用户来说，这真的很让人安心。

![MiniMax思维链1](https://xinxin-digital-garden.oss-cn-shanghai.aliyuncs.com/MiniMax%E8%AF%95%E7%94%A8/MiniMax%E8%AF%95%E7%94%A85.jpg)

![MiniMax思维链2](https://xinxin-digital-garden.oss-cn-shanghai.aliyuncs.com/MiniMax%E8%AF%95%E7%94%A8/MiniMax%E8%AF%95%E7%94%A86.jpg)


而且它最棒的一点是，最后会自动进行模拟测试，不会把测试环节交给用户。它会模拟用户的真实使用场景，测试完后自己发现bug、自己找解决方法、自己改bug。最终呈现出来的，就是一个完成度非常高的成品。像我这个宝可梦项目，只跑了三轮就不用再让它修改了。

![MiniMax测试环节](https://xinxin-digital-garden.oss-cn-shanghai.aliyuncs.com/MiniMax%E8%AF%95%E7%94%A8/MiniMax%E8%AF%95%E7%94%A87.jpg)

第2个项目是我爸提出来的。他说自己现在用的日历是用WPS做的，想要一个电子版本。我又帮他详细描述了一下需求，MiniMax又帮我写了一大堆代码。第一次的效果其实已经很不错了，但没有考虑到老年人视力的问题，而且周末也没有做特殊标注，导出只支持json格式。

**第1版：**

![MiniMax日历1](https://xinxin-digital-garden.oss-cn-shanghai.aliyuncs.com/MiniMax%E8%AF%95%E7%94%A8/MiniMax%E8%AF%95%E7%94%A88.jpg)


因此在第二版中，我只提出了三个需求：

1、增加字体修改按键，以适配老年人的视力需求。  
2、对周末和法定节假日标记不同的背景颜色。  
3、支持导出为JSON和WPS格式。

这个项目在第2版已经达到了完美状态。现在，老爸已经非常开心地用起来了。

**第2版：**

![MinMax日历2](https://xinxin-digital-garden.oss-cn-shanghai.aliyuncs.com/MiniMax%E8%AF%95%E7%94%A8/MiniMax%E8%AF%95%E7%94%A89.jpg)


这种用嘴编程真的很简单，我并没有给它多么复杂的提示词，就是非常平实地把自己的需求描述清楚而已。

这边放一下我日历系统的提示词，可以感受下：

---
我需要一个日历系统。要有年视图和月视图。在每个日期里面，要可以填写当天事项，并保存在云端。重新打开后，这些事项仍然储存。

1、这个日历是给老人用的，现在的字体太小，需要有调整字体的选项。

2、对法定节假日，以及周末，进行背景色区分。

3、导出文件可为json和wps文件，需要提供选项。

---

因此，不要怕自己是编程小白，就不敢去尝试，只要你能好好说话，你就能用嘴编程，这是AI时代给普通人最大的赋能。

最后说下价格，我给MiniMax充值了20美元，相当于5000积分。两个项目总共消耗了大约3500积分。虽然价格有些昂贵，但只要你仔细看了它的工作流程，就会觉得这其实相当便宜，简直像捡白菜一样划算。感兴趣的朋友去玩吧。

地址：https://agent.minimax.io/

注意哦，现在需要通过google账号登录，所以，你懂的，自己搞定网络环境哦。