---
title: “安卓电脑”，能用吗？
date: 2026-04-03 21:04:26
tags: [Operating Systems,Videos]
categories: 视频稿
published: true
cover: /img/blissos/cover.png
---

> 视频稿，成品视频见https://www.bilibili.com/video/BV1MJDmBkErD

（视频：户子“安卓电脑”）
所谓“安卓电脑”具体指什么操作系统，现在的网络上也是众说纷纭，但大致上可以分为ChromeOS与BlissOS，至于ChromeOS，各位可以参考一下之前讲过的FydeOS，大差不差。本期视频，就让我们走进BlissOS，一窥手机操作系统能否在PC上大放异彩。

# 1. 根源

## 1.1 Bliss家族
说到BlissOS，就不得不提它的前身：BlissROM。BlissROM最初开始于大约2014年，在那时只是基于AOSP进行二改的定制ROM，主要注重的是高度自定义性（可惜在体验时并没有看出来这一点），并且借鉴了众多LineageOS的组件（图：目录命名）。根据官网描述：
> An open-source operating system built to deliver a harmonious blend of **customization**, options, and security features.

BlissROM在设计上有着Pixel，Havoc-OS等ROM的设计影子，并且基本保留了原生安卓的Material You设计理念，“卖点”（当然它是开源项目辣）是其详细的Blissify面板，基本上涵盖了所有可以进行自定义的组件，比如电源菜单、虚拟按键等等。BlissROM的ROM这个词就表明它其实主要注重的是arm64设备，可惜的是（截至3月14日）它仅仅官方支持10种型号设备。

在2016年，BlissOS正式对外发布，虽然并不像Android-x86那样历史悠久，但是却是后来者居上，算得上是开发最活跃的一个了，即使近年来版本发布放缓，但在2025年8月的时候还是在跟进上游内核，更新了新的开发进展：

> Let me tell you how busy we are without telling you we're busy... We are entering the end of the **60 day mark** for transitioning on Bliss OS side of things. 

目前的开发团队的最新进度是在2025年Jon West公布的新的BlissOS安装界面，之后就没了动静。

而且，BlissOS的上游开发团队BlissLab还参与开发Linux上的Waydroid，可以说专注Android开发一十年了。

## 1.2. 商业化？

截至写稿前，Bliss OS几乎关闭了所有社区讨论与联系方式，并且只能从SourceForge下载安装镜像。官网公告称正在开发新版本：
> This is an important announcement regarding the current status of the BlissOS project. We have placed the project under a temporary LOCKDOWN. The lockdown includes our Telegram support group, and Discord chat platforms, along with all BlissOS websites. Our Development chats will remain open for contributors throughout this time.
>
> At this time, **we cannot provide an estimated time of arrival (ETA) for when we will lift the lockdown.**
> 
> Feel free to dive into our archives on Sourceforge and explore past Bliss OS releases. Please keep in mind, these are snapshots in time and won't be receiving any further updates or support. **Our full focus is on crafting the next chapter for Bliss OS**, and we're excited for you to be a part of it when it arrives! The upcoming changes are so substantial that they make all existing documentation obsolete. It is crucial for us to prioritize rewriting our documentation and group notes to ensure that you have a smooth and successful experience with the new builds. Releasing new builds without accurate documentation would lead to confusion and a poor user experience.
> 
> All previous public releases will be **incompatible** with the new code base that we are preparing to deploy. This means that current users running existing builds will not be able to perform OTA (Over-the-Air) or manual updates to the new system. A complete reinstallation from scratch will be required.
> 
> We sincerely apologize for any inconvenience this may cause and we are incredibly grateful for your continued support and understanding. We have confidence that your patience will be worth it.

这种情况从2025年五月起，已经持续了快一年，这意味着用户有将近一年无法通过官方渠道反馈任何问题，不知当前开发进展如何。但BlissLabs的成员，如CTO@electrikjesus的Github贡献基本不在Bliss OS，而是在Bass OS等Bliss OS的衍生与兄弟项目上。值得注意的是，Bass OS由Navotpala Tech(Blissful Innovation)开发，这家公司是BlissLabs的赞助商，并且其创始人也是前面所提到的@electrikjesus，而Bass OS又也在2025年首次推出，是需要进行付费的Bliss OS衍生物，这很难不让人怀疑Bliss OS是否已经被废弃或是仅作为基本发行版用作商业化运行。讽刺的是，CTO本人还在Substack上发文谴责那些将开源项目视作Free R&D的商业公司。

可惜我钱包空空，买不起Bass OS，还是让我们回到Bliss OS本身吧，当第一次了解这个操作系统的时候，我生出了一个疑问：将安卓这样的移动端设备逻辑移花接木到PC端，用户体验真的能够舒适吗？

> BlissOS的开机Slogan: Have A Truly Blissful Experience


# 2. 上手

## 2.1 Advantages

在YouTube上，有很多科技播主给出了不错的评价，有人用它复活了远古Surface，有人运行谷歌全家桶流畅无压力，还有人用它畅玩大量手机游戏，看起来用来日常使用完全没有问题。

Bliss OS目前主要有三个大版本，提供GApps与FOSSApps可选，还有十分多样的安装方法，我这里选择的是基于Android13的v16.9.7 GApps版本+实体机安装。和众多基于Linux内核的系统一样，其LiveDVD采用Grub作为引导器。但有意思的是，其安装程序由于安卓系统的安全限制，并不是直接在LiveDVD中运行，而是有单独的Installation选项。复古的DOS样式，让我瞬间感觉我在操作raspi-config，但是对于普通用户，这样的体验算不上舒适。BlissOS内置了cfdisk与cgdisk两种分区工具，适配不同的分区表，还贴心的进行了标注。选完EFI分区与安装分区，还可以预装Grub或是rEFInd，十分贴心，但可惜并不支持原本的较新引导程序。

安装之后，熟悉的Material You设计扑面而来，Blissify面板十分详细，并且还自带了KernelISU和Termux，十分适合用来倒腾。

However, the "blissful experience" 在日常使用中给我的感觉其实并没有那么blissful。

## 2.2 Shortcomings

BlissOS分为了普通模式和桌面模式，但初次配置的时候使用Desktop Mode会出现稀奇古怪的应用终止和止不住的鬼畜。作为一个电脑操作系统，BlissOS有着十分割裂的任务栏：有自带的Taskbar，有Launcher 3，有Smart Dock，还有安卓自带的任务栏（关不掉只能共存的那种！）。
对桌面环境的适配也十分拉跨：高得夸张的DPI，HD界面的应用，要拖动小白条上滑关闭的设置页面，完全不符合键鼠操作逻辑。甚至在使用触控板时，还经常会出现拖动鼠标被当成按住拖拽的情形。甚至，有意思的是，BlissOS的官方文档里的“Install Legacy From Bootable USB”竟然还是是Android-x86借来的。
至于软件生态，理想很美好，现实很骨感。本以为能够背靠安卓系统强大的Play Store和第三方应用商店，却发现连一个具有桌面级完整功能的Office套件都没有。众所周知，很多人都这样讽刺鸿蒙电脑是大号平板：

> 登个QQ给我手机QQ顶掉了

但有意思的是，鸿蒙没有实现的特性，BlissOS实现了，甚至都没有平板登录的选项。
应用的兼容性似乎也不佳，由于BlissOS运行于x86架构，在运行多数安卓应用时需要转译，由于libhoudini的授权收紧，BlissOS改用了libndk，而其兼容性却相对较差，而这就会导致各种问题与性能损失。并且在驱动问题上也几乎没有解决办法，Bliss OS无法连接家里的Wifi网络，和我之前用Android TV无法连接IPv6网络几乎是完全一致的表现。我发的Reddit帖子下也有一些用户发出了所遇到的问题（展示）。

之前在讲FydeOS的时候就有人评论：

> FydeOS最大的用途就是给设备性能较弱或需要续航延长点的X86A平板设备，比如Surface早期设备安装了Windows 8.1这种性能较弱的设备，有Linux容器让生产力成为可能。
> @LyonHyrik

还有人推荐BlissOS：

> x86平台上，我觉得BlissOS好多了
> @明风の岚

但我的个人感觉是BlissOS的粗糙程度要远大于FydeOS，甚至还不如装Xfce的GNU/Linux：好歹有像样的桌面应用与环境能用，而BlissOS连浏览器都是手机操作逻辑，更不要提日用。



# 3. 对象

讲真，写稿写到这里，我个人是有点心虚的。BlissOS现在主要仅由两位开发者维护，精力自然不足，并且本身的市场就不怎么大，我个人认为主要适合的是类似某些ChromeBook那样的可翻折触屏电脑。但是，ChromeOS还要比BlissOS多出一个Linux子系统，我想不明白有什么理由要丢了芝麻捡西瓜去选择一个称得上是“残废”的操作系统。有人会说可以用在服务终端，但是显然arm架构要比x86成本更低，占地更小，功耗还低。目前的应用，我只能想到老掉牙到FydeOS和ChromeOS都跑不动的设备，又或者是某些工业设备，但参考资料不多。

本质上，BlissOS的问题就是逻辑与对象的问题，手机的点击逻辑强行接到了手中的鼠标自然会十分难受，本不适合作桌面端办公娱乐的系统被搬到了大屏幕上。去年，Google宣布要使用安卓内核替换ChromiumOS，推出Aluminum OS，桌面逻辑的布局终究还是将要被专业团队与清晰的定位来完成。

上期视频下有很多留言，我都一一看过，有讨论自己折腾经历的，有分享失败经验的，当然也不乏孤傲的指点与AI宣传大使。当我们在讨论某个操作系统没有想象中的容易，亦或是没有想象中的那么难的时候，我们至少需要找到自己的定位，亦或是换位思考：我是谁？我的需求是什么？我的能力水平在哪里？不然特别容易闹出让40岁老妈学命令行语言的笑话。

不过我在这里回应一下质疑学习难度的人：我见过连解压文件下载Steam都不会的人能够用流畅Windows编辑文档，而没见过哪个小白能在Linux流畅装中文输入法装mscorefonts排查文件格式问题。

诚然，逻辑的照搬，定位的不清，自然会招致体验的不舒适与批评声。

至于先前的问题，想必各位也有了自己的答案。

观点仅供参考，汝之蜜糖，吾之毒药。