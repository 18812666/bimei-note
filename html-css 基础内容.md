##css继承性:
+ 字体颜色继承
  -块元素继承父类颜色,a标签不继承.
##a标签的打开方式
+ target属性表现形式

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
