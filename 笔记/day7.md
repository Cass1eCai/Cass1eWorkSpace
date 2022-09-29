<!-- 定位-->
<!-- 1.相对定位:相对于元素原来的位置进行定位
不脱离文档流（保留元素原本的位置）
百分比是父盒子宽高的百分比  -->
position:relative
top:50%
left:50%

<!-- 2.固定定位：相对于窗口的位置进行定位
脱离文档流
 -->
 position:fixed

 <!-- 3.绝对定位：
 脱离文档流
 （1如果绝对定位的所有父元素都没有设置定位属性时，
 bottom的参照物是首屏
 top的参照物是html
 （2当元素脱离文档流后可以设置宽高,它的宽高也可以不设置而被内容撑开，
 （3margin无法操作脱离文档流的元素
 （4子绝父相：
 当子元素设置了绝对定位时，它的某一级父元素最好是相对定位，因为相对定位不会改变父元素在文档流中的位置，不会影响布局
  -->
position:absolute

  <!-- 4.粘性定位：
        达到阈值前，是相对定位
        达到阈值后，是固定定位 -->
position:sticky


<!-- 元素层级：
1.position: relative;
        可以使定位的文本层级高于其他元素 -->


<!-- 2.只有当元素的position为relative、absolute、fixed时，
z-index才可以生效  -->
position: absolute;
z-index: 1;


<!-- 制作三角形：
步骤一，宽高为0
步骤二，边框透明
步骤三，给需要的边框加上颜色 -->
width:0;
height:0;
border:px solid transparent
border-xx-color:;


<!-- 使元素水平垂直（对任何元素都有效） -->
<!-- 方法一： -->
position:absolute
top: 50%;
margin-top: -100px;
left: 50%;
margin-left: -100px;

<!-- 方法二： -->
position:absolute
top: calc(50% - 100px);
left: calc(50% - 100px);

<!-- 方法三： -->
position:absolute
top: 0;
left: 0;
bottom: 0;
right: 0;
margin: auto;


<!-- 锚点 -->

<!-- 1.跳转本页面内不同地点 -->
<a href="#id名"></a>
<div id="id名"></div>

<!-- 2.跳转不同页面的不同地点 -->
<a href="url#id名"></a>