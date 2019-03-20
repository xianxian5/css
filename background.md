## background 是下列属性的缩写，不写几个也没关系
### background： [background-color] [background-image] [background-repeat] [background-attachment] [background-position] / [ background-size] [background-origin] [background-clip];

1. background-color 背景色，如有背景图片，除了背景图片用这个颜色填充元素，如果没有背景图片全用这个颜色填充
2. background-image 背景图片
3. background-repeat：repeat（默认值）|repeat-x|repeat-y|no-repeat|inherit; 背景图片是不是重复
4. background-attachment： scroll(默认值) | fixed | inherit;  背景图片是不是随着页面一起滚动
5. background-position：0px 0px; 设置背景图像的起始位置 --- 前一个值是横坐标，后一个值是纵坐标，有三种表达方式，第一种（top left）等，第二种像素，第三种百分比。
6. background-size：length|percentage|cover|contain; 规定背景图像的尺寸
7. background-origin： padding-box(默认值) | border-box | content-box; 相对于什么来定位背景图片
8. background-clip：border-box(默认值) | padding-box | content-box; 指定从哪个区域向外裁剪背景。

### 大背景自适应demo
```
<!doctype html>
<html>
<head>
<meta charset="utf-8">
<title>无标题文档</title>
<style>
*{ padding:0px; margin:0px;}
html,body{ height:100%; width:100%;}
.bg{ height:100%; width:100%; background: url(images/yaoqing_bg.png) no-repeat 0px 0px/100% 100%;}
</style>
</head>

<body>
	<div class="bg"></div>
</body>
</html>
```
