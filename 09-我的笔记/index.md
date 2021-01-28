# 一、定位

​		1.1.定位 = 定位模式 + 边偏移

​		1.2.position：relative：相对定位，相对于它原来的位置（自恋型定位）// 应用：给绝对定位当爹

​		1.3.position：absolute：绝对定位，相当与父级（拼爹型）// 应用：参照加了定位的父级

​		1.4.子绝父相：父级要占用位置，子级不需要占用位置，所以父级要用相对定位，子级要用绝对定位

​		1.5.脱标可以设置宽高

​		1.6.fixed：固定定位，以浏览器的可视窗口有直接关系，不占用位置，跟父元素无关 // 通常设置百分比，加配margin值微调

​		1.7.position：sticky，// 粘性定位，必须添加top或者left，right，bottom中的一个才生效

# 二、元素的显示和隐藏

​		2.1.display：none隐藏

​		2.2.display：block显示

​		2.3.visibility：visible显示，hidden隐藏 // 可见性，占有位置

​		2.4.overflow：hidden隐藏，scroll滚动条+隐藏，visible不隐藏，auto根据文字的长度进行隐藏 // 对盒子有定位的情况下慎用