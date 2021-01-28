# 一、浮动float

​		1.1.标准流：块级元素会独占一行，从上向下顺序排列/行内元素从左到右排列

​		1.2.可以改变默认的排列形式

​		1.3.边缘贴着对齐

​		1.4.浮动会脱离标准流（脱标）

​		1.5.浮动的盒子不再保留原先的位置

# 二、清除浮动

​		2.1.额外标签法：在浮动元素末尾添加一个空的div，设置div的样式为clear：both

​		2.2.overflow：hidden/auto/scroll，默认是hidden比较好

​		2.3.伪元素： ：：after

​						

```css
.clearfix::after {
  content: '';
  display: block;
  clear: both;
  visibility: hidden;
  height: 0;
}
```

​		2.4.双伪元素

```css
.clearfix::before,
.clearfix::after {
  content: '';
  display: table;
}

.clearfix::after {
  clear: both;
}
```