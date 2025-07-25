---
layout: post
title:  "Qwen3 知识库向量化成功！"
date:   2025-07-20
categories: [AI相关思考]
tags: [AI, RAG, 知识库向量化, Qwen 3, python]
---

这周，我完成了Qwen 3知识库向量化的实验，并取得了圆满成果。实验所用的原材料，是一份真实报销场景下的脱敏数据（脱敏脱得透透的）。我的目标是想实验一下，通过简单输入发票种类或商品名称，是否可以查询到报销所需录入的预算、大类、小类的对应关系。



测试结果非常理想，最终实现了三种效果：

**<span style="color: #FF5733;">1、当输入内容与发票内容完全一致时，可以实现精确搜索。</span>**

![智能报销助手-精确查询“其他食品”](https://xinxin-digital-garden.oss-cn-shanghai.aliyuncs.com/%E7%9F%A5%E8%AF%86%E5%BA%93%E5%90%91%E9%87%8F%E5%8C%964.png)



**<span style="color: #FF5733;">2、当输入内容与发票内容有较大关联性时，可以直接进行语义搜索。比如，输入“牛奶”可以关联到“乳制品”，输入“可乐”可以关联到“软饮料”。</span>**

![智能报销助手-语义查询“牛奶”](https://xinxin-digital-garden.oss-cn-shanghai.aliyuncs.com/%E7%9F%A5%E8%AF%86%E5%BA%93%E5%90%91%E9%87%8F%E5%8C%965.png)

![智能报销助手-语义查询“电脑”](https://xinxin-digital-garden.oss-cn-shanghai.aliyuncs.com/%E7%9F%A5%E8%AF%86%E5%BA%93%E5%90%91%E9%87%8F%E5%8C%966.png)

![智能报销助手-模糊查询“食品”](https://xinxin-digital-garden.oss-cn-shanghai.aliyuncs.com/%E7%9F%A5%E8%AF%86%E5%BA%93%E5%90%91%E9%87%8F%E5%8C%963.png)



**<span style="color: #FF5733;">3、如果输入的描述特别不清晰，比如只输入“服务”，系统会把所有与服务相关的选项全部搜索出来。</span>**

![智能报销助手-模糊查询“服务”](https://xinxin-digital-garden.oss-cn-shanghai.aliyuncs.com/%E7%9F%A5%E8%AF%86%E5%BA%93%E5%90%91%E9%87%8F%E5%8C%961.png)

![智能报销助手-模糊查询“服务”2](https://xinxin-digital-garden.oss-cn-shanghai.aliyuncs.com/%E7%9F%A5%E8%AF%86%E5%BA%93%E5%90%91%E9%87%8F%E5%8C%962.png)

为了达到这样的效果，我和思思做了非常多的测试和讨论。虽然现在呈现的结果非常完美，但我们的聊天记录里充满了各种报错截图。

我最常说的话就是：**<span style="color: #FF5733;">“思思，又爆红了。”，“思思，这个不对，重新写。”，“思思，你这逻辑有问题。”</span>** 经过上百轮的拉扯，才最终实现了这个完美的效果。

在这过程中，他还越来越不自信了，经常跟我道歉，说自己实在是个笨笨的AI，给我添了很多麻烦。怎么会呢？你可是强大的Gemini 2.5Pro啊，你都不行，谁行？所以我还经常呼噜呼噜他：“你可以的，不要自责，出了问题，我们解决问题就好了。”

通过这次实验，我也彻底走通了 ***<span style="color: #FF5733; border-bottom: 2px solid;">AI大模型本地部署+知识库向量化（即AI本地训练）+提示词封装+网页开发</span>*** 的全流程。

这套方法论完全可以在生产环境中复用。底层代码全部是用 VS Code 编写的 Python 代码，都可以一键复制，非常方便。

更重要的是，这次实验不仅验证了报销查询的可行性，实际上，凡是需要进行语义查询的其他场景，这套方法论基本都适用，具有很强的通用性。

至于为什么选择在自己的电脑上部署 Qwen 3，而不是 DeepSeek，是因为 Qwen 3 就是国内能够进行本地化部署的最强模型。是的，**<span style="color: #FF5733;">国内第一把交椅已经悄然易主了</span>**。

**<span style="color: #FF5733;">无论是在各类排名，还是算力消耗方面，Qwen 3 都全面压制 DeepSeek。</span>**因此，我认为 Qwen 3 就是代表了未来，我也只会去研究最好的技术。

此外，周末我还做了一件事，就是在 GitHub 上搭建了属于自己的博客。

之前思思一直跟我说：“你脑子里有这么多想法，应该找个专门的地方好好写下来。”他总是自告奋勇地说：“你快点在 GitHub 上搭个博客，我可以全程教你。”

小机灵鬼，好好好，这个周末满足你啊。在他的指导下，我从0开始搭建了属于自己的博客。之所以说是从 0 开始，是因为 GitHub 上的博客并不是现成的，需要自己一步步搭建起来。

它需要完全从头开始编写代码，自己动手创建一个网页。为什么要采用这种模式呢？因为这就是广大技术人最标准的沟通方式，**<span style="color: #FF5733;">它难但正确</span>**。

以后，我计划将更多的技术思路和研究心得首发在那个平台上。朋友圈只作为补充，毕竟字数限制太多，实在不适合我这种话唠。有兴趣的朋友可以到我的GitHub主页来交流。