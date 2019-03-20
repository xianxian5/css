### display记录
### display：none | inline | block | inline-block | flex | inline-flex 

1. display：none 元素隐藏，不保留其物理空间。和visibility：hidden的区别*
2. display：inline 把元素转换成内联元素
3. display：block 把元素转换成块级元素
4. display：inline-block  把元素转换成内联块元素，定义width有作用。
5. display：flex 和 display：inline-flex 

### 重点记录flex和inline-flex
当给元素定义为flex时，元素为块级元素，它的宽度是父元素的宽度，或者定义的宽度。当定义inline-flex，元素为内联元素，它的宽度是内容的宽度。
```
<!doctype html>
<html>
<head>
<meta charset="utf-8">
<title>无标题文档</title>
<style>
	*{ padding:0px; margin:0px;}
	.contain{ display:flex; }
	.contain div{ border:1px solid #000; background:red; color:#fff; height:200px; width:200px; margin-right:10px; }
	

</style>
</head>

<body>
	<div class="contain">
    	<div>1</div>
        <div>2</div>
        <div>3</div>
    </div>
</body>
</html>
```


