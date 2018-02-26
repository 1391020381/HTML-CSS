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