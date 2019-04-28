## css继承性: ##
+ 字体颜色继承
  - 块元素继承父类颜色,a标签不继承.
  - 字体相关的属性  文本相关的属性(text-align , line-height)可以继承

## a标签的打开方式 ##
+ target属性表现形式
  - _parent 父类窗口打开  _top  顶级窗口打开 self 当前窗口打开

```html
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Document</title>
</head>
<body>
	这是一个测试页面
	<!-- _parent 父类窗口打开
	_top  顶级窗口打开 self 当前窗口打开 -->
	<a href="https://www.baidu.com/" target="_self">当前窗口打开</a>
	<a href="https://www.baidu.com/" target="_parent">父类窗口打开</a>
	<a href="https://www.baidu.com/" target="_top">顶级窗口打开</a>
</body>
</html>

```
## css颜色 ##
+ rgb:   rgb(0,0,255) ==> 绿色 ；rgb(0,0,0) ==> 黑色 rgb和十六进制是可以互换的。
+ rgba:  rgba(0,0,255,0.5) ==> 跟rgb一样，a是透明度：0~1； 0.5==> .5
+ 单独设透明度 opacity:0~1 

## form表单 ##
+ form 表单 <input type="text">
+ 密码框 <input type="password">

## 盒子模型 ##
+ 对盒子设置的宽高作用在content(内容区域),盒子的边框内外边距都会改变盒子的大小.
+ 外边距margin:垂直方向上的margin会出现重叠现象,里边盒子设置的 margin-top  作用用在了外部盒子身上,谁大谁生效.
  - 解决办法:1. 外边盒子设置 overflow:hidden;
             2. 给父类盒子加一个极小的padding;

## 显示和隐藏##
+ 隐藏后不占据位置,依然可以在位置上设置其他元素: display:none;
+ 隐藏后占据位置,其他元素按文档流继续设置: visibility: hidden;

## 清除float属性浮动的影响 ##
+ 对float属性元素设置明确的宽高.
+ 清除浮动的影响,在父类盒子设置: overflow: hidden;
+ 在浮动元素后边放一个空盒子设置: clear: left/right/both 
  - 不允许当前元素的left/right/both有浮动元素。
  - 例: 

  .foot {
			clear: both; 
		}




