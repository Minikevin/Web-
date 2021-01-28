# 一、选择器

​		1.1.标签选择器：按照标签名来寻找标签

​				例如：

```html
div {    
color: red; 
}
```

​		1.2.类标签选择器：按照用户自己分类

​				例如：

HTML

```html
<div class="big" >
    大的div
</div>
<div class="small" >
    小的div
</div>
```

**CSS**

```css
.big {
    color: red;
}

.small {
    color: green;
}
```

​		1.3.ID选择器：#，为了后期`JavaScript`而使用的 

**HTML**

```html
<div id="root" >
    id 选择器
</div>
```

**CSS**

```css
#root{
  color: red;
}
```

​		1.4.通配符选择器：*，可以选中所有标签

# 二、CSS/字体

​		2.1.font-family:定义字体系列

​		2.2.font-size:字体大小

​		2.3.font-weight:字体加粗 // 默认正常，bold加粗，lighter细体，bolder特粗，400=正常，700=加粗

​		2.4.font-style：字体样式，normal为默认的样式，italic为倾斜

​		2.5.font：符合属性写法 // font: font-style font-weight font-size/line-height font-family,size和family				不能省略

# 三、文本属性

​		3.1.color：颜色属性

​		3.2.text-align:对齐文本 // 有center居中对齐，left左对齐，right右对齐

​		3.3.text-decoration:设置文字的下划线 // none默认没有下划线，underline下划线，overline上划线，line-through删除线

​		3.4.line-height：行高

# 四、CSS三种引入方式

​		4.1.内嵌式：在 `html` 文件内 新建 `style` 标签 在 `style` 中 来书写 `css` 代码 这个方式叫内部样式

​		4.2.行内式：在目标标签上 直接添加 `style` 属性 ,来书写样式

**要仔细看清楚这个小语法哦!**

```html
<div style="color:red;width:100px;height:100px;" ></div>
```

行内的方式 是以后学 **js** 的时候会用得多一点

如果站在纯静态页面布局的角度来看的话 它也是**很少用**的!

​		4.3.外链式：最常用，方便管理，分门别类，方便复用，多个网页可以使用同一套css样式

```
css/index.css
div {
    color:red;
    background-color: yellow;
}
index1.html
<head>
    <title>页面1</title>
    <link rel="stylesheet" href="./css/style.css" />
</head>

<body>
    <div>页面1的内容</div>
</body>
index2.html
<head>
    <title>页面1</title>
    <link rel="stylesheet" href="./css/style.css" />
</head>

<body> 
    <div>页面1的内容</div>
</body>
```