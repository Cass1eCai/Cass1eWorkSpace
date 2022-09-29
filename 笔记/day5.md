<!-- 高度塌陷：
当子元素设定了float属性后，父盒子会出现高度塌陷的问题，遇到这样的问题，我们有这几种解决办法：
    1.如果不是float造成的高度塌陷：
    给定父盒子高度 
    2.如果是float造成的高度塌陷：
    给父盒子设置overflow:hidden，触发bfc机制
    3.万金油  
    通过css创建一个虚拟标签
     .clearfloat::after {
        content: "";
        display: block;
        clear: both;
        visibility: hidden;
        height: 0;
    }
    4.给子元素添加一个兄弟元素并给他设置
    clear：both -->
<!-- 
    clear：
    clear:使元素不与浮动元素在一排 -->

<!-- 
    margin：使元素水平居中 -->
margin: 0 auto;

<!-- css通用样式 -->
* {
    margin: 0;
    padding: 0;
}

a {
    text-decoration: none;
}

ul {
    list-style: none;
}

<!-- 使图片元素居中显示
给图片元素添加：
    position: relative;
    left: 50%;
    margin-left: -图片的宽的一半px;
给父元素添加（可以不写）：
    overflow: hidden; -->