---
title: "建站日志"
description: '介绍建站过程 日志'
pubDate: 2026-10-18
categories: ['Blog']
tags: ['astro', 'vercel']
excerpt: 介绍建站原因及过程
---

> 由于本人能力有限，这篇blog作为第一篇只是试水，不提供操作指南，相关内容请咨询AI，或者看themes原作者的[网站](https://d-sketon.github.io/)

> 文中有的地方大量使用英语不是我想装，其实是不认识的太多，高考完全还给老师了...

## 缘起

建站的直接原因是学校开展了**人工智能通识课**，结课作业是从 个人网站 小程序 APP 三个里面选择一个，在人工智能的辅助下完成。由于我假期自学过H5以及CSS，所以果断选择搭建个人网站。并且由于我折腾过服务器，所以想挑战下自己，于是堂堂建站之路开启ᕕ( ᐛ )ᕗ!!!

## 过程

### 第一天

和ChatGPT交流后，由于Ubuntu上有`node`，`npm`，`git`，所以决定在Ubuntu上进行操作。接着就让我`npm create astro@latest`。那么，这一步是什么呢？ChatGPT说是启动Astro的创建程序。我以前学习HTML以及CSS的原因就是想自己写个个人的网站，那是我天真且固执地想自己完全的写出来，这样的弊端就是完全不可能。所以当提到Astro的时候我完全不知道这是什么，~~虽然现在也是不太懂吧~~。在B站检索了下，发现了这个：[用 Astro 搭建一个高性能博客](https://www.bilibili.com/video/BV1i1421Z7ia/)。

按照他的步骤走了遍流程，其中themes使用的是up推荐的AstroPaper，部署使用的是Vercel，使用git在Ubuntu将网站传到github，Vercel监听github，部署网站，然后通过解析域名将网站从Vercel给到服务器。下面就是改改config.ts里的东西，搞成自己的就可以了。这个过程行云流水，万事俱备只欠东风，现在只需要写点内容就可以了...吗？

当我改完config，准备写内容时突然发现一个**小**问题，这个theme好像不支持中文啊!!!这不早说，我当时心态快炸了。我懒得搞什么i18n了，果断决定换一个theme。根据 ChatGPT 的推荐，我选择了现在使用的这个，由[D-Sketon](https://github.com/D-Sketon)大佬开发，一款hexo-theme-reimu的 Astro移植版本，博丽灵梦风格的 Astro [主题](https://github.com/D-Sketon/astro-theme-reimu)。

当时天色渐晚，我想快刀斩乱麻，直接将这个替换掉原来的那个，毕竟前面的那个我也没干什么，弃了就齐了。可是越忙越乱，ChatGPT给我的操作提示全是基于保护原来的那个，并且一直连不上github失败。当时我快着急死了，因为我电脑马上要没电了。我索性全删了，准备从头来过。

我重建了个repository，重新进行ssh，不知道由于什么原因，克隆下来后传到 Vercel 上又显示什么字体不对。我正打算问问ChatGPT大人，结果电脑关机了... (っ˘Д˘)ノ<沉默不是代表我的错

### 第二天

早上7点40多起来，距离9点半的选修课还有不到两个小时，~~ChatGPt~~我决定开始反击，ChatGPT叽里咕噜说了一大堆，基本没看懂，他猜测什么什么地方有错误，让我输入东西，然后结果复制给他，然后缩小范围，再输入东西...后来好像是 `pnpm run build` 发力了，就可以了( ﾟ∀。)

这个搞完，我就准备开始按照教程修改 config 了，由于有前面的经验，这次比较轻松。等到个性化的时候，由于个人头像大小不合适，又按照ChatGPT的指导，使用 `Pillow`将图片成功转化（这个家没ChatGPT迟早得散）。banner和ico目前还没找到合适的，就先用的原作者的。

接下来就是~~枯燥无味的~~内容了，正如你现在看到的，我在写日志...

## 展望
接下来可能是进一步丰富网站内容吧，把banner、icon什么的搞好。内容的话，还没想好分享什么，考虑下要不要做个小游戏什么的...就先写到这里吧，我头太疼了，得去补觉了


# 推荐[《草莓棉花糖》](https://www.bilibili.com/video/BV1Fx411w7m3/?spm_id_from=333.337.search-card.all.click&vd_source=24e6f5cc6bc1e84a76bd5dd182e9c980)
<iframe
  src="https://player.bilibili.com/player.html?isOutside=true&aid=111244&bvid=BV1Fx411w7m3&cid=185223&p=1&autoplay=0"
  scrolling="no"
  frameborder="0"
  allowfullscreen
  style="width: 100%; aspect-ratio: 16 / 9; border: none;"
  loading="lazy"
  title="Bilibili 视频播放器"></iframe>