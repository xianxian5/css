### display 记录
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

### 用在比较flex元素上的属性有六个属性作用于全体子元素
1. flex-direction：row|row-reverse|column|column-reverse  子元素的排序方向
2. flex-wrap：nowrap|wrap|warp-reverse   里面的元素一行排不下的时候换不换行，类似于文字
3. flex-flow：column nowrap ; 是flex-direction和flex-wrap的缩写。
4. justify-content：flex-start|flex-end|center|space-between|space-around   子元素横向的的对其方式
5. align-items：stretch|flex-start|flex-end|center|baseline 子元素纵向对其方式
6. align-content：flex-start|flex-end|center|space-between|space-around|stretch

### 用在子元素上，最用于子元素本身
1. order：0 默认值0，数值越小越往前排。
2. flex-grow：0， 默认值0，就算有空余空间也不放大，定义项目放大比例
3. flex-shrink：1，默认值1，如果空间不够将缩小，定义项目的缩小比例
4. flex-basis：auto，默认值auto，项目本来大小。它定义项目分配多余空间前，项目占的父的空间
5. flex：0 1 auto ，他是flex-grow，flex-shrink，和flex-basis的缩写
6. align-self：默认继承父亲的 align-items属性，没有则stretch


