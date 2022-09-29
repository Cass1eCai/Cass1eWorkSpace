<!-- html标签 -->

<!-- 表格标签 -->

<!-- 无序列表：
type虽然已被弃用，但是仍可使用，为none值时则列表符号为空
 -->
<ul>
    <li></li>
</ul>

<!-- 有序列表：
type可以控制序号的样式
start可以控制开始的序号，用数字表示
reversed为倒叙
 -->
<ol>
    <li></li>
</ol>

 <!-- 自定义列表：
 dl和dd标签必须和dt标签一起使用
  -->
<dl>
    <dt>
    </dt>
    <dd>
    </dd>
</dl>

<!-- 表单标签:
        name表单的名字
        action数据提交的地址
        method数据提交的方式（get，post） -->
<form action="" name="" method="">
    <input type="" name="">
</form>

<!-- CSS样式：
1.<b>,<strong>,<i>,<em>,<del>,<u>,<span>等文本修饰标签默认情况下都不可以设置宽高
2.如果想要给body的子元素设置百分比高度，那么就需要给html和body都设置100%的高度
3.border只写solid时，颜色的默认值为元素内部的文字颜色
4.宽度为每个浏览器设置的默认宽度
 -->

<!-- CSS样式表:
优先级：行内样式表>（谁在后就会覆盖在前的样式表，在不考虑权重的情况下）
 -->

<!-- 行内样式表 -->
<div style="width:500px;"></div>

<!-- 内部样式表 -->
<style>
</style>

<!-- 外部样式表:
    1.rel为关联样式表
    2.两种写法的区别：
    差别1：本质的差别：link属于XHTML标签，而 @import完全是CSS提供的一种方式。
    差别2：加载顺序的差别：当一个页面被加载的时候（就是被浏览者浏览的时候），link引用的CSS会同时被加载，而@import引用的CSS会等到页面全部被加载完再被加载。所以有时候浏览@import加载CSS的页面时开始会没有样式（就是闪烁），网速慢的时候还挺明显。
    差别3：兼容性的差别：@import是CSS2.1提出的，所以老的浏览器不支持，@import只有在IE5以上的才能识别，而link标签无此问题。
 -->
<link rel="stylesheet" href="">
@import url()

<!-- 修改网页的logo -->
<link rel="icon" href="图片地址">