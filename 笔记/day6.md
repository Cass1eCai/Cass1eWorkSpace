<!-- overflow:文本溢出属性
        visible（默认值）:允许超出，正常显示
        hidden:超出隐藏
        scroll:不论是否超出都显示滚动条
        auto:超出部分显示滚动条
    1.当使用overflow-x或者overflow-y时，如果他们俩的属性值为scroll或者auto 时，会有一个默认值为overflow：auto -->

 <!-- white-space:
        pre 不换行 ，空格和回车原样输出
        nowrap 不换行，所有空格和回车解析成一个空格显示
        pre-wrap：换行，所有空格和回车原样输出
        pre-line 换行，回车原样输出，所有空格解析成一个空格显示 -->

<!-- 如何让单行文本显示省略号： -->
<!-- 步骤一，元素设置宽高 -->
        width: 200px;
        height: 200px;
<!-- 步骤二，不允许换行 -->
        white-space: nowrap;
<!-- 步骤三，超出隐藏  -->
        overflow: hidden;
<!-- 步骤四，显示省略号  -->
        text-overflow: ellipsis;

<!-- 解决基线对齐造成的图片幽灵空白节点： -->
<!-- 1.给图片设置和盒子一样的高 -->
        height: 112px; 
<!-- 2.将图片改为块状元素 -->
        display: block; 
<!-- 3.改变基线（只能加给图片） top,bottom,middle都可以 -->
        vertical-align: top;
<!-- 4.给盒子设置字号为0  -->
        font-size: 0;

<!-- 让一张图片在元素内水平垂直居中显示： -->
<!-- 给盒子设置：
text-align:水平居中
line-height:因为图片的vertical-align是根据行高来居中
font-size:不加这个的话，还会有1-2像素的区别
 -->
        text-align: center;
        line-height: 400px;
        font-size: 0;
<!-- 给图片设置：
vertical-align：根据行高，垂直居中
 -->
        vertical-align: middle;