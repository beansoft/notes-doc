---
title: Get started
icon: start1
---

```flow
st=>start: Start
cfg=>parallel: Config
op1=>subroutine: Add project name
op2=>subroutine: Add env name
op20=>operation: Set domain
op21=>parallel: Return main interface
op3=>operation: Select project
op4=>operation: Select env
op5=>inputoutput: Click rocket button on method left
op6=>operation: Click send button 
e=>end: End

st(bottom)->cfg(path1,right)->op1(bottom)->op20->op21(path1,right)->op3->op5
st(bottom)->cfg(path2,left)->op2(bottom)->op20->op21(path2,bottom)->op4->op5
op5->op6->e
```

::: tip How to  
* Step1: Click Manager config then add project name[example:wx card] and env[example:local、dev]  
* Step2: set target domain  
* Step3: open toolwindow(at the top-right corner),select project and env  
* Step4: click fastRequest icon on method left(generate url and param)  
* Step5: click send button for sending request  
:::

![](../../../.vuepress/public/img/howToUse_en.gif)









