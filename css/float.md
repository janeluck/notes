css属性float总结
================

一、float特点
----------------

1. float属性的默认值为"none",继承性为no，还有三个可选的值:left,right和inherit（IE8以下不支持该值）
2. 应用float属性的元素脱离普通流，使父元素得不到其的高度（这里可以展开“清除浮动”）
3. 应用float属性的元素相当于拥有了方位且display为inline-block属性
4. 块级元素float后的width将不再是默认的父元素width的100%,而默认值成为0

二、float和position同用时
-------------------------

1. 与position:relative同用时，元素先浮动到相应的方位，然后再根据（top / left / bottom / right）所设置的值进行偏移
2. 与position:absolute或者fixed同用时，float失效

三、清楚浮动的常用方法
-----------------------

1. 父元素内部结尾添加一个HTML标签,设置clear:both.来手工清理浮动
2. 父元素设置 overflow:hidden 或 overflow:auto,配合可以设置zoom:1样式触发IE6 haslayout特性，来兼容所有浏览器清理浮动

####参考链接: http://w3help.org/zh-cn/casestudies/001 



