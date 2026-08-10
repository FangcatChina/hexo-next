---
title: 改变世界的文件格式
date: 2026-04-27 22:43:38
tags: [Videos]
categories: 视频稿
published: true
cover: /img/a-file-format-that-changed-the-world/cover.png
---

> 视频稿，成品视频见https://www.bilibili.com/video/BV1T37Q6BEnt

1980年代，伯纳斯·李在CERN发明了“探寻”，尼尔森的“上都”计划逐渐搁浅，自由软件基金会成立，FTP协议日趋流行。（引用自：超文本与超链接 - 李恪）而在1982年，一位42岁的中年人Warnock从施乐离职，在一个车库里同自己同样离职的上司创立了一家在40年后跻身全球500强的公司。他们以车库附近一条小溪的名字为这个刚出生的婴儿命名。这条小溪叫做Adobe Creek，因而，这家公司得名：Adobe。谁也没想到，这个车库里的小公司，在后来发明了真正改变世界的文件格式。


# Chapter 1: 印刷难题

八十年代初，计算机迅速发展，办公套件层出不穷，不过在推广时，却有经理这样反驳推销员：“Why should a manager use a computer? He has a secretary.”。这句在现在看起来荒唐可笑的推辞，却是那个年代的缩影。1984年，HP推出了第一款桌面LaserJet激光打印机，打印机自此开始接替了打字机的位置，出现在世界大大小小的办公室里。而新技术的到来必然伴随着新的问题。各位职场的牛马们肯定也见识过：在这一台电脑编辑完成的文档，到了另一台电脑就字体丢失、排版乱掉、图片错位，而打印出来的效果也极其不可控。

而说到这个难题，我们就不得不将时间倒回七十年代。1978年，在东方，改革开放的春风吹过大地。而远在地球另一边的Warnock去了施乐PARC，和另一位同事做了一个叫 JaM（John and Martin） 的页面描述语言。当时的PARC已经有激光打印机，但打印语言（Press）太弱，于是基于 JaM 开发了 Interpress，功能强大还不挑设备。正当他们信心满满，想要将这个成果推向市场时，目光短浅的施乐高层却摆了摆手：不，“打印机语言卖不出钱”。1982 年底，心灰意冷的Warnock离开施乐，决心把 Interpress 的思想做成真正能用的产品。

两年后的1984年，在Adobe，基于Interpress重写的PostScript发布。PS是一门十分强大的语言，支持矢量图形、任意字体、任意分辨率，并且关键的是：能保持跨设备一致。第二年，乔布斯就看中了这门语言，出资投资Adobe，并且把 PostScript 装进了苹果激光打印机 LaserWriter——桌面出版（DTP）革命正式开始。一夜之间，PostScript成为了印刷行业的标杆，并且不断迭代到了Level 2，加入对JPEG、分色、复杂色彩、字体内嵌的支持。一切欣然向好，不过，在PS统治打印领域的鼎盛时期，一位互联网时代的新秀也逐渐崭露头角。

# Chapter 2: 为文档而生，为共享而生

首先，让我们来回答一个疑问：既然PostScript已经足够好，为什么它却被埋没在时代的浪潮里？让我们首先拆解下PostScript这个词：PostScript直译为附言、后记，Post在这里有双重含义：一是Postfix，后缀表示法，这个学算法的各位信竟选手肯定再熟悉不过，这里指其采用的组织运算的方式，二是指“之后”，也意味着这是在打印前最后被处理的描述语言。Script这个词指脚本，还记得我们刚刚说的吗？PS是“在打印前最后被处理的描述**语言**”，也就是说PS并不能算作文档，而是一门实打实的编程语言。这就意味着要查看PostScript，我们必须要事前下载解释器或兼容软件。并且在互联网发展时期，它主要面向的是打印，而非屏幕查看和共享。

打开当前主流办公软件与操作系统的打印页面，打印机栏里总是缺不了一个有些“特立独行”的身影：Print to PDF，这是现代打印机打印的必备步骤：转换（打印）为PDF格式。我们视频今天的主角——PDF，国标译名便携式文件格式（Portable Document Format）。1991年，Warnock提出"The Camelot Project"，提出：
>  This project’s goal is to solve a fundamental problem that confronts today’s companies. The problem is concerned with our ability to communicate visual material between different computer applications and systems. The specific problem is that most programs print to a wide range of printers, but there is no universal way to communicate and view this printed information electronically.
>
> 这个项目的目标旨在解决一个困扰当今企业的根本性问题。该问题关乎我们如何在不同的计算机应用和系统之间传递视觉资料。具体而言，虽然大多数程序都能支持多种打印机输出，但却缺乏一种通用的方式来以电子化形式传递并查阅这些打印信息。
>
> （使用Gemini翻译）
> 
> （引用自：The Camelot Project - Dr. John Warnock）

到1992年，Camelot在PostScript的基础上发展成了现如今的PDF。这个新生的文档格式广泛支持矢量图形、位图，并且支持内嵌字体，能够便捷地跨设备移动。从1.4版本加入真图形透明度开始，PDF的功能正式脱离了PostScript。Adobe Systems在1993年免费提供了PDF规范。在HTML文本尚未兴起时，PDF在桌面出版工作流技术当中很受欢迎。（引用自：百度百科）
> It has helped transform the digital landscape, and has adapted through the years, bringing ever more powerful features into the fray.
>
> 它助力重塑了数字化版图，并在岁月的洗礼中不断演进，将愈发强大的功能引入这场变革之中。
>
> （使用Gemini翻译）
>
> （引用自：30 years of PDF: The file format that changed the world - TechRadar）

> “If Adobe Systems Inc. gets its way, corporate managers around the U.S. may soon be saying ‘PDF it to me’ instead of ‘Fed-Ex it,’” according to a Wall Street Journal story covering the launch.
>
> 《华尔街日报》在报道 PDF 发布时曾写道：“如果 Adobe 公司的如愿以偿，全美企业管理者的口头禅很快就会从‘用联邦快递寄给我’变成‘把 PDF 发给我’。”
>
> （使用Gemini翻译）
>
> （引用自：Evolution of the Digital Document: Celebrating Adobe Acrobat’s 25th Anniversary - Adobe）

> “In terms of employee satisfaction alone, Acrobat pays for itself,” an IRS official told Adobe. “Add to that the benefits of easier document administration and less paper storage, and it’s clear that Acrobat and Adobe PDF provide real returns to the agency and the people we serve.”
>
> Clearly there’s some fluff in that quote, but the IRS was very much a microcosm of the business world at large. The PDF, in a very short amount of time, became one of the most important ways business users shared documents. (Academia, of course, quickly bought in as well.)
>
> 一位美国国税局（IRS）官员曾对 Adobe 表示：“单从提升员工满意度这一点来看，购买 Acrobat 的钱就花值了。再加上更便捷的文档管理和纸质存储空间的缩减，显然 Acrobat 和 PDF 为我们机构及服务对象带来了实打实的回报。”

> 这段引言中显然带有些水分，但国税局确实是当时整个商业世界的缩影。在极短的时间内，PDF 便一跃成为企业用户分享文档最核心的方式之一。（当然，学术界也迅速接纳了它。）
>
> （使用Gemini翻译）
>
> （引用自：Why the PDF Is Secretly the World’s Most Important File Format - VICE）


在现如今，PDF已经成为了世界互联网上第三大流行的文件格式，被广泛应用于办公职场、学习教育、商务法律、设计出版等生活领域，政府公文、合同协议、电子书都有着PDF的一席之地。

但，在这场改革与狂欢中，一个难以忽视的问题，也日益显露出来。

# Chapter 3: 被垄断的编辑权

打开当今的搜索引擎，搜索“PDF编辑器”，各种选择令人头晕目眩，但是这些热门、专业选项都离不开同一个核心：付费。

在PDF刚刚发布时，PDF为Adobe所控制的专有格式，想要编辑PDF文件必须要先花五十美元购买Adobe Acrobat。

> 和 PostScript 一开始便受到大量追捧不同的是，PDF 和 Acrobat 刚发布的时候，它并没有立即取得成功。当时，Adobe 的首个 PDF 制作程序需要用户花费约 700 美元去购买，Acrobat Reader 则需要花费 50 美元。虽然 PDF 文件格式是免费开放的，但昂贵的软件使用费用依然阻止着机构与个人用户对 PDF 的接纳。除了成本因素外，PDF 还比纯文本使用起来更麻烦，在当时的网络环境下其下载速度也更慢。
>
> （引用自：不知不觉间，PDF 走过了 30 年的岁月 - WHYLAB）

直到2008年，PDF才被官方以开放标准发行，并由国际标准化组织发布。此后，标准的控制权便移转到了产业专家志愿者所组的ISO委员会底下。2008年，Adobe在ISO 32000-1 发布了公共专利许可，对于制作、使用、销售及发布PDF兼容的应用所需的专利，皆赋予**买断式授权**。（引用自：百度百科）对于制作、使用及发布 PDF 兼容应用所需的专利，Adobe 赋予了**免版税（Royalty-free）**的永久授权。看似是打破了垄断，但在实际操作中，它并未真正实现PDF编辑权的普惠。‘免版税’不等于‘零门槛’，PDF标准文档长达近千页，其内部逻辑极其复杂，中小开发者想要从零构建一个完美的渲染引擎，面临的是极高的研发成本和技术深水区。Adobe虽开放了专利，却凭借先发优势和技术暗箱，依然稳坐垂帘听政的位子。

2013年5月，Adobe开启了重要的商业模式转型——从传统的买断式授权，转向订阅制，宣布停止开发Creative Suite的买断版本，转而全力推行Creative Cloud订阅制。看似降低了使用门槛，却也让用户长期绑定在Adobe的生态中，难以脱离。

有的观众可能这个时候就要提到了：我们有强大的开源社区，现在有很多的开源编辑器可以作为替代品。诚然，当前的PDF免费编辑器也并不算少，然而这些看似强大的编辑器却暗藏着功能的缺失：复杂透明图形样式在开源编辑器下成了“黑哥们”，字体不兼容也展现的淋漓尽致。

不过，好在越来越多的其他格式正在打破这样“霸王条款”式的垄断。1980年代末，蒂姆·伯纳斯-李在CERN设计了最初的HTML，1945年布什用Memex所提出的超前的类“超文本”概念在2026年的今天仍旧稳如泰山，屹立不倒，在全世界千千万万的网站上为用户展示详尽的信息。2025年5月26日，国家知识产权局发布《关于进一步推广使用可扩展标记语言（XML）格式提交专利电子申请文件的通知》，提出：
> 2026年，我局系统将逐步升级为仅能接收XML格式提交的专利电子申请文件。

并且要求：

> 申请日在2025年10月1日（含当日）之后的专利申请，请求专利优先审查、快速审查、专利审查高速路（PPH）、延迟审查和集中审查的，须以XML格式提交电子申请。

不过客观来看，PDF的难以编辑的优势也在逐渐丧失，以下内容报道于2018年：

> Just take former Trump campaign manager Paul Manafort, who may not be the average person, but who runs into issues with the PDF just like the best of us.
> 
> Justice Department Special Counsel Robert Mueller’s most recent indictment of Manafort noted how the lobbyist and his colleague, Richard Gates, collaborated on modifying a PDF document by converting the document into Word format, changing an amount in the document, then changing it back to a PDF.
>
> This created something called a paper trail, bolstering Mueller’s case against Manafort.
>
>以前特朗普竞选经理保罗·马纳福特（Paul Manafort）为例。他或许不是普通人，但和我们大多数人一样，他也会遇到 PDF 带来的麻烦。
>
>司法部特别检察官罗伯特·穆勒（Robert Mueller）最近对马纳福特的起诉书指出，这位说客和他的同事理查德·盖茨（Richard Gates）曾协作修改了一份 PDF 文档：他们先将文档转换为 Word 格式，修改了其中的金额，然后再将其转回 PDF。
>
> 这种操作留下了一种被称为‘纸面追踪’（paper trail）的数字痕迹，最终成为了穆勒指控马纳福特的有力证据。
>
> （使用Gemini翻译）
>
> （引用自：Why the PDF Is Secretly the World’s Most Important File Format - VICE）

这看似滑稽的一幕，却实实在在地凸显出了PDF的危机。唉，世界真就是一个巨大的草台班子。


# Postscript: 后记
2026年是PDF发布33周年，在这三十多年里，PDF走过了风风雨雨，见证了互联网从雏形到普及，见证了办公方式从纸质化到信息化的蜕变。未来，或许会有更先进的文档格式出现，或许PDF会继续迭代升级，褪去旧的光环，焕发新的活力。但无论时代如何变迁，我们都不会忘记，这个诞生于时代风口、源于解决印刷难题的小小格式，曾以一己之力改变了数字文档的传播方式，影响了一代又一代人的工作与学习。

最后，以Warnock的一句话来作为本期视频的结语：

> I have seen that technology has contributed to improved communication, that it's contributed to better health care, that it's contributed to better food supplies, that it has contributed to all the basic human needs.
>
> 我看到技术已经为改善沟通做出了贡献，为更好的医疗保健做出了贡献，为更好的粮食供应做出了贡献，它已经为人类所有的基本需求做出了贡献。
>
> （使用Gemini翻译）
