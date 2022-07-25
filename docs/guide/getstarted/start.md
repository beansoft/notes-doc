---
title: 快速开始
icon: start1
---


```flow
st=>start: 开始
cfg=>parallel: 配置
op1=>subroutine: 配置项目名
op2=>subroutine: 配置环境名
op20=>operation: 设置域名
op21=>parallel: 返回主界面
op3=>operation: 选择项目名
op4=>operation: 选择环境名
op5=>inputoutput: 点击方法左侧火箭🚀
op6=>operation: 点击发送按钮
e=>end: 结束|future
![img.png](img.png)
st(bottom)->cfg(path1,right)->op1(bottom)->op20->op21(path1,right)->op3->op5
st(bottom)->cfg(path2,left)->op2(bottom)->op20->op21(path2,bottom)->op4->op5
op5->op6->e
```

::: tip 使用入门
* Step1: 点击配置添加项目名[如微信卡片]和环境名[如local、dev]  
* Step2: 设置对应项目及环境的域名  
* Step3: 打开工具窗口(右上角位置),选择当前项目想要启用的环境  
* Step4: 点击在方法左侧的fastRequest的图标(自动生成参数和url)  
* Step5: 点击发送请求按钮发送请求  
:::

![](../../.vuepress/public/img/howToUse.gif)









