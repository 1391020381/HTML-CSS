# css 基础
 * Cascading Style Sheet
 * 层叠样式表
# 选择器的基本规则
  * 用于匹配HTML元素
  * 有不同的匹配规则
  * 多个选择器可以叠加
  * 分类
    1. 元素选择器 a{}
    2. 伪元素选择器 ::before{}
    3. 类选择器 .link{}
    4. 属性选择器  [type=radio]
    5. 伪类选择器  ::hover{}
    6. ID选择器 #id{}
    7. 组合选择器 [type=checkbox]+label{}
    8. 否定选择器  :not(.link){}
    9. 通用选择器 *{}
  * 权重
     1. ID选择器 #id{}  +100
     2. 类 属性  伪类  + 10
     3. 元素  伪元素  +1
     4. 其他选择器 +0 
     5. 只要出现优先级高的,优先级就高（不存在数学上的等价关系）
     6. !important优先级最高
     7. 内联样式优先级高
     8. 相同的优先级,后面的覆盖前面的 
  * 解析方式和性能
    1. 浏览器从右往左解析,加快css的解析,快速区分哪些不是
  * 非布局样式
    1. 字体、字重、颜色、大小、行高
      * 行高的构成
       1. 行高是有linebox(一群inlinebox)决定的
       2. 文本是按照基线对齐的(x的底面),可以通过vertical-align设置对齐方式
       3. lineHeight会称起外层的高度，当line-height大于字体的高度,line-height的高度会分布到上下的两侧即居中
      * 行高相关的现象和方案
         1. 图片下方的空白
           * 原理：默认排版是inline，涉及到文字对齐，默认是baseline,baseline与底线是有距离的。与字体大小有关
      * 行高的调整
      * 字体族(serif sans-serif monospace cursive fantasy)
      * 多字体 fallback(font-family:"PingFang SC","Microsft Yahei", monospace) 注意字体的平台适用性,例如 PingFang SC和Microsft Yahei的顺序调换，那么有Microsft Yahei字体的苹果电脑就会以Microsft Yahei显示，但没有PingFang SC好(安装了office的可能会有Microsft Yahei)
      * 网络字体、自定义字体
       1. 自定义字体(远程字体注意跨域)
         ``` 
         @font-face{
           font-family:"IF",
            src:url("./IndieFlower.ttf")
         }
         .custom-font{
           font-family:IF;
         }
         ```
      * iconfont
    2. 背景、边框
       * 背景颜色(rgba hsla   #fff)
       * 渐变色背景
       ``` 
       background: linear-gradient(135deg, transparent 0, transparent 49.5%, green 49.5%, green 50.5%, transparent 50.5%, transparent 100%), linear-gradient(45deg, transparent 0, transparent 49.5%, red 49.5%, red 50.5%, transparent 50.5%, transparent 100%);
    background-size: 30px 30px;
        ```
       * 多背景叠加
       * 多背景图片和属性(雪碧图)
       * base64和性能优化(图片转base64大小会增大1/3,会和css一起,增大解密的开销)
       * 多分辨率适配
       

       * 边框的属性：线型、大小、颜色
       * 边框背景图
       * 边框衔接(三角形)
    3. 滚动、换行  
    4. 粗体、斜体、下划线
    5. 其它
  * 值得关注的选择器
