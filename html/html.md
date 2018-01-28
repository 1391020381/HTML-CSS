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
  1. table td[colspan,rowspan]  
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