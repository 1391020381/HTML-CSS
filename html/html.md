# html常见元素
## head元素
* meta
    1. ```<meta charset="utf-8">```
    2. ```<meta name="viewport" content="width=device-width,initial-scale=1.0,maximum-scal=1.0,user-scalable=no">```
    3. ```<base href="/">```  <为后面所有的链接添加前缀>
* title
* style
* link
* script
* base
## body元素
* div / section / article / aside / header / footer
* p
* span / em / strong
* table / thead / tbody / tr / td
  1. table td[colspan,rowspan] <colspan 属性规定单元格可横跨的列数。> 
* ul / ol / li / dl / dt / dd
    1. 自定义列表不仅仅是一列项目，而是项目及其注释的组合。自定义列表以 ```<dl>``` 标签开始。每个自定义列表项以 ```<dt>``` 开始。每个自定义列表项的定义以 ```<dd>``` 开始。
* a
  1. a[href,target] 
* img
  1. img[src,alt]  
* form / input / select / textarea/ button
  1. form[target,method,enctype]
  2. input[type,value] <radio,checkbox,submit,hidden>
  3. button[type]<submit,button,reset>
  4. select>option[value]
* label
  1. label[for]
## html5提供的新的语义元素来明确一个web页面的不同部分<有利于理解seo>
   1. ```<header>```
   2. ```<nav>```
   3. ```<section>```定义文档中的节(section、区段)
   4. ```<article>```定义独立的内容
   5. ```<aside>```定义页面主区域内容之外的内容(比如侧边栏)
   6. ```<figcaption>```figure的标题
   7. ```<figure>```规定独立的流内容(图像、图标、照片、代码等等)
   8. ```<footer>```
   9. 表单增强
      * 日期、时间、搜索
      * 表单验证
      * Placeholder 自动聚焦
   10. em / strong 强调
   11. i icon   
 # HTML版本
 * HTML4 / 4.01(SGML)
 * XHTML(XML)
 * HTML5
 # HTML元素分类
 * 按默认样式
   * 块级元素 block
   * 行内元素 inline
   * inline-block
 * 按内容分
 # HTML元素嵌套关系(Content model)
 * 块级元素可以包含行内元素
 * 块级元素不一定能包含块级元素(p不能包含 div)  
 * 行内元素一般不能包含块级元素(a可以包含div)
 # HTMl元素默认样式 
 * list-style-postiton:inside
 * CSS Reset
    * reset css
    * yui css
    * * {margin:0;padding:0}
    * Normalize.css
 # HTML面试真题
  1. doctype的意思是什么
    * 让浏览器以标准模式渲染(比如 盒模型)
    * 让浏览器知道元素的合法性   
  2. HTML XHTML HTML5 的关系
    * HTML属于 SGML
    * XHTML属于xml ,是html进行xml严格化的结果
    * html5不属于 sgml或xml,比xhtml宽松  
  3. html5有什么变化
     * 新的语言化元素
     * 表单增强
     * 新的API(离线、音视频、图形、实时通信、本地存储、设备能力)
     * 分类和嵌套变更
  4. em和i有什么区别  
     * em是语义化的标签,表示强调
     * i 是純样式的标签,表斜体
     * HTML5中 i不推荐使用,一般用做图标   
  5. 语义化的意义是什么
     * 开发者容易理解
     * 机器容易理解结构(搜索、读屏软件)
     * 有利于seo
     * semantic microdata   
  6. 哪些元素可以自闭合
     * 表单元素 input
     * 图片 img
     * br hr
     * meta link 
  7. HTML和 dom的关系
     * html是死的
     * dom由html解析而来,是活的
     * js可以维护DOM
  8. property(特性,浏览器解析后获得,例如input的输入值)和 attribute(属性,写在html当中)的区别 (`<input value='1'>`)
     * attribute是死的
     * property 是活的
  9. form的作用有哪些
     * 直接提交表单
     * 使用submit/reset按钮
     * 便于浏览器保存表单
     * 第三方库可以整体提取值  
     * 第三库可以进行表单验证        