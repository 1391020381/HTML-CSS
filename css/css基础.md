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
       * 边框背景图(border-image,round<保证图片重复次数为整数>)
       * 边框衔接(三角形,边框的衔接地方斜切的,且边框不占content的位置,content为0就可以做三角形)
    3. 滚动、换行 
        * auto(超出显示滚条)  scroll(始终显示) hidden visible 
        * overflow-wrap(word-wrap)通用换行控制(是否保留单词)
        * word-break针对多个文字(中文也是单词)
        * white-space空白处是否断行
    4. 粗体、斜体、下划线
       * 字重(粗体)font-weight
       * 斜体font-style:itatic
       * 下划线 text-decoration
       * 指针 cursor
    5. 其它
       * CSS Hack
       * 雪碧图(减少http请求,某些情况可能减少图片大小)
       * 表单美化
       ```
       <input type="checkbox" id="aaa">
       <label for="aaa"></label>
       ```
       input:checked + label{

       }
       input +label{

       }
         1. 使用 单选做table选项卡,通过选中状态,改变对应内容的display:block/none
         2. tree
  * 值得关注的选择器
  * 自定义字体的使用场景
    1. 渲染/品牌/banner等固定文案
    2. 图标字体
  * base64的使用
    1. 减少Http请求
    2. 适用与小图片
    3. base64的体积约为原图的4/3
  * 伪类和伪元素的区别
    1. 伪类表状态(如link)
    2. 伪元素是真的有元素
    3. 前者单冒号,后者双冒号  
