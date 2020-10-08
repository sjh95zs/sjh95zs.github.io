---
title: HTML5中的Canvas元素
date: 2019-09-11
tags: HTML
categories: HTML
---

## HTML5中的Canvas元素

### 创建Canvas元素
向HTML5页面添加canvas元素，规定元素的id、宽度和高度：

```bash
<canvas id="myCanvas" width="200" height="100"><canvas>
```

### 通过JavaScript来绘制
canvas元素本身是没有绘制能力的。所有的绘制工作必须在JavaScript内部完成：

```bash
<script type="text/javascript">
        var mc = document.getElementById('myCanvas');
        var cxt = mc.getContext('2d');
        cxt.fillStyle = "#fff";
        ctx.fillRect(0,0,150,70);
</script>
```

JavaScript使用id来寻找canvas元素：

```bash
var mc = document.getElementById('myCanvas');
```

然后，创建context对象:

```bash
var cxt = mc.getContext('2d');
```

getContext('2d')对象是内建的HTML5对象，拥有多种绘制路径、矩形、圆形、字符以及添加图像的方法。

```bash
cxt.fillStyle = "#fff"; //fillStyle是染色的方法
ctx.fillRect(0,0,150,70); //fillRect 方法规定了形状、位置和尺寸。
```

### 理解坐标

上面的fillRect方法用于参数(0,0,175,70)。
意思是：在画布上绘制150*70的矩形，从左上角开始(0,0)

## 未完待续，更多实例请观看：https://www.w3school.com.cn/html5/html_5_canvas.asp