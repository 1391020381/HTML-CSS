* box-shadow
  1. 营造层次感(立体感)
  2. 充当没有宽度的边框
  3. 特殊效果
* text-shadow
   1. 立体感
   2. 印刷品质感
* border-radius
   1. 圆角矩形
   2. 圆形
   3. 半圆/扇形
   4. 一些奇怪的角角(width:0;height:0;调整border-radius<四个角可以不一样>) 
* background
    1. 纹理、图案
    2. 渐变(线性,圆形)
    3. 雪碧图动画
    ```
    .i {
        width:20px;
        height:20px;
        background:url(./background.png) no-repeat;
        background-size:20px 40px;
        transition:background-position .4s;
    }
    .i:hover{
        background-position:0 -20px;
    }
    ```
    4. 背景图尺寸适应   
* clip-path
 1. 对容器进行裁剪 
 2. 常见几何图形
 3. 自定义路径
 ```
 .container{
     width:400px;
     height:300px;
     clip-path:circle(50px at 100px 100px)
     transition:clip-path .4s
 }
 .container:hover{
     clip-path:circle(80px at 100px 100px);
 }
 ```
 * transform<3D变换>   (animation-iteration-count: infinite)

 * CSS面试题
   1. 如何用一个div画xxx
      * box-shadow无限投影
      * ::before  ::after
   2. 如何产生不占空间的边框
      * box-shadow
      * outline
      * box-sizing:border-box 
   3. 如何实习ios图标的圆角
       * clip-path(svg)     
