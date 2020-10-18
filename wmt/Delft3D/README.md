---
title: Delft3D介绍及资源分享
tags: 1000天持续行动,Delft3D
date:  2017-12-4 

---

#  Delft3D介绍及资源分享

·[389]|1000天行动计划

读书笔记/热点追踪/论文研读/**教程手册**
​    
开始之前，先扯淡下。目前自己的1000天计划的水环境学习计划已经进行389天了，几乎40%了，但是平心而论，仅仅是时间上的程度而已，对于专业程度而言，估计连10%都没有达到。

在之前多次的回顾时，在100天，300天（哎，眼看就400天了）都提到自己应该加载更多的行动量，可是几乎仍然按照原路径在继续着，最近《地表水模型》也进入最后一部分，同时也临近年底，又是一个为新年计划的时刻，该时机也刚刚好，准备转变自己输出的风格。

目前，据我所知，学习一门技术有两种模式，Top-down and Bottom-up，这个解释有很多，对于我自己的理解，Bottom-up就是一种传统路径，从理论基础开始然后逐渐过渡到应用，而Top-down模式刚好相反，从实际应用开始逐渐到理论基础。

两种模式各有优劣，我自己喜欢的模式就是Bottom-up模式，所以自己从基础、经典的书籍开始慢慢学，但是现在我认为有必要开拓点应用方面的内容了，因为理论太过于枯燥，且缺乏应用场景，使得学习的内容无法落地。

那么应用，无非就是实际的建模应用，当然我还没有到那种自己开发模型的水平，所以先从现有的成熟模型开始，前人的思考，我们的阶梯。想来想去，选定了Delft3D，主要的原因是：

1. 源代码开源。其计算的引擎部分是开源的，这有助于学习及研究应用。
2. 商业公司维护。其是商业公司在运营的，这使得其资料丰富，社区相对活跃，毕竟对于小众的领域，开源的弊端就是无人管理维护。



## Delft3D介绍

### 多功能

功能指数：⭐⭐⭐⭐⭐

> Delft3D由Deltares（其前身为Delft Hydraulics）研发，是适用于海岸、河流、湖泊与河口水沙动力与水环境数值模拟的大型专业软件，已经经过30多年的开发和应用。主要应用于自由地表水环境，能够模拟二维和三维的水流、波浪、水质、生态、泥沙输移及床底地貌，以及各个过程之间的相互作用。其核心模块为水动力模块（FLOW），共包括波浪模块（WAVE）、水质模块（WAQ）、颗粒跟踪模块（PART）、生态模块（ECO）、泥沙输移模块（SED）和床底地貌模块（MOR）等七大模块。

上面引用互联网的内容，简单说其能够应用在大尺度地表水的水动力及水质（生态）的模拟中，功能十分强悍。上面所说的模块，其代表着模型能够解决的问题，在Deflt3D中是内部耦合的，也就是能够同时进行模拟分析。至于缺点，由于目前我也没有深入进去，所以无法与其他模型进行功能上的对比。


### 易用性

说了其功能的模块，也就是能够解决什么问题，这明白之后，我们也需要看使用难度。由于商业公司支撑，其有着：


> Delft3D软件包具有完整的前后处理程序，网格生成工具（RGFGRID）、地形编辑工具（QUICKIN），后处理工具（GPP 和 QUICKPLOT）处理得到的数据。系统实现了与GIS的无缝链接，有强大的前后处理功能，并与Matlab环境结合，支持各种格式的图形、图像和动画仿真；基于Visual Basic的用户界面非常友好。系统的操作手册、在线帮助和理论说明全面、详细、易用，既适合一般的工程用户，也适合专业研究人员。Delft3D支持所有主要的操作系统，如Windows, Unix, Linux, Mac等。

也就是说其从学习角度并不难，因为有着大量的资料及手册。应用方面，其有着完善的界面程序，强大的前处理和后处理工具（简单说前处理就是模型计算前的设置，后处理就是对计算结果进行分析、展示），并且能够与一些常用软件进行无缝对接。

最重要的是其目前其计算引擎开源了，当然界面程序还未开源，但是可以申请试用，试用期长达一年（超级良心，有没有），怎么申请之前自己也写过一篇说明，[申请方法](http://url.cn/5GkkeTJ)。

综上，无论从功能上说，还是学习、使用难度上其都相对靠谱，所以如果想学水质模型的，就从它开始吧。

另外，自己之前在网络上下载过一些中文的介绍，年代比较久远，但是其主要的内容还是不过时的，让大家熟悉一下。

附件：


- 水动力模块：

![水动力模块][2]

![水动力模块2][3]

- 河流地貌

![河流地貌][4]
![河流地貌2][5]
![河流3][6]

## 学习资源

官网的资料非常的丰富，我只是搬运工，把其官网梳理了一下，后续也是把这些作为学习的素材。另外，我也会陆续更新这个帖子，会把我收集的资料以及资源都汇总到这里，由于这里限制，发布后不能更新且链接可能无法点击，感兴趣的可以点击 阅读原文 进入到我的博客，进行查看，后续的更新也在那里。

![主要资源目录][7]


0 基础及问答
[WIKI](http://oss.deltares.nl/web/delft3d/community-wiki)
用户自己制作的知识图谱

[FAQ：常见问答](http://oss.deltares.nl/web/delft3d/faq;jsessionid=A417103C1DE09B3CDAB345198380E241.v-oss002.dlt.proteon.nl)
涉及一些常用的安装及使用的问题

[1 视频课程](http://oss.deltares.nl/web/delft3d/screen-casts)
Delft3D的英文教程，一步步操作方法。

[2 模型教程](http://oss.deltares.nl/web/delft3d/modelling-guidelines)
模型的建模指导，主要从建模提出了一些建议。

[3 网络研讨会](http://oss.deltares.nl/web/delft3d/webinars)
这里是其官网历次举办的网络研讨会，其中涉及较多应用方面的内容，是一些高手的报告。后续我会陆续进行学习。

[4 案例中心]( http://oss.deltares.nl/web/delft3d/process-demos)
提供了一些Delft3D的模型案例，模仿是最好的学习方式。

[5 社区分享](http://oss.deltares.nl/web/delft3d/community-wiki)
用户自己提交的一些案例及操作教程。

[6 论坛]( http://oss.deltares.nl/web/delft3d/forum)
论坛就是有关D3D的任何内容，所以当你遇到问题，不妨来这里搜索下试试看。

[模型功能演示]( http://oss.deltares.nl/web/delft3d/animations)
提供了多种动画来展示Delft的强大技术示例。

[论文成果研究](http://oss.deltares.nl/web/delft3d/research)
使用D3D进行的研究报告。



---

![页尾](http://comieswater-1254012817.cossh.myqcloud.com/%E9%A1%B5%E5%B0%BE%E8%AF%86%E5%88%ABnew-2017-09-22.png)
微信公众号 | 水环境编Cheng长
网           站 | comieswater.com
[1] http://oss.deltares.nl/web/delft3d/home

![赞赏我](http://comieswater-1254012817.cossh.myqcloud.com/IMG_3077.JPG)
2017-12-4


[1]: ./attachments/Delft3D-FLOW-CHN_CN.pdf
[2]: http://comieswater-1254012817.cossh.myqcloud.com/comieswater/1512397608409.jpg
[3]: http://comieswater-1254012817.cossh.myqcloud.com/comieswater/1512397646482.jpg
[4]: http://comieswater-1254012817.cossh.myqcloud.com/comieswater/1512398240554.jpg
[5]: http://comieswater-1254012817.cossh.myqcloud.com/comieswater/1512398267220.jpg
[6]: http://comieswater-1254012817.cossh.myqcloud.com/comieswater/1512398287389.jpg
[7]: http://comieswater-1254012817.cossh.myqcloud.com/comieswater/1512397790929.jpg