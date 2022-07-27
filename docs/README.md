---
home: true
title: 主页
heroImage: /img/pluginIcon.svg
heroText: Notes 代码笔记
tagline: 为程序员笔记而生
actions:
      - text: 快速上手
        link: /guide/getstarted/start
        type: primary
features:
- title: 基于原生
  icon: origin
  details: 跨平台, 支持所有Jetbrains开发工具例如IDEA, WebStorm, Android Studio等, 在线离线均可使用,不再需要额外的诸如Evernote等笔记软件
  link: /guide/getstarted/start.html
- title: 效率至上
  icon: effective
  details: 选择代码, 然后使用快捷键Alt+M或者Alt+Enter，一键存储笔记, 筛选当前项目笔记, 快捷搞笑
  link: /guide/getstarted/start.html
- title: 功能丰富
  icon: features
  details: 虚拟文件夹, 变更笔记编程语言, 搜索, 删除, 废纸篓, 关联源文件, 查看 Evernote 笔记, 各种功能一应俱全
  link: /guide/getstarted/start.html
- title: 轻量、界面友好
  icon: code-box-fill
  details: 轻量,仅12M大小,界面直观, 提供全窗口笔记展示模式, 支持切换紧凑模式

head:
  - - meta
    - name: keywords
      content: Notes, 代码笔记, Evernote
  - - meta
    - name: description
      content: Notes, 代码笔记, 一款最好的适合程序员使用的笔记和书签管理软件, 不离开IDE完成创建修改搜索代码笔记功能, 支持 SQLite 本地数据库存储或者Evernote存储, 支持查看Evernote网页笔记和图片

---
代码笔记的目标是成为一款最好的适合程序员使用的笔记和书签管理软件, 不离开IDE完成创建修改搜索代码笔记功能, 支持 SQLite 本地数据库存储或者Evernote存储, 支持查看Evernote网页笔记和图片.

::: tip 一分钟快速入门
* 步骤 1: 点击开发工具底部 `⭐代码笔记` 工具窗口
* 步骤 2: 点击蓝色字体 `在用户目录创建数据库`
* 步骤 3: 打开项目, 编辑任意程序文件并选择要添加进入笔记的文本
* 步骤 4: 按下`Alt+M`快捷键, 或者 按下 `Alt+回车` 组合键或者点击右键, 选择 `将所选代码添加到笔记 ...`
* 步骤 5: 添加标题, 代码笔记成功保存到了 `⭐代码笔记` 工具窗口
  :::


为庆祝简体中文版的发布, 国内用户加QQ群 150453653, 新用户立享6折优惠并不定期送一年免费优惠码.

中文用户如遇到字体显示问题, 可点击 代码笔记 工具窗口中的 小齿轮 ![](/img/icon/gearPlain.svg) 打开设置界面的默认列表或者树字体为中文字体例如微软雅黑即可.

支持设计模式富文本笔记及内嵌代码编辑器(抢先体验功能), 可通过 文件 > 新建 创建一个笔记文件.

[//]: # (<a href="https://www.jetbrains.com"><img src="https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.svg" width = "10%" /></a>)

[//]: # (<a href="https://www.jetbrains.com/idea"><img src="https://resources.jetbrains.com/storage/products/company/brand/logos/IntelliJ_IDEA_icon.svg" width = "10%" /></a>)


[![Jetbrains Plugins][plugin-img]][plugin]
![Version](https://img.shields.io/jetbrains/plugin/v/17501?logo=IntelliJ%20IDEA) ![Downloads](https://img.shields.io/jetbrains/plugin/d/17501?color=FE2857) ![JetBrains Plugins](https://img.shields.io/jetbrains/plugin/r/rating/17501)

[//]: # (<iframe frameborder="none" width="245px" height="48px" src="https://plugins.jetbrains.com/embeddable/install/17501"></iframe>)

## 手不离开发工具 保存,修改, 复用代码笔记
在编辑器中选中要收藏的代码, 右键点击 `将所选代码添加到笔记 ...` 或者使用 Alt+Enter的编辑器意图选择添加笔记, 输入标题后按下Enter键就可以在编辑器行首间距图标显示一个⭐图标, 同时行尾也会显示对应的注释信息. 点击此⭐图标或者按下Alt+Enter后即可选择编辑笔记标题, 移动文件夹, 删除笔记等操作.

在开发工具底部会多出一个`⭐代码笔记` 工具窗口, 在这个工具窗口可以进行创建删除虚拟文件夹, 修改编程语言, 修改笔记标题和内容, 新建搜索删除笔记等操作.

代码笔记正在持续完善中, 欢迎反馈问题和建议.

### 功能  :100:

* [x] 类似于 Mac 备忘录的操作界面
* [x] 自动保存代码和笔记
* [x] SearchEveryWhere 支持
* [x] Evernote 同步支持
* [x] 多达 300 种代码格式高亮
* [x] ......


[//]: # (::: chart Fast Request功能玫瑰图)

[//]: # ()
[//]: # (```json)

[//]: # ({)

[//]: # (  "type": "polarArea",)

[//]: # (  "data": {)

[//]: # (    "labels": ["易用性","Swagger", "Java", "Kotlin", "压测", "集成"],)

[//]: # (    "datasets": [)

[//]: # (      {)

[//]: # (        "label": "My First Dataset",)

[//]: # (        "data": [95, 90, 90, 70, 40, 60],)

[//]: # (        "backgroundColor": [)

[//]: # (          "rgb&#40;255, 99, 132&#41;",)

[//]: # (          "rgb&#40;75, 192, 192&#41;",)

[//]: # (          "rgb&#40;255, 182, 193&#41;",)

[//]: # (          "rgb&#40;255, 215, 0&#41;",)

[//]: # (          "rgb&#40;54, 162, 235&#41;",)

[//]: # (          "rgb&#40;0, 250, 154&#41;")

[//]: # (        ])

[//]: # (      })

[//]: # (    ])

[//]: # (  })

[//]: # (})

[//]: # (```)

[//]: # ()
[//]: # (:::)

[//]: # (------)

[//]: # ()
[//]: # (::: chart API工具对比)

[//]: # ()
[//]: # (```json)

[//]: # ({)

[//]: # (  "type": "radar",)

[//]: # (  "data": {)

[//]: # (    "labels": ["易用性","Swagger", "Java", "Kotlin", "压测", "集成"],)

[//]: # (    "datasets": [)

[//]: # (      {)

[//]: # (        "label": "Fast Request",)

[//]: # (        "data": [95, 90, 90, 70, 40, 60],)

[//]: # (        "fill": true,)

[//]: # (        "backgroundColor": "rgba&#40;0, 250, 154, 0.2&#41;",)

[//]: # (        "borderColor": "rgb&#40;0, 250, 154&#41;",)

[//]: # (        "pointBackgroundColor": "rgb&#40;0, 250, 154&#41;",)

[//]: # (        "pointBorderColor": "#fff",)

[//]: # (        "pointHoverBackgroundColor": "#fff",)

[//]: # (        "pointHoverBorderColor": "rgb&#40;0, 250, 154&#41;")

[//]: # (      },)

[//]: # (      {)

[//]: # (        "label": "Postman",)

[//]: # (        "data": [80, 80, 80, 50, 90, 100],)

[//]: # (        "fill": true,)

[//]: # (        "backgroundColor": "rgba&#40;54, 162, 235, 0.2&#41;",)

[//]: # (        "borderColor": "rgb&#40;54, 162, 235&#41;",)

[//]: # (        "pointBackgroundColor": "rgb&#40;54, 162, 235&#41;",)

[//]: # (        "pointBorderColor": "#fff",)

[//]: # (        "pointHoverBackgroundColor": "#fff",)

[//]: # (        "pointHoverBorderColor": "rgb&#40;54, 162, 235&#41;")

[//]: # (      })

[//]: # (    ])

[//]: # (  },)

[//]: # (  "options": {)

[//]: # (    "elements": {)

[//]: # (      "line": {)

[//]: # (        "borderWidth": 3)

[//]: # (      })

[//]: # (    })

[//]: # (  })

[//]: # (})

[//]: # (```)

[//]: # ()
[//]: # (:::)


::: tip 注意  
请确保你的 IDEA, Android Studio 版本 >= 2020.3+

[//]: # (插件版本       | IDEA版本要求)

[//]: # (------------- | -------------)

[//]: # (2.0.0~2.1.3   | 2020.3+)

[//]: # (2022.1.4+     | 2021.3+)

当然如果插件有更新，请确保更新到最新版本
:::

<Badge text="加入微信群购买享6折️,六折码已放群公告" type="tip" vertical="middle"/>

::: info 加微信群享6折优惠
<img src="/img/wechat_group.jpg" style="zoom:25%">
:::

[comment]: <> (## 🧲 友情链接)

[comment]: <> (<span style="width:16%;  padding:15px 15px 15px 15px;display:inline-block">)

[comment]: <> (    <a href="https://hertzbeat.com/" target="_blank">)

[comment]: <> (        <img :src="$withBase&#40;'/img/link/hertzbeat.svg'&#41;" class="no-zoom" style="height:40px;max-width:150px;margin: 10px;">)

[comment]: <> (    </a>)

[comment]: <> (</span>)

[comment]: <> (<span style="width:16%;  padding:15px 15px 15px 15px;display:inline-block">)

[comment]: <> (    <a href="https://gitee.com/dromara/easy-es" target="_blank">)

[comment]: <> (        <img :src="$withBase&#40;'/img/link/easy-es.png'&#41;" class="no-zoom" style="height:40px;max-width:150px;margin: 10px;">)

[comment]: <> (    </a>)

[comment]: <> (</span>)

[comment]: <> (<span style="width:16%;  padding:15px 15px 15px 15px;display:inline-block">)

[comment]: <> (    <a href="https://gitee.com/dromara/TLog" target="_blank">)

[comment]: <> (        <img :src="$withBase&#40;'/img/link/tlog-logo.png'&#41;" class="no-zoom" style="height:40px;max-width:150px;margin: 10px;">)

[comment]: <> (    </a>)

[comment]: <> (</span>)

[comment]: <> (<span style="width:16%;  padding:15px 15px 15px 15px;display:inline-block">)

[comment]: <> (    <a href="https://liteflow.yomahub.com/" target="_blank">)

[comment]: <> (        <img :src="$withBase&#40;'/img/link/lite-flow.png'&#41;" class="no-zoom" style="height:40px;max-width:150px;margin: 10px;">)

[comment]: <> (    </a>)

[comment]: <> (</span>)

[comment]: <> (<span style="width:16%;  padding:15px 15px 15px 15px;display:inline-block">)

[comment]: <> (    <a href="https://gitee.com/dromara/sa-token" target="_blank">)

[comment]: <> (        <img :src="$withBase&#40;'/img/link/sa-token.png'&#41;" class="no-zoom" style="height:40px;max-width:150px;margin: 10px;">)

[comment]: <> (    </a>)

[comment]: <> (</span>)



[comment]: <> (<span style="width:16%;  padding:15px 15px 15px 15px;display:inline-block">)

[comment]: <> (    <a href="https://gitee.com/dromara/hutool" target="_blank">)

[comment]: <> (        <img :src="$withBase&#40;'/img/link/hutool-logo.png'&#41;" class="no-zoom" style="height:40px;max-width:150px;margin: 10px;">)

[comment]: <> (    </a>)

[comment]: <> (</span>)

[comment]: <> (<span style="width:16%;  padding:15px 15px 15px 15px;display:inline-block">)

[comment]: <> (    <a href="https://gitee.com/dromara/forest" target="_blank">)

[comment]: <> (        <img :src="$withBase&#40;'/img/link/forest-logo.png'&#41;" class="no-zoom" style="height:40px;max-width:150px;margin: 10px;">)

[comment]: <> (    </a>)

[comment]: <> (</span>)


[comment]: <> (<span style="width:16%;  padding:15px 15px 15px 15px;display:inline-block">)

[comment]: <> (    <a href="https://jpom-docs.keepbx.cn/" target="_blank">)

[comment]: <> (        <img :src="$withBase&#40;'/img/link/jpom-logo.png'&#41;" class="no-zoom" style="height:40px;max-width:150px;margin: 10px;">)

[comment]: <> (    </a>)

[comment]: <> (</span>)

[plugin]: https://plugins.jetbrains.com/plugin/17501

[plugin-img]: https://img.shields.io/badge/plugin-Notes-x.svg?logo=IntelliJ%20IDEA
