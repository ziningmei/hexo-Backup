---
title: html画页面的时候遇到的一些问题
date: 2016-04-09 03:07:17
tags:
- Html
- Css
- Js

---
## 图片垂直居中

### 父div设置"line-height"，当前img标签设置"vertical-align:middle;"
```bash
<div style="line-height:40px">
	<img src="" style="vertical-align:middle;">
</div>
```
<!-- more -->
## div用absolute后撑开父div
### 需要借助js来实现

```bash
/**html**/
<div class="parent" style="position:relative">
	<div class="son" style="position: absolute; background-color: #1FB8EB">
</div>
/**js**/
$(".parent").height($(".son").height());
```
## div布局中高度不能用百分比
### 使用js让其高度＝宽度＊n，这样可以实现div内部的元素自适应手机分辨率
```bash
$(".a").height($(".a").width()*0.5);
```
## 手机页面蒙板
### 使用background-size: cover和position: absolute;

```bash
<style>
#qrcodeShare img{
	margin-top:0px;
	width: 100%;
	display:block;
	height:100%;
	background-size: cover;
	position: absolute;
	z-index: 61;
	opacity:0.8;
}
</style>
<div id="qrcodeShare" style="display: none;">
	<img src="../images/share_index.png"/>
<div>
```

### 页面右滑出现白色的竖线
### div设置宽度100%，禁止左右滑动
```
$(document.body).css({
   "overflow-x":"hidden",
   "overflow-y":"hidden"
 });
```