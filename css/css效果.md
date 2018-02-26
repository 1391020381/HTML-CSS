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
